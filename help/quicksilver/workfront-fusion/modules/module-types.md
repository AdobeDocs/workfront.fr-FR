---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Types de modules
description: '''Adobe Workfront Fusion distingue cinq types de modules : modules d’action, modules de recherche, modules de déclenchement, agrégateurs et itérateurs. Les agrégateurs et les itérateurs sont destinés à des scénarios avancés."'
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---

# Types de modules

A[!UICONTROL Adobe Workfront Fusion] distingue cinq types de modules : modules d’action, modules de recherche, modules de déclenchement, agrégateurs et itérateurs. Les agrégateurs et les itérateurs sont destinés à des scénarios avancés.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter Adobe Workfront Fusion ainsi qu’Adobe Workfront pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Modules d&#39;action

Les modules d’action sont le type de module le plus courant. Un module d’action type renvoie un lot unique, qui est ensuite transmis au module suivant pour le traitement.

Contrairement aux modules de déclenchement, les modules d’action peuvent être placés au début, au milieu ou à la fin d’un scénario. Les scénarios peuvent contenir un nombre illimité de modules d’action.

>[!INFO]
>
>**Exemples:**
>
>* **[!DNL Workfront]> [!UICONTROL Chargement d’un fichier]** envoie un fichier à [!DNL Workfront] et renvoie son identifiant.
>* **[!UICONTROL Image] > [!UICONTROL Redimensionner]** reçoit une image, la redimensionne selon les dimensions spécifiées et la transmet à l’action suivante.


Le type d’action comporte quatre sous-types : Créer, lire, mettre à jour et supprimer. Le sous-type Mise à jour permet les trois opérations suivantes :

* **Effacer le contenu d’un champ**. Cette opération se produit lorsque le contenu du champ est évalué pour effacer un mot-clé (à ne pas confondre avec *empty*).

   ![](assets/erase-content-of-field.png)

* **Ne pas modifier le contenu d’un champ**. Cette opération se produit lorsque le champ est vide ou que le contenu du champ est évalué sur vide (représenté par une valeur nulle dans JSON).

   ![](assets/leave-content-field-unchanged-350x231.png)

* **Remplacer le contenu d’un champ**. Cette opération a lieu dans tous les autres cas que les deux décrits ci-dessus.

>[!NOTE]
>
>* Si vous ne voyez pas l’événement `erase` dans le panneau de mappage, le module n’est pas un module de mise à jour ou il n’a pas été mis à jour selon les dernières spécifications de l’application.
>* &quot;[!UICONTROL Vide]&quot; ne modifie pas le contenu du champ. S&#39;il est nécessaire d&#39;effacer le champ, vous pouvez utiliser la formule suivante :
>
>![](assets/formula-ifempty-name-erase.png)
>
>Il n’est actuellement pas possible de laisser un champ inchangé lorsque son contenu est évalué comme vide.

## Modules de recherche

Une recherche type renvoie zéro, un ou plusieurs lots, qui sont ensuite transmis au module suivant pour traitement.

Vous pouvez placer les recherches au début, au milieu ou à la fin d’un scénario.

Les scénarios peuvent contenir un nombre illimité de recherches.

>[!INFO]
>
>**Exemple:**
>
>**[!DNL Workfront]> [!UICONTROL Lire les enregistrements associés]**  lit les enregistrements correspondant à la requête de recherche que vous spécifiez, dans un objet parent particulier ;

## Déclencher des modules

Les déclencheurs génèrent des lots lorsqu’un service donné a été modifié. La modification peut être la création de nouveaux enregistrements, la suppression d’un enregistrement, la mise à jour d’un enregistrement, etc.

Chaque déclencheur peut renvoyer zéro, un ou plusieurs lots qui sont ensuite transmis au module suivant pour traitement.

Les déclencheurs ne peuvent être placés qu&#39;au début d&#39;un scénario.

Chaque scénario ne peut contenir qu’un seul déclencheur.

[!DNL Workfront Fusion] distingue deux types de déclencheurs : Déclencheurs d’interrogation et déclencheurs instantanés.

### Déclencheurs d’interrogation

Les déclencheurs d’interrogation interrogent régulièrement un service donné même s’il n’y a eu aucune modification depuis leur exécution précédente. Nous vous recommandons de planifier l’exécution à intervalles réguliers d’un scénario contenant un déclencheur d’interrogation. Si une *change*, le déclencheur renvoie les lots contenant des informations sur la modification. Si la variable *change*, le déclencheur ne génère aucun lot. Pour obtenir des instructions sur la planification d’un scénario, voir [Planification d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Les déclencheurs d’interrogation vous permettent de sélectionner le premier lot qu’ils doivent générer à partir du panneau d’époque. Le panneau s’affiche automatiquement après l’enregistrement ou la modification des paramètres du déclencheur. Pour plus d’informations, voir [Sélectionnez l’endroit où commence un module de déclenchement dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>Les paramètres définis dans le panneau Epoque n’affectent que la première exécution du module. Une fois le module exécuté, il mémorise le dernier lot sorti et vide les paramètres effectués via le panneau d’époque.

>[!INFO]
>
>**Exemples:**
>
>* **[!DNL Workfront]> [!UICONTROL Surveiller les enregistrements]** renvoie les fichiers qui ont été ajoutés depuis la dernière exécution du scénario.
>
>* **[!DNL Google Sheets]> [!UICONTROL Lignes de contrôle]** renvoie de nouvelles lignes ajoutées par l’utilisateur depuis la dernière exécution du scénario.


### Déclencheurs instantanés

Les déclencheurs instantanés permettent au service de notifier [!DNL Workfront Fusion] à propos d’un *change* immédiatement. Nous vous recommandons de planifier l’exécution immédiate d’un scénario contenant un déclencheur instantané. Pour obtenir des instructions, voir [Planification d’un scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Voir aussi [Déclencheurs instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) pour plus d’informations sur la gestion des données entrantes.

>[!INFO]
>
>**Exemples:**
>
>* **[!DNL Workfront]> [!UICONTROL Événements de contrôle]** renvoie des informations lorsqu’un certain type d’événement se produit dans Workfront, comme la création d’une tâche.
>* **[!DNL Google Sheets]> [!UICONTROL Watch Changes]** renvoie des informations chaque fois qu’une cellule est mise à jour.


## Agrégateurs

Un agrégateur est un type de module qui accumule plusieurs lots en un seul lot.

Chaque agrégateur ne renvoie qu’un seul lot, qui est ensuite transmis au module suivant pour un traitement ultérieur.

Vous pouvez placer les agrégateurs uniquement au milieu d’un scénario.

Les scénarios peuvent contenir un nombre illimité d’agrégateurs.

>[!INFO]
>
>**Exemples:**
>
>* **[!UICONTROL Archiver] > [!UICONTROL Création d’une archive]** compresse les fichiers reçus dans une archive zip
>* **[!UICONTROL CSV] > [!UICONTROL Agrégat au format CSV]** fusionne plusieurs chaînes d’un fichier CSV en une seule ligne ;
>* **[!UICONTROL Outils] > [!UICONTROL Agrégateur de texte]** combine plusieurs chaînes en une seule chaîne


Pour plus d’informations, voir [Module d’agrégation dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Itérateurs

Un itérateur est un type de module qui divise les tableaux en plusieurs lots distincts.

Chaque itérateur renvoie un ou plusieurs lots, qui sont ensuite transmis au module suivant pour le traitement.

Vous pouvez placer les itérateurs uniquement au milieu d’un scénario.

Les scénarios peuvent contenir un nombre illimité d’itérateurs.

>[!INFO]
>
>**Exemple:**
>
>**[!UICONTROL Email] > [!UICONTROL Récupération des pièces jointes]** interrompt un tableau de pièces jointes en lots distincts ;

Pour plus d’informations, voir [Module d’itérateur dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) et [Mappage d’un tableau dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
