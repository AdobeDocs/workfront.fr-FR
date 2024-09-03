---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Gérer les notifications pour les commentaires et les décisions des épreuves
description: Lorsque vous travaillez sur une épreuve, que vous soyez utilisateur ou utilisatrice d’Adobe Workfront ou un collaborateur ou une collaboratrice externe, vous pouvez indiquer les notifications par e-mail que vous souhaitez recevoir concernant les commentaires et les décisions sur l’épreuve. Pour plus d’informations, voir la vue d’ensemble des notifications pour les commentaires et les décisions d’épreuves.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: f252e3562b8ea73486d407138251b3d15d4b9f3a
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 100%

---

# Gérer les notifications pour les commentaires et les décisions des épreuves

Lorsque vous travaillez sur une épreuve, que vous soyez utilisateur ou utilisatrice d’Adobe Workfront ou un collaborateur ou une collaboratrice externe, vous pouvez indiquer les notifications par e-mail que vous souhaitez recevoir concernant les commentaires et les décisions sur l’épreuve. Pour plus d’informations, voir [Vue d’ensemble des notifications pour les commentaires et les décisions d’épreuves](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Ces notifications sont différentes des alertes par e-mail que vous pouvez recevoir concernant le flux d’une épreuve parmi les réviseurs et réviseuses. Elles sont également différentes des paramètres d’alerte par e-mail que vous pouvez configurer dans Workfront. 

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

1. Ouvrez l’épreuve pour laquelle vous souhaitez configurer les notifications que vous allez recevoir.
1. Si la barre d’outils de gauche ne s’affiche pas, cliquez sur l’icône **Menu**, située dans le coin supérieur gauche de la visionneuse de relecture web.

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Dans la barre d’outils de gauche, cliquez sur l’icône **Paramètres**. ![Settings_icon.png](assets/settings-icon.png)

1. Sous **M’envoyer des notifications par e-mail sur**, cliquez sur le paramètre souhaité pour l’épreuve.

   Le paramètre sélectionné reste en vigueur uniquement pour l’épreuve que vous avez ouverte.

   Le paramètres système par défaut est **Synthèse quotidienne**. Si vous ou vos réviseurs et réviseuses n’effectuez aucune autre modification, toutes vos épreuves disposent de ce paramètre.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toutes les activités</td> 
      <td>Un e-mail est envoyé au réviseur ou à la réviseuse chaque fois qu’une activité est présente sur l’épreuve, comme un nouveau commentaire, une nouvelle réponse ou une nouvelle décision.<br><p>Il s’agit d’une excellente option pour la personne qui gère le processus de relecture, car elle lui permet de voir l’activité au fur et à mesure qu’elle se produit. Les personnes ne reçoivent pas d’alerte par e-mail sur leur propre activité (par exemple, commentaires, réponses et décisions).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Réponses à mes commentaires</td> 
      <td>Un e-mail n’est envoyé à la personne réviseuse que si quelqu’un répond explicitement à son commentaire (cela exclut ses propres réponses sur ses propres commentaires). Cela signifie que si quelqu’un fait un nouveau commentaire sur l’épreuve, la personne réviseuse n’en est pas informée.<p>Ce paramètre est recommandé pour vos clientes et clients sur l’épreuve afin qu’ils ne soient pas informés des autres commentaires sur l’épreuve et qu’ils ne soient informés que des réponses à leurs propres commentaires.</p><p>Bien que les personnes réviseuses ne soient pas informées des autres nouveaux commentaires avec ce paramètre d’alerte par e-mail, elles peuvent toujours afficher tous les commentaires sur l’épreuve dans la visionneuse de relecture.<br></p><p>Pour plus d’informations, voir <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Afficher et répondre aux commentaires de l’épreuve</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décisions</td> 
      <td>Un e-mail n’est envoyé au réviseur ou à la réviseuse que lorsqu’une personne prend une décision.<br><p>Cette alerte par e-mail peut s’avérer utile pour la personne qui gère le processus d’approbation (par exemple, une personne responsable de projet), car elle permet à la personne qui gère le processus d’approbation de surveiller la progression de l’épreuve et de voir quelles personnes ont pris leur décision.<br></p><p>Vous ne recevez pas de notification au sujet de votre propre décision, sauf si vous sélectionnez une option de confirmation par e-mail lors de la soumission de votre décision.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décision finale</td> 
      <td>Un e-mail est envoyé lorsque la décision finale est prise sur l’épreuve (lorsque la dernière personne approbatrice de l’épreuve pris sa décision).<br><p>Cette alerte est souvent utilisée par la personne chargée de la conception, car celle-ci n’a pas besoin de participer à la discussion de révision proprement dite. Lorsque la décision finale est prise, le concepteur ou la conceptrice reçoit une notification et peut alors agir sur les modifications nécessaires.<br></p><p>Cette alerte peut également s’avérer utile pour une personne responsable de service qui n’a besoin d’être avertie que lorsque le processus de révision est achevé.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résumé horaire</td> 
      <td>Un e-mail est envoyé au réviseur ou à la réviseuse toutes les heures avec un résumé de tous les commentaires, réponses et décisions qui ont eu lieu au cours de la dernière heure.<br><p>L’e-mail n’est envoyé que lorsqu’une activité autre que la vôtre s’est produite au cours de la dernière heure. S’il n’y a aucune activité d’autres personnes, aucun e-mail n’est envoyé.<br></p><p>Cette alerte est une bonne manière d’avoir une vue d’ensemble du projet.<br></p><p>Un exemple de cas d’utilisation pour ce résumé est celui d’une personne expérimentée dans la révision qui a besoin d’une vue d’ensemble du projet, mais qui n’a pas besoin d’être informée de toute l’activité sur l’épreuve dans l’immédiat.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résumé quotidien</td> 
      <td>(Paramètre par défaut) : un e-mail est envoyé tous les jours avec tous les commentaires, réponses et décisions répertoriés. Un e-mail n’est envoyé que les jours où il y a une activité en plus de la vôtre.<br><p>Cette alerte est une bonne façon de voir un résumé du projet sans se laisser submerger par plusieurs mises à jour tout au long de la journée.<br></p><p>Un exemple de cas d’utilisation pour ce résumé est celui d’une personne gestionnaire de service qui souhaite surveiller la progression globale du projet.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aucun e-mail</td> 
      <td>Aucune alerte par e-mail n’est envoyée.<br><p>Ce paramètre est utile pour une personne qui n’est ajoutée à une épreuve qu’à titre de référence et qui n’a pas besoin d’être informée des modifications.</p><p>Note : <p>Cette option désactive uniquement les alertes par e-mail que vous pouvez recevoir concernant les commentaires et les décisions de l’épreuve. Elle ne désactive pas les alertes par e-mail que vous pouvez recevoir concernant le flux d’une épreuve, comme l’e-mail Nouvelle épreuve ou Épreuve en retard. Pour plus d’informations sur les alertes par e-mail concernant le flux d’une épreuve, consultez les articles suivants : </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">E-mail Nouvelle épreuve</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">E-mail Nouvelle version</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">E-mail d’épreuve en retard</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">E-mail Épreuve effectuée</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
