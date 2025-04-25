---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Créer une version d’une épreuve
description: Gérer les commentaires sur plusieurs versions ou révisions d’un travail peut s’avérer être un énorme défi. Workfront simplifie ce processus en vous permettant de créer et de comparer plusieurs versions d’une épreuve.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: daa46f0e2a5f656d048260d4a714ed02f01cdbbf
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 35%

---

# Créer une version d’une épreuve

<!-- Audited: 4/2025 -->

La gestion des commentaires sur plusieurs versions ou révisions d’un élément de travail peut s’avérer difficile. Adobe Workfront simplifie ce processus en vous permettant de créer et de comparer plusieurs versions d’une épreuve.

Tenez compte des informations suivantes lors de la création d’une nouvelle version d’une épreuve :

* Vous pouvez autoriser une personne à voir une version mais pas une autre. À l’inverse, si vous partagez une version ultérieure avec un utilisateur, celui-ci ne peut pas voir les versions antérieures, sauf si vous revenez en arrière et que vous lui accordez l’accès à ces versions antérieures.
* Vous devez disposer des droits de modification sur l’épreuve pour créer une version.

  Pour plus d’informations, voir [Gestion des rôles d’épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) et [Profils des autorisations d’épreuve dans Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

  Pour plus d’informations sur le partage des versions d’une épreuve, voir [Partager une épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Si une épreuve est créée dans Adobe Workfront, toute nouvelle version de cette épreuve doit également être créée dans Workfront. Vous ne pouvez pas créer de nouvelle version d’une épreuve dans Workfront Proof si cette épreuve a été créée dans Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Actuel : Pro ou supérieur</p> <p>ou</p> <p>Hérité : Select ou Premium</p> <p>Pour plus d’informations sur la relecture de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Actuel : Standard</p> 
   <p>Ou</p>
   <p>Hérité : travail ou plan (la relecture doit être activée pour l'utilisateur)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander un accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Création d’une version d’épreuve dans Workfront

Il existe plusieurs façons de charger une nouvelle version d’épreuve dans Workfront. Les paramètres par défaut de l’épreuve peuvent être transférés ou non de la version précédente, selon la méthode sélectionnée :

* **Générer automatiquement des épreuves lors du chargement de documents** : si ce paramètre est activé dans votre profil utilisateur, les paramètres d’épreuve par défaut ne sont pas transférés lorsque vous faites glisser et déposez une nouvelle version.
* **Créer une épreuve > Simple** : si vous sélectionnez cette option, les paramètres d’épreuve par défaut ne sont pas transférés depuis la version précédente.
* **Ajouter > Version > Épreuve** : si vous sélectionnez cette option, les paramètres d’épreuve par défaut sont transférés de la version précédente.
* **Créer une épreuve > Avancé** : si vous sélectionnez cette option, les paramètres d’épreuve par défaut sont transférés de la version précédente.

Pour créer une version d’une épreuve, procédez comme suit :

1. Ouvrez la liste des documents contenant l’épreuve.
1. À partir du système de fichiers de votre ordinateur, faites glisser et déposez un nouveau fichier sur l’épreuve.

   Ou

   Sélectionnez la ligne où l’épreuve est répertoriée, puis cliquez sur **Ajouter** > **Version**, puis cliquez sur l’option que vous souhaitez utiliser pour ajouter la nouvelle version de l’épreuve.

   ![Ajouter une nouvelle version](assets/add-new-proof-version.png)

## Création d’une nouvelle version de BAT à partir de la visionneuse de BAT (Workfront Proof uniquement)

Si vous utilisez la version autonome de Workfront Proof, vous pouvez créer une nouvelle version d’une épreuve contenant un seul fichier ou une capture web. 

>[!NOTE]
>
>Si votre compte est en formule Entreprise et que vous téléchargez plusieurs fichiers ou captures web, ils sont automatiquement combinés dans une seule nouvelle version. Veuillez consulter [Créer une épreuve de plusieurs pages](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) pour plus d’informations.

Pour créer une version d’une épreuve dans Workfront Proof :

1. Ouvrez l’épreuve.
1. Dans le coin supérieur gauche, cliquez sur le menu déroulant **Version**, puis sur **+ Nouvelle version** dans la zone qui s’affiche. La page de la nouvelle version de l’épreuve s’ouvre.

   ![Ajouter une nouvelle version](assets/new-version-button.png)

1. Dans la section **Ajouter des fichiers**, chargez un fichier en tant que nouvelle version d’épreuve en le faisant glisser depuis votre ordinateur ou en cliquant sur **parcourir** et en sélectionnant un fichier.

   Ou

   Capturez une page web en tant que nouvelle version de l’épreuve en saisissant une URL.

   >[!NOTE]
   >
   >Le glisser-déposer est disponible uniquement avec les navigateurs qui prennent entièrement en charge HTML5. Cela exclut Internet Explorer 7 à 9 et Safari.

1. (Facultatif) Sélectionnez le titre de l’épreuve et saisissez un nouveau **nom de l’épreuve** pour la version.

1. Dans la section **Workflow**, effectuez l’une des modifications suivantes pour ajouter des réviseurs à cette version de BAT (cette opération remplacera les réviseurs de la version précédente) :

   * (Facultatif) Remplacez le **Propriétaire** de la version par un autre utilisateur dans votre compte.

     Pour plus d’informations, voir [Profils d’autorisations d’épreuve dans Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * (Facultatif) Dans la zone **Saisir le nom du contact ou l’adresse e-mail pour ajouter un destinataire** ajoutez des réviseurs et des réviseuses à la version. Vous pouvez ensuite sélectionner un type **Rôle du BAT** et **Alertes par e-mail** pour chaque destinataire.

     Pour plus d’informations, voir [Ajouter des groupes à une épreuve](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md) et [Gérer les rôles d’épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

     >[!NOTE]
     >
     >Si le créateur ou le propriétaire de l’épreuve a désactivé par défaut l’e-mail Épreuve créée dans ses paramètres personnels, il ne recevra aucun e-mail Épreuve créée ou Nouvelle épreuve même si la case **Notifier les destinataires à propos de cette épreuve** est cochée sur la page Nouvelle épreuve. Pour plus d’informations, voir [Configuration des paramètres de notification par e-mail dans Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md), [E-mail créé pour l’épreuve](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) et [E-mail de nouvelle épreuve](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * (Facultatif) Définissez une date limite de BAT.

   * (Facultatif et conditionnel) Sélectionnez un nouveau décideur principal dans le menu déroulant **Transférer les droits de décision principaux vers**.

   * (Facultatif) Cochez la case **Une seule décision est requise pour cette étape** pour supprimer l’option permettant de définir un utilisateur comme nouveau décideur principal.

1. Dans la section **Notification par e-mail**, sélectionnez l’un des paramètres suivants :

   * (Facultatif) **Notifier les destinataires à propos de cette épreuve** : sélectionnez cette option pour notifier les réviseurs de la nouvelle version. Votre sélection sera consignée dans la section **Activité** de la page **Détails du BAT**. Pour plus d’informations, voir [Gérer les détails de l’épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * (Conditionnel et Facultatif) **Ajouter un objet et un message personnalisés** : sélectionnez cette option pour ajouter une ligne d’objet et un message personnalisés à la notification par e-mail.

1. Dans la section **Organisation**, sélectionnez l’un des paramètres suivants :

   * Appliquez une ou plusieurs balises à l’épreuve. Pour plus d’informations, voir [Créer et gérer des balises dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).

   * Ajoutez la version à un dossier. Le dossier sera copié à partir de la version précédente de l’épreuve. Si vous sélectionnez un autre dossier, l’ensemble de l’épreuve (qui comprend toutes les versions) est déplacé. Pour plus d’informations, voir [Gestion des dossiers dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

   * Les administrateurs et administratrices de facturation peuvent rendre le champ de dossier obligatoire pour l’ensemble du compte dans l’onglet **Paramètres**.

1. Dans la section **Paramètres de l’épreuve**, sélectionnez l’un des paramètres suivants :

   * Demander à un utilisateur de se connecter pour afficher l’épreuve.
   * Exiger des signatures électroniques sur le BAT (abonnement Entreprise uniquement).
   * Verrouillez l’épreuve lorsque toutes les décisions sont prises.
   * Autoriser le téléchargement du fichier original.
   * Autorisez le partage public de l’épreuve.
   * Autoriser l’abonnement au BAT.

     Les sélections effectuées dans cette section s’affichent dans la page **Détails du BAT** (où certains champs peuvent être modifiés). Pour plus d’informations, consultez la section [Gérer les détails d’une épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create a new version of a proof from the proofing viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new version from the proofing viewer</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof.</li>
<li value="2"> <p>Click the <strong>Version</strong> drop-down menu in the upper-left corner, then click <strong>+ New version</strong> in the box that appears.</p> <p>On the <strong>New proof version of</strong> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li>
<li value="3"> <p>Under <strong>Add files</strong>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <strong>browse</strong> and selecting the file you want. You can type a&nbsp;<strong>Proof name</strong>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
<br>
</note> </li>
<li value="4"> <p>Under <strong>Workflow</strong>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p>
<ul>
<li>Change the <strong>Owner</strong> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li>
<li> <p>Using the <strong>Type contact name or email address to add a recipient box</strong>, add reviewers to the version. You can specify a <strong>Proof role</strong> and an <strong>Email alerts</strong> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
If the creator or owner of&nbsp;&nbsp;the proof has
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see
<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
<br>
</note> </li>
<li>Set a proof deadline for the version.</li>
<li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li>
</ul> </li>
<li value="5">Under <strong>Email notification</strong>, do any of the following:
<ul>
<li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Proof activity section on the Proof details page.</li>
<li>Add a custom subject and message.</li>
</ul></li>
<li value="6">Under Proof settings, make any of the changes below:
<ul>
<li>Require login on the proof</li>
<li>Require electronic signatures on the proof (Enterprise plan only)</li>
<li>Lock the proof when all decisions are made</li>
<li>Allow or block download of original file</li>
<li>Public sharing of the proof,&nbsp;including public sharing settings</li>
<li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page.</li>
</ul></li>
</ol>
-->

## À propos des messages dans la nouvelle version

Si un objet ou un message personnalisé est inclus dans la version précédente de l’épreuve, il s’affiche par défaut sur la page Nouvelle version. Vous pouvez :

* Modifiez l’objet et le message.
* Désélectionnez la case « Notifier par e-mail ». Aucun e-mail n’est alors envoyé aux personnes chargées de votre révision pour les informer d’une nouvelle version à réviser.

  >[!NOTE]
  >
  >Aucun objet/message personnalisé par défaut enregistré dans vos paramètres personnels n’a d’incidence sur ce point.

Si un objet et un message par défaut sont enregistrés dans vos paramètres personnels, cela détermine le message affiché par défaut sur la page Nouvelle version :

* Si vous avez notifié vos réviseurs et réviseuses de la version précédente de l’épreuve à l’aide de l’e-mail standard (par exemple, aucun objet/message personnalisé), votre objet/message personnalisé par défaut (vos paramètres personnels) s’affichera sur la page Nouvelle version. Vous pouvez ensuite modifier l’objet et le message personnalisés ou désélectionner la case Notifier les personnes par e-mail , ce qui signifie qu’aucun e-mail ne sera envoyé à vos réviseurs pour les informer qu’ils disposent d’une nouvelle version à réviser.
* Si vous n’avez pas informé vos réviseurs de la version précédente de l’épreuve (par exemple, en l’absence d’e-mail standard ou personnalisé), la page Nouvelle version n’inclura pas de message par défaut. Pour notifier les personnes chargées de votre révision de la nouvelle version, cliquez sur le lien « Envoyer un message ». Vos objet/message personnalisés par défaut (selon vos paramètres personnels) s’affichent. Vous pouvez ensuite modifier l’objet et le message personnalisés selon vos besoins.

Si vous n’avez pas enregistré d’objet et de message par défaut dans vos paramètres personnels, le texte suivant s’affiche sur la nouvelle version :

* Si vous avez notifié vos réviseurs ou réviseuses de la version précédente de l’épreuve à l’aide de l’e-mail standard (par exemple, sans objet/message personnalisé), l’option Notifier les personnes par e-mail est sélectionnée par défaut sur la page Nouvelle version . Pour ajouter un message personnalisé, cliquez sur le lien.
* Si vous n’avez pas informé vos réviseurs de la version précédente de l’épreuve (par exemple, en l’absence d’e-mail standard ou personnalisé), la page Nouvelle version n’inclura aucun message par défaut. Pour notifier les personnes chargées de votre révision de la nouvelle version, cliquez sur le lien « Envoyer un message ». Vous pouvez ensuite ajouter un objet et un message personnalisés en cliquant sur le lien « Ajouter un message personnalisé ».
