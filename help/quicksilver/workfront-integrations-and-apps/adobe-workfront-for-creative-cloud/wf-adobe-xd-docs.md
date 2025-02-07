---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Charger des plans de travail XD tant que documents dans Workfront
description: Vous pouvez télécharger vos plans de travail en tant que documents pour une révision et une approbation rapides ou simplement les stocker dans Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 95%

---


# Charger les plans de travail [!DNL XD] en tant que documents dans [!DNL Workfront]

Vous pouvez télécharger vos plans de travail en tant que documents pour une révision et une approbation rapides ou simplement les stocker dans [!DNL Adobe Workfront].

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer d’une licence [!DNL Adobe Creative Cloud] en plus d’une licence [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux [!UICONTROL Documents]</p> <p>Note : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration [!DNL Workfront] si des restrictions supplémentaires sont définies pour votre niveau d’accès. Pour plus d’informations sur la manière dont l’administration [!DNL Workfront] peut modifier votre niveau d’accès, consultez la section <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès [!UICONTROL View] ou de niveau supérieur à l’objet dans lequel vous souhaitez charger un document.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander un accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez l’administration [!DNL Workfront].

+++

## Conditions préalables

* Vous devez installer le plug-in [!DNL Adobe Workfront for XD] avant de pouvoir charger les plans de travail XD en tant que documents vers Workfront.

Pour obtenir des instructions, voir [Installer [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Ajouter un nouveau document

1. Cliquez sur l’icône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![Icône de menu](assets/menu-350x440.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez charger un document.
1. Cliquez sur l’icône **[!UICONTROL Document]** ![icône de document](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL Nouveau fichier]** près du bas du plug-in.
1. Sélectionnez le plan de travail que vous souhaitez charger.

   >[!TIP]
   >
   >Pour sélectionner plusieurs plans de travail, cliquez et faites glisser la souris sur ceux désirés.
1. (Facultatif) Saisissez un commentaire dans la zone **[!UICONTROL Mises à jour]**.
1. Choisissez le **[!UICONTROL Type de ressource]** dans le menu déroulant :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Export Format]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Les plans de travail sont chargés au format PNG dans l’onglet [!UICONTROL Documents] de l’élément de travail.[!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Les plans de travail sont chargés en tant que JPG dans l’onglet [!UICONTROL Documents] de l’élément de travail [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Les plans de travail sont chargés en tant que SVG dans l’onglet [!UICONTROL Documents] de l’élément de travail.[!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Choisissez si vous souhaitez que les plans de travail sélectionnés soient chargés sous la forme d’un <strong>fichier PDF unique</strong> ou de <strong>plusieurs fichiers PDF</strong>. Les plans de travail sont chargés en tant que PDF dans l’onglet [!UICONTROL Documents] de l’élément de travail.[!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. Cliquez sur **[!UICONTROL Charger]**.\
   Le document apparaît dans la zone [!UICONTROL Documents] du plug-in et de l’application de bureau.

## Ajouter une nouvelle version

1. Cliquez sur l’icône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![Icône de menu](assets/menu-350x440.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez charger un document.
1. Cliquez sur l’icône **[!UICONTROL Document]** ![icône de document](assets/documents.png) dans la barre de navigation.

1. Cliquez sur le document auquel vous souhaitez ajouter une nouvelle version.
1. Cliquez sur **[!UICONTROL Nouvelle version]** près du bas du plug-in.
1. Sélectionnez les plans de travail que vous souhaitez charger.

   >[!NOTE]
   >
   >Si vous souhaitez charger une nouvelle version d’un fichier SVG, PNG ou JPG, vous ne pouvez charger qu’un seul plan de travail.

1. (Facultatif) Saisissez un commentaire dans la zone **[!UICONTROL Mises à jour]**.

1. Choisissez le **[!UICONTROL Type de ressource]** dans le menu déroulant :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">Format d’export</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Le plan de travail est téléchargé au format PNG dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Le plan de travail est téléchargé au format JPG dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Le plan de travail est téléchargé au format SVG dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>Les plans de travail sont chargés au format PDF dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront].</p>
      <p><strong>Note</strong> : vous ne pouvez charger qu’un seul plan de travail pour une nouvelle version de document.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Cliquez sur **[!UICONTROL Charger]**.\
   Le document apparaît dans la zone [!UICONTROL Documents] dans le plug-in et l’appli de bureau.
