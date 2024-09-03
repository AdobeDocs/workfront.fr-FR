---
title: Exporter un rapport dans la zone de travail de reporting
description: Exporter un rapport dans la zone de travail de reporting
hidefromtoc: true
hide: true
exl-id: bd9e2e6f-338e-4cfc-aee5-6de6ecff4f09
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 100%

---

# Exporter un rapport dans la zone de travail de reporting

Vous pouvez exporter un rapport entier (ou un bloc spécifique) dans un format de fichier adapté à vos besoins. Vous pouvez exporter aux formats suivants :

* PDF (actuellement désactivé)
* CSV
* PNG
* XLSX

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta de la zone de travail de reporting. Pour plus d’informations, voir [Version bêta de la zone de travail de reporting : vue d’ensemble](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Exporter un rapport

1. Accédez au rapport à exporter.
1. Dans l’en-tête du rapport, cliquez sur l’icône **Plus** ![](assets/more-icon-27x15.png), cliquez sur **Exporter**, puis sélectionnez le format de fichier à créer.

   >[!NOTE]
   >
   >Tenez compte des points suivants concernant vos fichiers exportés :
   >
   >   * Si vous exportez un rapport contenant plusieurs tableaux au format XLSX, le fichier exporté contient une feuille distincte pour chaque tableau.
   >   * Si vous exportez un rapport contenant plusieurs tableaux au format CSV, le résultat exporté est un dossier compressé contenant un fichier distinct pour chaque tableau.
   >   * Si vous exportez un tableau contenant des lignes regroupées au format CSV, le fichier CSV comprend toutes les lignes, mais elles ne sont pas affichées dans les groupes.
   >   

<!-- 1. (Conditional) If you selected **PDF**, configure the fields below to format the exported file, then click **Download PDF**.

   >[!TIP]
   >
   >The PDF preview in the right pane updates as you configure each field.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Document size</td> 
      <td> <p>Select a size for the exported file from the drop-down menu.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Orientation</td> 
      <td> <p>Select either <strong>Portrait</strong> or <strong>Landscape</strong>.</p> </td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Scaling options</td> 
       <td> <p>Select the scaling option for the exported file:</p> 
        <ul> 
         <li> <p><strong>Normal</strong> (default option)</p> </li> 
         <li> <p><strong>Fit to width</strong> </p> </li> 
         <li> <p><strong>Fit to height</strong> </p> </li> 
        </ul> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Heading settings</td> 
      <td> <p>Select all the content you want to display in the header.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Footer settings</td> 
      <td> <p>Select all the content you want to display in the footer.</p> <p>If you select <strong>Footer message</strong>, type the <strong>Footer text</strong> that you want to display in the footer. You can type up to 255 characters.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Watermark</td> 
      <td> <p>If you select <strong>Include watermark</strong>:</p> 
       <ul> 
        <li>Type the <strong>Watermark text</strong> that you want to display. You can type up to 20 characters.</li> 
        <li>Slide or enter the <strong>Opacity</strong> percentage that you want for the text.</li> 
        <li>Enter the degree of <strong>Rotation</strong> that you want for the text.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   The exported PDF file is named in the following format: REPORT_TITLE_YYYY-MM-DDTHH_MM_SS. -->
