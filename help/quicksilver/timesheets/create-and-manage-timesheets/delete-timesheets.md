---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Supprimer des feuilles de temps dans Adobe Workfront
description: Les modifications apportées à un profil de feuille de temps ne sont pas immédiatement appliquées aux feuilles de temps existantes, tel que décrit dans la section « Créer, modifier et affecter des profils de feuille de temps ». Pour rendre visibles les modifications sur les feuilles de temps existantes, supprimez les feuilles de temps générées et créez-en de nouvelles. Ceci ne s’applique qu’aux feuilles de temps qui ont été générées en associant des profils de feuilles de temps à des utilisateurs et des utilisatrices.
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 100%

---

# Supprimer des feuilles de temps dans Adobe Workfront

Les modifications que vous apportez à un profil de feuille de temps ne s’appliquent pas immédiatement aux feuilles de temps existantes, comme expliqué dans la section [Créer, modifier et affecter des profils de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Pour rendre visibles les modifications sur les feuilles de temps existantes, supprimez les feuilles de temps générées et créez-en de nouvelles. Ceci ne s’applique qu’aux feuilles de temps qui ont été générées en associant des profils de feuilles de temps à des utilisateurs et des utilisatrices.

>[!NOTE]
>
>Les feuilles de temps créées manuellement ne peuvent pas être recréées en générant de nouveau les feuilles de temps, sauf si un profil de feuille de temps a été affecté aux utilisateurs et aux utilisatrices depuis que la feuille de temps a été créée manuellement. Supprimer une feuille de temps créée manuellement peut entraîner une perte de données. Pour plus d’informations sur la création d’une feuille de temps unique, consultez la section [Créer une feuille de temps à usage unique](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

Les équipes d’administration ou de groupes d’Adobe Workfront peuvent générer des feuilles de temps pour tous les personnes utilisant le système. Pour plus d’informations sur la génération manuelle de feuilles de temps, consultez la section :

* [Générer manuellement des feuilles de temps](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [Créer et gérer des profils de feuille de temps d’un groupe](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* Il est impossible de récupérer une feuille de temps supprimée.
>* Il est recommandé de ne pas supprimer les feuilles de temps antérieures, car elles ne sont pas générées automatiquement en fonction des profils de feuilles de temps. Si vous souhaitez que les modifications apportées à vos profils de feuilles de temps soient immédiatement visibles dans les nouvelles feuilles de temps, vous pouvez supprimer les feuilles de temps actuelles et futures, puis les créer manuellement.
>* Lorsque vous supprimez des feuilles de temps, les heures enregistrées pour les tâches, problèmes et projets ne sont pas supprimées. Seules les heures générales sont supprimées avec la feuille de temps. Dans un autre éditeur de texte, saisissez les heures générales associées à la feuille de temps. Une fois la feuille de temps supprimée, vous pouvez les consigner dans la nouvelle feuille de temps.
>

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Vous devez disposer d’un accès administratif aux feuilles de temps. </p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder aux utilisateurs et aux utilisatrices un accès administratif à certaines zones</a>.</p> <p>Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Supprimer des feuilles de temps dans une liste

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Feuilles de temps**. Le filtre **Tous** est appliqué par défaut et affiche toutes les feuilles de temps auxquelles vous avez accès.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facultatif) Pour mettre à jour le filtre dans la liste des feuilles de temps, effectuez l’une des opérations suivantes :

   * Sélectionnez **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous approuvez.

     Ou

     Sélectionnez **Mes feuilles de temps** pour afficher uniquement vos feuilles de temps.

     Cela applique à la liste des feuilles de temps les filtres « Mes approbations de feuille de temps » ou « Mes feuilles de temps ».

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Cliquez sur l’icône Filtre ![](assets/filter-nwepng.png) pour appliquer un autre filtre ou en créer un nouveau. Pour plus d’informations sur la création ou la mise à jour de filtres, voir [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Si l’équipe d’administration de Workfront ou de groupes a supprimé les filtres « Mes approbations de feuilles de temps » et « Mes feuilles de temps » des contrôles de liste de la zone de configuration ou de votre modèle de mise en page, les options correspondantes ne s’afficheront pas en haut de la liste des feuilles de temps ou dans la liste des filtres.Pour plus d’informations, consultez les articles suivants :
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

1. Sélectionnez une ou plusieurs feuilles de temps que vous souhaitez supprimer et cliquez sur l’icône **Supprimer** ![](assets/delete.png) en haut de la liste des feuilles de temps.

1. Cliquez sur **Supprimer**.

   Les feuilles de temps sélectionnées sont supprimées et ne peuvent pas être récupérées.

   Pour générer de nouvelles feuilles de temps, assurez-vous qu’un profil de feuille de temps a été affecté aux utilisaeurs et utilisatrices, puis demandez à l’équipe d’administration de Workfront ou de groupes de les générer.

   Pour plus d’informations, consultez les sections suivantes :

   * [Créer, modifier et affecter des profils de feuilles de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [Générer manuellement des feuilles de temps](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [Créer et gérer des profils de feuille de temps d’un groupe](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## Supprimer une feuille de temps à partir de la page des feuilles de temps

1. Cliquez sur l’icône [!UICONTROL **Menu principal**] ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.
1. Cliquez sur la feuille de temps que vous souhaitez supprimer pour l’ouvrir.
1. Cliquez sur l’icône [!UICONTROL **Plus**] ![](assets/more-icon.png) à droite du nom de la feuille de temps, puis cliquez sur **Supprimer**.

   ![Suppression d’une feuille de temps de la page des feuilles de temps](assets/delete-timesheet-from-timesheet-page.png)
1. Cliquez sur [!UICONTROL **Supprimer**] pour confirmer.

   La feuille de temps est supprimée et ne peut pas être récupérée.
