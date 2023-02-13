---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Partage d’un BAT à partir de la visionneuse de vérification
description: Vous pouvez partager un BAT à partir de la visionneuse de vérification si le partage est activé par le propriétaire ou le créateur du BAT.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# Partage d’un BAT à partir de la visionneuse de vérification

Vous pouvez partager un BAT à partir de la visionneuse de vérification si le partage est activé par le propriétaire ou le créateur du BAT.

>[!IMPORTANT]
>
>Le paramètre Autoriser le partage du BAT via une URL publique ou le code incorporé doit être activé.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou version ultérieure</p> <p>ou</p> <p>Plan hérité : Sélectionner ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Travail ou plan</p> <p>Plan hérité : N’importe quel (la vérification doit être activée pour l’utilisateur)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront BAT.

## Partage de l’URL

Vous pouvez partager un BAT via une URL si le propriétaire a configuré le BAT pour le partage. Les propriétaires de BAT peuvent mettre à jour les paramètres de partage à tout moment. Pour plus d’informations, voir [Modification des paramètres du BAT](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Si le menu de l’icône de gauche n’est pas affiché, cliquez sur le bouton **Menu** dans le coin supérieur gauche de la visionneuse de vérification.

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. Dans le menu d’icône de gauche de la visionneuse de vérification, cliquez sur le bouton **Partager** icône .

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. Dans le **Partager le BAT** options qui s’affichent, veillez à **Obtenir un lien partageable** est sélectionnée.

1.  Effectuez l’une des opérations suivantes :

   * Pour copier le lien dans le presse-papiers, cliquez sur **Copier le lien**.

      Vous pouvez désormais diffuser le lien par le biais d&#39;un outil tiers, tel qu&#39;une messagerie instantanée ou une application de messagerie.

   * Pour envoyer le lien directement par courrier électronique à partir d’Adobe Workfront, procédez comme suit :

      1. Dans le **Ou lien de courrier électronique vers** , commencez à taper et sélectionnez le nom de votre destinataire. Vous pouvez également spécifier l’adresse électronique d’un utilisateur externe avec lequel vous souhaitez effectuer un partage.

         >[!NOTE]
         >
         >Si vous voyez un email d’alias lors du partage d’un BAT, ne créez pas un nouvel utilisateur invité en saisissant l’email d’origine s’il existe un email d’alias correspondant.

      1. Sélectionnez l’une des options suivantes :

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Envoyer le lien public</td>
            <td><p>Inclut un bouton dans la notification électronique qui dirige les utilisateurs vers le BAT dans la visionneuse de vérification qu’ils utilisent et leur accorde l’accès en mode Vue.</p><p>If <strong>Abonnez-vous au BAT via une URL publique ou un code intégré</strong> est désactivée pour le BAT, les utilisateurs peuvent se connecter à l’aide de leurs identifiants de connexion Workfront pour ajouter des commentaires au BAT. Si elle est activée, toute personne fournissant son adresse électronique et son nom (aucun mot de passe requis) peut signer et ajouter des commentaires au BAT.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Envoyer le lien de téléchargement</td>
            <td>Inclut un bouton dans la notification électronique qui dirige les utilisateurs vers une page de téléchargement, qui fournit les détails du fichier, le nom du fichier et la taille du fichier, avec le fichier affiché en ligne. Les utilisateurs peuvent cliquer sur le lien Télécharger de la page de téléchargement pour télécharger le fichier.</td>
           </tr>
           <tr>
            <td role="rowheader">Ajout d’un message personnalisé</td>
            <td>Permet de spécifier l’objet et le corps personnalisés de la notification électronique.</td>
           </tr>
          </tbody>
         </table>

      1. Cliquez sur **Envoyer**.

         Vos destinataires reçoivent une notification par email contenant des informations sur le BAT et les boutons que vous avez choisis d&#39;inclure.

         ![](assets/proof-share-email-350x87.png)

## Partage du code incorporé

Vous pouvez partager un BAT via un code incorporé si le propriétaire du BAT l’a configuré pour cela.

Pour partager un BAT via le code incorporé :

1. Dans la barre d’outils située à gauche de la visionneuse de vérification, cliquez sur le bouton **Partager** icône .

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. Dans le **Partager le BAT** options qui s’affichent, cliquez sur **Obtention du code incorporé**, puis cliquez sur **Copier**.

## Partager un BAT en y ajoutant des utilisateurs

Vous pouvez ajouter des utilisateurs à un BAT lors de la révision d’un BAT si vous disposez de l’une des autorisations suivantes :

* Autorisations de l’administrateur superviseur
* Autorisations de gestionnaire et vous êtes le créateur ou le propriétaire du BAT.
* Autorisations de gestionnaire avec le rôle de BAT de l’auteur ou du modérateur

Si le BAT comporte un workflow automatisé, vous pouvez ajouter l’utilisateur à une étape individuelle. Pour plus d’informations, voir [Présentation des processus automatisés](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Par défaut, les utilisateurs que vous ajoutez au BAT :

* Recevez une notification par email avec un lien vers le BAT.
* peuvent prendre des décisions d’approbation sur le BAT à partir de la zone Accueil ou Mon travail, comme décrit dans la section [Valider le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* Pour pouvoir passer en revue le BAT, il n’est pas nécessaire d’activer la vérification.

Lorsque le processus automatisé est activé et que vous ajoutez un utilisateur au BAT pour lequel la vérification n’est pas activée dans Workfront, une nouvelle étape est créée dans le processus automatisé. L’utilisateur que vous ajoutez est automatiquement ajouté à cette nouvelle étape lorsqu’il visualise le BAT pour la première fois. Pour plus d’informations, voir [Présentation des processus automatisés](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Pour partager un BAT avec des utilisateurs individuels :

1. Dans la barre d’outils située à gauche de la visionneuse de vérification, cliquez sur le bouton **Partager** icône .

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. Cliquez sur **Ajouter des destinataires** dans la liste à gauche.
1. Sous **Nouveaux destinataires de BAT**, commencez à saisir le nom d’un utilisateur avec lequel vous souhaitez partager le BAT, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.
1. (Facultatif) Modifiez toutes les options de réviseur à droite du nom de la personne :

   * **Rôle BAT**: Pour plus d’informations, voir [Gestion des rôles de BAT dans le BAT Workfront](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Évaluation**: (Disponible uniquement si le BAT comporte un workflow automatisé). Pour plus d’informations, voir  [Présentation des étapes de workflow automatisées](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **Alertes par email**: sélectionnez l’une des options suivantes pour indiquer comment la personne sera informée de l’activité sur le BAT.

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
        <td>Un email n'est envoyé au validant que si quelqu'un répond explicitement à son commentaire (cela exclut ses propres réponses sur ses propres commentaires). Cela signifie que si quelqu'un sur le BAT fait un nouveau commentaire, le validant n'en est pas informé.<p>Ce paramètre est recommandé pour vos clients sur le BAT afin qu’ils ne soient pas informés des autres commentaires sur le BAT et qu’ils ne soient informés que des réponses à leurs propres commentaires.</p><p>Bien que les réviseurs avec ce paramètre d’alerte par e-mail ne soient pas informés des autres nouveaux commentaires, ils peuvent toujours afficher tous les commentaires sur le BAT dans la visionneuse de vérification.</p><p>Pour plus d’informations sur les commentaires, voir <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Afficher et répondre aux commentaires du BAT</a>.</p></td> 
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
        <td>Workfront envoie un email contenant tous les commentaires, réponses et décisions répertoriés uniquement les jours où il y a une activité en dehors de la vôtre.<p>Cette alerte est une bonne façon de voir un résumé du projet sans être submergé par de multiples mises à jour tout au long de la journée.</p><p>Un exemple de cas d’utilisation pour ce résumé est un chef de département qui souhaite surveiller l’avancement global du projet.</p><p>Pour plus d’informations, voir <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestion des notifications pour les commentaires et les décisions de BAT</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Aucun email</td> 
        <td>Workfront n’envoie aucune alerte par courrier électronique.<br>Cela s’avère utile pour une personne qui n’est ajoutée à un BAT qu’à titre de référence et qui n’a pas besoin d’être informée des modifications.<p>La valeur par défaut du système est Résumé quotidien (également appelé Non défini). Si vous, ou vos réviseurs, n’effectuez aucune autre modification, tous vos BAT disposent de ce paramètre.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Facultatif) Répétez les deux étapes précédentes pour ajouter plusieurs utilisateurs au BAT. 
1. (Facultatif) Définissez une **Deadline** pour les opérateurs validants (disponible uniquement si le BAT ne dispose pas d&#39;un workflow automatisé).
1. (Facultatif) Sélectionnez **Envoyer une notification électronique aux nouveaux destinataires** pour leur faire savoir que vous les avez ajoutées au BAT.
1. Lorsque vous avez terminé d’ajouter des utilisateurs au BAT, cliquez sur **C&#39;est fait.**
