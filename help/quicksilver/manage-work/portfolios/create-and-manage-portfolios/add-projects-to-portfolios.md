---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Ajout de projets à un Portfolio
description: Nous vous recommandons d’ajouter des projets aux portfolios lorsque vous les lancez. Cependant, vous pouvez les ajouter à un portfolio à tout moment de leur durée de vie.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 97f36c18-3ac8-45ac-b5bc-dfe8b1363faf
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UkUQdW12tLqRjh5zmbwtjNfRxFwc-Uhj2gGwjmDyKb8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 397e5e36632872bb7be3f4e219b36e33b44136e9
workflow-type: tm+mt
source-wordcount: 674
ht-degree: 41%

---

# Ajouter des projets à un portfolio

<!--Audited: 08/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

Nous vous recommandons d’ajouter des projets aux portfolios lorsque vous les lancez. Cependant, vous pouvez les ajouter à un portfolio à tout moment de leur durée de vie.

Tenez compte des éléments suivants lorsque vous ajoutez des projets aux portfolios :

* Vous ne pouvez associer qu&#39;un seul portefeuille à un projet.
* Un projet reste dans un portfolio jusqu’à ce qu’il soit supprimé ou associé à un autre portfolio.
* Un portefeuille peut contenir un nombre illimité de projets.

>[!CAUTION]
>
>Les autorisations héritées peuvent ne pas être appliquées correctement lorsqu’elles sont utilisées sur un grand nombre d’objets enfants.
>   
>Pour éviter les problèmes d’autorisations héritées, nous vous recommandons de procéder comme suit :
>
>* Limitez le nombre d&#39;objets enfant (projets) sous un seul parent (portfolio ou programme). Nous ne recommandons pas plus de 10 000 projets par portefeuille ou programme.
>
>* Réduisez la profondeur d’héritage en appliquant des autorisations à un objet de niveau inférieur.
>
>  Par exemple, appliquez les autorisations directement au niveau du projet plutôt que de vous fier aux autorisations héritées du portfolio dans le programme, puis dans le projet.
>
>* Divisez les programmes pour contenir moins de projets, ce qui réduit la complexité des autorisations.
>


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquet</td> 
   <td> <p>Tous</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Standard</p> 
   <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Portefeuilles d'accès [!UICONTROL Edit]</p> <p>[!UICONTROL Edit] l’accès aux Projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour le portfolio</p> <p>[!UICONTROL Manage] les permissions des projets</p>  </td> 
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
   <td> <p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>[!UICONTROL Edit] access Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Ajouter un projet à un portfolio

1. Accédez à un portfolio, puis cliquez sur **[!UICONTROL Projets]** dans le panneau de gauche.

   ![Portfolio avec projets](assets/qs-portfolio-with-projects-350x90.png)

1. Cliquez sur **[!UICONTROL Nouveau projet]** et sélectionnez une méthode pour ajouter un projet.

   >[!TIP]
   >
   >Vous ne pouvez pas ajouter de projet lorsque vous affichez la liste des projets dans la vue [!UICONTROL Jalon].

   Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody>

   <tr> 
      <td role="rowheader">[!UICONTROL New Project]</td> 
      <td> <p>Ajoutez un nouveau projet. </p> <p>Pour en savoir plus sur la création d’un projet, voir <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Créer un projet</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nouveau projet (stockage hérité)]</td> 
      <td> <p>Ajoutez un nouveau projet de stockage Workfront. </p>
      <p>Cette option s’affiche uniquement lorsque votre entreprise utilise à la fois l’espace de stockage de documents cloud Workfront et Adobe. Votre instance Workfront peut ne pas avoir les deux types de stockage.</p>
       <p>Pour en savoir plus sur la création d’un projet, voir <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Créer un projet</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nouveau projet à partir d'un modèle]</td> 
      <td> <p>Ajouter un nouveau projet en utilisant un modèle existant. </p> <p>Pour plus d’informations sur la création d’un projet à partir d’un modèle, consultez la section <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Créer un projet à l’aide d’un modèle</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Import [!DNL MS Project]] </td> 
      <td> <p>Ajoutez un projet que vous avez précédemment exporté depuis [!DNL MS Project] et que vous avez enregistré sur votre ordinateur. </p> <p>Pour plus d’informations sur la création d’un nouveau projet en l’important à partir de [!DNL Microsoft Project], consultez la section <a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">Importer un projet à partir de [!DNL Microsoft Project]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Project]</td> 
      <td> <p>Demander l’approbation d’un projet.</p> <p>Pour plus d’informations sur la requête de projets, consultez la section <a href="../../../manage-work/projects/create-projects/request-project.md">Demander un projet</a>. </p> </td> 
     </tr> 
          <tr> 
      <td role="rowheader">[!UICONTROL Existing Project]</td> 
      <td> <p>Ajoutez un projet déjà créé.</p> </td> 
     </tr>
    </tbody> 
   </table>

   <!-- update screen shot for both kinds of storages??-->

   ![Liste déroulante du nouveau projet](assets/new-project-dropdown-expanded-from-portfolio-nwe-350x376.png)

1. (Conditionnel) Si vous avez choisi d’ajouter un projet existant, la boîte de dialogue **Ajouter des projets** s’ouvre. <!--check this after UI changes-->

   ![Ajouter un projet existant](assets/add-existing-projects-to-portfolios-box.png) <!--check this after UI changes-->

1. Commencez à saisir le nom d’un projet dans le champ **[!UICONTROL Ajouter des projets à ce portefeuille]**, puis cliquez dessus lorsqu’ils apparaissent dans la liste.  <!--check this after UI changes-->

   Vous pouvez ajouter plusieurs projets.

   >[!NOTE]
   >
   >Lorsque votre entreprise utilise à la fois l’espace de stockage cloud Workfront et Adobe hérité pour les documents, les scénarios suivants existent :
   >
   >
   >* Vous ne pouvez pas ajouter un projet de stockage hérité à un portefeuille de stockage cloud Adobe, ni un projet de stockage cloud Adobe à un portefeuille de stockage hérité.
   >* Vous ne pouvez pas créer de projet à partir d’un modèle de stockage cloud Adobe dans un portfolio de stockage hérité.
   >* Vous pouvez créer un projet à partir d’un modèle de stockage hérité dans un portfolio de stockage dans le cloud Adobe, mais les documents et dossiers du modèle ne sont pas ajoutés au nouveau projet. Le projet reçoit l’espace de stockage cloud Adobe.
   >
   >Pour plus d’informations, voir [Présentation de la gestion des documents pour les projets et les objets associés](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).
   >
   >Toutes les instances Workfront ne possèdent pas les deux types de stockage de documents.


1. (Facultatif) Cliquez sur l’icône **X** à droite du nom du projet pour le supprimer de la liste, si vous décidez de ne pas l’ajouter au portfolio.

   <!--replace last step with this, for unshim: 1. (Optional) Click the **Delete** icon ![Delete icon](assets/delete-icon.png) next to the name of a project if you decide not to add it to the portfolio.-->

1. Cliquez sur **[!UICONTROL Ajouter des projets]**. <!--check this after UI changes-->

   Le ou les projets sélectionnés sont désormais associés au portfolio.
