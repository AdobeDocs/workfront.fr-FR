---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Types de modules
description: '"Adobe Workfront Fusion" distingue cinq types de modules : modules d’action, modules de recherche, modules de déclenchement, agrégateurs et itérateurs. Les agrégateurs et les itérateurs sont destinés à des scénarios avancés."'
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 6%

---

# Types de modules

Une [!UICONTROL fusion Adobe Workfront] distingue cinq types de modules : modules d’action, modules de recherche, modules de déclenchement, agrégateurs et itérateurs. Les agrégateurs et les itérateurs sont destinés à des scénarios avancés.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter Adobe Workfront Fusion ainsi qu’Adobe Workfront pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Modules d&#39;action

Les modules d’action sont le type de module le plus courant. Un module d’action type renvoie un lot unique, qui est ensuite transmis au module suivant pour le traitement.

Contrairement aux modules de déclenchement, les modules d’action peuvent être placés au début, au milieu ou à la fin d’un scénario. Les scénarios peuvent contenir un nombre illimité de modules d’action.

>[!INFO]
>
>**Exemples :**
>
>* **[!DNL Workfront]> [!UICONTROL Télécharger un fichier]** envoie un fichier à [!DNL Workfront] et renvoie son identifiant.
>* **[!UICONTROL Image] > [!UICONTROL Redimensionner]** reçoit une image, la redimensionne selon des dimensions spécifiées et la transmet à l’action suivante.

Le type d’action comporte quatre sous-types : Créer, Lire, Mettre à jour et Supprimer. Le sous-type Mise à jour permet les trois opérations suivantes :

* **Effacez le contenu d’un champ**. Cette opération se produit lorsque le contenu du champ est évalué pour effacer le mot-clé (à ne pas confondre avec *vide*).

  ![](assets/erase-content-of-field.png)

* **Laissez le contenu d’un champ inchangé**. Cette opération se produit lorsque le champ est vide ou que le contenu du champ est évalué sur vide (représenté par une valeur nulle dans JSON).

  ![](assets/leave-content-field-unchanged-350x231.png)

* **Remplacez le contenu d’un champ**. Cette opération a lieu dans tous les autres cas que les deux décrits ci-dessus.

>[!NOTE]
>
>* Si vous ne voyez pas le mot-clé `erase` dans le panneau de mappage, le module n’est pas un module de mise à jour ou il n’a pas été mis à jour selon les dernières spécifications de l’application.
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
>**Exemple :**
>
>**[!DNL Workfront]> [!UICONTROL Lire les enregistrements associés]** lit les enregistrements qui correspondent à la requête de recherche que vous spécifiez, dans un objet parent particulier

## Modules déclencheurs

Les déclencheurs génèrent des lots lorsqu’un service donné a été modifié. La modification peut être la création de nouveaux enregistrements, la suppression d’un enregistrement, la mise à jour d’un enregistrement, etc.

Chaque déclencheur peut renvoyer zéro, un ou plusieurs lots qui sont ensuite transmis au module suivant pour traitement.

Les déclencheurs ne peuvent être placés qu&#39;au début d&#39;un scénario.

Chaque scénario ne peut contenir qu’un seul déclencheur.

[!DNL Workfront Fusion] fait la distinction entre deux types de déclencheurs : les déclencheurs d’interrogation et les déclencheurs instantanés.

### Déclencheurs d’interrogation

Les déclencheurs d’interrogation interrogent régulièrement un service donné même s’il n’y a eu aucune modification depuis leur exécution précédente. Nous vous recommandons de planifier l’exécution à intervalles réguliers d’un scénario contenant un déclencheur d’interrogation. S’il existe un *changement*, le déclencheur renvoie des lots contenant des informations sur la modification. S’il n’existe aucun *changement*, le déclencheur ne génère aucun lot. Pour plus d&#39;informations sur la planification d&#39;un scénario, voir [Planification d&#39;un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Les déclencheurs d’interrogation vous permettent de sélectionner le premier lot qu’ils doivent générer à partir du panneau d’époque. Le panneau s’affiche automatiquement après l’enregistrement ou la modification des paramètres du déclencheur. Pour plus d’informations, voir [Choix de l’endroit où commence un module de déclenchement dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>Les paramètres définis dans le panneau Epoque n’affectent que la première exécution du module. Une fois le module exécuté, il mémorise le dernier lot sorti et vide les paramètres effectués via le panneau d’époque.

>[!INFO]
>
>**Exemples :**
>
>* **[!DNL Workfront]> [!UICONTROL Surveiller les enregistrements]** renvoie les fichiers qui ont été ajoutés depuis la dernière exécution du scénario.
>
>* **[!DNL Google Sheets]> [!UICONTROL Regarder les lignes]** renvoie de nouvelles lignes ajoutées par l’utilisateur depuis la dernière exécution du scénario.

### Déclencheurs instantanés

Les déclencheurs instantanés permettent au service d&#39;informer immédiatement [!DNL Workfront Fusion] d&#39;un *changement*. Nous vous recommandons de planifier l’exécution immédiate d’un scénario contenant un déclencheur instantané. Pour obtenir des instructions, reportez-vous à la section [Planification d’un scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Voir aussi [Triggers instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) pour plus d’informations sur la façon dont les données entrantes sont traitées.

>[!INFO]
>
>**Exemples :**
>
>* **[!DNL Workfront]> [!UICONTROL Surveiller les événements]** renvoie des informations lorsqu’un certain type d’événement se produit dans Workfront, comme la création d’une tâche.
>* **[!DNL Google Sheets]> [!UICONTROL Watch Changes]** renvoie des informations chaque fois qu’une cellule est mise à jour.

## Agrégateurs

Un agrégateur est un type de module qui accumule plusieurs lots en un seul lot.

Chaque agrégateur ne renvoie qu’un seul lot, qui est ensuite transmis au module suivant pour un traitement ultérieur.

Vous pouvez placer les agrégateurs uniquement au milieu d’un scénario.

Les scénarios peuvent contenir un nombre illimité d’agrégateurs.

>[!INFO]
>
>**Exemples :**
>
>* **[!UICONTROL Archive] > [!UICONTROL Créer une archive]** compresse les fichiers reçus dans une archive zip.
>* **[!UICONTROL CSV] > [!UICONTROL Agrégat en CSV]** fusionne plusieurs chaînes d’un fichier CSV en une seule ligne.
>* **[!UICONTROL Outils] > [!UICONTROL Agrégateur de texte]** combine plusieurs chaînes en une seule chaîne.

Pour plus d’informations, voir [Module d’agrégation dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Itérateurs

Un itérateur est un type de module qui divise les tableaux en plusieurs lots distincts.

Chaque itérateur renvoie un ou plusieurs lots, qui sont ensuite transmis au module suivant pour le traitement.

Vous pouvez placer les itérateurs uniquement au milieu d’un scénario.

Les scénarios peuvent contenir un nombre illimité d’itérateurs.

>[!INFO]
>
>**Exemple :**
>
>**[!UICONTROL Email] > [!UICONTROL Récupérer les pièces jointes]** interrompt un tableau de pièces jointes en lots distincts

Pour plus d’informations, voir [Module d’itérateur dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) et [Mappage d’un tableau dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
