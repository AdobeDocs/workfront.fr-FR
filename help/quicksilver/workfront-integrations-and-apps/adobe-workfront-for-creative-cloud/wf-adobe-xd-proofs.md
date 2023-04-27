---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: Chargement de XD illustrations en tant que BAT vers Workfront
description: Vous pouvez télécharger vos tableaux de bord en tant que bons à tirer directement vers Adobe Workfront pour une révision et une approbation approfondies.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: d0afdfc7be9177f6ff45dcc247253faa9dc57967
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Télécharger [!DNL XD] les tableaux de bord en tant que bons à tirer [!DNL Workfront]

Vous pouvez charger vos tableaux de bord en tant que bons à tirer directement vers [!DNL Adobe Workfront] pour une révision et une approbation approfondies.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Formule actuelle : [!UICONTROL Pro] ou version ultérieure</p> <p>ou</p> <p>Plan hérité : [!UICONTROL Premium]</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>Formule actuelle : [!UICONTROL Work] ou [!UICONTROL Proof]</p> <p>Plan hérité : N’importe quel (la vérification doit être activée pour l’utilisateur)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer d’un [!DNL Adobe Creative Cloud] en plus d’une [!DNL Workfront] licence.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>[!UICONTROL Manager] ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Modifier l’accès aux [!UICONTROL Documents]</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir quel plan, rôle ou profil d’autorisation de BAT vous avez, contactez votre [!DNL Workfront] ou [!DNL Workfront Proof] administrateur.

## Conditions préalables

* Vous devez installer le [!DNL Adobe Workfront for XD] avant de pouvoir télécharger des bons à tirer dans [!DNL Adobe XD].

   Pour obtenir des instructions, voir [Installer [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Chargement d’un BAT statique

1. Cliquez sur le bouton **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de tâches]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![](assets/menu-350x440.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez charger un BAT statique.
1. Cliquez sur le bouton **[!UICONTROL Document]** icon ![](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL Nouveau fichier]** près du bas du module externe.
1. Sélectionnez les plans de travail que vous souhaitez charger.

   >[!TIP]
   >
   >Pour sélectionner plusieurs illustrations, cliquez dessus et faites glisser la souris.

1. Activer **[!UICONTROL Créer un bon à tirer]**.

1. Nommez le BAT.

1. Choisissez le type de validation du BAT que vous souhaitez :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic] : </td> 
      <td> <p>Les processus d’approbation de base sont ad hoc et peuvent inclure différents réviseurs si nécessaire : </p> 
       <ul> 
        <li> <p>(Facultatif) Ajoutez <strong>Approbateurs</strong> dans la boîte.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Les processus d’approbation automatisée sont préconfigurés par les administrateurs et incluent des réviseurs et des étapes spécifiques. Pour plus d’informations, voir <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Présentation des processus automatisés</a>.</p> 
       <ul> 
        <li> <p>Sélectionnez un [!UICONTROL Modèle de workflow] dans le menu déroulant.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Facultatif) Saisissez un commentaire dans le champ **[!UICONTROL Mises à jour]** zone.

   ![](assets/proof-approvals-xd-350x396.png)

1. Choisissez le format d&#39;export parmi les **[!UICONTROL Type de ressource]** menu déroulant.


1. (Facultatif) Si vous sélectionnez PDF comme type de ressource et que plusieurs plans de travail sont sélectionnés, choisissez si vous souhaitez exporter vos plans de travail en tant que **[!UICONTROL Fichier de PDF unique]s** ou **M[!UICONTROL plusieurs fichiers PDF ;]**.

1. (Facultatif) Nommez le PDF.

   ![](assets/pdf-options.png)

1. Cliquez sur **[!UICONTROL Télécharger]**.\
   Le document apparaît dans la [!UICONTROL Documents] dans le module externe et l’appli de bureau.

## Chargement d’un BAT interactif {#upload-an-interactive-proof}

Vous pouvez créer un BAT interactif pour vos tableaux de bord à l’aide de la fonction [!DNL Workfront for Adobe] module externe Il s’agit d’un processus en 2 étapes. Vous devez d’abord créer un lien interactif, puis télécharger le BAT vers un élément de travail.

### Création d’un lien interactif pour votre plan de travail  {#create-an-interactive-link-for-your-art-board}

1. Ouvrez votre plan de travail, puis cliquez sur **[!UICONTROL Partager]** dans la zone supérieure gauche de l’écran.
1. Définissez les paramètres du lien :

   1. Attribuez un nom au lien.
   1. Choisissez un paramètre d’affichage.
   1. Dans le **[!UICONTROL Lier l’accès]** , assurez-vous que **[!UICONTROL Toute personne disposant de ce lien]** est sélectionnée.

      Vous devez activer ce type d’accès pour générer un BAT interactif.

   1. Cliquez sur **[!UICONTROL Créer un lien]**.

1. Revenir à **[!UICONTROL Conception]** dans la zone supérieure gauche de l’écran. Passez à la [Chargement d’un BAT interactif](#upload-an-interactive-proof) ci-dessous.

   >[!NOTE]
   >
   >Vous devrez peut-être rouvrir le panneau du module externe dans le coin inférieur gauche de l’écran.

### Chargement d’un BAT interactif

1. Cliquez sur le bouton **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de tâches]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![](assets/menu-350x440.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez télécharger un BAT interactif.
1. Cliquez sur le bouton **[!UICONTROL Document]** icon ![](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL Nouveau fichier]** près du bas du module externe.
1. Activer **[!UICONTROL Créer un bon à tirer]**.

1. Choisissez le type de validation du BAT que vous souhaitez :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic] : </td> 
      <td> <p>Les processus d’approbation de base sont ad hoc et peuvent inclure différents réviseurs si nécessaire : </p> 
       <ul> 
        <li> <p>(Facultatif) Ajoutez <strong>Approbateurs</strong> dans la boîte.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Les processus d’approbation automatisée sont préconfigurés par les administrateurs et incluent des réviseurs et des étapes spécifiques. Pour plus d’informations, voir <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Présentation des processus automatisés</a>.</p> 
       <ul> 
        <li> <p>Sélectionnez un [!UICONTROL Modèle de workflow] dans le menu déroulant.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Facultatif) Saisissez un commentaire dans le champ **[!UICONTROL Mises à jour]** zone.

   ![](assets/proof-approvals-xd-350x396.png)

1. Dans le **[!UICONTROL Type de ressource]** , sélectionnez le lien que vous venez de créer sous le **Liens partagés** . Pour plus d’informations, voir [Création d’un lien interactif pour votre plan de travail](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. Cliquez sur **[!UICONTROL Télécharger]**.

   Le document apparaît dans la [!UICONTROL Documents] dans le module externe et l’appli de bureau.

   >[!IMPORTANT]
   >
   >Les utilisateurs doivent avoir accès au [!UICONTROL Visionneuse de vérification de poste de travail] pour examiner et approuver les bons à tirer interactifs. Pour plus d’informations, consultez [Installation [!UICONTROL du lecteur de vérification pour bureau]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Télécharger une nouvelle version du BAT

Vous pouvez télécharger une nouvelle version d’un BAT. Le module externe mémorise le workflow de vérification défini sur la version précédente, mais vous pouvez le modifier si vous le souhaitez.

1. Cliquez sur le bouton **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de tâches]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![](assets/menu-350x440.png)

1. Accédez à l’élément de travail sur lequel vous devez charger un document.
1. Cliquez sur le bouton **[!UICONTROL Document]** icon ![](assets/documents.png)dans la barre de navigation.

1. Cliquez sur **[!UICONTROL Nouvelle version]** près du bas du module externe.
1. Activer **[!UICONTROL Créer un bon à tirer]**.
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
      <td> <p>Les processus d’approbation de base sont ad hoc et peuvent inclure différents réviseurs si nécessaire : </p> 
       <ul> 
        <li> <p>(Facultatif) Ajoutez <strong>Approbateurs</strong> dans la boîte.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>Les processus d’approbation automatisée sont préconfigurés par les administrateurs et incluent des réviseurs et des étapes spécifiques. Pour plus d’informations, voir <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Présentation des processus automatisés</a>.</p> 
       <ul> 
        <li> <p>Sélectionnez un [!UICONTROL Modèle de workflow] dans le menu déroulant.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. Choisissez le format d&#39;export parmi les **[!UICONTROL Type de ressource]** menu déroulant.

   ![](assets/create-a-proof-xd-350x202.png)

1. (Facultatif) Saisissez un commentaire dans le champ **[!UICONTROL Mises à jour]** zone.

   ![](assets/proof-approvals-xd-350x396.png)

1. (Facultatif) Si vous sélectionnez PDF comme type de ressource et que plusieurs plans de travail sont sélectionnés, choisissez si vous souhaitez exporter vos plans de travail en tant que **[!UICONTROL Fichier de PDF unique]s** ou **M[!UICONTROL plusieurs fichiers PDF ;]**.

1. (Facultatif) Nommez le PDF.

   ![](assets/pdf-options.png)

1. Cliquez sur **[!UICONTROL Télécharger]**.\
   Le document apparaît dans la [!UICONTROL Documents] dans le module externe et l’appli de bureau.
