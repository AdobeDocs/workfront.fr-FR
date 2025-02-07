---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Configurer les paramètres de notification par e-mail dans  [!DNL Workfront Proof]
description: Les notifications par e-mail générées par Workfront Proof informent les collaborateurs et collaboratrices de l’activité récente sur les épreuves, comme les commentaires, les réponses ou les décisions.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '2065'
ht-degree: 98%

---

# Configurer les paramètres de notification par e-mail dans [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Les notifications par e-mail informent les collaborateurs et collaboratrices de l’activité récente sur les épreuves, comme les commentaires, les réponses ou les décisions.

Vous pouvez définir des notifications par e-mail pour les réviseurs et les réviseuses dans les zones suivantes :

Les notifications par e-mail destinées aux réviseurs et aux réviseuses peuvent être définies sur les pages Nouvelle épreuve et [!UICONTROL Nouvelle version], et gérées dans la section [!UICONTROL Workflow] de la page [!UICONTROL Détails de l’épreuve]. Pour plus d’informations, voir [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* Page Nouvelle épreuve
* Page [!UICONTROL Nouvelle version]
* Section [!UICONTROL Workflow] de la page [!UICONTROL Détails de l’épreuve].

Pour plus d’informations, voir [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)


* [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Gérez les détails des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).


Chaque personne peut également définir ses propres paramètres d’alerte par e-mail qui sont automatiquement appliqués lorsqu’une épreuve est partagée avec elle si les collaborateurs et collaboratrices ont leurs préférences ou si les administrateurs et administratrices de compte ont leurs recommandations sur la fréquence des alertes. Cela peut être défini comme valeur par défaut de l’épreuve sur les pages de détails des utilisateurs et utilisatrices.

Chaque personne peut également définir ses propres paramètres d’alerte par e-mail qui seront automatiquement appliqués lorsqu’une épreuve est partagée avec elle. <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>Ces paramètres sont suggérés lorsque les personnes créent les épreuves et ajoutent ces collaborateurs et collaboratrices. Cependant, il s’agit uniquement de suggestions. Elles peuvent donc être ajustées à tout moment pendant le processus de révision et les modifications s’appliquent à toutes les activités effectuées après la modification. Les paramètres par défaut des épreuves sont remplacés par les paramètres au niveau des épreuves.

Les personnes avec un profil [!UICONTROL Administrateur ou administratrice] ou [!UICONTROL Administrateur ou administratrice de facturation] peuvent également définir les valeurs par défaut des épreuves pour les autres utilisateurs et utilisatrices de leur compte dans les paramètres du compte.

Pour plus d’informations sur les profils, voir [Profils d’autorisations d’épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
<tr> 
   <td role="rowheader">Produit</td> 
   <td>Workfront Proof autonome</td> 
  </tr> 
</table>

+++

## Configurer les paramètres par défaut des épreuves dans les paramètres personnels (utilisateurs et utilisatrices [!DNL Workfront Proof] uniquement)

Vous pouvez configurer les paramètres des épreuves pour celles que vous créez.

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. Cliquez sur l’image de votre profil dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Paramètres personnels]**.

1. Cliquez sur l’onglet **[!UICONTROL Paramètres de relecture par défaut]**.
1. Cliquez sur **[!UICONTROL Paramètres de notification par e-mail par défaut]** pour le développer.
1. Dans la liste déroulante située à droite des deux paramètres suivants, sélectionnez l’une des options expliquées dans le tableau ci-dessous.

   * **[!UICONTROL Alerte par e-mail par défaut]** : affecte chaque épreuve partagée avec vous. Ce paramètre peut être remplacé au niveau de l’épreuve.
   * **[!UICONTROL Alertes par e-mail par défaut pour les nouveaux réviseurs et réviseuses invités]** : affecte les réviseurs et réviseuses qui n’existaient pas auparavant comme contacts dans votre compte.

   >[!NOTE]
   >
   >Si vous ne choisissez pas l’une des options suivantes, [!DNL Workfront Proof] vous envoie une synthèse quotidienne de l’activité sur vos épreuves.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All activity]</td> 
      <td>[!UICONTROL Workfront] envoie un e-mail au réviseur ou à la réviseuse chaque fois qu’il y a une activité sur l’épreuve, comme un nouveau commentaire, une nouvelle réponse ou une nouvelle décision. <p>Il s’agit d’une excellente option pour la personne qui gère le processus de relecture, car elle lui permet de voir l’activité au fur et à mesure qu’elle se produit. </p><p>Les personnes ne reçoivent pas d’alerte par e-mail sur leur propre activité.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Replies to my comments]</td> 
      <td>Un e-mail n’est envoyé à la personne réviseuse que si quelqu’un répond explicitement à son commentaire (cela exclut ses propres réponses sur ses propres commentaires). Cela signifie que si quelqu’un fait un nouveau commentaire sur l’épreuve, la personne réviseuse n’en est pas informée.<p>Ce paramètre est recommandé pour vos clientes et clients sur l’épreuve afin qu’ils ne soient pas informés des autres commentaires sur l’épreuve et qu’ils ne soient informés que des réponses à leurs propres commentaires.</p><p>Bien que les personnes réviseuses ne soient pas informées des autres nouveaux commentaires avec ce paramètre d’alerte par e-mail, elles peuvent toujours afficher tous les commentaires sur l’épreuve dans la visionneuse de relecture.</p><p>Pour plus d’informations sur les commentaires, consultez <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Afficher et répondre aux commentaires de l’épreuve</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisions]</td> 
      <td>[!DNL Workfront] envoie un e-mail à la personne chargée de la révision uniquement lorsqu’une personne prend une décision.<p>Cette fonctionnalité peut s’avérer utile pour la personne chargée de la gestion du processus d’approbation (par exemple, une personne responsable du projet) et qui doit surveiller la progression de l’épreuve et vérifier quels utilisateurs et utilisatrices ont pris leur décision.</p><p>Vous ne recevez pas de notification au sujet de votre propre décision, sauf si vous sélectionnez une option de confirmation par e-mail lors de la soumission de votre décision.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Final decision]</td> 
      <td>[!DNL Workfront] envoie un e-mail lorsque le dernier approbateur ou la dernière approbatrice de l’épreuve a pris sa décision.<p>Cette alerte est souvent utilisée par le concepteur ou la conceptrice, qui n’a généralement pas besoin de prendre part à la discussion de révision en elle-même. Lorsque la décision finale est prise, le concepteur ou la conceptrice reçoit une notification et peut alors agir sur les modifications nécessaires.</p><p>Cette alerte peut également s’avérer utile pour une personne responsable de service qui n’a besoin d’être avertie que lorsque le processus de révision est achevé.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Hourly Summary]</td> 
      <td>[!DNL Workfront] envoie toutes les heures à la personne chargée de la révision un e-mail comprenant un résumé de tous les commentaires, réponses et décisions de l’heure.<p>L’e-mail n’est envoyé que lorsqu’une activité autre que la vôtre s’est produite au cours de la dernière heure. </p><p>Cette alerte est une bonne manière d’avoir une vue d’ensemble du projet.</p><p>Un exemple de cas d’utilisation pour ce résumé est celui d’une personne expérimentée dans la révision qui a besoin d’une vue d’ensemble du projet, mais qui n’a pas besoin d’être informée de toute l’activité sur l’épreuve dans l’immédiat.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Daily Summary]</td> 
      <td>[!DNL Workfront] envoie un e-mail contenant tous les commentaires, réponses et décisions répertoriés uniquement les jours comportant une activité autre que la vôtre.<p>Cette alerte est une bonne façon de voir un résumé du projet sans se laisser submerger par plusieurs mises à jour tout au long de la journée.</p><p>Un exemple de cas d’utilisation pour ce résumé est celui d’une personne gestionnaire de service qui souhaite surveiller la progression globale du projet.</p><p>Pour plus d’informations, consultez <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gérer les notifications pour les commentaires et les décisions sur l’épreuve</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL No email]</td> 
      <td>[!DNL Workfront] n’envoie aucune alerte par e-mail.<br>Cela s’avère utile pour une personne qui n’est ajoutée à une épreuve qu’à titre de référence et qui n’a pas besoin d’être informée des modifications.<p>La valeur par défaut du système est [!UICONTROL Daily summary] (également appelée [!UICONTROL Not Set]). Si vous ou vos réviseurs et réviseuses n’effectuez aucune autre modification, toutes vos épreuves disposent de ce paramètre.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Modifiez l’un des éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>Indiquez si vous souhaitez recevoir un e-mail [!UICONTROL Proof made] lors de la création d’une épreuve. Pour plus d’informations, voir <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">l’e-mail [!UICONTROL Proof Made]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format of emails sent to me] </td> 
      <td> <p>Choisissez entre les e-mails au style HTML et les e-mails en texte brut. </p> <p><b>NOTE</b></p>
      <p>Les paramètres de relecture par défaut sont remplacés par les paramètres à l’échelle de l’épreuve. Toutefois, si les notifications par e-mail de l’épreuve sont désactivées pour l’ensemble du compte dans les paramètres du [!UICONTROL Account], aucune alerte par e-mail n’est envoyée aux collaborateurs et aux collaboratrices, même si [!UICONTROL Disabled email alert] n’est pas sélectionnée sur les épreuves.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Sous **[!UICONTROL Paramètres des messages]**, modifiez l’une des options suivantes :

   | Modèle d’épreuve | Description |
   |---|---|
   | **[!UICONTROL Modèle d’objet d’épreuve]** | S’affiche sur les pages Nouvelle épreuve, Nouvelle version, Message et Rappel. Peut être modifié avant envoi. |
   | **[!UICONTROL Modèle de message d’épreuve]** | S’affiche sur les pages Nouvelle épreuve, Nouvelle version, Message et Rappel. Peut être modifié avant envoi. |

## Modifier les alertes par e-mail d’une personne destinataire

Vous pouvez modifier les alertes par e-mail destinées à une personne destinataire spécifique dans une action par lot.

1. Cliquez sur **[!UICONTROL Contacts]** dans le panneau de navigation de gauche.
1. Cliquez sur le menu **[!UICONTROL Plus]** ![Plus](assets/more-button-small.png) du destinataire, puis cliquez sur **[!UICONTROL Afficher les détails du membre]** dans le menu déroulant.

1. Ouvrez la section **[!UICONTROL Éléments partagés]**.
1. Cochez la case à gauche de chaque élément pour lequel vous souhaitez modifier l’alerte par e-mail.
1. Cliquez sur **[!UICONTROL Plus]** au-dessus de la liste des éléments partagés, puis cliquez sur **[!UICONTROL Modifier l’alerte par e-mail]** dans le menu déroulant.

1. Modifiez l’alerte par e-mail, puis cliquez sur **[!UICONTROL Soumettre]**.

## Configurer les valeurs par défaut d’une épreuve pour une personne

Si vous êtes un administrateur ou une administratrice [!DNL Workfront Proof], vous pouvez définir les valeurs par défaut d’une épreuve pour les personnes de votre compte.

1. Cliquez sur **[!UICONTROL Paramètres du compte]** en haut de l’écran.

1. Ouvrez l’onglet **[!UICONTROL Utilisateurs et utilisatrices]**.
1. Ouvrez le menu **[!UICONTROL Plus]** ![More_button_small.png](assets/more-button-small.png) à droite du nom de la personne.

1. Cliquez sur **[!UICONTROL Afficher les détails des utilisateurs et utilisatrices]** dans le menu déroulant.
1. Sous **[!UICONTROL Paramètres]**, cliquez sur **[!UICONTROL Paramètres d’alerte par e-mail par défaut]** pour le développer.

1. Dans la liste déroulante située à droite des deux paramètres suivants, sélectionnez l’une des options expliquées dans le tableau ci-dessous :

   * **[!UICONTROL Alerte par e-mail par défaut]** : affecte chaque épreuve partagée avec vous. Ce paramètre peut être remplacé au niveau de l’épreuve.
   * **[!UICONTROL Alertes par e-mail par défaut pour les nouveaux réviseurs et réviseuses invités]** : affecte les réviseurs et réviseuses qui n’existaient pas comme contacts dans votre compte.

   >[!NOTE]
   >
   >Si vous ne choisissez pas l’une des options suivantes pour une personne, [!DNL Workfront Proof] envoie aux personnes une synthèse quotidienne de l’activité sur leurs épreuves.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL All activity]</td>
      <td>[!DNL Workfront] envoie un e-mail à la personne réviseuse chaque fois qu’il y a une activité sur l’épreuve, comme un nouveau commentaire, une nouvelle réponse ou une nouvelle décision. <p>Il s’agit d’une excellente option pour la personne qui gère le processus de relecture, car elle lui permet de voir l’activité au fur et à mesure qu’elle se produit. </p><p>Les personnes ne reçoivent pas d’alerte par e-mail sur leur propre activité.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Replies to my comments]</td>
      <td>Un e-mail n’est envoyé à la personne réviseuse que si quelqu’un répond explicitement à son commentaire (cela exclut ses propres réponses sur ses propres commentaires). Cela signifie que si quelqu’un fait un nouveau commentaire sur l’épreuve, la personne réviseuse n’en est pas informée.<p>Ce paramètre est recommandé pour vos clientes et clients sur l’épreuve afin qu’ils ne soient pas informés des autres commentaires sur l’épreuve et qu’ils ne soient informés que des réponses à leurs propres commentaires.</p><p>Bien que les personnes réviseuses ne soient pas informées des autres nouveaux commentaires avec ce paramètre d’alerte par e-mail, elles peuvent toujours afficher tous les commentaires sur l’épreuve dans la visionneuse de relecture.</p><p>Pour plus d’informations sur les commentaires, consultez <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Afficher et répondre aux commentaires de l’épreuve</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisions]</td>
      <td>[!DNL Workfront] envoie un e-mail à la personne chargée de la révision uniquement lorsqu’une personne prend une décision.<p>Cette fonctionnalité peut s’avérer utile pour la personne chargée de la gestion du processus d’approbation (par exemple, une personne responsable du projet) et qui doit surveiller la progression de l’épreuve et vérifier quels utilisateurs et utilisatrices ont pris leur décision.</p><p>Vous ne recevez pas de notification au sujet de votre propre décision, sauf si vous sélectionnez une option de confirmation par e-mail lors de la soumission de votre décision.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Final decision]</td>
      <td>[!DNL Workfront] envoie un e-mail lorsque le dernier approbateur ou la dernière approbatrice de l’épreuve a pris sa décision.<p>Cette alerte est souvent utilisée par le concepteur ou la conceptrice, qui n’a généralement pas besoin de prendre part à la discussion de révision en elle-même. Lorsque la décision finale est prise, le concepteur ou la conceptrice reçoit une notification et peut alors agir sur les modifications nécessaires.</p><p>Cette alerte peut également s’avérer utile pour une personne responsable de service qui n’a besoin d’être avertie que lorsque le processus de révision est achevé.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Hourly Summary]</td>
      <td>[!DNL Workfront] envoie toutes les heures à la personne chargée de la révision un e-mail comprenant un résumé de tous les commentaires, réponses et décisions de l’heure.<p>L’e-mail n’est envoyé que lorsqu’une activité autre que la vôtre s’est produite au cours de la dernière heure. </p><p>Cette alerte est une bonne manière d’avoir une vue d’ensemble du projet.</p><p>Un exemple de cas d’utilisation pour ce résumé est celui d’une personne expérimentée dans la révision qui a besoin d’une vue d’ensemble du projet, mais qui n’a pas besoin d’être informée de toute l’activité sur l’épreuve dans l’immédiat.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Daily Summary]</td>
      <td>[!DNL Workfront] envoie un e-mail contenant tous les commentaires, réponses et décisions répertoriés uniquement les jours comportant une activité autre que la vôtre.<p>Cette alerte est une bonne façon de voir un résumé du projet sans se laisser submerger par plusieurs mises à jour tout au long de la journée.</p><p>Un exemple de cas d’utilisation pour ce résumé est celui d’une personne gestionnaire de service qui souhaite surveiller la progression globale du projet.</p><p>Pour plus d’informations, consultez <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gérer les notifications pour les commentaires et les décisions sur l’épreuve</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL No email]</td>
      <td>[!DNL Workfront] n’envoie aucune alerte par e-mail.<br>Cela s’avère utile pour une personne qui n’est ajoutée à une épreuve qu’à titre de référence et qui n’a pas besoin d’être informée des modifications.<p>La valeur par défaut du système est [!UICONTROL Daily summary] (également appelée [!UICONTROL Not Set]). Si vous ou vos réviseurs et réviseuses n’effectuez aucune autre modification, toutes vos épreuves disposent de ce paramètre.</p></td>
     </tr>
    </tbody>
   </table>

1. Dans le reste des **[!UICONTROL Paramètres d’alerte par e-mail par défaut]**, modifiez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>Indiquez si vous souhaitez recevoir un e-mail [!UICONTROL Proof made] lors de la création d’une épreuve. Pour plus d’informations, voir <a href="https://support.workfront.com/hc/en-us/article">l’e-mail [!UICONTROL Proof Made].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format of emails sent to me] </td> 
      <td> <p>Choisissez entre les e-mails au style HTML et les e-mails en texte brut. </p> <p><b>NOTE</b></p> <p>Les paramètres de relecture par défaut sont remplacés par les paramètres à l’échelle de l’épreuve. Toutefois, si les notifications par e-mail de l’épreuve sont désactivées pour l’ensemble du compte dans les paramètres du [!UICONTROL Account], aucune alerte par e-mail n’est envoyée aux collaborateurs et aux collaboratrices, même si [!UICONTROL Disabled email alert] n’est pas sélectionnée sur les épreuves.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
