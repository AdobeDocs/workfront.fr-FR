---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Créer, modifier et attribuer des profils de feuilles de temps
description: Vous pouvez créer, modifier et attribuer des profils de feuilles de temps qui génèrent des feuilles de temps récurrentes pour les utilisateurs et utilisatrices sans autre intervention de votre part. Cela vous permet de gagner du temps et d’assurer la cohérence entre les utilisateurs et utilisatrices.
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 84%

---

# Créer, modifier et attribuer des profils de feuilles de temps

<!--Audited: 06/2025-->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div> -->

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

<!--
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

   Le nouveau profil de feuille de temps ou le profil existant s’affiche.


1. Cliquez sur l&#39;onglet **Définir les détails**, puis mettez à jour les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nom</strong> </td> 
      <td> <p> Ajoutez un nom pour le profil de feuille de temps. Il peut s’agir du nom d’une équipe ou d’un groupe dont les personnes partagent le même délai pour leurs feuilles de temps. </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Ajoutez plus d’informations sur le profil de feuille de temps.     
      </p> </td> 
     </tr>



   <tr> 
      <td role="rowheader"><strong>Groupe disposant d’un accès administrateur</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Si vous créez un profil de feuille de temps au niveau du système, laissez ce champ vide.</p> <p>Toute personne qui peut modifier des comptes peut attacher une feuille de temps au niveau du système à d’autres utilisateurs et utilisatrices.</p> <p>Seule une personne dotée des droits d’administration Workfront peut modifier un profil de feuille de temps au niveau du système.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Si vous créez un profil de feuille de temps pour un groupe que vous administrez, identifiez le groupe ici.</p> <p>Cela n’affecte pas le profil de feuille de temps aux utilisateurs et utilisatrices du groupe ; cela permet seulement aux administrateurs et administratrices du groupe de modifier le profil de feuille de temps. Vous attribuerez le profil aux utilisateurs et utilisatrices à l’étape 6.</p>

   <p><b>NOTE</b> : lorsque des utilisateurs et utilisatrices extérieurs au groupe attachent des profils de feuilles de temps à d’autres personnes, ils ne pourront pas voir ou attacher ce profil de feuille de temps.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Créer des feuilles de temps</strong> </td> 
      <td> <p> <p>Spécifiez quand le profil de feuille de temps doit générer les feuilles de temps. Une feuille de temps peut être générée automatiquement sur une base hebdomadaire, bihebdomadaire, bimensuelle ou mensuelle. Sélectionnez le jour de la semaine où vous souhaitez que la feuille de temps soit produite.</p>
      <p>Une feuille de temps hebdomadaire commence à la date à laquelle elle est générée. Par exemple, si vous créez des feuilles de temps hebdomadaires tous les jeudis, le premier jour de la semaine sur la feuille de temps est le jeudi.</p>


   <p><b>NOTE</b> : Workfront crée toujours deux feuilles de temps à la fois. La première feuille de temps inclut toujours la date du jour, et la seconde feuille de temps commence lorsque la période de temps de la première se termine.</p> </p> </td> 
    </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approbateurs</strong></p> </td> 
      <td> <p> <p>Les approbateurs et approbatrices sont des utilisateurs et utilisatrices qui approuvent la feuille de temps pour les utilisateurs et utilisatrices associés à la feuille de temps. Vous pouvez définir jusqu’à 7 personnes dotées du droit d’approbation sur une feuille de temps. Définir plusieurs personnes est utile pour s’assurer qu’un approbateur ou une approbatrice est disponible même en cas d’absence d’une autre personne. Tous les approbateurs et approbatrices sont notifiés lorsqu’une personne soumet la feuille de temps pour approbation. La feuille de temps n’a besoin d’être approuvée que par une personne.</p> <p>Seules les personnes disposant de droits d’administration sur les feuilles de temps peuvent être définies comme approbateurs ou approbatrices. Pour plus d’informations sur les droits d’administration des feuilles de temps, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones</a>.</p> <p>Utilisez le menu déroulant pour sélectionner l’approbateur ou l’approbatrice de la feuille de temps (si un approbateur ou une approbatrice est nécessaire). Vous pouvez sélectionner l’une des options suivantes :</p> 
      <ul> 
      <li><strong>Aucun</strong> : la feuille de temps n’a pas besoin d’être approuvée.</li> 
      <li><strong>Leur responsable</strong> : il s’agit de la personne chargée de l’approbation par défaut, définie par le système. Dans ce cas, la personne désignée comme responsable approuve la feuille de temps lorsqu’elle est soumise à approbation.</li> 
      <li><strong>Personnes spécifiques :</strong> vous pouvez désigner des utilisateurs et utilisatrices spécifiques, par leur nom, comme approbateurs et approbatrices des feuilles de temps. Vous pouvez avoir plusieurs approbateurs et approbatrices pour une feuille de temps. Dans ce cas, une fois que l’un des approbateurs ou l’une des approbatrices a approuvé la feuille de temps, celle-ci est marquée comme <strong>Fermée</strong> et disparaît de la liste des approbations de tous les autres approbateurs et approbatrices.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Peut modifier l’heure</strong> </td> 
      <td> <p> <p>Sélectionnez cette option pour permettre aux approbateurs et approbatrices de modifier les heures de la feuille de temps.

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

   <p>

   <b>NOTE</b> : une fois que vous avez soumis une feuille de temps pour approbation, vous ne pouvez plus modifier les heures. Pour remettre une feuille de temps soumise à l’état modifiable, rappelez la feuille de temps ou demandez à l’approbateur ou à l’approbatrice de rejeter la feuille de temps. Pour plus d’informations, voir <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Soumettre une feuille de temps pour approbation</a> et <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approuver une feuille de temps</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Types d’heures disponibles</strong> </td> 
      <td><p>Ce paramètre ne concerne que les types d’heures généraux, et non les types d’heures spécifiques à un projet. </p>
      <p>Par défaut, les utilisateurs et utilisatrices voient toutes les heures générales d’une feuille de temps. Toutefois, si votre organisation souhaite que seules des heures générales spécifiques s’affichent pour un groupe particulier d’utilisateurs et utilisatrices, vous pouvez choisir les heures générales qu’ils doivent voir sur leurs feuilles de temps en les sélectionnant dans leur profil de feuille de temps dans ce champ. Si vous souhaitez désactiver toutes les heures générales, désélectionnez tous les types d’heures pour générer la feuille de temps sans section pour les heures générales.</p></td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong> Notifications de rappel </strong> </td> 
      <td> <p> Ajoutez une notification de rappel. Workfront enverra des rappels aux utilisateurs pour leur demander de remplir ou d’approuver leurs feuilles de temps. Vous devez créer des notifications de rappel avant de pouvoir les associer à un profil de feuille de temps.  </p> </td> 
     </tr>

   <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Heures supplémentaires</span> </td> 
      <td>Vous pouvez masquer la case Heures supplémentaires dans les feuilles de temps. Cette option est désactivée par défaut.</td> 
     </tr> 
    </tbody> 
    </table>

1. Cliquez sur l’onglet **Affecter des personnes** pour associer le profil de feuille de temps à des utilisateurs et utilisatrices, des groupes ou (si vous êtes un administrateur ou une administratrice Workfront) des équipes spécifiques. Commencez à taper le nom de l’utilisateur ou de l’utilisatrice, du groupe ou de l’équipe, puis cliquez dessus lorsqu’il ou elle apparaît dans la liste déroulante.

   Si vous êtes administrateur ou administratrice de groupes, vous pouvez attribuer le profil de feuille de temps aux groupes que vous administrez, mais pas aux équipes. Pour plus d’informations, voir [Limites pour un administrateur ou une administratrice de groupes qui attribue un profil de feuille de temps](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) dans cet article.

   >[!NOTE]
   >
   >* Vous pouvez également associer un utilisateur ou une utilisatrice à un profil de feuille de temps en modifiant le profil de l’utilisateur ou l’utilisatrice. Pour plus d’informations, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Lorsque vous ajoutez un groupe, seul le nom du groupe apparaît dans l’onglet Affecter des personnes, et non pas la liste des personnes membres du groupe. Si vous souhaitez voir les personnes membres du groupe, cliquez sur Enregistrer les modifications, puis sur le nom du profil de feuille de temps que vous venez de créer.
   >* Lorsque vous avez terminé ces étapes, le profil de feuille de temps génère des feuilles de temps uniquement pour les utilisateurs et utilisatrices ou les personnes membres du groupe attribués qui n’ont pas de feuilles de temps existantes pour la période en cours.

1. Cliquer sur **Enregistrer**.

1. En haut de la liste des profils de feuille de temps, cliquez sur l&#39;icône **Plus** ![icône Plus](assets/more-icon.png) pour les profils de feuille de temps au niveau du système, ou **Plus** pour les profils de feuille de temps de groupe, puis cliquez sur **Générer des feuilles de temps**.

   Une confirmation s’affiche en bas de l’écran indiquant que les feuilles de temps ont bien été générées. De nouvelles feuilles de temps sont générées en fonction des nouveaux profils que vous avez créés.

   Pour plus d’informations, voir [ Générer manuellement des feuilles de temps ](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

   La première fois que le profil de feuille de temps génère des feuilles de temps, 2 feuilles de temps sont créées pour chaque utilisateur, tant pour la période qui inclut l’heure actuelle que pour la période suivante.

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
