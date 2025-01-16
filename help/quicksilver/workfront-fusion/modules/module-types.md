---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Types de modules
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 92%

---

# Types de modules

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Présentation du module](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/module-overview.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

[!UICONTROL Adobe Workfront Fusion] distingue cinq types de modules : modules d’action, modules de recherche, modules de déclenchement, agrégateurs et itérateurs. Les agrégateurs et les itérateurs sont destinés à des scénarios avancés.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter Adobe Workfront Fusion ainsi qu’Adobe Workfront pour utiliser les fonctionnalités décrites dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Modules d’action

Les modules d’action sont le type de module le plus courant. Un module d’action type renvoie un lot unique, qui est ensuite transmis au module suivant pour traitement.

Contrairement aux modules de déclenchement, les modules d’action peuvent être placés au début, au milieu ou à la fin d’un scénario. Les scénarios peuvent contenir un nombre illimité de modules d’action.

>[!INFO]
>
>**Exemples :**
>
>* **[!DNL Workfront]> [!UICONTROL Charger un fichier]** envoie un fichier à [!DNL Workfront] et renvoie son identifiant.
>* **[!UICONTROL Image] > [!UICONTROL Redimensionner]** reçoit une image, la redimensionne selon les dimensions spécifiées et la transmet à l’action suivante.

Le type d’action comporte quatre sous-types : Créer, Lire, Mettre à jour et Supprimer. Le sous-type Mise à jour permet les trois opérations suivantes :

* **Effacer le contenu d’un champ**. Cette opération se produit lorsque le contenu du champ est évalué pour effacer un mot-clé (à ne pas confondre avec *vide*).

  ![](assets/erase-content-of-field.png)

* **Ne pas modifier le contenu d’un champ**. Cette opération se produit lorsque le champ est vide ou que le contenu du champ est évalué sur vide (représenté par une valeur nulle dans JSON).

  ![](assets/leave-content-field-unchanged-350x231.png)

* **Remplacer le contenu d’un champ**. Cette opération a lieu dans tous les autres cas que les deux décrits ci-dessus.

>[!NOTE]
>
>* Si vous ne voyez pas le mot-clé `erase` dans le panneau de mappage, le module n’est pas un module de mise à jour ou il n’a pas été mis à jour selon les dernières spécifications de l’application.
>* « [!UICONTROL Vide] » ne modifie pas le contenu du champ. S’il est nécessaire d’effacer le champ, vous pouvez utiliser la formule suivante :
>
>![](assets/formula-ifempty-name-erase.png)
>
>Il n’est actuellement pas possible de laisser un champ inchangé lorsque son contenu est évalué comme vide.

## Modules de recherche

Une recherche typique renvoie zéro, un ou plusieurs paquets, qui sont ensuite transmis au module suivant pour traitement.

Vous pouvez placer des recherches au début, au milieu ou à la fin d’un scénario.

Les scénarios peuvent contenir un nombre illimité de recherches.

>[!INFO]
>
>**Exemple :**
>
>**[!DNL Workfront]> [!UICONTROL Lire les enregistrements associés]** lit les enregistrements qui correspondent à la requête de recherche que vous avez spécifiée, dans un objet parent particulier.

## Modules déclencheurs

Les déclencheurs génèrent des lots lorsqu’il y a eu un changement dans un service donné. La modification peut consister en la création d’enregistrements, la suppression d’un enregistrement, la mise à jour d’un enregistrement, etc.

Chaque déclencheur peut renvoyer zéro, un ou plusieurs paquets qui sont ensuite transmis au module suivant pour traitement.

Les déclencheurs ne peuvent être placés qu’au début d’un scénario.

Chaque scénario ne peut contenir qu’un seul déclencheur.

[!DNL Workfront Fusion] fait la distinction entre deux types de déclencheurs : les déclencheurs d’attente active et les déclencheurs instantanés.

### Déclencheurs d’attente active

Les déclencheurs d’attente active interrogent régulièrement un service donné, même s’il n’y a pas eu de changement depuis leur dernière exécution. Nous vous recommandons de planifier l’exécution d’un scénario contenant un déclencheur d’attente active à intervalles réguliers. En cas de *changement*, le déclencheur renvoie des lots contenant des informations sur la modification. S’il n’y a pas de *changement*, le déclencheur ne renvoie aucun lot. Pour obtenir des instructions sur la planification d’un scénario, voir [Planifier un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Les déclencheurs d’attente active vous permettent de sélectionner le premier lot qu’ils doivent renvoyer via le panneau d’époque. Le panneau s’affiche automatiquement après l’enregistrement d’un déclencheur ou la modification de ses paramètres. Pour plus d’informations, voir [Choisir où commence un module déclencheur dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>Les réglages effectués dans le panneau d’époque n’affectent que la première exécution du module. Une fois le module exécuté, il se souvient du dernier lot renvoyé et annule les réglages effectués via le panneau d’époque.

>[!INFO]
>
>**Exemples :**
>
>* **[!DNL Workfront]> [!UICONTROL Surveiller les enregistrements]** renvoie les fichiers qui ont été ajoutés depuis la dernière exécution du scénario.
>
>* **[!DNL Google Sheets]> [!UICONTROL Surveiller les lignes]** renvoie les nouvelles lignes ajoutées par l’utilisateur ou utilisatrice depuis la dernière exécution du scénario.

### Déclencheurs instantanés

Les déclencheurs instantanés permettent au service d’informer immédiatement [!DNL Workfront Fusion] d’un *changement*. Nous vous recommandons de planifier l’exécution immédiate d’un scénario contenant un déclencheur instantané. Pour obtenir des instructions, voir [Planifier un scénario dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Voir également [Déclencheurs instantanés (webhooks) dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) pour plus de détails sur le traitement des données entrantes.

>[!INFO]
>
>**Exemples :**
>
>* **[!DNL Workfront]> [!UICONTROL Surveiller les événements]** renvoie des informations lorsqu’un certain type d’événement se produit dans Workfront, comme la création d’une tâche.
>* **[!DNL Google Sheets]> [!UICONTROL Surveiller les modifications]** renvoie des informations chaque fois qu’une cellule est mise à jour.

## Agrégateurs

Un agrégateur est un type de module qui rassemble plusieurs lots en un seul.

Chaque agrégateur ne renvoie qu’un seul lot, qui est ensuite transmis au module suivant pour traitement.

Vous ne pouvez placer des agrégateurs qu’au milieu d’un scénario.

Les scénarios peuvent contenir un nombre illimité d’agrégateurs.

>[!INFO]
>
>**Exemples :**
>
>* **[!UICONTROL Archive] > [!UICONTROL Créer une archive]** compresse les fichiers reçus dans une archive ZIP.
>* **[!UICONTROL CSV] > [!UICONTROL Agréger en CSV]** fusionne plusieurs chaînes d’un fichier CSV en une seule ligne.
>* **[!UICONTROL Outils] > [!UICONTROL Agrégateur de texte]** combine plusieurs chaînes de caractères en une seule.

Pour plus d’informations, voir [Module agrégateur dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Itérateurs

Un itérateur est un type de module qui divise les tableaux en plusieurs lots distincts.

Chaque itérateur renvoie un ou plusieurs lots, qui sont ensuite transmis au module suivant pour traitement.

Vous ne pouvez placer des itérateurs qu’au milieu d’un scénario.

Les scénarios peuvent contenir un nombre illimité d’itérateurs.

>[!INFO]
>
>**Exemple :**
>
>**[!UICONTROL E-mail] > [!UICONTROL Récupérer les pièces jointes]** divise un ensemble de pièces jointes en lots distincts.

Pour plus d’informations, voir [Module itérateur dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) et [Mapper un tableau dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
