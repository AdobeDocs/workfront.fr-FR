---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Partager une épreuve à partir de la visionneuse de relecture
description: Vous pouvez partager une épreuve à partir de la visionneuse de relecture si le partage est activé par la personne propriétaire ou créatrice de l’épreuve.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 98%

---

# Partager une épreuve à partir de la visionneuse de relecture

Vous pouvez partager une épreuve à partir de la visionneuse de relecture si le partage est activé par la personne propriétaire ou créatrice de l’épreuve.

>[!IMPORTANT]
>
>Le paramètre Autoriser le partage de l’épreuve via une URL publique ou un code intégré doit être activé.

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
   <td> <p>Modifier l’accès aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander un accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation d’épreuve dont vous disposez, contactez votre administrateur ou administratrice Workfront ou Workfront Proof.

+++

## Partager l’URL

Vous pouvez partager une épreuve via une URL si la personne propriétaire a configuré l’épreuve pour le partage. Les propriétaires d’épreuve peuvent mettre à jour les paramètres de partage à tout moment. Pour plus d’informations, voir [Modifier les paramètres de l’épreuve](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Si le menu d’icône de gauche n’est pas affiché, cliquez sur l’icône **Menu** dans le coin supérieur gauche de la visionneuse de relecture.

   ![Icône de menu](assets/menu-icon-in-proofing-viewer-350x188.png)

1. Dans le menu des icônes de gauche de la visionneuse de relecture, cliquez sur l’icône **Partager** 

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. Dans les options **Partager l’épreuve** qui s’affichent, veillez à ce que **Obtenir un lien partageable** soit sélectionné.

1. Faites ce qui suit :

   * Pour copier le lien dans le presse-papiers, cliquez sur **Copier le lien**.

     Vous pouvez désormais diffuser le lien par le biais d’un outil tiers, tel qu’une messagerie instantanée ou une application de messagerie.

   * Pour envoyer le lien directement par e-mail à partir d’Adobe Workfront, procédez comme suit :

      1. Dans le champ **Ou envoyer le lien par e-mail à**, commencez à taper et sélectionnez le nom de votre destinataire. Vous pouvez également spécifier l’adresse e-mail d’une personne externe avec laquelle vous souhaitez effectuer un partage.

         >[!NOTE]
         >
         >Si vous voyez un e-mail d’alias lors du partage de l’épreuve, ne créez pas un nouvel utilisateur ou une nouvelle utilisatrice invité en saisissant l’e-mail d’origine s’il existe un e-mail d’alias correspondant.

      1. Sélectionnez l’une des options suivantes :

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Envoyer un lien public</td>
            <td><p>Inclut un bouton dans la notification par e-mail qui dirige les utilisateurs et utilisatrices vers l’épreuve dans la visionneuse de relcture qu’ils utilisent et leur accorde l’accès en affichage.</p><p>Si l’option <strong>S’abonner à l’épreuve via une URL publique ou un code intégré</strong> est désactivée pour l’épreuve, les utilisateurs et utilisatrices peuvent se connecter à l’aide de leurs informations de connexion Workfront pour ajouter des commentaires à l’épreuve. Si elle est activée, toute personne fournissant son adresse e-mail et son nom (aucun mot de passe requis) peut se connecter et ajouter des commentaires à l’épreuve.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Envoyer un lien de téléchargement</td>
            <td>Inclut un bouton dans la notification par e-mail qui dirige les utilisateurs et utilisatrices vers une page de téléchargement, qui fournit les détails du fichier, son nom et sa taille, avec le fichier affiché en ligne. Les utilisateurs et utilisatrices peuvent cliquer sur le lien Télécharger de la page de téléchargement pour télécharger le fichier.</td>
           </tr>
           <tr>
            <td role="rowheader">Ajouter un message personnalisé</td>
            <td>Permet de spécifier l’objet et le corps personnalisés de la notification par e-mail.</td>
           </tr>
          </tbody>
         </table>

      1. Cliquez sur **Envoyer**.

         Vos destinataires reçoivent une notification par e-mail contenant des informations sur l’épreuve et les boutons que vous avez choisis d’inclure.

         ![](assets/proof-share-email-350x87.png)

## Partager le code intégré

Vous pouvez partager une épreuve via un code intégré si la personne propriétaire de l’épreuve l’a configurée pour cela.

Pour partager une épreuve via le code intégré :

1. Dans la barre d’outils située à gauche de la visionneuse de relecture, cliquez sur l’icône **Partager**.

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. Dans les options de **Partager une épreuve** qui apparaissent, cliquez sur **Obtenir un code intégré**, puis cliquez sur **Copier**.

## Partager une épreuve en y ajoutant des utilisateurs et utilisatrices

Vous pouvez ajouter des personnes à une épreuve lors de la révision d’une épreuve si vous disposez de l’une des autorisations suivantes :

* Autorisations d’administration ou de supervision
* Autorisations de gestion et vous êtes la personne créatrice ou propriétaire de l’épreuve
* Autorisations de gestion avec le rôle d’épreuve de création ou de modération

Si l’épreuve comporte un workflow automatisé, vous pouvez ajouter la personne à une étape individuelle. Pour plus d’informations, voir [Vue d’ensemble des workflows automatisés](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Par défaut, les personnes que vous ajoutez à l’épreuve :

* Reçoivent une notification par e-mail avec un lien vers l’épreuve.
* Peut prendre des décisions d’approbation concernant l’épreuve depuis la zone d’Accueil, comme décrit dans la section [Approuver le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* Pour pouvoir relire l’épreuve, il n’est pas nécessaire d’activer la relecture.

Lorsque le workflow automatisé est activé et que vous ajoutez une personne à l’épreuve qui n’a pas la relecture d’activée dans Workfront, une nouvelle étape est créée dans le workflow automatisé. La personne que vous ajoutez est automatiquement ajoutée à cette nouvelle étape lorsqu’elle consulte l’épreuve pour la première fois. Pour plus d’informations, voir [Vue d’ensemble des workflows automatisés](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Pour partager une épreuve avec des personnes :

1. Dans la barre d’outils située à gauche de la visionneuse de relecture, cliquez sur l’icône **Partager**.

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. Cliquez sur **Ajouter des destinataires** dans la liste à gauche.
1. Sous **Nouveaux destinataires d’épreuve**, commencez à saisir le nom d’une personne avec laquelle vous souhaitez partager l’épreuve, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.
1. (Facultatif) Modifiez toutes les options de révision à droite du nom de la personne :

   * **Rôle d’épreuve** : pour plus d’informations, voir [Gérer les rôles d’épreuve dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Étape** : (disponible uniquement si l’épreuve comporte un workflow automatisé). Pour plus d’informations, voir [Vue d’ensemble des étapes de workflow automatisé](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **Alertes par e-mail** : sélectionnez l’une des options suivantes pour indiquer comment la personne sera informée de l’activité sur l’épreuve.

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
        <td>Un e-mail n’est envoyé à la personne réviseuse que si quelqu’un répond explicitement à son commentaire (cela exclut ses propres réponses sur ses propres commentaires). Cela signifie que si quelqu’un fait un nouveau commentaire sur l’épreuve, la personne réviseuse n’en est pas informée.<p>Ce paramètre est recommandé pour vos clientes et clients sur l’épreuve afin qu’ils ne soient pas informés des autres commentaires sur l’épreuve et qu’ils ne soient informés que des réponses à leurs propres commentaires.</p><p>Bien que les personnes réviseuses ne soient pas informées des autres nouveaux commentaires avec ce paramètre d’alerte par e-mail, elles peuvent toujours afficher tous les commentaires sur l’épreuve dans la visionneuse de relecture.</p><p>Pour plus d’informations sur les commentaires, voir la section <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Afficher les commentaires de l’épreuve et y répondre</a>.</p></td> 
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
        <td>Workfront envoie un e-mail contenant tous les commentaires, réponses et décisions répertoriés uniquement les jours où se produit une activité différente de la vôtre.<p>Cette alerte est une bonne façon de voir un résumé du projet sans se laisser submerger par plusieurs mises à jour tout au long de la journée.</p><p>Un exemple de cas d’utilisation pour ce résumé est celui d’une personne gestionnaire de service qui souhaite surveiller la progression globale du projet.</p><p>Pour plus d’informations, voir la section <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gérer les notifications pour les commentaires et les décisions relatifs aux épreuves</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Aucun e-mail</td> 
        <td>Workfront n’envoie aucune alerte par e-mail.<br>Cela se révèle utile pour une personne qui n’est ajoutée à une épreuve qu’à titre de référence et qui n’a pas besoin d’être informée des modifications.<p>La valeur par défaut du système est Résumé quotidien (également appelé Non défini). Si vous ou vos réviseurs et réviseuses n’effectuez aucune autre modification, toutes vos épreuves disposent de ce paramètre.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Facultatif) Répétez les deux étapes précédentes pour ajouter plusieurs utilisateurs et utilisatrices à l’épreuve. 
1. (Facultatif) Définissez une **Échéance** pour les réviseurs et réviseuses (disponible uniquement si l’épreuve ne dispose pas d’un workflow automatisé).
1. (Facultatif) Sélectionnez **Envoyer une notification par e-mail aux nouveaux destinataires** pour les informer que vous les avez ajoutés à l’épreuve.
1. Lorsque vous avez terminé d’ajouter des utilisateurs et utilisatrices à l’épreuve, cliquez sur **Terminé**.
