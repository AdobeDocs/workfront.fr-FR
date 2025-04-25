---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Créer une épreuve avancée avec un workflow de base
description: Avec un workflow de base, vous pouvez créer plusieurs réviseurs et réviseuses sur une épreuve, mais ils ne sont pas organisés par étapes. Toutes les personnes chargées de la révision que vous ajoutez peuvent accéder à l’épreuve dès que vous l’avez créée.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 99%

---

# Créer une épreuve avancée avec un workflow de base

<!-- Audited: 1/2024 -->

Avec un workflow de base, vous pouvez créer plusieurs réviseurs et réviseuses sur une épreuve, mais ils ne sont pas organisés par étapes. Toutes les personnes chargées de la révision que vous ajoutez peuvent accéder à l’épreuve dès que vous l’avez créée.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>
   <p>Nouveau : Tous</p>
    <p>Plan actuel : Pro ou version supérieure</p>
   <p>Plan hérité : Select ou supérieur</p> <p>Pour plus d’informations sur la relecture de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
    <p>Actuelle : Travail ou Plan</p> <p>Plan hérité : n’importe lequel (la relecture doit être activée pour l’utilisateur ou l’utilisatrice)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux documents</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation d’épreuve dont vous disposez, contactez votre administrateur ou administratrice Workfront ou Workfront Proof.

+++

## Créer une épreuve avancée avec un workflow de base

1. Accédez à l’élément (projet, tâche ou problème) pour lequel vous souhaitez obtenir l’épreuve, puis cliquez sur l’onglet **Documents**.
1. Cliquez sur **Ajouter** > Épreuve, chargez le contenu, puis parcourez les sections répertoriées ci-dessous.

   ou

   Pointez sur un document existant, puis cliquez sur **Créer une épreuve** > **Épreuve avancée** et parcourir les sections répertoriées ci-dessous.

## Configurer le workflow et ajouter des réviseurs et réviseuses

1. Dans la section Type de workflow, choisissez **De base**.
1. Indiquez les utilisateurs et utilisatrices à ajouter, puis choisissez un rôle d’épreuve.

   ![Nouveaux rôles de BAT](assets/new-proof---roles-350x213.png)

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
      <th> <p><strong>Afficher une épreuve</strong> </p> </th> 
      <th> <p><strong>Ajouter des balises</strong> </p> </th> 
      <th> <p><strong>Ajouter des commentaires</strong> </p> </th> 
      <th> <p><strong>Modifier ses propres commentaires en l’absence de réponse</strong> </p> </th> 
      <th> <p><strong>Prendre une décision</strong> </p> </th> 
      <th> <p><strong>Supprimer des commentaires d’autres personnes</strong> </p> </th> 
      <th>Résoudre les commentaires</th> 
      <th>Appliquer des actions aux commentaires</th> 
      <th> <p><strong>Modifier l’épreuve</strong> </p> </th> 
      <th>Partager l’épreuve</th> 
      <th>Créer une nouvelle version</th> 
      <th> <p><strong>Afficher les demandes d’approbation dans la zone d’accueil</strong> </p> </th> 
      <th>Ajouter de nouveaux réviseurs et réviseuses</th> 
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
      <td> <p><strong>Réviseur et réviseuse, approbateur et approbatrice</strong> </p> </td> 
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
      <td> <p><strong>Auteur et autrice</strong> </p> </td> 
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

1. Les personnes disposant des nouveaux plans Workfront peuvent accorder des rôles de création ou de modération à n’importe quelle personne du système. Les personnes utilisant les plans hérités peuvent accorder des rôles de création ou de modération aux utilisateurs et utilisatrices disposant d’une licence de relecture dans le système.
1. (Facultatif) Avec le menu déroulant toujours ouvert, sélectionnez les autorisations supplémentaires disponibles en bas du menu :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Résoudre les commentaires et appliquer des actions </td> 
      <td> <p>Permet aux utilisateurs et utilisatrices de Workfront d’effectuer les opérations suivantes :</p> 
       <ul> 
        <li>Résolvez un commentaire une fois qu’il a été traité, en suivant la procédure décrite à la section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Résoudre les commentaires d’épreuve</a>.</li> 
        <li>Appliquez des actions aux commentaires, en suivant la procédure décrite à la section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Utiliser des actions sur les commentaires d’épreuve</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partager l'épreuve par balisage</td> 
      <td> <p>Permet au réviseur ou à la réviseuse d’ajouter n’importe quel utilisateur ou utilisatrice Workfront à l’épreuve, comme expliqué dans la section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Identifier des utilisateurs et utilisatrices pour partager une épreuve</a>.</p> <p>Note :  <p>Si ces deux options ne sont pas disponibles (grisées), l’utilisateur ou l’utilisatrice dispose déjà d’un profil d’autorisation lui permettant de résoudre les commentaires, d’appliquer des actions aux commentaires et de taguer une personne. </p> <p>Si les options ne s’affichent pas, la personne que vous avez ajoutée n’est pas titulaire d’une licence Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Répétez les étapes 1 à 3 pour tous les autres utilisateurs et utilisatrices que vous avez ajoutés à l’épreuve.
1. Pour chaque personne avec vous partagez l’épreuve, dans la liste déroulante **Alertes par e-mail**, sélectionnez le type d’alerte par e-mail qu’elle reçoit lorsqu’elle écrit des commentaires et prend des décisions sur l’épreuve :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toutes les activités</td> 
      <td>Workfront envoie un e-mail au réviseur ou à la réviseuse chaque fois qu’il y a une activité sur l’épreuve, comme un nouveau commentaire, une nouvelle réponse ou une nouvelle décision. <p>Il s’agit d’une excellente option pour la personne qui gère le processus de relecture, car elle lui permet de voir l’activité au fur et à mesure qu’elle se produit. </p><p>Les personnes ne reçoivent pas d’alerte par e-mail sur leur propre activité.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Réponses à mes commentaires</td> 
      <td>Un e-mail n’est envoyé à la personne réviseuse que si quelqu’un répond explicitement à son commentaire (cela exclut ses propres réponses sur ses propres commentaires). Cela signifie que si quelqu’un fait un nouveau commentaire sur l’épreuve, la personne réviseuse n’en est pas informée.<p>Ce paramètre est recommandé pour vos clientes et clients sur l’épreuve afin qu’ils ne soient pas informés des autres commentaires sur l’épreuve et qu’ils ne soient informés que des réponses à leurs propres commentaires.</p><p>Bien que les personnes réviseuses ne soient pas informées des autres nouveaux commentaires avec ce paramètre d’alerte par e-mail, elles peuvent toujours afficher tous les commentaires sur l’épreuve dans la visionneuse de relecture.</p><p>Pour plus d’informations sur les commentaires, voir la section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Afficher les commentaires de l’épreuve et y répondre</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décisions</td> 
      <td>Workfront n’envoie un e-mail à la personne chargée de la révision que lorsqu’une personne prend une décision.<p>Cette fonctionnalité peut s’avérer utile pour la personne chargée de la gestion du processus d’approbation (par exemple, une personne responsable du projet) et qui doit surveiller la progression de l’épreuve et vérifier quels utilisateurs et utilisatrices ont pris leur décision.</p><p>Vous ne recevez pas de notification au sujet de votre propre décision, sauf si vous sélectionnez une option de confirmation par e-mail lors de la soumission de votre décision.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décision finale</td> 
      <td>Workfront envoie un e-mail lorsque la dernière personne chargée de l’approbation de l’épreuve a pris sa décision.<p>Cette alerte est souvent utilisée par le concepteur ou la conceptrice, qui n’a généralement pas besoin de prendre part à la discussion de révision en elle-même. Lorsque la décision finale est prise, le concepteur ou la conceptrice reçoit une notification et peut alors agir sur les modifications nécessaires.</p><p>Cette alerte peut également s’avérer utile pour une personne responsable de service qui n’a besoin d’être avertie que lorsque le processus de révision est achevé.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résumé horaire</td> 
      <td>Toutes les heures, Workfront envoie un e-mail à la personne chargée de la révision contenant un résumé de tous les commentaires, réponses et décisions survenus au cours de l’heure.<p>L’e-mail n’est envoyé que lorsqu’une activité autre que la vôtre s’est produite au cours de la dernière heure. </p><p>Cette alerte est une bonne manière d’avoir une vue d’ensemble du projet.</p><p>Un exemple de cas d’utilisation pour ce résumé est celui d’une personne expérimentée dans la révision qui a besoin d’une vue d’ensemble du projet, mais qui n’a pas besoin d’être informée de toute l’activité sur l’épreuve dans l’immédiat.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résumé quotidien</td> 
      <td>Workfront envoie un e-mail contenant tous les commentaires, réponses et décisions répertoriés uniquement les jours où se produit une activité différente de la vôtre.<p>Cette alerte est une bonne façon de voir un résumé du projet sans se laisser submerger par plusieurs mises à jour tout au long de la journée.</p><p>Un exemple de cas d’utilisation pour ce résumé est celui d’une personne gestionnaire de service qui souhaite surveiller la progression globale du projet.</p><p>Pour plus d’informations, voir la section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gérer les notifications pour les commentaires et les décisions relatifs aux épreuves</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Aucun e-mail</td> 
      <td>Workfront n’envoie aucune alerte par e-mail.<br>Cela se révèle utile pour une personne qui n’est ajoutée à une épreuve qu’à titre de référence et qui n’a pas besoin d’être informée des modifications.<p>La valeur par défaut du système est Résumé quotidien (également appelé Non défini). Si vous ou vos réviseurs et réviseuses n’effectuez aucune autre modification, toutes vos épreuves disposent de ce paramètre.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Passez à [Configurer les paramètres d’e-mail pour l’épreuve](#configure-email-settings-for-the-proof) ci-dessous.

## Configurer les paramètres d’e-mail de l’épreuve {#configure-email-settings-for-the-proof}

1. Dans la section **Notification par e-mail**, choisissez si vous souhaitez envoyer des notifications par e-mail et un message personnalisé aux personnes que vous avez sélectionnées dans [Créer une épreuve avancée avec un workflow de base](#workflow) plus haut dans cet article :

   <table>
   <tbody>
   <tr>
   <td>Informer les personnes destinataires de l’épreuve</td>
   <td>Sélectionnez cette option pour envoyer une notification par e-mail aux utilisateurs et utilisatrices. Lorsque <strong>Partage de base</strong> est sélectionné dans la section <strong>Workflow</strong>, une notification par e-mail est envoyée lors de la création de l’épreuve. Lorsque <strong>Workflow automatisé</strong> est sélectionné dans la section <strong>Workflow</strong>, une notification par e-mail est envoyée lorsque l’épreuve entre dans l’étape du workflow automatisé auquel la personne est associée.</td>
   </tr>
   <tr>
   <td>Ajouter un message personnalisé</td>
   <td>Sélectionnez cette option pour inclure un message personnalisé dans la notification. Vous pouvez spécifier un objet et un corps de message. Le corps du message peut inclure une mise en forme en texte enrichi (gras, puces et liens hypertexte).</td>
   </tr>
   </tbody>
   </table>


1. Passez à [Configurer les paramètres de l’épreuve](#configure-proof-settings) ci-dessous.

## Configurer les paramètres de l’épreuve {#configure-proof-settings}

1. Dans la section **Paramètres de l’épreuve**, sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Connexion requise : l’épreuve ne peut être partagée qu’avec d’autres utilisateurs et utilisatrices.</td> 
      <td>Lorsque cette option est désactivée (par défaut), toute personne disposant de l’URL peut afficher l’épreuve. <br>Lorsque cette option est sélectionnée, ce qui suit s’applique :
       <ul>
        <li>Seuls les utilisateurs et utilisatrices de Workfront Proof peuvent afficher l’épreuve.</li>
        <li>Les utilisateurs et utilisatrices ne peuvent pas se connecter à l’épreuve à moins qu’ils n’aient été ajoutés à l’épreuve.</li>
        <li>Les abonnements ne peuvent pas être activés.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Une seule décision requise pour cette épreuve</td> 
      <td>Lorsque cette option est sélectionnée, la révision est terminée une fois que l’une des personnes décisionnaires a pris sa décision.<br>Cette option est désactivée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exiger que les décisions soient signées de manière électronique</td> 
      <td>Les utilisateurs et utilisatrices doivent indiquer leur nom d’utilisateur ou d’utilisatrice et leur mot de passe au moment où ils prennent une décision sur une épreuve.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller l’épreuve lorsque toutes les décisions requises sont prises.</td> 
      <td>Lorsque ce paramètre est activé, l’état de l’épreuve est verrouillé une fois toutes les décisions prises. L’état passe automatiquement de déverrouillé à verrouillé lorsque la dernière personne chargée de l’approbation prend sa décision.<br>Cette option est désactivée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Télécharger le fichier original</td> 
      <td>Lorsque cette option est sélectionnée, les réviseurs et réviseuses peuvent télécharger le fichier original à partir duquel l’épreuve a été créée.<br>Si cette option est désélectionnée, l’icône Télécharger n’est plus visible.<br>Cette option est activée par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partager l’épreuve via une URL publique ou un code intégré</td> 
      <td>Lorsque cette option est sélectionnée, l’épreuve peut être partagée via une URL publique ou un code intégré.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">S’abonner à l’épreuve via une URL publique ou un code intégré</td> 
      <td>Lorsque cette option est sélectionnée, les personnes qui n’ont pas été explicitement ajoutées à l’épreuve peuvent s’y abonner. La personne qui s’abonne à l’épreuve se voit attribuer le rôle et l’adresse e-mail que vous définissez dans les paramètres suivants :
       <ul>
        <li><strong>Rôle de personne abonnée :</strong> rôle par défaut pour l’épreuve affecté à toutes les personnes chargées de la révision qui s’abonnent à l’épreuve.</li>
        <li><strong>Paramètres des alertes par e-mail pour les personnes abonnées :</strong> alerte e-mail par défaut qui est affectée à toutes les personnes chargées de la révision qui s’abonnent à l’épreuve.</li>
       </ul><p>
        <ul>
         <li><strong>Un accès à l’épreuve via un lien e-mail requis pour :</strong> Indiquez si la personne abonnée reçoit un e-mail avec un lien vers l’épreuve. Vous pouvez sélectionner <strong>Aucun e-mail</strong> (aucun lien d’e-mail n’est nécessaire pour accéder à l’épreuve), <strong>E-mail de notification de l’épreuve uniquement</strong> (la personne abonnée reçoit un lien vers l’épreuve par e-mail sans vérification), ou <strong>E-mails de validation et de notification de l’épreuve</strong> (la personne abonnée reçoit un lien vers l’épreuve par e-mail et doit cliquer sur le lien pour accéder à une épreuve ; l’objectif de cette option est de s’assurer que la personne a saisi une adresse e-mail correcte à laquelle elle a accès).</li>
        </ul><p>Note : si un workflow automatisé est joint aux épreuves, tous les abonnements génèrent des e-mails de confirmation pour les personnes propriétaires des épreuves, afin qu’elles puissent décider à quelle étape la personne doit être ajoutée.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Créer une épreuve**.

   Workfront commence à générer une épreuve des documents ou des sites web sélectionnés.Selon la taille et le type du fichier, le délai de chargement d’un document peut varier. Faites preuve de patience, car la génération de fichiers volumineux prend plus de temps. Vous pouvez quitter la page et Workfront continue à générer votre fichier.La taille maximale du chargement de fichier est de 4 Go.

1. Une fois l’épreuve générée, cliquez sur **Ouvrir l’épreuve** pour lancer la visionneuse de relecture.

   ![Ouvrir l&#39;épreuve](assets/open-proof-350x132.png)

   Les personnes pour qui la vérification du compte n’est pas activée peuvent toujours afficher le document et effectuer des commentaires sur l’épreuve.
