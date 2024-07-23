---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Partager une épreuve dans Adobe Workfront
description: Vous pouvez partager un document révisé dans Adobe Workfront en partageant le document ou en ajoutant des utilisateurs au BAT.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '1233'
ht-degree: 5%

---

# Partager une épreuve dans Adobe Workfront

Vous pouvez partager un document révisé dans Adobe Workfront en partageant le document ou en ajoutant des utilisateurs au BAT.

Si vous partagez le BAT, comme expliqué dans cet article, votre destinataire a le même accès au document et au BAT. De plus, vous pouvez demander la validation du BAT au destinataire.

>[!TIP]
>
>Vous pouvez également partager un BAT depuis la visionneuse de vérification. Pour plus d&#39;informations, voir [Partage d&#39;un BAT à partir de la visionneuse de tests](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td role="rowheader">Rôle de l’épreuve</td> 
   <td>Auteur ou modérateur</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront Proof.

+++

## Partage d’un lien de BAT

Le partage d’un lien de BAT permet aux utilisateurs Workfront de consulter l’accès. Les utilisateurs peuvent commenter le BAT et s’abonner à des notifications électroniques pour le BAT à l’aide de leurs informations de connexion Workfront. Les utilisateurs qui ne sont pas en charge de la vérification de l’exactitude peuvent commenter et s’abonner à l’aide d’une adresse électronique et d’un nom d’affichage.

>[!IMPORTANT]
>
>Le paramètre Autoriser le partage du BAT via une URL publique ou le code incorporé doit être activé.

1. Sélectionnez le document contenant le BAT que vous souhaitez partager avec les utilisateurs.

   Vous pouvez sélectionner un seul document. Vous ne pouvez pas partager le lien de plusieurs documents simultanément.

1. Cliquez sur **Partager** > **Lien du bon à tirer**.
1. Dans la zone **Proof link** qui s’affiche, effectuez l’une des opérations suivantes :

   * Pour copier le lien dans le presse-papiers, cliquez sur **Copier le lien**.

     Vous pouvez désormais diffuser le lien par le biais d&#39;un outil tiers, tel qu&#39;une messagerie instantanée ou une application de messagerie.

   * Pour envoyer le lien directement par courrier électronique à partir d’Adobe Workfront, procédez comme suit :

      1. Dans le champ **Ou lien d&#39;email vers** , commencez à saisir le nom de votre destinataire et sélectionnez-le. Vous pouvez également spécifier l’adresse électronique d’un utilisateur externe avec lequel vous souhaitez effectuer un partage.

         >[!NOTE]
         >
         >Si vous voyez un email d’alias lors du partage d’un BAT, ne créez pas un nouvel utilisateur invité en saisissant l’email d’origine s’il existe un email d’alias correspondant.

      1. Sélectionnez l’une des options suivantes :

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Envoyer le lien public</td>
            <td><p>Inclut un bouton dans la notification électronique qui dirige les utilisateurs vers le BAT dans la visionneuse de vérification qu’ils utilisent et leur accorde l’accès en mode Vue.</p><p>Si <strong>S’abonner au BAT par le biais d’une URL publique ou du code incorporé</strong> est désactivé pour le BAT, les utilisateurs peuvent se connecter à l’aide de leurs informations d’identification de connexion Workfront pour ajouter des commentaires au BAT. Si elle est activée, toute personne fournissant son adresse électronique et son nom (aucun mot de passe requis) peut signer et ajouter des commentaires au BAT.</p></td>
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

## Ajout d’utilisateurs à un BAT

Vous pouvez ajouter n&#39;importe quel utilisateur Workfront au BAT si vous disposez des droits d&#39; édition sur le BAT. Si le BAT comporte plusieurs étapes, vous ajoutez l’utilisateur à une étape individuelle.

>[!WARNING]
>
>Outre les méthodes listées dans cet article, il est possible d&#39;ajouter des utilisateurs à un BAT en les marquant dans un commentaire à partir de l&#39;onglet Mises à jour d&#39;un BAT existant. Cependant, les utilisateurs ajoutés à un BAT de cette manière ne reçoivent pas de notification par email, sauf s’ils sont à nouveau balisés après avoir été ajoutés au workflow du BAT.
>
>Par conséquent, nous vous recommandons d’ajouter des utilisateurs à un BAT à l’aide de l’une des méthodes répertoriées ci-dessous, et non en les marquant dans un commentaire.
>

>[!NOTE]
>
>Gardez ce qui suit à l’esprit si vous utilisez un plan Workfront hérité dans lequel la vérification peut être activée et désactivée pour un utilisateur :
>
>* Les destinataires n&#39;ont pas besoin d&#39;activer la vérification pour pouvoir passer en revue le BAT.
>* Lorsque le processus automatisé est activé et que vous ajoutez un utilisateur au BAT pour lequel la vérification n’est pas activée dans Workfront, une nouvelle étape est créée dans le processus automatisé. L’utilisateur que vous ajoutez est automatiquement ajouté à cette nouvelle étape lorsqu’il visualise le BAT pour la première fois. (Pour plus d’informations, voir [Présentation du processus automatisé](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>

### Ajouter des utilisateurs à un BAT existant depuis l&#39;onglet Documents

1. Sélectionnez le document contenant le BAT auquel vous souhaitez ajouter des utilisateurs.
1. Si le BAT ne dispose pas d’un workflow automatisé (étapes), cliquez sur l’icône **Plus** dans le coin supérieur droit de la section Phase 1, puis cliquez sur **Partager** dans le menu déroulant.

   Ou

   Si le BAT dispose d’un workflow automatisé, cliquez sur l’icône **Plus** dans le coin supérieur droit de l’étape où vous souhaitez ajouter le réviseur, puis cliquez sur **Partager** dans le menu déroulant.

1. Dans la zone **Partager cette version** qui apparaît, sous **Partager**, commencez à saisir le nom ou l’adresse électronique d’un utilisateur avec lequel vous souhaitez partager le BAT, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

1. (Facultatif) Répétez cette étape pour ajouter plusieurs utilisateurs au BAT.
1. (Facultatif) Définissez un délai pour les réviseurs.
1. (Facultatif) Assurez-vous que l&#39;option **Avertir les personnes par email** est sélectionnée si vous souhaitez informer les réviseurs que vous les avez ajoutés au BAT.
1. (Facultatif) **Ajoutez un message personnalisé** à l’email.
1. Lorsque vous avez ajouté tous les réviseurs, cliquez sur **Partager**.

### Ajout d’utilisateurs à un BAT existant à partir de la visionneuse de vérification

Vous pouvez ajouter des utilisateurs à un BAT lorsque vous passez en revue un BAT dans la visionneuse de BAT Web et dans la visionneuse de BAT.

Pour plus d’informations, voir [Partager un BAT en y ajoutant des utilisateurs](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) dans l’article [Partager un BAT à partir de la visionneuse de correctifs](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Rapport sur les validations de vérification

Vous pouvez créer un rapport qui tient compte des approbations de vérification qui ont été partagées dans Workfront. Ce rapport fournit les informations de validation de BAT suivantes dans votre système :

* Document soumis à approbation
* Nom de l’approbateur
* Version du BAT
* ID de l&#39;épreuve
* Date de création du BAT

Vous accédez à cette approbation lors de la création d’un rapport basé sur un objet, comme décrit dans la section [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour plus d’informations sur le rapport d’objet Approbations de BAT, reportez-vous à la section [Rapport sur les objets](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) dans [Présentation des objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Approbation d’un BAT partagé

Lorsqu’un utilisateur vous ajoute à un BAT et accorde le rôle d’approbateur ou de réviseur et d’approbateur à l’aide d’un workflow automatisé, la demande d’approbation s’affiche dans l’onglet Approbations de votre page d’accueil ou de la zone Mon travail. Vous pouvez ensuite afficher le BAT et prendre une décision d’approbation sur le BAT directement depuis Workfront.

Pour plus d’informations sur la façon de prendre des décisions d’approbation à partir de la zone Mon travail, voir [Approuver le travail à partir de la zone d’accueil](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) ou [Valider le travail](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) dans [Valider le travail](../../../review-and-approve-work/manage-approvals/approving-work.md).
