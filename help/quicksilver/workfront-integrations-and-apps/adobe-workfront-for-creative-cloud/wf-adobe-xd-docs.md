---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Charger des plans de travail XD en tant que documents dans Workfront
description: Vous pouvez télécharger vos tableaux de bord en tant que documents pour une révision et une approbation rapides ou simplement les stocker dans Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: bf47ae15d2972e8ee11f76741f8e5c676d79e626
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 13%

---


# Télécharger [!DNL XD] artefacts en tant que documents vers [!DNL Workfront]

Vous pouvez télécharger vos tableaux de bord en tant que documents pour une révision et une approbation rapides ou simplement les stocker dans [!DNL Adobe Workfront].

## Conditions d’accès

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
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux [!UICONTROL Documents]</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès à [!UICONTROL View] ou supérieur à l’objet dans lequel vous souhaitez charger un document.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

* Vous devez installer le module externe [!DNL Adobe Workfront for XD] avant de pouvoir télécharger XD panoramas d’art en tant que documents vers Workfront.

Pour obtenir des instructions, voir [Installation [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Ajouter un nouveau document

1. Cliquez sur l’icône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![](assets/menu-350x440.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez charger un document.
1. Cliquez sur l’icône **[!UICONTROL Document]** ![](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL New File]** près du bas du module externe.
1. Sélectionnez le plan de travail que vous souhaitez charger.

   >[!TIP]
   >
   >Pour sélectionner plusieurs illustrations, cliquez dessus et faites glisser la souris.
1. (Facultatif) Saisissez un commentaire dans la zone **[!UICONTROL Mises à jour]**.
1. Sélectionnez le **[!UICONTROL Type de ressource]** dans le menu déroulant :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Export Format]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Les illustrations sont chargées au format PNG dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Les tableaux de bord sont téléchargés en tant que JPG dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Les tableaux de bord sont téléchargés en tant que SVG dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Choisissez si vous souhaitez que les plans de travail sélectionnés soient téléchargés sous la forme d’un <strong>fichier de PDF unique</strong> ou de <strong> fichiers de PDF multiples</strong>. Les plans de travail sont téléchargés en tant que PDF dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. Cliquez sur **[!UICONTROL Télécharger]**.\
   Le document apparaît dans la zone [!UICONTROL Documents] du module externe et de l’appli de bureau.

## Ajouter une nouvelle version

1. Cliquez sur l’icône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![](assets/menu-350x440.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez charger un document.
1. Cliquez sur l&#39;icône **[!UICONTROL Document]** ![](assets/documents.png) dans la barre de navigation.

1. Cliquez sur le document auquel vous souhaitez ajouter une nouvelle version.
1. Cliquez sur **[!UICONTROL Nouvelle version]** près du bas du module externe.
1. Sélectionnez les plans de travail que vous souhaitez charger.

   >[!NOTE]
   >
   >Si vous souhaitez charger une nouvelle version d’un SVG, d’un fichier PNG ou d’un JPG, vous ne pouvez charger qu’un seul plan de travail.

1. (Facultatif) Saisissez un commentaire dans la zone **[!UICONTROL Mises à jour]**.

1. Sélectionnez le **[!UICONTROL Type de ressource]** dans le menu déroulant :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">Format d’exportation</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>L’arboard est téléchargé au format PNG dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>L’artboard est téléchargé en tant que JPG dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>L’artboard est téléchargé en tant que SVG dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>Les tableaux de bord sont téléchargés en tant que PDF dans l’onglet [!UICONTROL Documents] de l’élément de travail dans [!DNL Workfront].</p>
      <p><strong>Remarque</strong> : vous ne pouvez charger qu’un seul plan de travail pour une nouvelle version de document.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Cliquez sur **[!UICONTROL Télécharger]**.\
   Le document apparaît dans la zone [!UICONTROL Documents] du module externe et de l’appli de bureau.
