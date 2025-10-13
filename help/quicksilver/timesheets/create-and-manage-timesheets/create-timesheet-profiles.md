---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Créer, modifier et attribuer des profils de feuilles de temps
description: Vous pouvez créer, modifier et attribuer des profils de feuilles de temps qui génèrent des feuilles de temps récurrentes pour les utilisateurs et utilisatrices sans autre intervention de votre part. Cela vous permet de gagner du temps et d’assurer la cohérence entre les utilisateurs et utilisatrices.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 395a7788ddfda71264b7b964953435affd7761e9
workflow-type: tm+mt
source-wordcount: '1597'
ht-degree: 68%

---

# Créer, modifier et attribuer des profils de feuilles de temps

<!--Audited: 06/2025-->

Vous pouvez créer, modifier et attribuer des profils de feuilles de temps qui génèrent des feuilles de temps récurrentes pour les utilisateurs et utilisatrices sans autre intervention de votre part. Vous gagnez ainsi du temps et vous vous assurez que les éléments suivants sont cohérents entre les utilisateurs et utilisatrices :

* Période de la feuille de temps
* Approbateurs
* Types d’heures généraux

Pour plus d’informations sur la création manuelle d’une feuille de temps, consultez l’article [Créer une feuille de temps à usage unique](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td> <p>Nouveau : Standard </p>
 <p>ou</p> 
<p>Actuel : formule </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez disposer d’un accès administratif aux feuilles de temps. </p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer ou modifier un profil de feuille de temps

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Pour activer les modifications du profil de feuille de temps dans les feuilles de temps actuelles, vous devez supprimer les feuilles de temps existantes avant d&#39;apporter les modifications aux profils des feuilles de temps, puis générer de nouvelles feuilles de temps. Pour plus d’informations, consultez les articles [Supprimer des feuilles de temps dans Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) et [Générer manuellement des feuilles de temps](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. Si vous créez ou modifiez un profil de feuille de temps à utiliser dans tout le système, cliquez sur **Feuille de temps et heures**.

   Ou

   Si vous créez ou modifiez un profil de feuille de temps pour un groupe, cliquez sur **Groupes**, puis sur le nom du groupe.

1. Cliquez sur **Profils de feuilles de temps**.
1. Pour créer un profil de feuille de temps, cliquez sur **Nouveau profil**.

   Ou

   Pour modifier un profil de feuille de temps existant, sélectionnez le profil de feuille de temps que vous souhaitez modifier, puis cliquez sur **Modifier**.

   La page de profil de feuille de temps nouvelle ou existante s’affiche.

1. Mettez à jour les informations suivantes :

   * **Nom** : ajoutez un nom pour le profil de feuille de temps. Il peut s’agir du nom d’une équipe ou d’un groupe dont les personnes partagent le même délai pour leurs feuilles de temps. Champ obligatoire.
   * **Description** : ajoutez des informations supplémentaires sur le profil de feuille de temps.
   * **Groupe avec accès administrateur** : si vous créez un profil de feuille de temps au niveau du système, laissez ce champ vide.

     Toute personne qui peut modifier des comptes peut attacher une feuille de temps au niveau du système à d’autres utilisateurs et utilisatrices.

     Seule une personne dotée des droits d’administration Workfront peut modifier un profil de feuille de temps au niveau du système.

     Si vous créez un profil de feuille de temps pour un groupe que vous administrez, identifiez le groupe ici.

     Cela n’affecte pas le profil de feuille de temps aux utilisateurs et utilisatrices du groupe ; cela permet seulement aux administrateurs et administratrices du groupe de modifier le profil de feuille de temps. Vous attribuerez le profil aux utilisateurs et utilisatrices à l’étape 6.

     >[!NOTE]
     >
     >Lorsque des utilisateurs extérieurs au groupe joignent des profils de feuille de temps à d’autres utilisateurs, ils ne pourront pas voir ni joindre ce profil de feuille de temps.

   * **Créer des feuilles de temps** : indiquez à quel moment le profil de feuille de temps doit générer les feuilles de temps. Une feuille de temps peut être générée automatiquement sur une base hebdomadaire, bihebdomadaire, bimensuelle ou mensuelle. Sélectionnez le jour de la semaine où vous souhaitez que la feuille de temps soit produite.

     Une feuille de temps hebdomadaire commence à la date à laquelle elle est générée. Par exemple, si vous créez des feuilles de temps hebdomadaires tous les jeudis, le premier jour de la semaine sur la feuille de temps est le jeudi.

     >[!NOTE]
     >
     >Workfront crée toujours deux feuilles de temps à la fois : la première feuille de temps inclut toujours la date actuelle, et la seconde commence lorsque la période de la première se termine.

   * **Approbateurs** : les approbateurs sont les utilisateurs qui approuvent la feuille de temps pour les utilisateurs qui y sont associés. Vous pouvez définir jusqu’à 7 personnes dotées du droit d’approbation sur une feuille de temps. Définir plusieurs personnes est utile pour s’assurer qu’un approbateur ou une approbatrice est disponible même en cas d’absence d’une autre personne. Tous les approbateurs et approbatrices sont notifiés lorsqu’une personne soumet la feuille de temps pour approbation. La feuille de temps n’a besoin d’être approuvée que par une personne.

     Seules les personnes disposant de droits d’administration sur les feuilles de temps peuvent être définies comme approbateurs ou approbatrices. Pour plus d’informations sur les droits d’administration des feuilles de temps, voir [Accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Utilisez le menu déroulant pour sélectionner l’approbateur de la feuille de temps (si un approbateur est requis). Vous pouvez sélectionner l’une des options suivantes :

      * **Aucune** : la feuille de temps n’a pas besoin d’être approuvée.
      * **Leur responsable** : il s’agit de la personne chargée de l’approbation par défaut, définie par le système. Dans ce cas, la personne désignée comme responsable approuve la feuille de temps lorsqu’elle est soumise à approbation.
      * **Personnes spécifiques** : vous pouvez désigner des utilisateurs spécifiques, par leur nom, en tant qu’approbateurs de feuilles de temps. Vous pouvez avoir plusieurs approbateurs et approbatrices pour une feuille de temps. Dans ce cas, une fois que l’un des approbateurs ou l’une des approbatrices a approuvé la feuille de temps, celle-ci est marquée comme **Fermée** et disparaît de la liste des approbations de tous les autres approbateurs et approbatrices.

   * **Peut modifier l’heure** : sélectionnez cette option pour permettre aux approbateurs de modifier les heures sur la feuille de temps.

     Cette option fonctionne avec le paramètre **Restreindre la modification des feuilles de temps aux personnes propriétaires et à l’équipe d’administration** dans la zone Configuration > Feuille de temps et heures > Préférences. Pour plus d’informations, voir [Configurer les préférences en matière de feuilles de temps et d’heures](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     Les scénarios suivants sont possibles :

     Lorsque l’option **Restreindre la modification des feuilles de temps aux personnes propriétaires et à l’équipe d’administration** est activée :

      * Les approbateurs peuvent uniquement approuver et rejeter des feuilles de temps, que l&#39;option Peut modifier l&#39;heure soit activée ou non.
      * Les personnes responsables des personnes propriétaires de feuilles de temps peuvent consulter uniquement les feuilles de temps de leurs personnes subordonnées directes.

     Lorsque l’option **Restreindre la modification des feuilles de temps aux personnes propriétaires et à l’équipe d’administration** est désactivée :

      * Lorsque l’option **Peut modifier l’heure** est activée, les approbateurs peuvent envoyer, rouvrir ou fermer la feuille de temps et modifier l’heure.
      * Lorsque l’option **Peut modifier l’heure** est désactivée, les approbateurs ne peuvent pas envoyer, rouvrir ou fermer la feuille de temps et ne peuvent pas modifier l’heure. Les approbateurs et approbatrices ne peuvent qu’approuver ou rejeter la feuille de temps.
      * Les personnes responsables des personnes propriétaires de feuilles de temps peuvent soumettre, rappeler, rouvrir et modifier les feuilles de temps de leurs personnes subordonnées directes.

     >[!NOTE]
     >
     >Une fois que vous avez soumis une feuille de temps pour approbation, vous ne pouvez plus modifier les heures. Pour remettre une feuille de temps soumise à l’état modifiable, rappelez la feuille de temps ou demandez à l’approbateur ou à l’approbatrice de rejeter la feuille de temps. Pour plus d’informations, voir [Soumettre une feuille de temps pour approbation](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) et [Approuver une feuille de temps](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md).

   * **Heures sup.** : vous pouvez masquer la zone Heures sup. dans les feuilles de temps. Cette option est désactivée par défaut.
   * **Types d’heures disponibles** : ce paramètre se rapporte uniquement aux types d’heures généraux et non aux types d’heures spécifiques à un projet.

     Par défaut, les utilisateurs et utilisatrices voient toutes les heures générales d’une feuille de temps. Toutefois, si votre organisation souhaite que seules des heures générales spécifiques s’affichent pour un groupe particulier d’utilisateurs et utilisatrices, vous pouvez choisir les heures générales qu’ils doivent voir sur leurs feuilles de temps en les sélectionnant dans leur profil de feuille de temps dans ce champ. Si vous souhaitez désactiver toutes les heures générales, désélectionnez tous les types d’heures pour générer la feuille de temps sans section pour les heures générales.

   * **Notifications de rappel** : ajoutez une notification de rappel. Workfront enverra des rappels aux utilisateurs pour leur demander de remplir ou d’approuver leurs feuilles de temps. Vous devez créer des notifications de rappel avant de pouvoir les associer à un profil de feuille de temps.

1. Pour associer le profil de feuille de temps à des utilisateurs, des groupes ou des équipes spécifiques (si vous êtes un administrateur Workfront), faites défiler la page vers le bas et recherchez la section **Attribuer des personnes**.

   Commencez à taper le nom de l’utilisateur ou de l’utilisatrice, du groupe ou de l’équipe, puis cliquez dessus lorsqu’il ou elle apparaît dans la liste déroulante.

   <!--To associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams, scroll towards the bottom of the page and find the **Assign People** section.-->

   Si vous êtes administrateur ou administratrice de groupes, vous pouvez attribuer le profil de feuille de temps aux groupes que vous administrez, mais pas aux équipes. Pour plus d’informations, voir [Limites pour un administrateur ou une administratrice de groupes qui attribue un profil de feuille de temps](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) dans cet article.

   >[!NOTE]
   >
   >* Vous pouvez également associer un utilisateur ou une utilisatrice à un profil de feuille de temps en modifiant le profil de l’utilisateur ou l’utilisatrice. Pour plus d’informations, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Lorsque vous ajoutez un groupe, seul le nom du groupe apparaît dans l’onglet Affecter des personnes, et non pas la liste des personnes membres du groupe. Si vous souhaitez voir les personnes membres du groupe, cliquez sur Enregistrer les modifications, puis sur le nom du profil de feuille de temps que vous venez de créer.
   >* Lorsque vous avez terminé ces étapes, le profil de feuille de temps génère des feuilles de temps uniquement pour les utilisateurs et utilisatrices ou les personnes membres du groupe attribués qui n’ont pas de feuilles de temps existantes pour la période en cours.

1. Cliquer sur **Enregistrer**.

1. En haut de la liste des profils de feuilles de temps, cliquez sur l’icône **Plus** ![Icône Plus](assets/more-icon.png), puis sur **Générer des feuilles de temps**.

   Une confirmation s’affiche en bas de l’écran indiquant que les feuilles de temps ont bien été générées. De nouvelles feuilles de temps sont générées en fonction des nouveaux profils que vous avez créés.

   Pour plus d’informations, voir [&#x200B; Générer manuellement des feuilles de temps &#x200B;](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

   La première fois que le profil de feuille de temps génère des feuilles de temps, deux feuilles de temps sont créées pour chaque utilisateur, pour la période qui inclut l’heure actuelle ainsi que pour la période suivante.

   Ensuite, chaque fois qu’elle génère de nouvelles feuilles de temps, une feuille de temps est créée par utilisateur.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Limites de l’affectation d’un profil de feuille de temps pour un administrateur ou une administratrice de groupes {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Si vous êtes administrateur ou administratrice de groupe et que l’option d’accès administratif Feuilles de temps et heures est désactivée à votre niveau d’accès, vous pouvez créer des profils de feuilles de temps, mais vous ne pouvez les affecter qu’aux entités suivantes :

* Les groupes que vous administrez.
* Les personnes à qui vous avez accès pour modifier les personnes membres d’un groupe que vous administrez.

Pour ces groupes et utilisateurs et utilisatrices, vous n’aurez pas accès aux feuilles de temps générées par le profil de feuille de temps.

De plus, si l’option Administration des utilisateurs et utilisatrices (utilisateurs et utilisatrices du groupe) est également désactivée à votre niveau d’accès, vous pouvez affecter le profil de feuille de temps à un groupe que vous administrez, mais cela n’affecte que les personnes membres du groupe que vous avez le droit de modifier. Si le groupe contient des utilisateurs et utilisatrices que vous n’avez pas le droit de modifier, le profil de feuille de temps ne leur est pas affecté en même temps qu’au reste du groupe.

Pour plus d’informations sur l’option Feuilles de temps et heures de votre niveau d’accès, voir la section [Accorder un accès administratif à certaines zones](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Pour plus d’informations sur l’option Administration des utilisateurs et utilisatrices (utilisateurs et utilisatrices du groupe) de votre niveau d’accès, voir la section [Accorder l’accès aux utilisateurs et utilisatrices](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Plusieurs profils récurrents de feuilles de temps

Vous pouvez disposer de plusieurs profils de feuille de temps pour votre organisation si les éléments suivants existent :

* Périodes de paie uniques pour différents groupes d’utilisateurs et d’utilisatrices
* Approbateurs et approbatrices uniques pour différents ensembles d’utilisateurs et d’utilisatrices
* Exigences uniques en matière d’heures générales pour différents ensembles d’utilisateurs et d’utilisatrices

Une personne ne peut pas être associée à plusieurs profils de feuille de temps à la fois.

<!--
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Add a name for the timesheet profile. It could be the name of a team or a group whose people share the same timeframe for their timesheets. </p> <p>This ia a required field.</p> </td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Add more information about the timesheet profile.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group's administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p>

   <p><b>NOTE</b>: When users outside the group are attaching timesheet profiles to other users, they won't be able to see or attach this timesheet profile.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p>
      <p>A weekly timesheet begins on the date it is generated. For example, if you create weekly timesheets every Thursday, the first day of the week on the timesheet is Thursday.</p>
    
      
   <p><b>NOTE</b>: Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet starts when the time frame of the first one ends.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvers</strong></p> </td> 
      <td> <p> <p>Approvers are users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
      <ul> 
      <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time </strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. 

   <p>This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.</p>

   <p>The following scenarios exist: </p>

   <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
      <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
      <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
    <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
      <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
      <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
      </ul>

   <p>

   <b>NOTE</b>: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Overtime</strong> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td><p>This setting refers only to General Hour Types, and not to project-specific hour types. </p>
      <p>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect all hour types to generate the timesheet without a section for general hours.</p></td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Reminder notifications</strong> </td> 
      <td> <p> Add a reminder notification. Workfront will send reminders to users to ask them to complete or approve their timesheets. You must create reminder notifications before you can associate them with a timesheet profile.  </p> </td> 
     </tr>
    </tbody> 
   </table>
-->