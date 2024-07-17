---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Créer une feuille de temps à usage unique
description: Vous pouvez créer manuellement une feuille de temps à usage unique si vous souhaitez qu’elle ne soit pas récurrente. Lorsque la date de fin de la feuille de temps est atteinte et que vous avez besoin d’autres feuilles de temps, vous devez en créer de nouvelles.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 13%

---

# Créer une feuille de temps à usage unique

Vous pouvez créer manuellement une feuille de temps à usage unique si vous souhaitez qu’elle ne soit pas récurrente. Lorsque la date de fin de la feuille de temps est atteinte et que vous avez besoin d’autres feuilles de temps, vous devez en créer de nouvelles.

Pour plus d’informations sur la création d’un profil de feuille de temps qui génère des feuilles de temps récurrentes pour vos utilisateurs sans intervention de votre part (recommandé), voir [Créer, modifier et affecter des profils de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* Il n’est pas possible de créer des feuilles de temps à usage unique pour les groupes.
>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Lors de la création d’une feuille de temps à usage unique, vous ne pouvez pas sélectionner de types d’heures généraux spécifiques à inclure dans votre feuille de temps. Tous les types d’heures généraux activés dans votre système s’affichent dans les feuilles de temps créées manuellement.
>
>  Si vous souhaitez sélectionner uniquement certains types d’heures généraux à afficher dans vos feuilles de temps, utilisez un profil de feuille de temps. Pour plus d’informations sur les profils de feuille de temps, voir [Créer, modifier et affecter des profils de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
>

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Vous devez disposer d’un accès administratif aux feuilles de calcul. </p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder aux utilisateurs et aux utilisatrices un accès administratif à certaines zones</a>.</p> <p><b> NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Créer une feuille de temps à usage unique

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Feuilles de temps**. Le filtre **Tous** est sélectionné par défaut. Cette option affiche toutes les feuilles de temps auxquelles vous avez accès.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facultatif) Pour mettre à jour le filtre dans la liste des feuilles de temps, effectuez l’une des opérations suivantes :

   * Sélectionnez **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous approuvez.

     Ou

     Sélectionnez **Mes feuilles de calcul** pour n’afficher que vos feuilles de calcul.

     Cela applique les filtres Mes approbations de feuille de temps ou Ma feuille de temps à la liste des feuilles de temps.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Cliquez sur l’icône Filtrer ![](assets/filter-nwepng.png) pour appliquer un autre filtre ou en créer un nouveau. Pour plus d’informations sur la création ou la mise à jour de filtres, voir [Création ou modification de filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Les options Mes approbations de feuille de temps et Mes feuilles de temps ne s’affichent pas en haut de la liste de feuille de temps ni dans la liste des filtres si votre administrateur Workfront ou un administrateur de groupe a supprimé les filtres Mes approbations de feuille de temps et Mes feuilles de temps des commandes de liste de la zone Configuration ou de votre modèle de mise en page. Pour plus d’informations, voir les articles suivants :
   > 
   >   * [Personnaliser les filtres, les vues et les regroupements à l’aide d’un modèle de disposition](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Facultatif) Cliquez sur l’icône **Rechercher** ![](assets/search-icon.png) pour saisir un mot-clé et rechercher une feuille de temps spécifique. Par exemple, vous pouvez rechercher une période de feuille de temps du nom du propriétaire.

1. (Facultatif) Cliquez sur les icônes **View** ![](assets/view-icon.png) ou **Grouping** ![](assets/grouping.png) pour appliquer une autre vue ou un autre regroupement ou en créer un nouveau.

   Pour plus d’informations sur la création de filtres, de vues ou de regroupements, consultez les articles suivants :

   * [Création ou modification de filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Créer ou modifier des vues dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Créer des regroupements dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Cliquez sur **Nouvelle feuille de temps** en haut de la liste des feuilles de temps.

   Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Créer une feuille de temps pour</strong> </td> 
      <td>Saisissez le nom de l’utilisateur, un rôle de tâche ou une équipe pour laquelle vous créez la feuille de temps, puis cliquez dessus lorsqu’il s’affiche dans la liste.</td> 
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
      <td role="rowheader"><strong>Approbateurs</strong> </td> 
      <td>Les approbateurs sont des utilisateurs qui approuvent la feuille de temps pour les utilisateurs associés à la feuille de temps. Seuls les utilisateurs disposant de droits d’administration pour la feuille de temps peuvent être définis comme approbateurs. Pour plus d'informations sur les droits d'administration de la feuille de temps, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs d'un accès administratif à certaines zones</a>.<br>Commencez à saisir les noms des approbateurs de la feuille de temps et cliquez dessus lorsqu’ils apparaissent dans la liste.<br>Vous pouvez avoir plusieurs approbateurs sur une feuille de temps. Dans ce cas, une fois que l’un des approbateurs a approuvé la feuille de temps, celle-ci est marquée comme <strong>Fermée</strong> et disparaît de la liste des approbations de la feuille de temps de tous les approbateurs restants.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Peut modifier l’heure</strong> </td>

   <td> <p>Sélectionnez cette option si vous souhaitez autoriser les approbateurs à modifier les heures sur la feuille de temps.</p>

   Cette option fonctionne avec le paramètre **Limiter la modification de la feuille de temps aux propriétaires et aux administrateurs** dans la zone Configuration > Frise chronologique et heures > Préférences . Pour plus d’informations, consultez <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurer les préférences de feuilles de temps et d’heures</a>.

   Les scénarios suivants sont possibles :

   <ul>
      <li>Lorsque l’option <b>Restreindre l’édition de la feuille de temps aux propriétaires et aux administrateurs</b> est activée :</li>
   <ul><li>Les approbateurs ne peuvent approuver et rejeter que la feuille de temps, que l’option <b>Possibilité de modifier l’heure</b> soit activée ou non. </li>
   <li>Les gestionnaires des propriétaires de feuilles de calcul peuvent uniquement afficher les feuilles de temps de leurs rapports directs.</li></ul>
   <li>Lorsque l'option <b>Restreindre l'édition de la feuille de temps aux propriétaires et aux administrateurs</b> est désactivée :</li>
   <ul><li>Lorsque l’option <b>Peut modifier l’heure</b> est activée, les approbateurs peuvent envoyer, rouvrir ou fermer la feuille de temps et peuvent modifier l’heure.</li>
   <li>Lorsque l’option <b> Peut modifier l’heure</b> est désactivée, les approbateurs ne peuvent pas envoyer, rouvrir ou fermer la feuille de temps et ne peuvent pas modifier l’heure. Les approbateurs peuvent uniquement approuver ou rejeter la feuille de temps. </li>
   <li>Les gestionnaires des propriétaires de feuilles de calcul peuvent envoyer, révoquer, rouvrir et modifier les feuilles de temps de leurs rapports directs.</li></ul>
   </ul>

   <p><b>NOTE</b>

   Une fois que vous avez soumis une feuille de temps pour approbation, vous ne pouvez plus modifier les heures. Pour renvoyer une feuille de temps envoyée à un état modifiable, rappelez-la ou demandez à l’approbateur de rejeter la feuille de temps. Pour plus d’informations, voir <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Envoyer une feuille de temps pour approbation</a> et <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approuver une feuille de temps</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Overtime</span> </td> 
      <td>Vous pouvez choisir de masquer la zone Heures supplémentaires sur la feuille de temps. Cette option est désactivée par défaut.</td> 
      </tr> 
      </tbody> 
   </table>

1. Cliquez sur **Créer une feuille de temps**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Lorsque des tâches et des problèmes apparaissent sur les feuilles de temps des utilisateurs

Une tâche ou un problème assigné à un utilisateur apparaît automatiquement sur la feuille de temps d’un utilisateur si la tâche ou le problème répond à l’un des critères suivants :

* L’utilisateur a consigné des heures sur la tâche ou le problème.
* Les dates prévues de la tâche ou du problème se situent dans les dates de la feuille de temps.
* La tâche ou le problème a une Date de début réelle (la tâche ou le statut du problème est En cours)
* La tâche ou le problème est épinglé dans la feuille de temps
* La date d’achèvement prévue se situe dans la plage de dates de la feuille de temps et l’état est En cours .

Si les **Fiches horaires préremplies avec les préférences ...** (situées dans les préférences Fiches horaires et Heure) sont désélectionnées, la feuille de temps affiche les problèmes et les tâches dont l’état est En cours. Pour plus d’informations sur les préférences de la feuille de temps et de l’heure, voir [ Configuration des préférences de la feuille de temps et de l’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
