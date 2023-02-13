---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Afficher le total des heures sur la feuille de temps
description: Vous pouvez afficher le nombre total d’heures sur votre feuille de temps. Le nombre total d’heures de la feuille de temps inclut les heures consignées pour les projets, les tâches, les problèmes et toutes les heures générales.
author: Alina
feature: Timesheets
exl-id: ff0823f2-61d0-453f-ae1c-68f0f1465d73
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

# Afficher le total des heures sur la feuille de temps

Vous pouvez afficher le nombre total d’heures sur votre feuille de temps. Le nombre total d’heures de la feuille de temps inclut les heures consignées pour les projets, les tâches, les problèmes et toutes les heures générales.

Le nombre total d’heures correspond aux heures envoyées par le biais de la feuille de temps, de la zone Mises à jour ou de la zone Heures pour les projets, tâches ou problèmes.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Vérifier </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Afficher l’accès ou une version ultérieure à Tâches et problèmes</p> <p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures pour les tâches et les problèmes</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Afficher le nombre total d’heures d’une feuille de temps dans l’en-tête de la feuille de temps

Vous pouvez afficher le nombre total d’heures d’une feuille de temps dans l’en-tête de la feuille de temps.

![](assets/timesheet-total-hours-in-header-highlighted-redesigned.png)

## Afficher le total des heures sur votre feuille de temps dans une liste de feuilles de temps

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Feuilles de temps**. Le **Tous** est sélectionné par défaut et affiche toutes les feuilles de temps auxquelles vous avez accès.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facultatif) Pour mettre à jour le filtre dans la liste des feuilles de temps, effectuez l’une des opérations suivantes :

   * Sélectionner **Mes approbations de la feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous approuvez

      Ou

      Sélectionner **Mes feuilles de calcul** pour afficher uniquement vos feuilles de temps.

      Cela applique les filtres Mes approbations de feuille de temps ou Ma feuille de temps à la liste des feuilles de temps.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Cliquez sur l’icône Filtrer ![](assets/filter-nwepng.png) pour appliquer un autre filtre ou en créer un nouveau. Pour plus d’informations sur la création ou la mise à jour de filtres, voir [Création ou modification de filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Les options Mes approbations de feuille de temps et Mes feuilles de temps ne s’affichent pas en haut de la liste de feuille de temps ni dans la liste des filtres si votre administrateur Workfront ou un administrateur de groupe a supprimé les filtres Mes approbations de feuille de temps et Mes feuilles de temps des commandes de liste de la zone Configuration ou de votre modèle de mise en page. Pour plus d’informations, voir les articles suivants :
   * [Personnalisation des filtres, des vues et des groupes à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Facultatif) Cliquez sur le **Affichage** ![](assets/view-icon.png) ou **Regroupement** ![](assets/grouping.png) pour appliquer une autre vue ou un autre groupement ou en créer une nouvelle.

   Pour plus d’informations sur la création de filtres, de vues ou de regroupements, consultez les articles suivants :

   * [Création ou modification de filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Création ou modification de vues dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Création de groupes dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Le nombre total d’heures pour chaque feuille de temps s’affiche dans la variable **Nombre total d’heures** colonne .

   ![](assets/total-hours-column-highlighted-all-timesheets-list-nwe-350x120.png)

   >[!TIP]
   Lors de l’utilisation de la vue Standard pour une liste de feuilles de temps, la colonne Heures totales s’affiche en rouge si la durée consignée pour les éléments de la feuille de temps dépasse le nombre d’heures pendant la période de la feuille de temps. Pour plus d’informations, voir le champ &quot;Nombre total d’heures&quot; dans [Glossaire de la terminologie Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
