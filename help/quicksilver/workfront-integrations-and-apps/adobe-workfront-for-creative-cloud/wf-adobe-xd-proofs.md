---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: Charger des plans de travail XD en tant qu’épreuves dans Workfront
description: Vous pouvez télécharger vos tableaux de bord en tant que bons à tirer directement vers Adobe Workfront pour une révision et une approbation approfondies.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: d5255968a96452d9501a285408f67be7da10d933
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 4%

---

# Télécharger [!DNL XD] artefacts en tant que bons à tirer vers [!DNL Workfront]

Vous pouvez télécharger vos plans de travail en tant que bons à tirer directement vers [!DNL Adobe Workfront] pour une révision et une approbation approfondies.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>Formule actuelle : [!UICONTROL Pro] ou version ultérieure</p> <p>ou</p> <p>Formule héritée : [!UICONTROL Premium]</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>Plan actuel : [!UICONTROL Travail] ou [!UICONTROL Preuve]</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer d’une licence [!DNL Adobe Creative Cloud] en plus d’une licence [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>[!UICONTROL Manager] ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Modifier l’accès aux [!UICONTROL Documents]</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir quel plan, rôle ou profil d’autorisation de BAT vous avez, contactez votre administrateur [!DNL Workfront] ou [!DNL Workfront Proof].

## Conditions préalables

* Vous devez installer le module externe [!DNL Adobe Workfront for XD] avant de pouvoir télécharger des bons à tirer dans [!DNL Adobe XD].

  Pour obtenir des instructions, voir [Installation [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Chargement d’un BAT statique

1. Cliquez sur l’icône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![](assets/menu-350x440.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez charger un BAT statique.
1. Cliquez sur l’icône **[!UICONTROL Document]** ![](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL New File]** près du bas du module externe.
1. Sélectionnez les plans de travail que vous souhaitez charger.

   >[!TIP]
   >
   >* Les tableaux d’affichage apparaîtront dans le BAT dans l’ordre dans lequel ils ont été sélectionnés. Le premier plan de travail sélectionné sera la première page du BAT, etc.
   >* Pour sélectionner rapidement plusieurs plans de travail, cliquez et faites glisser la souris sur les plans de travail de votre choix. Cela ne vous permet pas de contrôler l’ordre des tableaux dans le BAT.

1. Activez **[!UICONTROL Créer un bon à tirer]**.

1. Nommez le BAT.

1. Choisissez le type de validation du BAT que vous souhaitez :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic] : </td> 
      <td> <p>Les processus d’approbation de base sont ad hoc et peuvent inclure différents réviseurs selon les besoins : </p> 
       <ul> 
        <li> <p>(Facultatif) Ajoutez <strong>Approvers</strong> dans la zone.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Les processus d’approbation automatisée sont préconfigurés par les administrateurs et incluent des réviseurs et des étapes spécifiques. Pour plus d’informations, voir <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Présentation du processus automatisé</a>.</p> 
       <ul> 
        <li> <p>Sélectionnez un [!UICONTROL Modèle de workflow] dans le menu déroulant.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Facultatif) Saisissez un commentaire dans la zone **[!UICONTROL Mises à jour]**.

   ![](assets/proof-approvals-xd-350x396.png)

1. Choisissez le format d’exportation dans le menu déroulant **[!UICONTROL Type de ressource]**.


1. (Facultatif) Si vous sélectionnez PDF comme type de ressource et que plusieurs artefacts sont sélectionnés, choisissez si vous souhaitez exporter vos artefacts en tant que **[!UICONTROL Fichier de PDF unique]s** ou **M[!UICONTROL plusieurs fichiers de PDF]**.

1. (Facultatif) Nommez le PDF.

   ![](assets/pdf-options.png)

1. Cliquez sur **[!UICONTROL Télécharger]**.\
   Le document apparaît dans la zone [!UICONTROL Documents] du module externe et de l’appli de bureau.

## Chargement d’un BAT interactif {#upload-an-interactive-proof}

Vous pouvez créer un BAT interactif pour vos tableaux de bord à l’aide du module externe [!DNL Workfront for Adobe]. Il s’agit d’un processus en 2 étapes. Vous devez d’abord créer un lien interactif, puis télécharger le BAT vers un élément de travail.

### Création d’un lien interactif pour votre plan de travail  {#create-an-interactive-link-for-your-art-board}

1. Ouvrez votre plan de travail, puis cliquez sur **[!UICONTROL Partager]** dans la zone supérieure gauche de l’écran.
1. Définissez les paramètres du lien :

   1. Nommez le lien.
   1. Choisissez un paramètre d’affichage.
   1. Dans la section **[!UICONTROL Accès aux liens]** , assurez-vous que **[!UICONTROL Toute personne disposant de ce lien]** est sélectionnée.

      Vous devez activer ce type d’accès pour générer un BAT interactif.

   1. Cliquez sur **[!UICONTROL Créer un lien]**.

1. Cliquez sur **[!UICONTROL Conception]** dans la zone supérieure gauche de l’écran. Passez à la section [Télécharger un BAT interactif](#upload-an-interactive-proof) ci-dessous.

   >[!NOTE]
   >
   >Vous devrez peut-être rouvrir le panneau du module externe dans le coin inférieur gauche de l’écran.

### Chargement d’un BAT interactif

1. Cliquez sur l’icône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![](assets/menu-350x440.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez télécharger un BAT interactif.
1. Cliquez sur l’icône **[!UICONTROL Document]** ![](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL New File]** près du bas du module externe.
1. Activez **[!UICONTROL Créer un bon à tirer]**.

1. Choisissez le type de validation du BAT que vous souhaitez :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic] : </td> 
      <td> <p>Les processus d’approbation de base sont ad hoc et peuvent inclure différents réviseurs selon les besoins : </p> 
       <ul> 
        <li> <p>(Facultatif) Ajoutez <strong>Approvers</strong> dans la zone.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Les processus d’approbation automatisée sont préconfigurés par les administrateurs et incluent des réviseurs et des étapes spécifiques. Pour plus d’informations, voir <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Présentation du processus automatisé</a>.</p> 
       <ul> 
        <li> <p>Sélectionnez un [!UICONTROL Modèle de workflow] dans le menu déroulant.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Facultatif) Saisissez un commentaire dans la zone **[!UICONTROL Mises à jour]**.

   ![](assets/proof-approvals-xd-350x396.png)

1. Dans le menu déroulant **[!UICONTROL Type de ressource]**, sélectionnez le lien que vous venez de créer sous l’onglet **Liens partagés** . Pour plus d’informations, voir [Création d’un lien interactif pour votre plan de travail](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. Cliquez sur **[!UICONTROL Télécharger]**.

   Le document apparaît dans la zone [!UICONTROL Documents] du module externe et de l’appli de bureau.

   >[!IMPORTANT]
   >
   >Les utilisateurs doivent avoir accès à la [!UICONTROL Visionneuse de vérification de l’appli de bureau] pour passer en revue et approuver les bons à tirer interactifs. Pour plus d’informations, voir [Installation de la [!UICONTROL visionneuse de vérification de l’appli de bureau]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Télécharger une nouvelle version du BAT

Vous pouvez télécharger une nouvelle version d’un BAT. Le module externe mémorise le workflow de vérification défini sur la version précédente, mais vous pouvez le modifier si vous le souhaitez.

1. Cliquez sur l’icône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![](assets/menu-350x440.png)

1. Accédez à l’élément de travail sur lequel vous devez charger un document.
1. Cliquez sur l&#39;icône **[!UICONTROL Document]** ![](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL Nouvelle version]** près du bas du module externe.
1. Activez **[!UICONTROL Créer un bon à tirer]**.
1. Sélectionnez les plans de travail que vous souhaitez charger.

   >[!NOTE]
   >
   >Si vous souhaitez charger une nouvelle version d’un fichier .svg, .png ou .jpg, vous ne pouvez charger qu’un seul plan de travail.

1. Choisissez le type de validation du BAT que vous souhaitez :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic] : </td> 
      <td> <p>Les processus d’approbation de base sont ad hoc et peuvent inclure différents réviseurs selon les besoins : </p> 
       <ul> 
        <li> <p>(Facultatif) Ajoutez <strong>Approvers</strong> dans la zone.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Les processus d’approbation automatisée sont préconfigurés par les administrateurs et incluent des réviseurs et des étapes spécifiques. Pour plus d’informations, voir <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Présentation du processus automatisé</a>.</p> 
       <ul> 
        <li> <p>Sélectionnez un [!UICONTROL Modèle de workflow] dans le menu déroulant.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. Choisissez le format d’exportation dans le menu déroulant **[!UICONTROL Type de ressource]**.

   ![](assets/create-a-proof-xd-350x202.png)

1. (Facultatif) Saisissez un commentaire dans la zone **[!UICONTROL Mises à jour]**.

   ![](assets/proof-approvals-xd-350x396.png)

1. (Facultatif) Si vous sélectionnez PDF comme type de ressource et que plusieurs artefacts sont sélectionnés, choisissez si vous souhaitez exporter vos artefacts en tant que **[!UICONTROL Fichier de PDF unique]s** ou **M[!UICONTROL plusieurs fichiers de PDF]**.

1. (Facultatif) Nommez le PDF.

   ![](assets/pdf-options.png)

1. Cliquez sur **[!UICONTROL Télécharger]**.\
   Le document apparaît dans la zone [!UICONTROL Documents] du module externe et de l’appli de bureau.
