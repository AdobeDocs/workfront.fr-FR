---
product-area: documents
navigation-topic: approvals
title: Ajouter des approbateurs ou des réviseurs supplémentaires à un workflow d’approbation de document
description: Vous pouvez ajouter des réviseurs et réviseuses ou des approbateurs et approbatrices supplémentaires à un document ayant déjà des approbations en attente.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jo3N878hmvHRqo6kCepxPDk2-zlalLvqQbMjHHB8aGE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 532
ht-degree: 18%

---

# Ajouter des approbateurs ou des réviseurs supplémentaires à un workflow d’approbation de document

Vous pouvez ajouter d&#39;autres approbateurs ou réviseurs à un workflow d&#39;approbation de document qui a déjà des approbations en attente.

>[!IMPORTANT]
>
>Le contenu de cet article fait référence à la fonctionnalité d’approbation de document mise à jour, disponible uniquement pour des comptes spécifiques. Pour plus d’informations sur les processus d’approbation standard, reportez-vous aux articles répertoriés dans la section [Approbations de travail](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tout package Workfront pour gérer les approbations à l’aide du stockage Workfront hérité</p>
<p>Tout package de workflow pour gérer les validations à l’aide de l’espace de stockage dans le cloud Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Contributeur ou supérieur</p>
   <p>Révision ou supérieur</p> 
   <p>Si vous utilisez l'intégration Frame.io, vous devez disposer d'une licence Standard pour créer des workflows d'approbation.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accédez en lecture seule ou à un accès plus étendu aux projets, tâches, événements, modèles, portefeuilles, programmes, rapports, tableaux de bord, calendriers et documents</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher ou avoir un accès supérieur à l’objet associé à l’approbation ou à l’accès à la demande </p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Ajoutez d&#39;autres approbateurs ou réviseurs à partir du Résumé du document dans la zone des documents hérités

Si votre organisation utilise le stockage Workfront, la zone des documents hérités s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage Workfront, voir [Différences entre le stockage cloud Adobe et le stockage Workfront hérité](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Pour ajouter des approbateurs ou des réviseurs supplémentaires à partir du résumé du document :

1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document dont vous avez besoin pour ouvrir le panneau Résumé du document correspondant.

1. Sélectionnez la version du document auquel vous souhaitez ajouter un approbateur ou un réviseur dans le menu déroulant Version. La dernière version est sélectionnée par défaut.

1. Faites défiler l’écran jusqu’à la section **Validations**, puis cliquez sur **Modifier le workflow**.

   ![modifier le workflow d’approbation](assets/edit-approval-in-legacy.png)

1. Localisez l’étape à laquelle vous souhaitez ajouter des approbateurs ou des réviseurs, puis ajoutez le nom ou l’adresse électronique de l’utilisateur dans la zone de texte. Vous pouvez également ajouter une équipe entière si nécessaire.

1. Une fois leur nom ajouté, choisissez s’ils sont approbateurs ou réviseurs.

   ![liste déroulante approbateur ou réviseur](assets/choose-approver-or-reviewer.png)

1. Répétez les étapes 5 à 6 pour ajouter d’autres approbateurs ou réviseurs ou réviseuses.
Une fois le document enregistré, les participants ajoutés reçoivent une notification par e-mail indiquant que leur approbation ou révision est nécessaire pour le document.



## Ajoutez d&#39;autres approbateurs ou réviseurs à partir du Résumé du document dans la zone des nouveaux Documents

Si votre entreprise utilise l’espace de stockage Adobe dans le cloud, la nouvelle zone Documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur l’espace de stockage dans le cloud Adobe, consultez [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Accédez au projet, à la tâche ou à l’événement contenant le document, puis sélectionnez **Documents** dans le panneau de gauche.

1. Cliquez sur le document, puis sur l’icône **Validations** sur le côté droit de la page.

   ![Ajouter des approbateurs dans le résumé du document](assets/approvals-icon-new.png)


1. Cliquez sur **Modifier le workflow**.

1. Localisez l’étape à laquelle vous souhaitez ajouter des approbateurs ou des réviseurs, puis ajoutez le nom ou l’adresse électronique de l’utilisateur dans la zone de texte. Vous pouvez également ajouter une équipe entière si nécessaire.

1. Une fois leur nom ajouté, choisissez s’ils sont approbateurs ou réviseurs.

   ![liste déroulante approbateur ou réviseur](assets/choose-approver-or-reviewer.png)

1. Répétez les étapes 5 à 6 pour ajouter d’autres approbateurs ou réviseurs ou réviseuses.
Une fois le document enregistré, les participants ajoutés reçoivent une notification par e-mail indiquant que leur approbation ou révision est nécessaire pour le document.







<!--
## Add additional approvers or reviewers from Home

1. Click the **Home** icon ![Home icon](assets/home-icon-30x29.png) in the upper-left corner of Adobe Workfront.

   >[!NOTE]
   >
   >Your Workfront administrator might make the following changes to the Home icon in your environment:
   >
   >* Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. 
   >* Replace the page linked to it with a different page. In this case, click the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of the page, then click **Home**.

1. In the **Work List** area, Go to the **Approvals I've Submitted** grouping.

1. Select a **Document** approval.  

1. Click **Manage Approvals**&nbsp;in the upper-right corner of the right panel.
1. In the **Have someone approve this document** box, type the name of the approver.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

1. Click **Save**.
-->
