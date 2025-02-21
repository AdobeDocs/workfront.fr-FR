---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Créer une version d’une épreuve
description: Gérer les commentaires sur plusieurs versions ou révisions d’un travail peut s’avérer être un énorme défi. Workfront simplifie ce processus en vous permettant de créer et de comparer plusieurs versions d’une épreuve.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1737'
ht-degree: 98%

---

# Créer une version d’une épreuve

Gérer les commentaires sur plusieurs versions ou révisions d’un travail peut s’avérer être un énorme défi. Workfront simplifie ce processus en vous permettant de créer et de comparer plusieurs versions d’une épreuve.

Tenez compte des informations suivantes lorsque vous créez une version d’une épreuve :

* Vous pouvez autoriser une personne à voir une version mais pas une autre. À l’inverse, si vous partagez une version ultérieure avec une personne, celle-ci ne peut pas voir les versions antérieures, sauf si vous revenez en arrière et accordez explicitement à la personne l’accès à ces versions antérieures.
* Pour créer une version d’une épreuve, vous devez disposer des droits de modification sur l’épreuve.

  Voir [Gérer les rôles des épreuves dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) et [Profils d’autorisations d’épreuves dans Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) pour obtenir plus d’informations sur qui dispose de droits de modification sur une épreuve.

  Pour plus d’informations sur le partage des versions d’une épreuve, voir [Partager une épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Si une épreuve est créée dans Adobe Workfront, toutes les nouvelles versions créées pour cette épreuve doivent également être créées dans Workfront. Vous ne pouvez pas créer de version d’une épreuve dans Workfront Proof si cette épreuve a été créée dans Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Plan actuel : Pro ou version supérieure</p> <p>ou</p> <p>Formule héritée : Select ou Premium</p> <p>Pour plus d’informations sur la relecture de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Plan hérité : n’importe lequel (la relecture doit être activée pour l’utilisateur ou l’utilisatrice)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander un accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation d’épreuve dont vous disposez, contactez votre équipe d’administration Workfront ou Workfront Proof.

+++

## Créer une version d’une épreuve dans Workfront

Il existe plusieurs façons de charger une nouvelle version d’épreuve dans Workfront. Les paramètres par défaut de l’épreuve peuvent être transférés ou non depuis la version précédente, selon la méthode que vous choisissez :

* **Générer automatiquement des épreuves lors du chargement de documents** : les paramètres par défaut de l’épreuve ne sont pas transférés. Si ce paramètre est activé dans votre profil d’utilisation, les paramètres par défaut de l’épreuve ne sont pas transférés lorsque vous faites glisser et déposez une nouvelle version.
* **Créer une épreuve > Simple** : les paramètres par défaut de l’épreuve ne sont pas transférés. Si vous sélectionnez Simple lors de la création d’une version d’épreuve, les paramètres par défaut de l’épreuve ne sont pas transférés de la version précédente.
* **Ajouter > Version > Épreuve** : les paramètres par défaut de l’épreuve sont transférés depuis la version précédente.
* **Créer une épreuve > Avancé** : les paramètres par défaut de l’épreuve sont transférés depuis la version précédente.

  <table>
  <tbody>
  <tr>
  <td>Générer des épreuves automatiquement lors du chargement de documents</td>
  <td>Les paramètres par défaut de l’épreuve ne sont pas transférés. Si ce paramètre est activé dans votre profil d’utilisation, les paramètres par défaut de l’épreuve ne sont pas transférés lorsque vous faites glisser et déposez une nouvelle version.</td>
  </tr>
  <tr>
  <td>Créer une épreuve &gt; Simple</td>
  <td>Les paramètres par défaut de l’épreuve ne sont pas transférés. Si vous sélectionnez Simple lors de la création d’une version d’épreuve, les paramètres par défaut de l’épreuve ne sont pas transférés de la version précédente.</td>
  </tr>
  <tr>
  <td>Ajouter &gt; Version &gt; Épreuve</td>
  <td>Les paramètres par défaut de l’épreuve sont transférés depuis la version précédente.</td>
  </tr>
  <tr>
  <td>Créer une épreuve &gt; Avancé</td>
  <td>Les paramètres par défaut de l’épreuve sont transférés depuis la version précédente.</td>
  </tr>
  </tbody>
  </table>




Pour créer une version d’une épreuve, procédez comme suit :

1. Ouvrez la liste des documents contenant l’épreuve.
1. À partir du système de fichiers de votre ordinateur, faites glisser et déposez un nouveau fichier sur l’épreuve.

   Ou

   Sélectionnez la ligne où l’épreuve est répertoriée, puis cliquez sur **Ajouter** > **Version**, puis cliquez sur l’option que vous souhaitez utiliser pour ajouter la nouvelle version de l’épreuve.

   ![Ajouter une nouvelle version](assets/add-new-version-350x185.png)

## Créer une version d’une épreuve à partir de la visionneuse de relecture (Workfront Proof uniquement)

Si vous utilisez la version autonome de Workfront Proof, vous pouvez créer une nouvelle version d’une épreuve contenant un seul fichier ou une capture web. 

>[!NOTE]
>
>Si votre compte est en formule Entreprise et que vous téléchargez plusieurs fichiers ou captures web, ils sont automatiquement combinés dans une seule nouvelle version. Veuillez consulter [Créer une épreuve de plusieurs pages](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) pour plus d’informations.

Pour créer une version d’une épreuve dans Workfront Proof :

1. Ouvrez l’épreuve.
1. Cliquez sur le menu déroulant de la **Version** dans le coin supérieur gauche, puis cliquez sur **+ Nouvelle version** dans la zone qui s’affiche.

   Sur la page **Nouvelle version de l’épreuve** qui s’affiche, vous pouvez voir tous les réviseurs et toutes réviseuses de la version précédente, y compris leurs rôles et leurs paramètres de notification par e-mail. Vous pouvez facilement modifier les rôles et notifications des réviseurs et réviseuses existants ou supprimer les réviseurs et réviseuses existants de la nouvelle version sur cette page.

1. Sous **Ajouter des fichiers**, chargez un fichier en tant que nouvelle version de l’épreuve en faisant un glisser-déposer depuis votre ordinateur ou en cliquant sur **parcourir** et en sélectionnant le fichier de votre choix. Vous pouvez saisir un **Nom d’épreuve** pour la version ou laissez ce champ vide pour utiliser le même nom de fichier avec un numéro de version ajouté à la fin.

   Ou

   Capturez une page web en tant que nouvelle version de l’épreuve en saisissant une URL.

   >[!NOTE]
   >
   >Le glisser-déposer est disponible uniquement avec les navigateurs qui prennent entièrement en charge HTML5. Cela exclut Internet Explorer 7 à 9 et Safari.

1. Sous **Workflow**, effectuez l’une des modifications suivantes pour spécifier les réviseurs et réviseuses pour cette version de l’épreuve.

   Les réviseurs et réviseuses de la version précédente sont remplacés par les réviseurs et réviseuses que vous ajoutez.

   * Modifiez la **Personne propriétaire** de la version en une autre personne de votre compte.\
     Pour plus d’informations sur les autorisations de la personne propriétaire, voir [Profils d’autorisations d’épreuve dans Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * En utilisant la **zone Saisir le nom ou l’adresse e-mail du contact auquel ajouter une personne destinataire**, ajoutez des réviseurs et des réviseuses à la version. Vous pouvez définir un **Rôle d’épreuve** et un type d’**Alertes par e-mail** pour chaque personne destinataire.

     Pour plus d’informations sur l’ajout de groupes à l’épreuve, voir [Ajouter des groupes à une épreuve](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md).Pour plus d’informations sur les rôles, voir [Gérer les rôles d’épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

     >[!NOTE]
     >
     >Si la personne créatrice ou propriétaire de l’épreuve a l’option [E-mail d’épreuve effectuée](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) désactivée par défaut (dans ses paramètres personnels), elle ne recevra aucun e-mail Épreuve ou Nouvelle épreuve, même si la case à cocher Notifier les personnes par e-mail est cochée sur la page de la nouvelle épreuve. Pour plus d’informations sur les notifications par e-mail, voir [Configurer les paramètres de notification par e-mail dans Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).Voir aussi [E-mail d’épreuve effectuée](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) et [E-mail de nouvelle épreuve](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * Définissez une date d’échéance pour la relecture pour la version.
   * Passez la souris sur le nom d’une personne réviseuse pour afficher les décisions qu’elle a prises sur une version précédente.

1. Sous **Notification par e-mail**, effectuez l’une des opérations suivantes :

   * Indiquez si vous souhaitez informer les réviseurs et réviseuses de la nouvelle version.\
     Votre sélection sera enregistrée dans la section Activité de la page de détails de l’épreuve. Pour plus d’informations, voir [Gérer les détails de l’épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * Ajoutez un objet et un message personnalisés.

1. Dans la section **Entreprise**, effectuez l’une des opérations suivantes :

   * Appliquez une ou plusieurs balises à l’épreuve. Pour plus d’informations, voir [Créer et gérer des balises dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
     Notez que les balises sont également héritées de la version précédente de l’épreuve. Si vous ajoutez une nouvelle balise à la nouvelle version, les versions précédentes sont également balisées.

   * Ajoutez la version à un dossier. Voir [Gérer les dossiers dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) pour plus d’informations. Le dossier sera copié à partir de la version précédente de l’épreuve. Si vous sélectionnez un autre dossier, l’épreuve entière (toutes les versions) sera déplacée.

   * Les administrateurs et administratrices de facturation et les équipes d’administration peuvent rendre le champ Dossier obligatoire pour l’ensemble du compte dans l’onglet Paramètres. Consultez pour plus d’informations.

1. Sous Paramètres de l’épreuve, effectuez l’une des modifications ci-dessous :

   * Exiger une connexion pour accéder à une épreuve
   * Exiger des signatures électroniques sur une épreuve (formule Entreprise uniquement)
   * Verrouiller une épreuve lorsque toutes les décisions sont prises.
   * Autoriser ou bloquer le téléchargement du fichier original
   * Partager publiquement l’épreuve, y compris les paramètres de partage public
   * Abonnement à l’épreuve\
     Les sélections effectuées dans cette section seront affichées dans la page de détails d’une épreuve (où certains champs peuvent être modifiés). Pour plus d’informations, consultez la section [Gérer les détails d’une épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

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

Si vous avez enregistré un objet et un message par défaut dans vos paramètres personnels, le message affiché par défaut sur la page Nouvelle version est affecté :

* Si vous choisissez de notifier les personnes chargées de votre révision de la version précédente de l’épreuve en utilisant un e-mail standard (par exemple, sans objet/message personnalisé), vos objet/message personnalisés par défaut (vos paramètres personnels) s’affichent sur la page Nouvelle version. Vous pouvez ensuite modifier l’objet et le message personnalisé ou désélectionner la case de notification des personnes par e-mail (aucun e-mail n’est alors envoyé aux personnes chargées de votre révision pour les informer d’une nouvelle version à réviser).
* Si vous choisissez de ne pas notifier les personnes chargées de votre révision de la version précédente de l’épreuve par e-mail standard (par exemple, pas d’e-mail standard ou personnalisé), la nouvelle version n’inclut pas de message par défaut. Pour notifier les personnes chargées de votre révision de la nouvelle version, cliquez sur le lien « Envoyer un message ». Vos objet/message personnalisés par défaut (selon vos paramètres personnels) s’affichent. Vous pouvez ensuite modifier l’objet et le message personnalisés si nécessaire.

Si vous n’avez pas enregistré d’objet et de message par défaut dans vos paramètres personnels, le texte suivant s’affiche sur la nouvelle version :

* Si vous choisissez de notifier les personnes chargées de votre révision de la version précédente de l’épreuve en utilisant un e-mail standard (par exemple, sans objet/message personnalisé), l’option de notification des personnes par e-mail est sélectionnée par défaut sur la page Nouvelle version. Pour ajouter un message personnalisé, cliquez sur le lien.
* Si vous choisissez de ne pas notifier les personnes chargées de votre révision de la version précédente de l’épreuve par e-mail standard (par exemple, pas d’e-mail standard ou personnalisé), la nouvelle version n’inclut pas de message par défaut. Pour notifier les personnes chargées de votre révision de la nouvelle version, cliquez sur le lien « Envoyer un message ». Vous pouvez ensuite ajouter un objet et un message personnalisés en cliquant sur le lien « Ajouter un message personnalisé ».
