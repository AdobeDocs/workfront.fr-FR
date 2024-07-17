---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Configuration des paramètres de notification électronique dans  [!DNL Workfront Proof]
description: Les notifications électroniques générées par Workfront Proof informent les collaborateurs de l’activité récente sur les bons à tirer (commentaires, réponses ou décisions).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '2049'
ht-degree: 0%

---

# Configuration des paramètres de notification électronique dans [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Les notifications par e-mail informent les collaborateurs de l’activité récente sur les bons à tirer, comme les commentaires, les réponses ou les décisions.

Vous pouvez définir des notifications par email pour les réviseurs dans les zones suivantes :

Les notifications électroniques destinées aux réviseurs peuvent être définies sur la page New BAT, la page [!UICONTROL New version] et gérées dans la section [!UICONTROL Workflow] de la page [!UICONTROL Détails du BAT]. Pour plus d’informations, voir [Générer des bons à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* La page Nouveau BAT
* La page [!UICONTROL Nouvelle version]
* La section [!UICONTROL Workflow] de la page [!UICONTROL Détails du bon à tirer] .

Pour plus d’informations, voir [Générer des bons à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)


* [Générer un bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Gérer les détails du BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).


Chaque utilisateur peut également définir ses propres paramètres d’alerte par email qui sont automatiquement appliqués lorsqu’un BAT est partagé avec lui si les collaborateurs ont leurs préférences ou si les administrateurs de compte ont leurs recommandations sur la fréquence des alertes. Il peut être défini comme valeur par défaut du BAT sur les pages de détails des utilisateurs.

Chaque utilisateur peut également définir ses propres paramètres d’alerte par email qui seront automatiquement appliqués lorsqu’un BAT est partagé avec lui. <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>Ces paramètres sont suggérés lorsque les utilisateurs créent les bons à tirer et ajoutent ces collaborateurs. Cependant, il s’agit uniquement de suggestions. Elles peuvent donc être ajustées à tout moment pendant le processus de révision et les modifications s’appliquent à toutes les activités effectuées après la modification. Les paramètres par défaut du BAT sont remplacés par les paramètres au niveau du BAT.

Les utilisateurs disposant de profils [!UICONTROL Administrator] ou [!UICONTROL Billing Administrator] peuvent également définir les paramètres par défaut du BAT pour les autres utilisateurs de leur compte dans les paramètres du compte.

Pour plus d’informations sur les profils, voir [Profils d’autorisations de BAT dans [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

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

## Configuration des paramètres par défaut du BAT dans les paramètres personnels ([!DNL Workfront Proof] utilisateurs uniquement)

Vous pouvez configurer les paramètres du BAT pour les BAT que vous créez.

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres personnels]**.

1. Cliquez sur l’onglet **[!UICONTROL Valeurs par défaut du contrôle d’accès]** .
1. Cliquez sur **[!UICONTROL Paramètres de notification par défaut]** pour le développer.
1. Dans la liste déroulante située à droite des deux paramètres suivants, sélectionnez l’une des options expliquées dans le tableau ci-dessous.

   * **[!UICONTROL Alerte par défaut par e-mail]** : affecte chaque BAT partagé avec vous. Ce paramètre peut être remplacé au niveau du BAT.
   * **[!UICONTROL Alerte par défaut pour les nouveaux réviseurs invités]** : affecte les réviseurs qui n’existaient pas auparavant en tant que contacts dans votre compte.

   >[!NOTE]
   >
   >Si vous ne choisissez pas l’une des options suivantes, [!DNL Workfront Proof] vous envoie un résumé quotidien de l’activité sur vos bons à tirer.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Toutes les activités]</td> 
      <td>[!UICONTROL Workfront] envoie un courrier électronique au réviseur chaque fois qu’il y a une activité sur le BAT, comme un nouveau commentaire, une nouvelle réponse ou une nouvelle décision. <p>Il s’agit d’une excellente option pour la personne qui gère le processus de vérification car elle lui permet de voir l’activité telle qu’elle se produit. </p><p>Les utilisateurs ne reçoivent pas d’alerte par e-mail sur leur propre activité.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Réponses à mes commentaires]</td> 
      <td>Un email n'est envoyé au validant que si quelqu'un répond explicitement à son commentaire (cela exclut ses propres réponses sur ses propres commentaires). Cela signifie que si quelqu'un sur le BAT fait un nouveau commentaire, le validant n'en est pas informé.<p>Ce paramètre est recommandé pour vos clients sur le BAT afin qu’ils ne soient pas informés des autres commentaires sur le BAT et qu’ils ne soient informés que des réponses à leurs propres commentaires.</p><p>Bien que les réviseurs avec ce paramètre d’alerte par e-mail ne soient pas informés des autres nouveaux commentaires, ils peuvent toujours afficher tous les commentaires sur le BAT dans la visionneuse de vérification.</p><p>Pour plus d’informations sur les commentaires, voir <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Affichage et réponse aux commentaires du BAT</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisions]</td> 
      <td>[!DNL Workfront] envoie un courrier électronique au réviseur uniquement lorsqu’une personne prend une décision.<p>Cela peut s’avérer utile pour la personne qui gère le processus de validation (par exemple, un chef de projet) et qui doit surveiller l’avancement du BAT et voir quels utilisateurs ont pris leur décision.</p><p>Vous n’êtes pas informé de votre propre décision, sauf si vous sélectionnez une option de confirmation par courrier électronique lors de l’envoi de votre décision.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Décision finale]</td> 
      <td>[!DNL Workfront] envoie un email lorsque le dernier approbateur du BAT a pris sa décision.<p>Cette alerte est souvent utilisée par le concepteur, qui n’a généralement pas besoin de prendre part à la discussion de révision proprement dite. Lorsque la décision finale est prise, le concepteur est informé et peut alors prendre des mesures sur les modifications nécessaires.</p><p>Cette alerte peut également s’avérer utile pour un responsable de service qui n’a besoin d’être averti que lorsque le processus de révision est terminé.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Résumé horaire]</td> 
      <td>[!DNL Workfront] envoie un email au validant toutes les heures avec un résumé de tous les commentaires, réponses et décisions de l'heure.<p>L’e-mail n’est envoyé que lorsque l’activité se produit au-delà de la vôtre au cours de la dernière heure. </p><p>Cette alerte est une bonne manière de visualiser un aperçu du projet.</p><p>Un exemple de cas d’utilisation pour ce résumé est un validant principal qui a besoin d’une vue d’ensemble du projet, mais qui n’a pas besoin d’être informé immédiatement de toute l’activité sur le BAT.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Résumé quotidien]</td> 
      <td>[!DNL Workfront] envoie un email contenant tous les commentaires, réponses et décisions répertoriés uniquement les jours où il y a une activité en dehors de la vôtre.<p>Cette alerte est une bonne façon de voir un résumé du projet sans être submergé par de multiples mises à jour tout au long de la journée.</p><p>Un exemple de cas d’utilisation pour ce résumé est un chef de département qui souhaite surveiller l’avancement global du projet.</p><p>Pour plus d’informations, voir <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestion des notifications pour les commentaires et les décisions de BAT</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Aucun courrier électronique]</td> 
      <td>[!DNL Workfront] n’envoie aucune alerte par courrier électronique.<br>Cela s’avère utile pour une personne qui n’est ajoutée à un BAT qu’à titre de référence et qui n’a pas besoin d’être informée des modifications.<p>La valeur par défaut du système est [!UICONTROL Résumé quotidien] (également appelé [!UICONTROL Non défini]). Si vous ou vos réviseurs n’effectuez aucune autre modification, tous vos BAT disposent de ce paramètre.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Modifiez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Confirmation par e-mail lorsque les bons à tirer sont prêts]</td> 
      <td>Indiquez si vous souhaitez recevoir un email [!UICONTROL BAT effectué] lors de la création d’un BAT. Pour plus d’informations, voir <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">L’'email [!UICONTROL BAT Made]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format des emails m’étant envoyés] </td> 
      <td> <p>Choisissez entre HTML des emails stylisés et des emails texte brut. </p> <p><b>NOTE</b></p>
      <p>Les paramètres par défaut de la vérification sont remplacés par les paramètres au niveau du BAT. Toutefois, si les notifications par courrier électronique du BAT sont désactivées pour l’ensemble du compte dans les paramètres du [!UICONTROL Compte] , aucune alerte par courrier électronique n’est envoyée aux collaborateurs, même si l’[!UICONTROL Désactivé] n’est pas sélectionnée sur les bons à tirer.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Sous **[!UICONTROL Paramètres du message]**, modifiez l’une des options suivantes :

   | Modèle de BAT | Description |
   |---|---|
   | **[!UICONTROL Modèle d’objet de BAT]** | S’affiche sur les pages Nouveau BAT, Nouvelle version, Message et Remind . Peut être modifié avant d’être envoyé. |
   | **[!UICONTROL Modèle de message de BAT]** | S’affiche sur les pages Nouveau BAT, Nouvelle version, Message et Rappel . Peut être modifié avant d’être envoyé. |

## Modifier les alertes par email d&#39;un destinataire

Vous pouvez modifier les alertes par email d’un destinataire spécifique dans une action par lot.

1. Cliquez sur **[!UICONTROL Contacts]** dans le panneau de navigation de gauche.
1. Cliquez sur le menu **[!UICONTROL Plus]** ![](assets/more-button-small.png) du destinataire, puis sur **[!UICONTROL Afficher les détails du membre]** dans le menu déroulant.

1. Ouvrez la section **[!UICONTROL Éléments partagés]** .
1. Cochez la case à gauche de chaque élément pour lequel vous souhaitez modifier l’alerte par courrier électronique.
1. Cliquez sur **[!UICONTROL Plus]** au-dessus de la liste des éléments partagés, puis cliquez sur **[!UICONTROL Modifier l’alerte par courrier électronique]** dans le menu déroulant.

1. Modifiez l’alerte par courrier électronique, puis cliquez sur **[!UICONTROL Envoyer]**.

## Configuration des paramètres par défaut d’un BAT pour un utilisateur

Si vous êtes administrateur [!DNL Workfront Proof], vous pouvez définir les paramètres par défaut du BAT pour les utilisateurs de votre compte.

1. Cliquez sur **[!UICONTROL Paramètres]** > **[!UICONTROL Paramètres du compte]**.

1. Ouvrez l’onglet **[!UICONTROL Utilisateurs]** .
1. Ouvrez le menu **[!UICONTROL Plus]** ![More_button_small.png](assets/more-button-small.png) à droite du nom de l’utilisateur.

1. Cliquez sur **[!UICONTROL Afficher les détails des utilisateurs]** dans le menu déroulant.
1. Sous **[!UICONTROL Paramètres]**, cliquez sur **[!UICONTROL Paramètres d’alerte par défaut]** pour le développer.

1. Dans la liste déroulante située à droite des deux paramètres suivants, sélectionnez l’une des options expliquées dans le tableau ci-dessous :

   * **[!UICONTROL Alerte par défaut par e-mail]** : affecte chaque BAT partagé avec vous. Ce paramètre peut être remplacé au niveau du BAT.
   * **[!UICONTROL Alerte par défaut pour les nouveaux réviseurs invités]** : affecte les réviseurs qui n’existaient pas auparavant en tant que contacts dans votre compte.

   >[!NOTE]
   >
   >Si vous ne choisissez pas l’une des options suivantes pour un utilisateur, [!DNL Workfront Proof] envoie aux utilisateurs un résumé quotidien de l’activité sur leurs bons à tirer.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL Toutes les activités]</td>
      <td>[!DNL Workfront] envoie un email au validant chaque fois qu'il y a une activité sur le BAT, comme un nouveau commentaire, une nouvelle réponse ou une nouvelle décision. <p>Il s’agit d’une excellente option pour la personne qui gère le processus de vérification car elle lui permet de voir l’activité telle qu’elle se produit. </p><p>Les utilisateurs ne reçoivent pas d’alerte par e-mail sur leur propre activité.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Réponses à mes commentaires]</td>
      <td>Un email n'est envoyé au validant que si quelqu'un répond explicitement à son commentaire (cela exclut ses propres réponses sur ses propres commentaires). Cela signifie que si quelqu'un sur le BAT fait un nouveau commentaire, le validant n'en est pas informé.<p>Ce paramètre est recommandé pour vos clients sur le BAT afin qu’ils ne soient pas informés des autres commentaires sur le BAT et qu’ils ne soient informés que des réponses à leurs propres commentaires.</p><p>Bien que les réviseurs avec ce paramètre d’alerte par e-mail ne soient pas informés des autres nouveaux commentaires, ils peuvent toujours afficher tous les commentaires sur le BAT dans la visionneuse de vérification.</p><p>Pour plus d’informations sur les commentaires, voir <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Affichage et réponse aux commentaires du BAT</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisions]</td>
      <td>[!DNL Workfront] envoie un courrier électronique au réviseur uniquement lorsqu’une personne prend une décision.<p>Cela peut s’avérer utile pour la personne qui gère le processus de validation (par exemple, un chef de projet) et qui doit surveiller l’avancement du BAT et voir quels utilisateurs ont pris leur décision.</p><p>Vous n’êtes pas informé de votre propre décision, sauf si vous sélectionnez une option de confirmation par courrier électronique lors de l’envoi de votre décision.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Décision finale]</td>
      <td>[!DNL Workfront] envoie un email lorsque le dernier approbateur du BAT a pris sa décision.<p>Cette alerte est souvent utilisée par le concepteur, qui n’a généralement pas besoin de prendre part à la discussion de révision proprement dite. Lorsque la décision finale est prise, le concepteur est informé et peut alors prendre des mesures sur les modifications nécessaires.</p><p>Cette alerte peut également s’avérer utile pour un responsable de service qui n’a besoin d’être averti que lorsque le processus de révision est terminé.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Résumé horaire]</td>
      <td>[!DNL Workfront] envoie un email au validant toutes les heures avec un résumé de tous les commentaires, réponses et décisions de l'heure.<p>L’e-mail n’est envoyé que lorsque l’activité se produit au-delà de la vôtre au cours de la dernière heure. </p><p>Cette alerte est une bonne manière de visualiser un aperçu du projet.</p><p>Un exemple de cas d’utilisation pour ce résumé est un validant principal qui a besoin d’une vue d’ensemble du projet, mais qui n’a pas besoin d’être informé immédiatement de toute l’activité sur le BAT.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Résumé quotidien]</td>
      <td>[!DNL Workfront] envoie un email contenant tous les commentaires, réponses et décisions répertoriés uniquement les jours où il y a une activité en dehors de la vôtre.<p>Cette alerte est une bonne façon de voir un résumé du projet sans être submergé par de multiples mises à jour tout au long de la journée.</p><p>Un exemple de cas d’utilisation pour ce résumé est un chef de département qui souhaite surveiller l’avancement global du projet.</p><p>Pour plus d’informations, voir <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gestion des notifications pour les commentaires et les décisions de BAT</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL Aucun courrier électronique]</td>
      <td>[!DNL Workfront] n’envoie aucune alerte par courrier électronique.<br>Cela s’avère utile pour une personne qui n’est ajoutée à un BAT qu’à titre de référence et qui n’a pas besoin d’être informée des modifications.<p>La valeur par défaut du système est [!UICONTROL Résumé quotidien] (également appelé [!UICONTROL Non défini]). Si vous ou vos réviseurs n’effectuez aucune autre modification, tous vos BAT disposent de ce paramètre.</p></td>
     </tr>
    </tbody>
   </table>

1. Dans les **[!UICONTROL paramètres d’alerte par défaut]** restants, modifiez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Confirmation par e-mail lorsque les bons à tirer sont prêts]</td> 
      <td>Indiquez si vous souhaitez recevoir un email [!UICONTROL BAT effectué] lors de la création d’un BAT. Pour plus d’informations, voir <a href="https://support.workfront.com/hc/en-us/article">L’'email [!UICONTROL BAT Made].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format des emails m’étant envoyés] </td> 
      <td> <p>Choisissez entre HTML des emails stylisés et des emails texte brut. </p> <p><b>NOTE</b></p> <p>Les paramètres par défaut de la vérification sont remplacés par les paramètres au niveau du BAT. Toutefois, si les notifications par courrier électronique du BAT sont désactivées pour l’ensemble du compte dans les paramètres du [!UICONTROL Compte] , aucune alerte par courrier électronique n’est envoyée aux collaborateurs, même si l’[!UICONTROL Désactivé] n’est pas sélectionnée sur les bons à tirer.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
