---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Modifier les informations de la feuille de temps
description: En tant qu’utilisateur disposant d’un accès administratif aux feuilles de calcul, vous pouvez modifier les informations relatives aux feuilles de calcul existantes dans Adobe Workfront . Vous pouvez par exemple modifier le propriétaire, les approbateurs ou la période de la feuille de temps.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 3a2745437e00ac968f2a4590be2637dbc01594ad
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 2%

---

# Modifier les informations de la feuille de temps

En tant qu’utilisateur disposant d’un accès administratif aux feuilles de calcul, vous pouvez modifier les informations relatives aux feuilles de calcul existantes dans Adobe Workfront . Vous pouvez par exemple modifier le propriétaire, les approbateurs ou la période de la feuille de temps.

Vous pouvez modifier les informations d’une seule feuille de temps ou modifier plusieurs feuilles de temps en bloc.

>[!IMPORTANT]
>
>Si les utilisateurs sont associés aux profils de feuille de temps et que les feuilles de temps sont générées automatiquement, les modifications que vous apportez aux feuilles de temps existantes ne se répercutent pas sur les feuilles de temps qui seront générées pour les dates futures. Les paramètres de toutes les feuilles de temps générées automatiquement sont définis dans les profils de la feuille de temps. Pour plus d’informations, voir [Création de profils de feuille de temps](../create-and-manage-timesheets/create-timesheet-profiles.md)


## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez disposer d’un accès administratif aux feuilles de calcul. </p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Modifier les feuilles de temps

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Feuilles de temps**.

   La variable **Tous** est sélectionné par défaut, ce qui affiche toutes les feuilles de temps que vous avez accès à la vue.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facultatif) Cliquez sur le **search** icon ![](assets/search-icon.png) et saisissez un mot-clé et recherchez une feuille de temps spécifique. Par exemple, vous pouvez rechercher une période de la feuille de temps ou le nom du propriétaire.

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
   >
   >   
   >   
   * [Personnalisation des filtres, des vues et des groupes à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Facultatif) Cliquez sur le **Affichage** ![](assets/view-icon.png) ou **Regroupement** ![](assets/grouping.png) pour appliquer une autre vue ou un autre groupement ou en créer une nouvelle.

   Pour plus d’informations sur la création de filtres, de vues ou de regroupements, consultez les articles suivants :

   * [Création ou modification de filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Création ou modification de vues dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Création de groupes dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Sélectionnez une ou plusieurs feuilles de temps, puis cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png) en haut de la liste des feuilles de temps.
1. Affichez ou spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Propriétaire</strong> </td> 
      <td> <p>Il s’agit du nom de l’utilisateur pour lequel la feuille de temps a été créée. Vous ne pouvez pas modifier ce champ. </p> <p>Le champ ne s’affiche pas lorsque vous sélectionnez plusieurs feuilles de temps. </p> </td> 
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
      <td> Il s’agit de l’état de la feuille de temps.
      Voici les options d’état possibles de la feuille de temps : 
      <ul><li><b>Ouvrir</b>: la feuille de temps est ouverte et les entrées d’heure peuvent être modifiées.</li>
      <li><b>Envoyé</b>: la feuille de temps est soumise à validation aux approbateurs désignés.</li>
      <li><b>Rejetés</b>: la feuille de temps n’a pas été approuvée par les approbateurs et est à nouveau disponible pour que l’utilisateur puisse modifier les entrées de temps.</li>
      <li><b>Fermé</b>: la feuille de temps est fermée par l’utilisateur ou validée par l’approbateur ; elle est donc maintenant fermée. Vous ne pouvez pas ajouter de temps à une feuille de temps fermée.</li>
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approbateurs</strong> </td> 
      <td> <p>Les approbateurs sont des utilisateurs qui approuvent la feuille de temps pour les utilisateurs associés à la feuille de temps. Seuls les utilisateurs disposant d’un accès administratif aux feuilles de calcul peuvent être définis comme approbateurs. </p> <p>Pour plus d’informations sur les droits d’administration de la feuille de temps, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> <p>Saisissez les noms des approbateurs de la feuille de temps et sélectionnez-les lorsqu’ils apparaissent dans la liste.</p> <p>Vous pouvez avoir plusieurs approbateurs sur une feuille de temps. Dans ce cas, une fois que l’un des approbateurs a approuvé la feuille de temps, celle-ci est marquée comme <strong>Fermé</strong> et il disparaît de la liste d’approbations de la feuille de temps de tous les approbateurs restants.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Peut modifier l’heure</strong> </td> 
      <td> <p>Sélectionnez cette option si vous souhaitez autoriser les approbateurs à modifier les heures sur la feuille de temps.</p> <p>Cette option n’est pas disponible lorsque vous sélectionnez plusieurs feuilles de temps. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Hrs supp</span> </td> 
      <td> <p>Vous pouvez choisir de masquer la zone Heures supplémentaires sur la feuille de temps.</p> <p>Cette option est désactivée par défaut.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.
