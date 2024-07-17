---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Gérer les notifications pour les commentaires et les décisions concernant les épreuves
description: Lorsque vous travaillez sur un BAT, que vous soyez un utilisateur d’Adobe Workfront ou un collaborateur externe, vous pouvez spécifier les notifications électroniques que vous souhaitez recevoir concernant les commentaires et les décisions pris sur le BAT. Pour plus d’informations, voir la présentation des notifications pour les commentaires de BAT et les décisions .
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 9%

---

# Gérer les notifications pour les commentaires et les décisions concernant les épreuves

Lorsque vous travaillez sur un BAT, que vous soyez un utilisateur d’Adobe Workfront ou un collaborateur externe, vous pouvez spécifier les notifications électroniques que vous souhaitez recevoir concernant les commentaires et les décisions pris sur le BAT. Pour plus d’informations, voir [Notifications pour les commentaires de BAT et la présentation des décisions](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Ces notifications sont différentes des alertes par email que vous pouvez recevoir concernant le flux d&#39;un BAT parmi les validants. Ils sont également différents des paramètres d’alerte par e-mail que vous pouvez configurer dans Workfront. 

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou supérieure</p> <p>ou</p> <p>Formule héritée : sélectionnez ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront Proof.

## Gérer les notifications pour les commentaires et les décisions concernant les épreuves

1. Ouvrez le BAT pour lequel vous souhaitez configurer les notifications que vous allez recevoir.
1. Si la barre d’outils de gauche ne s’affiche pas, cliquez sur l’icône **Menu** située dans le coin supérieur gauche de la visionneuse de Web Proofing.

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Dans la barre d’outils de gauche, cliquez sur l’icône **Paramètres** . ![Settings_icon.png](assets/settings-icon.png)

1. Sous **Envoyer-moi des notifications par courrier électronique concernant**, cliquez sur le paramètre souhaité pour le BAT.

   Le paramètre sélectionné reste en vigueur uniquement pour le BAT que vous avez ouvert.

   La valeur par défaut du système est **Résumé quotidien**. Si vous ou vos réviseurs n’effectuez aucune autre modification, tous vos BAT disposent de ce paramètre.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toutes les activités</td> 
      <td>Un email est envoyé au validant chaque fois qu'une activité est présente sur le BAT, comme un nouveau commentaire, une nouvelle réponse ou une nouvelle décision.<br><p>Il s’agit d’une excellente option pour la personne qui gère le processus de vérification car elle lui permet de voir l’activité telle qu’elle se produit. Les utilisateurs ne reçoivent pas d’alerte par e-mail sur leur propre activité (par exemple, commentaires, réponses et décisions).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Réponses à mes commentaires</td> 
      <td>Un email n'est envoyé au validant que si quelqu'un répond explicitement à son commentaire (cela exclut ses propres réponses sur ses propres commentaires). Cela signifie que si quelqu'un sur le BAT fait un nouveau commentaire, le validant n'en est pas informé.<p>Ce paramètre est recommandé pour vos clients sur le BAT afin qu’ils ne soient pas informés des autres commentaires sur le BAT et qu’ils ne soient informés que des réponses à leurs propres commentaires.</p><p>Bien que les réviseurs avec ce paramètre d’alerte par e-mail ne soient pas informés des autres nouveaux commentaires, ils peuvent toujours afficher tous les commentaires sur le BAT dans la visionneuse de vérification.<br></p><p>Pour plus d’informations, reportez-vous à la section <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Affichage des commentaires de BAT et réponse à ces commentaires</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décisions</td> 
      <td>Un email n'est envoyé au validant que lorsqu'une personne prend une décision.<br><p>Cette alerte par email peut s’avérer utile pour la personne qui gère le processus de validation (par exemple, un chef de projet), car elle permet à la personne qui gère le processus de validation de surveiller la progression du BAT et de voir quels utilisateurs ont pris leur décision.<br></p><p>Vous n’êtes pas informé de votre propre décision, sauf si vous sélectionnez une option de confirmation par courrier électronique lors de l’envoi de votre décision.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décision finale</td> 
      <td>Un email est envoyé lorsque la décision finale est prise sur le BAT (lorsque le dernier approbateur du BAT a pris sa décision).<br><p>Cette alerte est souvent utilisée par le concepteur, car celui-ci n’a pas besoin de participer à la discussion de révision proprement dite. Lorsque la décision finale est prise, le concepteur est informé et peut alors prendre des mesures sur les modifications nécessaires.<br></p><p>Cette alerte peut également s’avérer utile pour un responsable de service qui n’a besoin d’être averti que lorsque le processus de révision est terminé.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résumé horaire</td> 
      <td>Un email est envoyé au réviseur toutes les heures avec un résumé de tous les commentaires, réponses et décisions qui ont eu lieu au cours de la dernière heure.<br><p>L’e-mail n’est envoyé que lorsque l’activité se produit au-delà de la vôtre au cours de la dernière heure. S’il n’y a aucune activité d’autres utilisateurs, aucun courrier électronique n’est envoyé.<br></p><p>Cette alerte est une bonne manière de visualiser un aperçu du projet.<br></p><p>Un exemple de cas d’utilisation pour ce résumé est un validant principal qui a besoin d’une vue d’ensemble du projet, mais qui n’a pas besoin d’être informé immédiatement de toute l’activité sur le BAT.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résumé quotidien</td> 
      <td>(Paramètre par défaut) : un email est envoyé tous les jours avec tous les commentaires, réponses et décisions répertoriés. Un email n’est envoyé que les jours où il y a une activité en plus de la vôtre.<br><p>Cette alerte est une bonne façon de voir un résumé du projet sans être submergé par de multiples mises à jour tout au long de la journée.<br></p><p>Un exemple de cas d’utilisation pour ce résumé est un chef de département qui souhaite surveiller l’avancement global du projet.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aucun email</td> 
      <td>Aucune alerte par email n’est envoyée.<br><p>Ce paramètre est utile pour une personne qui n’est ajoutée à un BAT qu’à titre de référence et qui n’a pas besoin d’être informée des modifications.</p><p>Remarque : <p>Cette option désactive uniquement les alertes par e-mail que vous pouvez recevoir concernant les commentaires et les décisions du BAT. Elle ne désactive pas les alertes par email que vous pouvez recevoir concernant le flux d'un BAT, comme l'email Nouveau BAT ou Bon à tirer tardif. Pour plus d'informations sur les alertes par email concernant le flux d'un BAT, consultez les articles suivants : </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">Nouvel e-mail d’épreuve</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">E-mail de la nouvelle version</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">E-mail d’épreuve tardif</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">E-mail fait par épreuve</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
