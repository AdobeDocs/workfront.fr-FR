---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Partager une épreuve dans Adobe Workfront
description: Vous pouvez partager un document révisé dans Adobe Workfront en partageant le document ou en ajoutant des utilisateurs et utilisatrices à l’épreuve.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '1233'
ht-degree: 100%

---

# Partager une épreuve dans Adobe Workfront

Vous pouvez partager un document révisé dans Adobe Workfront en partageant le document ou en ajoutant des utilisateurs et utilisatrices à l’épreuve.

Si vous partagez l’épreuve, comme expliqué dans cet article, votre destinataire a le même accès au document et à l’épreuve. De plus, vous pouvez demander un approbation de l’épreuve à la personne destinataire.

>[!TIP]
>
>Vous pouvez également partager une épreuve depuis la visionneuse de relecture. Pour obtenir des instructions, voir [Partager une épreuve à partir de la visionneuse de relecture](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

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
   <td role="rowheader">Rôle de l’épreuve</td> 
   <td>Auteur ou autrice, ou modérateur ou modératrice</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander un accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation d’épreuve dont vous disposez, contactez votre administrateur ou administratrice de Workfront ou Workfront Proof.

+++

## Partager un lien vers l’épreuve

Le partage d’un lien vers l’épreuve accorde aux utilisateurs et utilisatrices Workfront un accès à l’affichage. Les utilisateurs et utilisatrices peuvent commenter l’épreuve et s’abonner à des notifications par e-mail pour l’épreuve à l’aide de leurs informations de connexion Workfront. Les personnes qui ne sont pas en charge de la relecture peuvent commenter et s’abonner à l’aide d’une adresse e-mail et d’un nom d’affichage.

>[!IMPORTANT]
>
>Le paramètre Autoriser le partage de l’épreuve via une URL publique ou un code intégré doit être activé.

1. Sélectionnez le document contenant l’épreuve que vous souhaitez partager avec les utilisateurs et utilisatrices.

   Vous ne pouvez sélectionner qu’un seul document. Vous ne pouvez pas partager le lien de plusieurs documents simultanément.

1. Cliquez sur **Partager** > **Lien de l’épreuve**.
1. Dans la zone **Lien de l’épreuve** qui s’affiche, effectuez l’une des opérations suivantes :

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

## Ajouter des utilisateurs et utilisatrices à une épreuve

Vous pouvez ajouter n&#39;importe quel utilisateur ou utilisatrice Workfront à l’épreuve si vous disposez des droits de modification sur l’épreuve. Si l’épreuve comporte plusieurs étapes, vous ajoutez l’utilisateur ou utilisatrice à une étape individuelle.

>[!WARNING]
>
>Outre les méthodes listées dans cet article, il est possible d’ajouter des utilisateurs et utilisatrices à une épreuve en les taguant dans un commentaire à partir de l’onglet Mises à jour d’une épreuve existante. Cependant, les personnes ajoutées à une épreuve de cette manière ne reçoivent pas de notification par e-mail, sauf si elles sont à nouveau taguées après avoir été ajoutées au workflow de l’épreuve.
>
>Par conséquent, nous vous recommandons d’ajouter des personnes à une épreuve à l’aide de l’une des méthodes répertoriées ci-dessous, et non en les taguant dans un commentaire.
>

>[!NOTE]
>
>Gardez ce qui suit à l’esprit si vous utilisez un plan Workfront hérité dans lequel la relecture peut être activée et désactivée pour un utilisateur ou une utilisatrice :
>
>* Les destinataires n’ont pas besoin d’activer la relecture pour pouvoir réviser l’épreuve.
>* Lorsque le workflow automatisé est activé et que vous ajoutez une personne à l’épreuve qui n’a pas la relecture d’activée dans Workfront, une nouvelle étape est créée dans le workflow automatisé. La personne que vous ajoutez est automatiquement ajoutée à cette nouvelle étape lorsqu’elle consulte l’épreuve pour la première fois. Pour plus d’informations, voir [Vue d’ensemble du workflow automatisé](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).
>

### Ajouter des utilisateurs et utilisatrices à une épreuve existante depuis l’onglet Documents

1. Sélectionnez le document contenant l’épreuve à laquelle vous souhaitez ajouter des utilisateurs et des utilisatrices.
1. Si l’épreuve ne dispose pas d’un workflow automatisé (étapes), cliquez sur l’icône **Plus** dans le coin supérieur droit de la section Étape 1, puis cliquez sur **Partager** dans le menu déroulant.

   Ou

   Si l’épreuve dispose d’un workflow automatisé, cliquez sur l’icône **Plus** dans le coin supérieur droit de l’étape où vous souhaitez ajouter la personne chargée de la révision, puis cliquez sur **Partager** dans le menu déroulant.

1. Dans la zone **Partager cette version** qui apparaît, sous **Partager**, commencez à saisir le nom ou l’adresse e-mail d’un utilisateur ou d’une utilisatrice avec qui vous souhaitez partager l’épreuve, puis cliquez sur son nom lorsqu’il apparaît dans la liste déroulante.

1. (Facultatif) Répétez cette étape pour ajouter plusieurs utilisateurs et utilisatrices à l’épreuve.
1. (Facultatif) Définir une date d’échéance pour les personnes chargées de la révision.
1. (Facultatif) Assurez-vous que l’option **Notifier les personnes par e-mail** est sélectionnée si vous souhaitez informer les personnes chargées de la révision que vous les avez ajoutées à l’épreuve.
1. (Facultatif) **Ajoutez un message personnalisé** à l’e-mail.
1. Lorsque vous avez ajouté toutes les personnes chargées de la révision, cliquez sur **Partager**.

### Ajouter des utilisateurs et utilisatrices à une épreuve existante à partir de la visionneuse de relecture

Vous pouvez ajouter des utilisateurs et utilisatrices à une épreuve lorsque vous révisez une épreuve dans la visionneuse de relecture web ou dans la visionneuse de relecture de bureau.

Pour plus d’informations, voir [Partager une épreuve en y ajoutant des utilisateurs et des utilisatrices](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) dans l’article [Partager une épreuve à partir de la visionneuse de relecture](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Rapport sur les approbations de relecture

Vous pouvez créer un rapport qui tient compte des approbations d’épreuves partagées dans Workfront. Ce rapport fournit les informations d’approbation d’épreuve suivantes dans votre système :

* Document soumis à approbation
* Nom de la personne chargée de l’approbation
* Version de l’épreuve
* ID de l&#39;épreuve
* Date de création de l’épreuve

Vous accédez à cette approbation lorsque vous créez un rapport basé sur un objet, comme décrit dans la section [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour plus d’informations sur le rapport d’objet des approbations d’épreuves, voir [Rapport sur les objets](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) dans [Vue d’ensemble des objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## Approuver une épreuve partagée

Lorsqu’un utilisateur ou une utilisatrice vous ajoute à une épreuve et vous attribue soit le rôle de personne chargée de l’approbation, soit le rôle de personne chargée de la révision et de l’approbation à l’aide du workflow automatisé, la demande d’approbation s’affiche dans l’onglet des approbations de votre zone d’accueil ou de votre zone Mon travail. Vous pouvez ensuite afficher l’épreuve et prendre une décision d’approbation sur l’épreuve directement à partir de Workfront.

Pour plus d’informations sur la manière de prendre des décisions d’approbation à partir de la zone « Mon travail », consultez les sections [Approuver du travail à partir de la zone d’accueil](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) ou [Approuver du travail](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) dans [Approuver du travail](../../../review-and-approve-work/manage-approvals/approving-work.md).
