---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Afficher le nombre total d’heures sur la feuille de temps
description: Vous pouvez afficher le nombre total d’heures sur votre feuille de temps. Le nombre total d’heures de la feuille de temps inclut les heures consignées pour les projets, les tâches, les problèmes et toutes les heures générales.
author: Alina
feature: Timesheets
exl-id: ff0823f2-61d0-453f-ae1c-68f0f1465d73
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 87%

---

# Afficher le nombre total d’heures sur la feuille de temps

<!--Audited: 8/2024-->

Vous pouvez afficher le nombre total d’heures sur votre feuille de temps. Le nombre total d’heures de la feuille de temps inclut les heures consignées pour les projets, les tâches, les problèmes et toutes les heures générales.

Le nombre total d’heures correspond aux heures envoyées par le biais de la feuille de temps, de la zone Mises à jour ou de la zone Heures pour les projets, tâches ou problèmes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Léger ou supérieur </p>
   <p>Actuel : révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Affichage ou accès supérieur aux tâches et aux problèmes</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures pour les tâches et les problèmes</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher le nombre total d’heures d’une feuille de temps dans l’en-tête de la feuille de temps

Vous pouvez afficher le nombre total d’heures d’une feuille de temps dans l’en-tête de la feuille de temps.

![](assets/timesheet-total-hours-in-header-highlighted-redesigned.png)

## Afficher le nombre total d’heures de votre feuille de temps dans une liste de feuilles de temps

{{step1-to-timesheets}}

La zone **Fiches horaires** s’ouvre.

![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facultatif) Pour mettre à jour le filtre dans la liste des feuilles de temps, effectuez l’une des opérations suivantes :

   * Sélectionnez **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous approuvez.

     Ou

     Sélectionnez **Mes feuilles de temps** pour afficher uniquement vos feuilles de temps.

     Cela applique les filtres Mes approbations de feuille de temps ou Mes feuilles de temps à la liste des feuilles de temps.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Cliquez sur l’icône Filtrer ![](assets/filter-nwepng.png) pour appliquer un autre filtre ou en créer un nouveau. Pour plus d’informations sur la création ou la mise à jour de filtres, voir [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Les options Mes approbations de feuille de temps et Mes feuilles de temps ne s’affichent pas en haut de la liste de feuille de temps ni dans la liste des filtres si votre administrateur ou admnistratrice ou un administrateur ou une administratrice de groupes Workfront a supprimé les filtres Mes approbations de feuille de temps et Mes feuilles de temps des contrôles de liste de la zone Configuration ou de votre modèle de disposition. Pour plus d’informations, voir les articles suivants :
   >
   >   
   >   
   >   * [Personnaliser des filtres, des vues et des regroupements à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Facultatif) Cliquez sur les icônes **Vue** ![](assets/view-icon.png) ou **Regroupement** ![](assets/grouping.png) pour appliquer une autre vue ou un autre regroupement ou en créer de nouveaux.

   Pour plus d’informations sur la création de filtres, de vues ou de regroupements, voir les articles suivants :

   * [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Créer ou modifier des vues dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Créer des regroupements dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Le nombre total d’heures pour chaque feuille de temps s’affiche dans la colonne **Nombre total d’heures**.

   ![](assets/total-hours-column-highlighted-all-timesheets-list-nwe-350x120.png)

   >[!TIP]
   >
   >Lors de l’utilisation de la vue Standard pour une liste de feuilles de temps, la colonne Heures totales s’affiche en rouge si la durée consignée pour les éléments de la feuille de temps dépasse le nombre d’heures pendant la période de la feuille de temps. Pour plus d’informations, voir le champ &quot;Nombre total d’heures&quot; dans le [Glossaire de la terminologie Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
