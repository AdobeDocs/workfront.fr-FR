---
product-area: documents;setup
navigation-topic: review-a-proof
title: Configuration des paramètres de la visionneuse de vérification
description: Vous pouvez configurer les paramètres suivants pour la visionneuse de vérification de l’intégrité Web et la visionneuse de vérification de l’intégrité de l’appli de bureau - Modifiez-moi.
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1412'
ht-degree: 0%

---

# Configuration des paramètres de la visionneuse de vérification

Vous pouvez configurer les paramètres suivants pour la visionneuse de vérification de l’intégrité Web et la visionneuse de vérification de l’intégrité du bureau :

* Indique si les annotations de commentaire et les pin’s s’affichent sur les bons à tirer.
* Si les outils de balisage s’affichent dans la partie supérieure de la visionneuse de vérification ou dans un menu déroulant.
* Les notifications électroniques que vous recevez en tant que validant sur le BAT que vous avez ouvert.

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

Vous pouvez configurer les paramètres suivants pour la visionneuse de vérification de l’appli de bureau :

* Cette section décrit comment vous souhaitez que les liens du contenu du site web s’ouvrent dans la visionneuse.

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* Que se passe-t-il lorsque vous cliquez sur un lien défini pour s’ouvrir dans un nouvel onglet ou une nouvelle fenêtre du navigateur ?
* Effacez les données du cache pouvant être enregistrées avec le BAT que vous affichez afin de permettre l’affichage dans la visionneuse de contenu tel que des fenêtres contextuelles (qui peuvent être bloquées par les données du cache du navigateur).

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
   <td> <p>Modifier l’accès aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront BAT.

## Configuration des paramètres de la visionneuse de vérification

Pour configurer les paramètres de la visionneuse de vérification :

1. Ouvrez la visionneuse de test Web ou la visionneuse de test de bureau de l’une des manières suivantes :

   * Si vous utilisez le BAT dans Adobe Workfront, accédez à une liste de documents contenant un BAT que vous souhaitez afficher, survolez le document avec la souris, puis cliquez sur **BAT ouvert**.
   * Si vous utilisez le Bon à tirer Workfront, cliquez sur le bouton **Accéder à Bon à tirer** Icône du BAT dans le tableau de bord ou une liste d’affichages ![](assets/go-to-proof-blue-icon.png).

1. Si la barre d’outils gauche ne s’affiche pas, cliquez sur le bouton **Menu** , située dans le coin supérieur gauche de la visionneuse de BAT Web.

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Dans la barre d’outils de gauche, cliquez sur le bouton **Paramètres** icon ![](assets/settings-icon-in-pv.png).

1. Configurez l’une des options suivantes : **Paramètres** qui s’affichent.

   Les paramètres disponibles peuvent varier en fonction du type de BAT ouvert.

   * **Afficher les balises** (toujours disponible dans la visionneuse de proxy web et la visionneuse de vérification de l’appli de bureau) : Il s’agit des marques de commentaire que les réviseurs ajoutent aux bons à tirer lorsqu’ils utilisent les outils de balisage. Si vous les désactivez, vous pouvez toujours les voir lorsque vous cliquez sur un commentaire dans la liste de commentaires.

      Ce paramètre affecte tous les bons à tirer que vous ouvrez.

   * **Afficher les épingles** (toujours disponible dans la visionneuse de proxy web et la visionneuse de vérification de l’appli de bureau) : Il s’agit des pin’s numérotés que les réviseurs ajoutent aux BAT lorsqu’ils utilisent les outils de balisage. Ils indiquent où et dans quel ordre le validant a ajouté des commentaires. Si vous les désactivez, vous pouvez toujours les voir lorsque vous cliquez sur un commentaire dans la liste de commentaires.

      Ce paramètre affecte tous les bons à tirer que vous ouvrez.

   * **Utilisation d’outils de balisage étendus** (toujours disponible dans la visionneuse de proxy web et la visionneuse de vérification de l’appli de bureau) : Par défaut, les options de l’outil de balisage s’affichent dans la partie supérieure de la visionneuse de vérification. Vous pouvez les configurer pour qu’ils s’affichent dans un menu vertical qui s’ouvre uniquement lorsque vous cliquez dessus.

      Ce paramètre est appliqué à tous les bons à tirer que vous ouvrez.

   * **M’envoyer des notifications par e-mail sur** (toujours disponible dans la visionneuse de proxy web et la visionneuse de vérification de l’appli de bureau) : Cliquez sur l’une des options ci-dessous. Ce paramètre affecte uniquement le BAT que vous avez ouvert. Pour plus d’informations, voir [Présentation des notifications pour les commentaires de BAT et les décisions](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

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
        <td>Workfront n’envoie aucune alerte par courrier électronique.<br>Cela s’avère utile pour une personne qui n’est ajoutée à un BAT qu’à titre de référence et qui n’a pas besoin d’être informée des modifications.<p>La valeur par défaut du système est Résumé quotidien (également appelé Non défini). Si vous, ou vos réviseurs, n’effectuez aucune autre modification, tous vos BAT disposent de ce paramètre.</p></td> 
       </tr> 
      </tbody> 
     </table>

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **Lorsque vous cliquez sur des liens hypertexte dans un BAT** (disponible uniquement dans la visionneuse de vérification de l’appli de bureau) : Sélectionnez une option pour spécifier ce qui se passe dans la visionneuse de vérification de l’appli de bureau lorsque vous cliquez sur un lien défini pour s’ouvrir dans un nouvel onglet ou une nouvelle fenêtre du navigateur.

      Ce paramètre est appliqué à tous les BAT interactifs que vous ouvrez.

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Ouvrir dans la visionneuse de vérification</td> 
        <td>Les liens s’ouvrent toujours dans la visionneuse de vérification de l’appli de bureau et vous pouvez tester le contenu lié. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Ouvrir dans le navigateur</td> 
        <td>Les liens s’ouvrent toujours dans le navigateur, et non dans une visionneuse de vérification. Vous ne pouvez pas prouver le contenu lié.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Me demander à chaque fois</td> 
        <td> <p>Vous êtes invité à chaque fois que vous souhaitez ouvrir le lien dans la visionneuse de vérification de l’appli de bureau ou dans le navigateur. Si vous ouvrez le lien dans la visionneuse de vérification de l’appli de bureau, vous pouvez tester le contenu lié. Si vous ouvrez le lien dans le navigateur, vous ne pourrez pas tester le contenu lié.</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>Ce paramètre affecte uniquement le BAT que vous avez ouvert.</p> </td> 
       </tr> 
      </tbody> 
     </table>

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **Effacer le cache**: Efface les données du cache du navigateur qui peuvent être enregistrées avec un BAT interactif que vous affichez. Cela permet à un contenu tel que des fenêtres contextuelles (qui peuvent être bloquées par les données du cache du navigateur) de s’afficher dans la visionneuse de vérification de l’appli de bureau.

      Les données effacées comprennent le cache HTTP (par exemple les images à réutiliser après l’actualisation de la page suivante) et le cache de données de stockage Web (comme les cookies et les données qui identifient les utilisateurs).

      Ce paramètre affecte uniquement le BAT que vous avez ouvert.
