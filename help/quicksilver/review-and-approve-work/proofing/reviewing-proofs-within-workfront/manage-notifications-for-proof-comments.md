---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Gérer les notifications pour les commentaires et les décisions des épreuves
description: Lorsque vous travaillez sur une épreuve, que vous soyez un utilisateur d’Adobe Workfront ou un collaborateur externe, vous pouvez spécifier les notifications par e-mail que vous souhaitez recevoir concernant les commentaires et les décisions pris sur l’épreuve. Pour plus d’informations, voir la vue d’ensemble des notifications pour les commentaires et les décisions d’épreuves.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 28%

---

# Gérer les notifications pour les commentaires et les décisions des épreuves

<!-- Audited: 4/2025 -->

Lorsque vous travaillez sur une épreuve, que vous soyez un utilisateur d’Adobe Workfront ou un collaborateur externe, vous pouvez spécifier les notifications par e-mail que vous souhaitez recevoir concernant les commentaires et les décisions pris sur l’épreuve. Pour plus d’informations, voir [Vue d’ensemble des notifications pour les commentaires et les décisions d’épreuves](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Ces notifications sont différentes des alertes par e-mail que vous pouvez recevoir sur le flux d’un BAT entre les réviseurs, ainsi que des paramètres d’alerte par e-mail que vous pouvez configurer dans Workfront.

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

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation d’épreuve dont vous disposez, contactez votre administrateur ou administratrice de Workfront ou Workfront Proof.

+++

## Gérer les notifications pour les commentaires et les décisions des épreuves

1. Ouvrez l’épreuve pour laquelle vous souhaitez configurer des notifications.
1. Si la barre d’outils de gauche ne s’affiche pas, cliquez sur l’icône **Menu** dans le coin supérieur gauche de la visionneuse de relecture Web.

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Dans la barre d’outils de gauche, cliquez sur l’icône **Settings** ![Settings_icon.png](assets/settings-icon.png) .

1. Dans la section **M’envoyer des notifications par e-mail concernant** , sélectionnez le paramètre de notification de cette épreuve.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toutes les activités</td> 
      <td>Un e-mail est envoyé au réviseur ou à la réviseuse chaque fois que l’épreuve comporte une activité, comme un nouveau commentaire, une nouvelle réponse ou une nouvelle décision.<br><p>Ce paramètre est recommandé à la personne qui gère le processus de relecture, car il lui permet de voir l’activité au fur et à mesure qu’elle se produit. Les utilisateurs ne reçoivent pas d’alerte par e-mail concernant leur propre activité (par exemple, les commentaires, les réponses ou les décisions prises).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Réponses à mes commentaires</td> 
      <td>Un e-mail n'est envoyé au réviseur que si une personne répond directement à son commentaire (à l'exclusion de ses réponses à ses propres commentaires).<p>Ce paramètre est recommandé pour vos clients afin qu’ils ne soient avertis que des réponses à leurs propres commentaires et non des autres commentaires ajoutés sur l’épreuve. Cependant, ils peuvent toujours afficher tous les commentaires dans la visionneuse de relecture.</p>
      <p>Pour plus d’informations, voir <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Afficher et répondre aux commentaires de l’épreuve</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décisions</td> 
      <td>Un e-mail est envoyé au réviseur uniquement lorsqu’une personne prend une décision.<br><p>Cette alerte par e-mail peut s’avérer utile pour la personne qui gère le processus d’approbation, car elle permet à la personne qui gère le processus d’approbation de surveiller la progression du BAT et de voir quels utilisateurs ont pris leur décision.<br></p><p>Vous ne recevez pas de notification au sujet de votre propre décision, sauf si vous sélectionnez une option de confirmation par e-mail lors de la soumission de votre décision.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décision finale</td> 
      <td>Un e-mail est envoyé lorsque la décision finale est prise sur le BAT.<br><p>Cette alerte est souvent utilisée par le concepteur, qui n’a pas besoin de prendre part à la discussion de révision proprement dite. Une fois la décision finale prise, le concepteur en est informé et peut prendre des mesures pour apporter les modifications nécessaires.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résumé horaire</td> 
      <td>Un e-mail est envoyé au réviseur toutes les heures avec un résumé de tous les commentaires, réponses et décisions qui se sont produits au cours de la dernière heure.<br><p>L’e-mail n’est envoyé que lorsque d’autres activités que la vôtre ont lieu au cours de la dernière heure. Si aucune activité n’est effectuée par d’autres utilisateurs, aucun e-mail n’est envoyé.<br></p><p>Cette alerte est un bon moyen de voir un aperçu du projet au fur et à mesure de son avancement.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résumé quotidien</td> 
      <td>(Paramètre par défaut) : un e-mail est envoyé chaque jour avec tous les commentaires, réponses et décisions répertoriés. Elle est envoyée uniquement les jours où il y a une activité en dehors de la vôtre.<br><p>Cette alerte est un bon moyen d’afficher un résumé du projet sans être submergé par de multiples mises à jour tout au long de la journée.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aucun e-mail</td> 
      <td>Aucune alerte par e-mail n’est envoyée.<br><p>Ce paramètre est utile pour une personne ajoutée à une épreuve uniquement à titre de référence et qui n’a pas besoin d’être avertie des modifications.</p><p>Note : <p>Cette option désactive uniquement les alertes par e-mail concernant les commentaires et les décisions sur les épreuves. Elle ne désactive pas les alertes par e-mail que vous pouvez recevoir sur le flux d’une épreuve, telles que l’e-mail Nouvelle épreuve ou Épreuve en retard. Pour plus d’informations, consultez les articles suivants : </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">E-mail Nouvelle épreuve</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">E-mail Nouvelle version</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">E-mail d’épreuve en retard</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">E-mail Épreuve effectuée</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
