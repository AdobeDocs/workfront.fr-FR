---
product-area: programs
navigation-topic: create and manage programs
title: Ajout d’un programme existant à un Portfolio
description: Vous pouvez ajouter des programmes existants à un portfolio. Les programmes ne pouvant exister dans deux portfolios différents, l’ajout d’un programme existant le fait passer définitivement d’un portfolio à l’autre.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 73dbe277-12d2-4041-8a02-91ccf5f8b465
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/LkyWuPHqv0muTinWZT1PMKPGUNErWulIIxHmXVtPIVg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 382
ht-degree: 34%

---

# Ajouter un programme existant à un portfolio

<!--Audited: 05/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

Vous pouvez ajouter des programmes existants à un portfolio. Les programmes ne pouvant exister dans deux portfolios différents, l’ajout d’un programme existant le fait passer définitivement d’un portfolio à l’autre.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquet</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>[!UICONTROL Standard]</p><p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès de [!UICONTROL Edit] aux [!UICONTROL Portfolios] et [!UICONTROL Programmes] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour le portfolio et le programme</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard] </p><p>Or </p><p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio and the program</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Ajouter un programme existant à un portfolio

>[!NOTE]
>
>Lorsque votre entreprise utilise à la fois l’espace de stockage cloud Workfront et Adobe hérité pour les documents, les scénarios suivants existent :
>
>
>* Lorsque vous ajoutez un programme de stockage dans le cloud Adobe à un portfolio de stockage Workfront hérité et que ce portfolio n’est associé à aucun document, le portfolio est converti en stockage dans le cloud Adobe.
>* Lorsque vous ajoutez un programme de stockage dans le cloud Adobe à un portfolio de stockage Workfront hérité auquel des documents sont associés, le stockage des documents du portfolio reste sur le stockage Workfront. Toutefois, l’icône de stockage Workfront héritée ![icône de stockage Workfront héritée](assets/legacy-storage-project-icon.png) est supprimée du portfolio.
>* Vous ne pouvez pas ajouter un ancien programme de stockage Workfront à un portefeuille de stockage dans le cloud Adobe.
>
>Pour plus d’informations, voir [Présentation de la gestion des documents pour les projets et les objets associés](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).
>
>Toutes les instances Workfront ne possèdent pas les deux types de stockage de documents.

Pour ajouter un programme existant à un autre portefeuille :

1. Accédez à un portfolio, puis cliquez sur **[!UICONTROL Programmes]** dans le panneau de gauche.
1. Cliquez sur **[!UICONTROL Nouveau programme]**.
1. Cliquez sur **[!UICONTROL Programme existant]**.

   La boîte de dialogue **Ajouter des programmes** s’ouvre. <!--check screen shot - I logged changes for this casing-->

   ![Boîte Ajouter un programme](assets/add-programs-box.png)

   >[!IMPORTANT]
   >
   >L’ajout d’un programme existant transfère tous les projets associés à ce programme dans le portfolio. Veillez à ne pas déplacer involontairement des projets de cette manière.

1. Dans le champ **[!UICONTROL Ajouter des programmes à ce portefeuille]**, saisissez le nom d&#39;un programme, puis sélectionnez-le lorsqu&#39;il s&#39;affiche dans la liste. <!--see the name of this field, I suggested changes here-->

   Vous pouvez ajouter plusieurs programmes.

1. (Facultatif) Cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/delete-icon.png) en regard du nom d’un programme si vous décidez de ne pas l’ajouter au portfolio.

1. Cliquez sur **[!UICONTROL Ajouter des programmes]**.

   Le programme s’affiche dans l’onglet **[!UICONTROL Programmes]** du portefeuille que vous avez sélectionné.

