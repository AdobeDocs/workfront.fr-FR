---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: Charger des plans de travail XD en tant qu’épreuves sur Workfront
description: Vous pouvez charger vos plans de travail en tant qu’épreuves directement sur Adobe Workfront pour une révision et une approbation approfondies.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 93%

---

# Charger des plans de travail [!DNL XD] en tant qu’épreuves sur [!DNL Workfront]

Vous pouvez charger vos plans de travail en tant qu’épreuves directement sur [!DNL Adobe Workfront] pour une révision et une approbation approfondies.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquet</td> 
   <td>Tous </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Standard</p> <p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produits supplémentaires</td> 
   <td>Vous devez disposer d’une licence [!DNL Adobe Creative Cloud] en plus d’une licence [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>[!UICONTROL Manager] ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Modifier l’accès aux [!UICONTROL Documents]</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, consultez la section <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Conditions préalables

* Vous devez installer le plug-in [!DNL Adobe Workfront for XD] avant de pouvoir charger des épreuves sur [!DNL Adobe XD].

  Pour obtenir des instructions, consultez la section [Installer [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Charger une épreuve statique

1. Cliquez sur le bouton **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![Icône de menu](assets/menu-350x440.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez charger une épreuve statique.
1. Cliquez sur l’icône **[!UICONTROL Document]** ![icône de document](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL Nouveau fichier]** au bas du plug-in.
1. Sélectionnez les plans de travail que vous souhaitez charger.

   >[!TIP]
   >
   >* Les plans de travail s’affichent dans l’épreuve suivant l’ordre de sélection. Le premier plan de travail sélectionné constituera la première page de l’épreuve, etc.
   >* Pour sélectionner rapidement plusieurs plans de travail, cliquez et faites glisser la souris sur les plans de travail souhaités. Cela ne vous permet pas de contrôler l’ordre des plans de travail dans l’épreuve.

1. Cochez **[!UICONTROL Créer une épreuve]**.

1. Nommez l’épreuve.

1. Choisissez le type d’approbation de l’épreuve que vous souhaitez :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic] : </td> 
      <td> <p>Les processus d’approbation de base sont ad hoc et peuvent inclure différentes personnes chargées de la révision selon les besoins : </p> 
       <ul> 
        <li> <p>(Facultatif) Ajoutez des <strong>Approbateurs et approbatrices</strong> dans la zone.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Les processus d’approbation automatisée sont préconfigurés par l’équipe d’administration et incluent des réviseurs et réviseuses et des étapes spécifiques. Pour plus d’informations, consultez la section <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Vue d’ensemble des workflows automatisés</a>.</p> 
       <ul> 
        <li> <p>Sélectionnez un [!UICONTROL Workflow Template] dans le menu déroulant.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Facultatif) Apportez un commentaire dans la zone **[!UICONTROL Mises à jour]**.

   ![Validations d’épreuves dans XD](assets/proof-approvals-xd-350x396.png)

1. Choisissez le format d’export dans le menu déroulant **[!UICONTROL Type de ressource]**.


1. (Facultatif) Si vous sélectionnez le type de ressource PDF et que plusieurs plans de travail sont sélectionnés, choisissez si vous souhaitez exporter vos plans de travail en tant que **[!UICONTROL Fichiers PDF uniques]** ou en tant que **[!UICONTROL Plusieurs fichiers PDF]**.

1. (Facultatif) Nommez le PDF.

   ![Options PDF](assets/pdf-options.png)

1. Cliquez sur **[!UICONTROL Charger]**.\
   Le document apparaît dans la zone [!UICONTROL Documents] dans le plug-in et l’application de bureau.

## Charger une épreuve interactive {#upload-an-interactive-proof}

Vous pouvez créer une épreuve interactive pour vos tableaux de bord à l’aide du plug-in [!DNL Workfront for Adobe]. Il s’agit d’un processus en 2 étapes. Vous devez d’abord créer un lien interactif, puis charger l’épreuve dans un élément de travail.

### Créer un lien interactif pour votre plan de travail  {#create-an-interactive-link-for-your-art-board}

1. Ouvrez votre plan de travail, puis cliquez sur **[!UICONTROL Partager]** dans la zone supérieure gauche de l’écran.
1. Indiquez les paramètres du lien :

   1. Nommez le lien.
   1. Choisissez un paramètre de vue.
   1. Dans la section **[!UICONTROL Lier l’accès]**, assurez-vous que l’option **[!UICONTROL Toute personne disposant de ce lien]** est sélectionnée.

      Vous devez activer ce type d’accès pour générer une épreuve interactive.

   1. Cliquez sur **[!UICONTROL Créer un lien]**.

1. Cliquez pour revenir à **[!UICONTROL Conception]** dans la zone supérieure gauche de l’écran. Passez à la section [Charger une épreuve interactive](#upload-an-interactive-proof) ci-dessous.

   >[!NOTE]
   >
   >Vous devrez peut-être rouvrir le panneau du plug-in dans le coin inférieur gauche de l’écran.

### Charger une épreuve interactive

1. Cliquez sur l’icône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![Icône de menu](assets/menu-350x440.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez charger une épreuve interactive.
1. Cliquez sur l’icône **[!UICONTROL Document]** ![icône de document](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL Nouveau fichier]** près du bas du plug-in.
1. Activez **[!UICONTROL Créer une épreuve]**.

1. Choisissez le type d’approbation de l’épreuve que vous souhaitez :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic] : </td> 
      <td> <p>Les processus d’approbation de base sont ad hoc et peuvent inclure différentes personnes chargées de la révision selon les besoins : </p> 
       <ul> 
        <li> <p>(Facultatif) Ajoutez des <strong>Approbateurs et approbatrices</strong> dans la zone.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Les processus d’approbation automatisée sont préconfigurés par l’équipe d’administration et incluent des réviseurs et réviseuses et des étapes spécifiques. Pour plus d’informations, consultez la section <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Vue d’ensemble des workflows automatisés</a>.</p> 
       <ul> 
        <li> <p>Sélectionnez un [!UICONTROL Workflow Template] dans le menu déroulant.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Facultatif) Apportez un commentaire dans la zone **[!UICONTROL Mises à jour]**.

   ![Validations d’épreuves dans XD](assets/proof-approvals-xd-350x396.png)

1. Dans le menu déroulant **[!UICONTROL Type de ressource]**, sélectionnez le lien que vous venez de créer sous l’onglet **Liens partagés**. Pour plus d’informations, voir [Créer un lien interactif pour votre plan de travail](#create-an-interactive-link-for-your-artboard).\
   ![Liens partagés dans XDS](assets/shared-links-xd-350x870.png)

1. Cliquez sur **[!UICONTROL Charger]**.

   Le document apparaît dans la zone [!UICONTROL Documents] dans le plug-in et l’application de bureau.

   >[!IMPORTANT]
   >
   >Les personnes doivent avoir accès à la [!UICONTROL visionneuse de relecture de bureau] pour réviser et approuver les épreuves interactives. Pour plus d’informations, consultez [Installer la [!UICONTROL visionneuse de relecture de bureau]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Charger une nouvelle version d’épreuve

Vous pouvez charger une nouvelle version d’une épreuve. Le plug-in conserve en mémoire le workflow de relecture défini sur la version précédente, mais vous pouvez modifier ce paramètre si vous le souhaitez.

1. Cliquez sur l’cône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![Icône de menu](assets/menu-350x440.png)

1. Accédez à l’élément de travail dans lequel vous devez charger un document.
1. Cliquez sur l’icône **[!UICONTROL Document]** ![icône de document](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL Nouvelle version]** près du bas du plug-in.
1. Activez **[!UICONTROL Créer une épreuve]**.
1. Sélectionnez les plans de travail que vous souhaitez charger.

   >[!NOTE]
   >
   >Si vous souhaitez charger une nouvelle version d’un fichier .svg, .png ou .jpg, vous ne pouvez charger qu’un seul plan de travail.

1. Choisissez le type d’approbation de l’épreuve que vous souhaitez :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic] : </td> 
      <td> <p>Les processus d’approbation de base sont ad hoc et peuvent inclure différentes personnes chargées de la révision selon les besoins : </p> 
       <ul> 
        <li> <p>(Facultatif) Ajoutez des <strong>Approbateurs et approbatrices</strong> dans la zone.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Les processus d’approbation automatisée sont préconfigurés par l’équipe d’administration et incluent des réviseurs et réviseuses et des étapes spécifiques. Pour plus d’informations, consultez la section <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Vue d’ensemble des workflows automatisés</a>.</p> 
       <ul> 
        <li> <p>Sélectionnez un [!UICONTROL Workflow Template] dans le menu déroulant.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. Choisissez le format d’export dans le menu déroulant **[!UICONTROL Type de ressource]**.

   ![Création d’une épreuve dans XD](assets/create-a-proof-xd-350x202.png)

1. (Facultatif) Saisissez un commentaire dans la zone **[!UICONTROL Mises à jour]**.

   ![Validations d’épreuves dans XD](assets/proof-approvals-xd-350x396.png)

1. (Facultatif) Si vous sélectionnez le type de ressource PDF et que plusieurs plans de travail sont sélectionnés, choisissez si vous souhaitez exporter vos plans de travail en tant que **[!UICONTROL Fichiers PDF uniques]** ou en tant que **[!UICONTROL Plusieurs fichiers PDF]**.

1. (Facultatif) Nommez le PDF.

   Options de PDF

1. Cliquez sur **[!UICONTROL Charger]**.\
   Le document apparaît dans la zone [!UICONTROL Documents] dans le plug-in et l’appli de bureau.
