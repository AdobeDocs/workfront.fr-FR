---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Modifier les informations de la feuille de temps
description: Les utilisateurs disposant d’un accès administratif aux feuilles de temps peuvent modifier les informations des feuilles de temps existantes dans Adobe Workfront. Vous pouvez par exemple modifier la personne propriétaire, les approbateurs et approbatrices ou la période de la feuille de temps.
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 94%

---

# Modifier les informations de la feuille de temps

Les utilisateurs disposant d’un accès administratif aux feuilles de temps peuvent modifier les informations des feuilles de temps existantes dans Adobe Workfront. Vous pouvez par exemple modifier la personne propriétaire, les approbateurs et approbatrices ou la période de la feuille de temps.

Vous pouvez modifier les informations d’une seule feuille de temps ou modifier plusieurs feuilles de temps en masse.

>[!IMPORTANT]
>
>Si des utilisateurs et utilisatrices sont associés aux profils de feuille de temps et que les feuilles de temps sont générées automatiquement, les modifications que vous apportez aux feuilles de temps existantes ne se répercutent pas sur les feuilles de temps qui seront générées pour les dates futures. Les paramètres de toutes les feuilles de temps générées automatiquement sont définis dans les profils de feuille de temps. Pour plus d’informations, voir [Créer des profils de feuille de temps](../create-and-manage-timesheets/create-timesheet-profiles.md)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td><p>Accès administratif aux feuilles de temps</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier les feuilles de temps

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Feuilles de temps**.

   Le filtre **Tous** est sélectionné par défaut, ce qui affiche toutes les feuilles de temps que vous pouvez afficher.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facultatif) Cliquez sur l’icône de **recherche** ![](assets/search-icon.png), saisissez un mot-clé et recherchez une feuille de temps spécifique. Par exemple, vous pouvez rechercher une période de la feuille de temps ou le nom de la personne propriétaire.

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

1. (Facultatif) Cliquez sur les icônes **Vue** ![](assets/view-icon.png) ou **Regroupement** ![](assets/grouping.png) pour appliquer une autre vue ou un autre regroupement, ou en créer un nouveau ou une nouvelle.

   Pour plus d’informations sur la création de filtres, de vues ou de regroupements, voir les articles suivants :

   * [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Créer ou modifier des vues dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Créer des regroupements dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Sélectionnez une ou plusieurs feuilles de temps, puis cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) en haut de la liste des feuilles de temps.
1. Affichez ou spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Personne propriétaire</strong> </td> 
      <td> <p>Il s’agit du nom de la personne pour laquelle la feuille de temps a été créée.Vous ne pouvez pas modifier ce champ. </p> <p>Le champ ne s’affiche pas lorsque vous sélectionnez plusieurs feuilles de temps. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Date de début</strong> </td> 
      <td>Il s’agit de la date de début de la feuille de temps.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Date de fin</strong> </td> 
      <td> Il s’agit de la date de fin de la feuille de temps.</td> 
     </tr>
<tr> 
      <td role="rowheader"><strong>Statut</strong> </td> 
      <td> Il s’agit du statut de la feuille de temps.
      Voici les options de statut possibles de la feuille de temps : 
      <ul><li><b>Ouverte</b> : la feuille de temps est ouverte et les entrées d’heure peuvent être modifiées.</li>
      <li><b>Envoyée</b> : la feuille de temps est soumise pour approbation aux approbateurs et approbatrices désignés.</li>
      <li><b>Rejetée</b> : la feuille de temps n’a pas été approuvée par les approbateurs et approbatrices et est à nouveau disponible pour que l’utilisateur ou l’utilisatrice puisse modifier les entrées de temps.</li>
      <li><b>Fermée</b> : la feuille de temps est fermée par l’utilisateur ou l’utilisatrice,ou approuvée par l’approbateur ou l’approbatrice ; elle est donc maintenant fermée. Vous ne pouvez pas ajouter d’heures à une feuille de temps fermée.</li>
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approbateurs et approbatrices</strong> </td> 
      <td> <p>Les approbateurs et approbatrices sont des personnes qui approuvent la feuille de temps pour les utilisateurs et utilisatrices associés à la feuille de temps. Seuls les utilisateurs et utilisatrices disposant d’un accès administratif aux feuilles de temps peuvent être définis comme approbateurs et approbatrices. </p> <p>Pour plus d’informations sur les droits d’administration de la feuille de temps, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder un accès administratif à certaines zones aux utilisateurs et utilisatrices</a>.</p> <p>Commencez à saisir les noms des approbateurs et approbatrices de la feuille de temps et sélectionnez-les lorsqu’ils apparaissent dans la liste.</p> <p>Vous pouvez avoir plusieurs approbateurs et approbatrices pour une feuille de temps. Dans ce cas, une fois que l’un des approbateurs et approbatrices a approuvé la feuille de temps, celle-ci est marquée comme <strong>Fermée</strong> et elle disparaît de la liste des approbations de feuille de temps de tous les approbateurs et approbatrices restants.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Peut modifier l’heure</strong> </td> 
      <td> <p>Sélectionnez cette option si vous souhaitez permettre aux approbateurs et approbatrices de modifier les heures de la feuille de temps.</p> <p>Cette option n’est pas disponible lorsque vous sélectionnez plusieurs feuilles de temps. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Heures supplémentaires</span> </td> 
      <td> <p>Vous pouvez choisir de masquer la zone Heures supplémentaires sur la feuille de temps.</p> <p>Cette option est désactivée par défaut.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.
