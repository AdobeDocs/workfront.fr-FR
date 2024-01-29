---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Créer un BAT avancé avec un workflow de base
description: Avec un workflow de base, vous pouvez créer plusieurs validants sur un BAT, mais ils ne sont pas organisés par étapes. Tous les opérateurs validants que vous ajoutez peuvent accéder au BAT immédiatement après sa création.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: d71ee30378c39975366f4f257e3f7b17aba0c0ae
workflow-type: tm+mt
source-wordcount: '1842'
ht-degree: 1%

---

# Créer un BAT avancé avec un workflow de base

<!-- Audited: 1/2024 -->

Avec un workflow de base, vous pouvez créer plusieurs validants sur un BAT, mais ils ne sont pas organisés par étapes. Tous les opérateurs validants que vous ajoutez peuvent accéder au BAT immédiatement après sa création.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>
   <p>Nouveau : Quelconque</p>
    <p>Formule actuelle : Pro ou supérieure</p>
   <p>Formule héritée : sélection ou supérieure</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
    <p>Actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Modifier l’accès aux documents</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront BAT.

## Créer un BAT avancé avec un workflow de base

1. Accédez au projet, à la tâche ou au problème pour lequel vous souhaitez obtenir le BAT, puis cliquez sur le bouton **Documents** .
1. Cliquez sur **Ajouter** > Bon à tirer, téléchargez le contenu, puis parcourez les sections répertoriées ci-dessous.

   ou

   Passez la souris sur un document existant, puis cliquez sur l’icône **Créer un bon à tirer** > **Bon à tirer avancé** et parcourir les sections répertoriées ci-dessous.

## Configurer le workflow et ajouter les opérateurs validants

1. Dans la section Type de workflow , choisissez **De base**.
1. Indiquez les utilisateurs à ajouter, puis choisissez un rôle Bon à tirer .

   ![](assets/new-proof---roles-350x213.png)

1. Le tableau suivant répertorie chaque rôle et les droits qui lui sont associés.

   <table border="1" cellspacing="15" cellpadding="1"> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p> </p> </th> 
      <th> <p><strong>Afficher un bon à tirer</strong> </p> </th> 
      <th> <p><strong>Ajouter des balises</strong> </p> </th> 
      <th> <p><strong>Ajouter des commentaires</strong> </p> </th> 
      <th> <p><strong>Modifier ses propres commentaires en l’absence de réponse</strong> </p> </th> 
      <th> <p><strong>Prendre une décision</strong> </p> </th> 
      <th> <p><strong>Supprimer les commentaires d’autres utilisateurs</strong> </p> </th> 
      <th>Résoudre les commentaires</th> 
      <th>Application d’actions aux commentaires</th> 
      <th> <p><strong>Modifier le BAT</strong> </p> </th> 
      <th>Partager le BAT avec les autres</th> 
      <th>Créer une version</th> 
      <th> <p><strong>Affichage des demandes d’approbation dans la zone d’accueil</strong> </p> </th> 
      <th>Ajouter de nouveaux opérateurs validants</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>Lecture seule</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Réviseur</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Approbateur</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Réviseur et approbateur</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Auteur</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> </td> 
      <td>✓</td> 
     </tr> 
     <tr> 
      <td> <p><strong>Modérateur</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p><strong>✓</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
     </tr> 
    </tbody> 
   </table>

1. Les utilisateurs des nouveaux plans Workfront peuvent accorder des rôles d’auteur ou de modérateur à n’importe quel utilisateur du système. Les utilisateurs sur les plans hérités peuvent accorder des rôles d’auteur ou de modérateur à tout utilisateur disposant d’une licence de BAT dans le système.
1. (Facultatif) Avec le menu déroulant toujours ouvert, sélectionnez les autorisations supplémentaires disponibles en bas du menu :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Résoudre les commentaires et appliquer des actions </td> 
      <td> <p>Permet à l’utilisateur de Workfront d’effectuer les opérations suivantes :</p> 
       <ul> 
        <li>Résolvez un commentaire une fois qu’il a été traité, en suivant la procédure décrite à la section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Résoudre les commentaires de BAT</a>.</li> 
        <li>Appliquez les actions aux commentaires, en suivant la procédure décrite à la section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Utilisation d’actions sur les commentaires du BAT</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partager l'épreuve par balisage</td> 
      <td> <p>Permet au réviseur d’ajouter n’importe quel utilisateur Workfront au BAT, comme expliqué dans la section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Balisage des utilisateurs pour partager un BAT</a>.</p> <p>Remarque :  <p>Si ces deux options ne sont pas disponibles (grisées), l’utilisateur dispose déjà d’un profil d’autorisation lui permettant de résoudre les commentaires, d’appliquer des actions aux commentaires et de baliser n’importe quel utilisateur. </p> <p>Si les options ne s’affichent pas, la personne que vous avez ajoutée n’est pas titulaire de licence Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Répétez les étapes 1 à 3 pour tous les autres utilisateurs que vous avez ajoutés au BAT.
1. Pour chaque utilisateur que vous partagez, dans la variable **Alertes par email** dans la liste déroulante, sélectionnez le type d&#39;alerte par email que reçoit cet utilisateur lorsqu&#39;il fait des commentaires et prend des décisions sur le BAT :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toutes les activités</td> 
      <td>Workfront envoie un email au réviseur chaque fois qu’il y a une activité sur le BAT, comme un nouveau commentaire, une nouvelle réponse ou une nouvelle décision. <p>Il s’agit d’une excellente option pour la personne qui gère le processus de vérification car elle lui permet de voir l’activité telle qu’elle se produit. </p><p>Les utilisateurs ne reçoivent pas d’alerte par e-mail sur leur propre activité.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Réponses à mes commentaires</td> 
      <td>Un email n'est envoyé au validant que si quelqu'un répond explicitement à son commentaire (cela exclut ses propres réponses sur ses propres commentaires). Cela signifie que si quelqu'un sur le BAT fait un nouveau commentaire, le validant n'en est pas informé.<p>Ce paramètre est recommandé pour vos clients sur le BAT afin qu’ils ne soient pas informés des autres commentaires sur le BAT et qu’ils ne soient informés que des réponses à leurs propres commentaires.</p><p>Bien que les réviseurs avec ce paramètre d’alerte par e-mail ne soient pas informés des autres nouveaux commentaires, ils peuvent toujours afficher tous les commentaires sur le BAT dans la visionneuse de vérification.</p><p>Pour plus d’informations sur les commentaires, voir <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Afficher et répondre aux commentaires du BAT</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décisions</td> 
      <td>Workfront n’envoie un courrier électronique au réviseur que lorsqu’une personne prend une décision.<p>Cela peut s’avérer utile pour la personne qui gère le processus de validation (par exemple, un chef de projet) et qui doit surveiller l’avancement du BAT et voir quels utilisateurs ont pris leur décision.</p><p>Vous n’êtes pas informé de votre propre décision, sauf si vous sélectionnez une option de confirmation par courrier électronique lors de l’envoi de votre décision.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décision finale</td> 
      <td>Workfront envoie un courrier électronique lorsque le dernier approbateur du BAT a pris sa décision.<p>Cette alerte est souvent utilisée par le concepteur, qui n’a généralement pas besoin de prendre part à la discussion de révision proprement dite. Lorsque la décision finale est prise, le concepteur est informé et peut alors prendre des mesures sur les modifications nécessaires.</p><p>Cette alerte peut également s’avérer utile pour un responsable de service qui n’a besoin d’être averti que lorsque le processus de révision est terminé.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résumé horaire</td> 
      <td>Workfront envoie au réviseur un courrier électronique toutes les heures contenant un résumé de tous les commentaires, réponses et décisions survenus au cours de l’heure.<p>L’e-mail n’est envoyé que lorsque l’activité se produit au-delà de la vôtre au cours de la dernière heure. </p><p>Cette alerte est une bonne manière de visualiser un aperçu du projet.</p><p>Un exemple de cas d’utilisation pour ce résumé est un validant principal qui a besoin d’une vue d’ensemble du projet, mais qui n’a pas besoin d’être informé immédiatement de toute l’activité sur le BAT.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résumé quotidien</td> 
      <td>Workfront envoie un email contenant tous les commentaires, réponses et décisions répertoriés uniquement les jours où il y a une activité en dehors de la vôtre.<p>Cette alerte est une bonne façon de voir un résumé du projet sans être submergé par de multiples mises à jour tout au long de la journée.</p><p>Un exemple de cas d’utilisation pour ce résumé est un chef de département qui souhaite surveiller l’avancement global du projet.</p><p>Pour plus d’informations, voir <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestion des notifications pour les commentaires et les décisions de BAT</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Aucun email</td> 
      <td>Workfront n’envoie aucune alerte par courrier électronique.<br>Cela s’avère utile pour une personne qui n’est ajoutée à un BAT qu’à titre de référence et qui n’a pas besoin d’être informée des modifications.<p>La valeur par défaut du système est Résumé quotidien (également appelé Non défini). Si vous ou vos réviseurs n’effectuez aucune autre modification, tous vos BAT disposent de ce paramètre.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Passez à la [Configuration des paramètres de courrier électronique pour le BAT](#configure-email-settings-for-the-proof) ci-dessous

## Configuration des paramètres de courrier électronique pour le BAT {#configure-email-settings-for-the-proof}

1. Dans le **Notification par email** , choisissez d’envoyer des notifications par e-mail et un message personnalisé aux utilisateurs que vous avez sélectionnés dans [Créer un BAT avancé avec un workflow de base](#workflow) plus tôt dans cet article :

   <table>
   <tbody>
   <tr>
   <td>Informer les destinataires de ce BAT</td>
   <td>Sélectionnez cette option pour envoyer une notification électronique aux utilisateurs. When <strong>Partage de base</strong> est sélectionné dans la variable <strong>Workflow</strong> , une notification électronique est envoyée lors de la création du BAT. When <strong>Processus automatisé</strong> est sélectionné dans la variable <strong>Workflow</strong> , une notification par e-mail est envoyée lorsque le BAT entre dans l’étape du workflow automatisé auquel l’utilisateur est associé.</td>
   </tr>
   <tr>
   <td>Ajout d’un message personnalisé</td>
   <td>Sélectionnez cette option pour inclure un message personnalisé dans la notification. Vous pouvez spécifier un objet et un corps de message. Le corps du message peut inclure une mise en forme en texte enrichi (gras, puces et liens hypertexte).</td>
   </tr>
   </tbody>
   </table>


1. Passez à la [Configuration des paramètres du BAT](#configure-proof-settings) ci-dessous

## Configuration des paramètres du BAT {#configure-proof-settings}

1. Dans le **Paramètres de BAT** sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Connexion requise : le BAT ne peut être partagé qu’avec d’autres utilisateurs.</td> 
      <td>Lorsque cette option est désactivée (par défaut), toute personne disposant de l’URL peut afficher le BAT. <br>Lorsque cette option est sélectionnée :
       <ul>
        <li>Seuls les utilisateurs du BAT Workfront peuvent afficher le BAT.</li>
        <li>Les utilisateurs ne peuvent pas se connecter au BAT à moins qu’ils n’aient été ajoutés au BAT.</li>
        <li>Les abonnements ne peuvent pas être activés.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Une seule décision requise pour ce BAT</td> 
      <td>Lorsque cette option est sélectionnée, la révision est terminée une fois que l’un des décideurs a pris sa décision.<br>Cette option est désactivée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exiger que les décisions soient signées de manière électronique</td> 
      <td>Les utilisateurs doivent indiquer leur nom d’utilisateur et leur mot de passe au moment où ils prennent une décision sur un BAT.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller le BAT lorsque toutes les décisions requises sont prises</td> 
      <td>Lorsque ce paramètre est activé, l’état du BAT est verrouillé une fois toutes les décisions prises. L’état est automatiquement modifié du déverrouillé au verrouillé lorsque l’approbateur final prend sa décision.<br>Cette option est désactivée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Télécharger le fichier d’origine</td> 
      <td>Lorsque cette option est sélectionnée, les réviseurs peuvent télécharger le fichier d'origine à partir duquel le BAT a été créé.<br>Si cette option est désélectionnée, l’icône Télécharger n’est plus visible.<br>Cette option est activée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partage du BAT via une URL publique ou un code intégré</td> 
      <td>Lorsque cette option est sélectionnée, le BAT peut être partagé via une URL publique ou un code intégré.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abonnez-vous au BAT via une URL publique ou un code intégré</td> 
      <td>Lorsque cette option est sélectionnée, les personnes qui n’ont pas été explicitement ajoutées au BAT peuvent s’abonner au BAT. La personne qui s'abonne au BAT se voit attribuer le rôle et l'email que vous définissez dans les paramètres suivants :
       <ul>
        <li><strong>Rôle d’abonné :</strong> Le rôle de BAT par défaut attribué à tous les réviseurs qui souscrivent au BAT. </li>
        <li><strong>Paramètres des alertes par email pour les abonnés :</strong> L’alerte par défaut qui est affectée à tous les réviseurs qui souscrivent au BAT.</li>
       </ul><p>
        <ul>
         <li><strong>Un accès BAT via un lien email requis pour :</strong> Indiquez si l'abonné reçoit un email avec un lien vers le BAT. Vous pouvez sélectionner <strong>Aucun email</strong> (aucun lien d'email n'est nécessaire pour accéder au BAT), <strong>Email de notification de BAT uniquement</strong> (l'abonné reçoit un lien vers le BAT par email sans vérification), ou <strong>Emails de validation et de notification de BAT</strong> (l'abonné reçoit un lien vers le BAT par email et doit cliquer sur le lien pour accéder à un BAT, l'objectif de cette option est de s'assurer que la personne a saisi une adresse email correcte à laquelle elle a accès).</li>
        </ul><p>Remarque : Si le workflow automatisé est joint aux bons à tirer, tous les abonnements génèrent des emails de confirmation pour les propriétaires du BAT, afin qu’ils puissent décider à quelle étape la personne doit être ajoutée.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Créer un bon à tirer**.

   Workfront commence à générer un bon à tirer des documents ou des sites Web sélectionnés. Selon la taille et le type du fichier, le délai de téléchargement d’un document peut varier. Soyez patient car la génération de fichiers plus volumineux prend plus de temps. Vous pouvez quitter la page et Workfront continue à générer votre fichier. La taille maximale du téléchargement de fichier est de 4 Go.

1. Une fois le BAT généré, cliquez sur **BAT ouvert** pour lancer la visionneuse de vérification.

   ![](assets/open-proof-350x132.png)

   Les utilisateurs dont le compte ne contient pas de vérification peuvent toujours afficher le document et envoyer des commentaires au BAT.