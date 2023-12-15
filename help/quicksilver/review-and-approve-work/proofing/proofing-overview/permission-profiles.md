---
content-type: overview
product-area: documents
keywords: BAT,permission
navigation-topic: proofing-overview
title: Aperçu du profil d’autorisation de preuve
description: Les profils d’autorisation de BAT déterminent les autorisations globales dont disposent les utilisateurs sur tous les bons à tirer de votre compte. Les profils d’autorisation de BAT sont attribués aux utilisateurs dans leur profil utilisateur. Les profils d’autorisation de BAT diffèrent des rôles de BAT.
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 1%

---

# Aperçu du profil d’autorisation de preuve

<!--Audited: 12/2023-->

Les profils d’autorisation de BAT déterminent les autorisations globales dont disposent les utilisateurs sur tous les bons à tirer de votre compte. Les profils d’autorisation de BAT sont attribués aux utilisateurs dans leur profil utilisateur.

Les profils d’autorisation de BAT diffèrent des rôles de BAT. Pour plus d’informations sur les rôles de BAT, voir [Rôles de BAT - Aperçu](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).

>[!NOTE]
>
>Si vous êtes administrateur, vous pouvez créer des profils personnalisés pour les utilisateurs de votre entreprise. Pour plus d’informations, voir [Configuration de profils personnalisés dans le bon à tirer Workfront](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the account settings and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them. </li>
</ul>
-->

## Profils d’autorisation de preuve

Le tableau suivant affiche les autorisations disponibles pour chaque profil d’autorisation de BAT.

<table>
  <tr>
   <td colspan="1" ><strong></strong>
   </td>
   <td colspan="4" ><strong>Éléments propres</strong>
   </td>
   <td colspan="3" ><strong>Autres éléments d’utilisateur</strong>
   </td>
   <td><strong>Administration</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>Ajouter</strong>
   </td>
   <td><strong>Affichage</strong>
   </td>
   <td><strong>Modifier</strong>
   </td>
   <td><strong>Supprimer</strong>
   </td>
   <td><strong>Affichage</strong>
   </td>
   <td><strong>Modifier</strong>
   </td>
   <td><strong>Supprimer</strong>
   </td>
   <td><strong>Modification et suppression</strong>
   </td>
  </tr>
  <tr>
   <td>Administration
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
  </tr>
  <tr>
   <td>Superviseur
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Gestionnaire
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### Administrateur

Les administrateurs ont accès aux [Paramètres du compte](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) et disposent des autorisations suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Les administrateurs peuvent :</td> 
   <td>Les administrateurs ne peuvent pas :</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Créer des bons à tirer, charger des fichiers et créer des dossiers</p> </li> 
     <li> <p>Afficher, modifier et supprimer les BAT et les fichiers qu’ils ont créés</p> </li> 
     <li> <p>Afficher, modifier et supprimer les bons à tirer et les fichiers créés par tous les utilisateurs de l’entreprise</p> </li> 
     <li> <p>Suppression des dossiers publics d’autres utilisateurs</p> </li> 
     <li> <p>Modifier tous les BAT créés dans le compte</p> </li> 
     <li> <p>Être défini comme propriétaire de zone de dépôt*</p> </li> 
     <li> <p>Accédez à la page Paramètres du compte et modifiez les détails du compte.</p> </li> 
     <li> <p>Vider la corbeille</p> </li> 
     <li> <p>Ajout, modification et suppression d’utilisateurs</p> </li> 
     <li> <p>Créer des groupes et ajouter de nouveaux contacts</p> </li> 
     <li> <p>Supprimer des contacts</p> </li> 
     <li> <p>Editer les BAT s'il n'y a pas de réponse</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Modifiez les réponses du BAT.</p> </li> 
     <li> <p>Suppression des dossiers privés des autres utilisateurs</p> </li> 
     <li> <p>Accédez à la page Facturation ou modifiez les détails de facturation</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Disponible uniquement dans le produit autonome Bon à tirer de Workfront.

### Superviseur

Les superviseurs disposent des autorisations suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Les superviseurs peuvent :</td> 
   <td>Les superviseurs ne peuvent pas :</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Créer des bons à tirer, charger des fichiers et créer des dossiers</p> </li> 
     <li> <p>Afficher, modifier et supprimer les BAT et les fichiers qu’ils ont créés</p> </li> 
     <li> <p>Afficher, modifier et supprimer les bons à tirer et les fichiers créés par tous les utilisateurs de l’entreprise</p> </li> 
     <li> <p>Suppression des dossiers publics d’autres utilisateurs</p> </li> 
     <li> <p>Modifier tous les BAT créés dans le compte</p> </li> 
     <li> <p>Créer des groupes et ajouter de nouveaux contacts</p> </li> 
     <li> <p>Supprimer des contacts</p> </li> 
     <li> <p>Editer les BAT s'il n'y a pas de réponse</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Modifiez les réponses du BAT.</p> </li> 
     <li> <p>Suppression des dossiers privés d’autres utilisateurs</p> </li> 
     <li> <p>Accédez à la page Facturation ou modifiez les détails de facturation</p> </li> 
     <li> <p>Ajout, modification ou suppression d’utilisateurs</p> </li> 
     <li> <p>Vider la corbeille</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gestionnaire

Les gestionnaires disposent des autorisations suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Les responsables peuvent :</td> 
   <td>Les gestionnaires ne peuvent pas :</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Créer des bons à tirer, charger des fichiers et créer des dossiers</p> </li> 
     <li> <p>Afficher, modifier et supprimer les BAT et les fichiers qu’ils ont créés</p> </li> 
     <li> <p>Voir, réviser et approuver les BAT d’autres utilisateurs qui sont explicitement partagés avec eux (droits en lecture seule sur tous les éléments d’un dossier partagé).</p> </li> 
     <li> <p>Modifier tous les BAT créés dans le compte</p> </li> 
     <li> <p>Créer des groupes et ajouter de nouveaux contacts</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Affichez, modifiez ou supprimez des BAT et des fichiers créés par d’autres utilisateurs de l’entreprise. </p> </li><li><p>Modifiez les réponses du BAT.</p> </li> 
     <li> <p>Suppression des dossiers privés ou publics d’autres utilisateurs</p> </li> 
     <li> <p>Accédez à la page Facturation ou modifiez les détails de facturation</p> </li> 
     <li> <p>Ajout, modification ou suppression d’utilisateurs</p> </li> 
     <li> <p> Supprimer des contacts</p> </li> 
     <li> <p>Vider la corbeille</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Observer</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers have the following permissions:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a> and <a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts. </p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited. </p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings: Account settings, Billing </li>>
>  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Guest</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Guest profile is used to give access to proofs for reviewers who do not have their own Workfront Proof account. Guests can access proofs shared with them directly via their personal email notifications.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view, review, and approve proofs that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Dashboard.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot have folders shared with them. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be added as Authors or Moderators to the proofs. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<note type="note">
 Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->
