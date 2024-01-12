---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Création, modification et affectation de profils de feuille de temps
description: Vous pouvez créer, modifier et affecter des profils de feuille de temps qui génèrent des feuilles de temps récurrentes pour vos utilisateurs sans intervention de votre part. Vous gagnez ainsi du temps et garantissez la cohérence entre les utilisateurs.
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 0%

---

# Création, modification et affectation de profils de feuille de temps

Vous pouvez créer, modifier et affecter des profils de feuille de temps qui génèrent des feuilles de temps récurrentes pour vos utilisateurs sans intervention de votre part. Cela vous permet de gagner du temps et de vous assurer que les éléments suivants sont cohérents entre les utilisateurs :

* Période de la feuille de temps
* Approbateurs
* Types d’heures généraux

Pour plus d’informations sur la création manuelle d’une feuille de temps, voir [Création d’une feuille de temps à usage unique](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard </p>
 <p>ou</p> 
<p>Actuel : formule </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez disposer d’un accès administratif aux feuilles de calcul. </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Création ou modification d’un profil de feuille de temps

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Pour activer les modifications de profil de la feuille de temps dans les feuilles de temps actuelles, vous devez supprimer les feuilles de temps existantes, puis en générer de nouvelles. Pour obtenir des instructions, voir [Suppression de feuilles de temps dans Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) et [Génération manuelle de feuilles de temps](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. Si vous créez ou modifiez un profil de feuille de temps à utiliser dans tout le système, cliquez sur **Frise chronologique et heures**.

   Ou

   Si vous créez ou modifiez un profil de feuille de temps pour un groupe, cliquez sur **Groupes**, puis cliquez sur le nom du groupe.

1. Cliquez sur **Profils de feuille de temps**.
1. Pour créer un profil de feuille de temps, cliquez sur **Nouveau profil**.

   Ou

   Pour modifier un profil de feuille de temps existant, sélectionnez le profil de feuille de temps à modifier, puis cliquez sur **Modifier**.

   Le profil de feuille de temps nouveau ou existant s’affiche.


1. Sur le **Définir les détails** , saisissez une **Nom** et **Description** pour le profil de la feuille de temps et fournissez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Groupe avec accès Administration</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Si vous créez un profil de feuille de temps au niveau du système, laissez ce champ vide.</p> <p>Tout utilisateur qui peut modifier des comptes d’utilisateurs peut joindre une feuille de temps au niveau du système à d’autres utilisateurs.</p> <p>Seul un administrateur Workfront peut modifier un profil de feuille de temps au niveau du système.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Si vous créez un profil de feuille de temps pour un groupe que vous administrez, identifiez-le ici.</p> <p>Cela n’affecte pas le profil de la feuille de temps aux utilisateurs du groupe ; cela permet uniquement aux administrateurs du groupe de modifier le profil de la feuille de temps. Vous attribuerez le profil aux utilisateurs à l’étape 6.</p>

   <p><b>REMARQUE</b>: lorsque des utilisateurs en dehors du groupe associent des profils de feuille de temps à d’autres utilisateurs, ils ne pourront pas afficher ni joindre ce profil de feuille de temps.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Création de feuilles de temps</strong> </td> 
      <td> <p> <p>Spécifiez quand le profil de la feuille de temps doit générer les feuilles de temps. Une feuille de temps peut être définie pour une génération automatique sur une base hebdomadaire, bimensuelle, semestrielle ou mensuelle. Sélectionnez le jour de la semaine où vous souhaitez que la feuille de temps soit générée.</p>
      <p>Une feuille de temps hebdomadaire commence à la date de sa génération. Par exemple, si vous créez des feuilles de temps hebdomadaires tous les jeudis, le premier jour de la semaine sur la feuille de temps est jeudi.</p>


   <p><b>REMARQUE</b>: Workfront crée toujours deux feuilles de temps à la fois : la première feuille de temps inclut toujours la date actuelle et la seconde commence à la fin de la première période.</p> </p> </td> 
    </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approbateurs</strong></p> </td> 
      <td> <p> <p>Les approbateurs sont des utilisateurs qui approuvent la feuille de temps pour les utilisateurs associés à la feuille de temps. Vous pouvez identifier jusqu’à 7 utilisateurs en tant qu’approbateurs sur une feuille de temps. L’identification de plusieurs utilisateurs s’avère utile pour s’assurer qu’un approbateur est disponible lorsqu’une personne est absente du bureau. Tous les approbateurs sont avertis lorsqu’un utilisateur envoie la feuille de temps pour approbation. Un seul utilisateur doit approuver la feuille de temps pour qu’elle soit approuvée.</p> <p>Seuls les utilisateurs disposant de droits d’administration pour la feuille de temps peuvent être définis comme approbateurs. Pour plus d’informations sur les droits d’administration de la feuille de temps, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> <p>Utilisez le menu déroulant pour sélectionner l’approbateur de la feuille de temps (si un approbateur est requis). Vous pouvez sélectionner l’une des options suivantes :</p> 
      <ul> 
      <li><strong>Aucun</strong>: la feuille de temps n’a pas besoin d’être approuvée.</li> 
      <li><strong>Leur responsable</strong>: il s’agit de l’approbateur par défaut, défini par le système. Dans ce cas, l’utilisateur désigné comme leur responsable valide la feuille de temps lorsqu’elle est soumise à validation.</li> 
      <li><strong>Personnes spécifiques :</strong> Vous pouvez désigner des utilisateurs spécifiques, par nom, comme approbateurs de feuille de temps. Vous pouvez avoir plusieurs approbateurs sur une feuille de temps. Dans ce cas, une fois que l’un des approbateurs a approuvé la feuille de temps, celle-ci est marquée comme <strong>Fermé</strong> et il disparaît de la liste d’approbations de la feuille de temps de tous les approbateurs restants.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Peut modifier l’heure </strong> </td> 
      <td> <p> <p>Sélectionnez cette option pour permettre aux approbateurs de modifier les heures sur la feuille de temps.

   Cette option fonctionne avec la fonction **Limitation de la modification de la feuille de temps aux propriétaires et aux administrateurs** dans la zone Configuration > Frise chronologique et heures > Préférences . Pour plus d’informations, voir <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configuration des préférences de feuille de temps et d’heure</a>.

   Les scénarios suivants existent :

   <ul>
      <li>Lorsque la variable <b>Limitation de la modification de la feuille de temps aux propriétaires et aux administrateurs</b> est activée :</li>
      <ul><li>Les approbateurs ne peuvent approuver et rejeter que la feuille de temps, que la <b>Peut modifier l’heure</b> est activé ou non. </li>
      <li>Les gestionnaires des propriétaires de feuilles de calcul peuvent uniquement afficher les feuilles de temps de leurs rapports directs.</li></ul>
      <li>Lorsque la variable <b>Limitation de la modification de la feuille de temps aux propriétaires et aux administrateurs</b> est désactivée :</li>
    <ul><li>Lorsque la variable <b>Peut modifier l’heure</b> est activée, les approbateurs peuvent envoyer, rouvrir ou fermer la feuille de temps et peuvent modifier l’heure.</li>
      <li>Lorsque la variable <b>Peut modifier l’heure</b> est désactivée, les approbateurs ne peuvent pas envoyer, rouvrir ou fermer la feuille de temps et ne peuvent pas modifier l’heure. Les approbateurs peuvent uniquement approuver ou rejeter la feuille de temps. </li>
      <li>Les gestionnaires des propriétaires de feuilles de calcul peuvent envoyer, révoquer, rouvrir et modifier les feuilles de temps de leurs rapports directs.</li></ul>
      </ul>

   <p>

   <b>REMARQUE</b>: une fois que vous avez soumis une feuille de temps pour approbation, vous ne pouvez plus modifier les heures. Pour renvoyer une feuille de temps envoyée à un état modifiable, rappelez-la ou demandez à l’approbateur de rejeter la feuille de temps. Pour plus d’informations, voir <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Envoyer une feuille de temps pour approbation</a> et<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approbation d’une feuille de temps</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Types d’heure disponibles</strong> </td> 
      <td><p>Ce paramètre fait uniquement référence aux types d’heures généraux, et non aux types d’heures spécifiques au projet. </p>
      <p>Par défaut, les utilisateurs voient toutes les heures générales sur une feuille de temps. Cependant, si votre entreprise souhaite que seules des heures générales spécifiques s’affichent pour un ensemble particulier d’utilisateurs, vous pouvez sélectionner dans ce champ les heures générales dont ils ont besoin dans leurs feuilles de temps en les sélectionnant dans leur profil de feuille de temps. Si vous souhaitez désactiver toutes les heures générales, désélectionnez tous les types d’heures pour générer la feuille de temps sans section pour les heures générales.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Overtime</span> </td> 
      <td>Vous pouvez choisir de masquer la zone Heures d’activation dans les feuilles de temps. Cette option est désactivée par défaut.</td> 
     </tr> 
    </tbody> 
    </table>

1. Cliquez sur le bouton **Affecter des personnes** pour associer le profil de la feuille de temps à des utilisateurs, groupes ou équipes spécifiques (si vous êtes administrateur Workfront). Commencez à saisir le nom de l’utilisateur, du groupe ou de l’équipe, puis cliquez dessus lorsqu’il apparaît dans la liste déroulante.

   Si vous êtes administrateur de groupe, vous pouvez affecter le profil de feuille de temps aux groupes que vous administrez, mais pas aux équipes. Pour plus d’informations, voir [Limites d’attribution d’un profil de feuille de temps à un administrateur de groupe](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) dans cet article.

   >[!NOTE]
   >
   >* Vous pouvez également associer un utilisateur à un profil de feuille de temps en modifiant son profil. Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Lorsque vous ajoutez un groupe, seul le nom du groupe s’affiche dans l’onglet Attribuer des personnes , et non dans la liste des membres du groupe. Si vous souhaitez que les membres du groupe soient répertoriés ici, cliquez sur Enregistrer les modifications, puis cliquez sur le nom du profil de la feuille de temps que vous venez de créer.
   >* Une fois ces étapes terminées, le profil de la feuille de temps génère des feuilles de temps uniquement pour les utilisateurs affectés ou les membres du groupe qui n’ont pas de feuilles de temps existantes pour la période en cours.

1. Cliquez sur **Enregistrer les modifications**.

   La première fois que le profil de la feuille de temps génère des feuilles de temps, deux feuilles de temps sont créées pour chaque utilisateur. Ensuite, chaque fois qu’elle génère de nouvelles feuilles de temps, une feuille de temps est créée par utilisateur.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Limites d’attribution d’un profil de feuille de temps à un administrateur de groupe {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Si vous êtes administrateur de groupe et que l’option d’accès administrateur Heures et heures est désactivée dans votre niveau d’accès, vous pouvez créer des profils de feuille de temps, mais vous pouvez uniquement les affecter à :

* Groupes que vous gérez
* Utilisateurs individuels que vous avez accès à la modification dans un groupe que vous administrez.

Pour ces groupes et utilisateurs, vous n’aurez pas accès aux feuilles de temps générées par le profil de la feuille de temps.

De plus, si l’option Administration des utilisateurs (utilisateurs du groupe) est également désactivée dans votre niveau d’accès, vous pouvez affecter le profil de la feuille de temps à un groupe que vous administrez, mais cela affecte uniquement les utilisateurs du groupe que vous avez accès à la modification. Si le groupe contient des utilisateurs que vous n’avez pas accès à la modification, le profil de la feuille de temps ne leur est pas associé avec le reste du groupe.

Pour plus d’informations sur l’option Fiches horaires et heures de votre niveau d’accès, voir [Octroi aux utilisateurs un accès administratif à certaines zones](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Pour plus d’informations sur l’option Administration des utilisateurs (utilisateurs de groupe) de votre niveau d’accès, voir [Accorder l’accès aux utilisateurs](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Plusieurs profils de feuille de temps récurrente

Vous pouvez avoir plusieurs profils de feuille de temps pour votre organisation en cas de :

* Périodes de paie uniques pour différents ensembles d’utilisateurs
* Approbateurs uniques pour différents ensembles d’utilisateurs
* Heures générales uniques requises pour différents ensembles d’utilisateurs

Un utilisateur ne peut pas être associé à plusieurs profils de feuille de temps à la fois. 
