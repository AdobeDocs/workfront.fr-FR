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
ht-degree: 100%

---

# Créer une feuille de temps à usage unique

Vous pouvez créer manuellement une feuille de temps à usage unique si vous souhaitez qu’elle ne soit pas récurrente. Lorsque la date de fin de la feuille de temps est atteinte et que vous avez besoin d’autres feuilles de temps, vous devez en créer de nouvelles.

Pour plus d’informations sur la création d’un profil de feuille de temps qui génère des feuilles de temps récurrentes pour vos utilisateurs et utilisatrices sans intervention de votre part (recommandé), voir [Créer, modifier et affecter des profils de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

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
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Vous devez disposer d’un accès administratif aux feuilles de temps. </p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones</a>.</p> <p><b> NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Créer une feuille de temps à usage unique

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Feuilles de temps**. Le filtre **Tous** est sélectionné par défaut. Cela permet d’afficher toutes les feuilles de temps auxquelles vous avez accès.

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
   >   * [Personnaliser des filtres, des vues et des regroupements à l’aide d’un modèle de disposition](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Facultatif) Cliquez sur l’icône **Rechercher** ![](assets/search-icon.png) pour saisir un mot-clé et rechercher une feuille de temps spécifique. Par exemple, vous pouvez rechercher une période de feuille de temps avec le nom du ou de la propriétaire.

1. (Facultatif) Cliquez sur les icônes **Vue** ![](assets/view-icon.png) ou **Regroupement** ![](assets/grouping.png) pour appliquer une autre vue ou un autre regroupement ou en créer de nouveaux.

   Pour plus d’informations sur la création de filtres, de vues ou de regroupements, voir les articles suivants :

   * [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Créer ou modifier des vues dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Créer des regroupements dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Cliquez sur **Nouvelle feuille de temps** en haut de la liste des feuilles de temps.

   Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Créer une feuille de temps pour</strong> </td> 
      <td>Commencez à saisir le nom de l’utilisateur ou de l’utilisatrice, une fonction ou une équipe pour lesquels vous créez la feuille de temps, puis cliquez dessus lorsqu’ils s’affichent dans la liste.</td> 
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
      <td role="rowheader"><strong>Approbateurs ou approbatrices</strong> </td> 
      <td>Les approbateurs et approbatrices sont des utilisateurs et utilisatrices qui approuvent la feuille de temps pour les utilisateurs et utilisatrices associés à la feuille de temps. Seules les personnes disposant de droits d’administration sur les feuilles de temps peuvent être définies comme approbateurs ou approbatrices. Pour plus d’informations sur les droits d’administration des feuilles de temps, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones</a>.<br>Commencez à saisir les noms des approbateurs et des approbatrices de la feuille de temps et cliquez dessus lorsqu’ils apparaissent dans la liste.<br>Vous pouvez avoir plusieurs approbateurs et approbatrices pour une feuille de temps. Dans ce cas, une fois que l’un des approbateurs ou l’une des approbatrices a approuvé la feuille de temps, celle-ci est marquée comme <strong>Fermée</strong> et disparaît de la liste des approbations de tous les autres approbateurs et approbatrices.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Peut modifier l’heure</strong> </td>

   <td> <p>Sélectionnez cette option si vous souhaitez permettre aux approbateurs et approbatrices de modifier les heures de la feuille de temps.</p>

   Cette option fonctionne avec le paramètre **Restreindre la modification des feuilles de temps aux personnes propriétaires et à l’équipe d’administration** dans la zone Configuration > Feuille de temps et heures > Préférences. Pour plus d’informations, voir <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurer les préférences en matière de feuilles de temps et d’heures</a>.

   Les scénarios suivants sont possibles :

   <ul>
      <li>Lorsque l’option <b>Restreindre la modification des feuilles de temps aux personnes propriétaires et à l’équipe d’administration</b> est activée :</li>
   <ul><li>Les approbateurs et approbatrices peuvent uniquement approuver et rejeter les feuilles de temps, que l’option <b>Peut modifier l’heure</b> soit activée ou non. </li>
   <li>Les personnes responsables des personnes propriétaires de feuilles de temps peuvent consulter uniquement les feuilles de temps de leurs personnes subordonnées directes.</li></ul>
   <li>Lorsque l’option <b>Restreindre la modification des feuilles de temps aux personnes propriétaires et à l’équipe d’administration</b> est désactivée :</li>
   <ul><li>Lorsque l’option <b>Peut modifier l’heure</b> est activée, les approbateurs et approbatrices peuvent soumettre, rouvrir ou fermer la feuille de temps et modifier les heures.</li>
   <li>Lorsque l’option <b>Peut modifier l’heure</b> est désactivée, les approbateurs et approbatrices ne peuvent pas soumettre, rouvrir ou fermer la feuille de temps et ne peuvent pas modifier les heures. Les approbateurs et approbatrices ne peuvent qu’approuver ou rejeter la feuille de temps. </li>
   <li>Les personnes responsables des personnes propriétaires de feuilles de temps peuvent soumettre, rappeler, rouvrir et modifier les feuilles de temps de leurs personnes subordonnées directes.</li></ul>
   </ul>

   <p><b>NOTE</b>

   Une fois que vous avez soumis une feuille de temps pour approbation, vous ne pouvez plus modifier les heures. Pour remettre une feuille de temps soumise à l’état modifiable, rappelez la feuille de temps ou demandez à l’approbateur ou à l’approbatrice de rejeter la feuille de temps. Pour plus d’informations, voir <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Soumettre une feuille de temps pour approbation</a> et <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approuver une feuille de temps</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Heures supplémentaires</span> </td> 
      <td>Vous pouvez choisir de masquer la zone Heures supplémentaires sur la feuille de temps. Cette option est désactivée par défaut.</td> 
      </tr> 
      </tbody> 
   </table>

1. Cliquez sur **Créer une feuille de temps**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Lorsque des tâches et des problèmes apparaissent sur les feuilles de temps des utilisateurs et utilisatrices

Une tâche ou un problème attribué à un utilisateur ou à une utilisatrice apparaît automatiquement sur sa feuille de temps si la tâche ou le problème répond à l’un des critères suivants :

* L’utilisateur ou l’utilisatrice a consigné des heures dans la tâche ou le problème.
* Les dates prévues de la tâche ou du problème sont comprises dans les dates de la feuille de temps.
* La tâche ou le problème a une date de début effectif (le statut de la tâche ou du problème est En cours).
* La tâche ou le problème est épinglé à la feuille de temps.
* La date d’achèvement prévue est comprise dans la période de la feuille de temps et le statut est En cours.

Si les préférences de **Préremplir les feuilles de temps avec...** (situées dans les préférences en matière de feuilles de temps et d’heures) sont désélectionnées, la feuille de temps affiche les problèmes et les tâches dont le statut est En cours. Pour plus d’informations sur les préférences en matière de feuilles de temps et d’heures, voir [Configurer les préférences en matière de feuilles de temps et d’heures](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
