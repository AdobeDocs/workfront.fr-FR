---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Modifier les documents en bloc
description: Vous pouvez modifier plusieurs documents à la fois dans la zone Documents.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: e8badce6-86f5-416c-a238-f9b7f19cdd2d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 77%

---

# Modifier les documents en bloc

Vous pouvez modifier la description, ajouter des formulaires personnalisés et les modifier simultanément dans plusieurs documents.

## Remarques concernant la modification des formulaires personnalisés

Tenez compte des points suivants lorsque vous modifiez des formulaires personnalisés dans des documents en bloc :

* Les informations que vous modifiez sur tous les documents sélectionnés remplacent les informations existantes sur des documents individuels.
* Lorsque vous sélectionnez des documents qui ont des valeurs différentes pour le même champ, le champ affiche un indicateur « Plusieurs valeurs ». L’indicateur « Plusieurs valeurs » s’affiche en regard des champs qui sont des cases à cocher, des cases d’option et des boutons bascules.
* Lorsque vous mettez à jour une option dans un champ à options multiples (tel qu’un champ qui s’affiche sous la forme d’un ensemble de boutons bascules ou de cases à cocher), toutes les autres options doivent correspondre entre les documents sélectionnés.

>[!BEGINSHADEBOX]

**Example**
You might have a custom form with a checkbox field with three checkboxes (Option1, Option 2, and Option 3) and Option 1 is unchecked for all selected documents, and Option 2 and 3 are checked for some and unchecked for other documents that you selected. Si vous souhaitez cocher l’optio  1 pour tous les documents, vous devez également faire correspondre les options 2 et 3 pour tous les projets sélectionnés avant de pouvoir enregistrer vos modifications. Vous devez donc les sélectionner ou les désélectionner afin qu’elles correspondent à tous les projets sélectionnés. Si vous ne modifiez aucune des options, vous pouvez enregistrer le champ tel quel et les documents conservent leur sélection actuelle pour toutes les options.

>[!ENDSHADEBOX]

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tout package Workfront pour gérer les documents à l’aide du stockage Workfront hérité</p>
<p>Tout package de workflow pour gérer les documents à l’aide du stockage d’entreprise Adobe</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td><p>Contributeur ou supérieur</p> 
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux documents</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer l’accès aux documents</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Edit documents in bulk in the legacy documents area

Si votre organisation utilise un stockage Workfront hérité, la zone des documents hérités s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage Workfront, voir [Différences entre le stockage d’entreprise Adobe et le stockage Workfront hérité](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

Pour modifier des documents en bloc, procédez comme suit :

1. Accédez à l’onglet Documents d’un projet ou à la zone Documents à partir du menu principal.
1. Appuyez sur la touche Ctrl ou Cmd du clavier, puis sélectionnez les documents à modifier.
1. Cliquez sur l’icône Modifier ![icône Modifier](assets/edit-icon.png).
   ![emplacement de l’icône Modifier sur la page](assets/edit-multiple-documents.png)
1. (Facultatif) Ajoutez ou modifiez la **Description**. Si la description de chaque document est différente, vous verrez _Valeurs multiples_ dans la zone de description. Vous pouvez ajouter la même description pour tous les documents, mais vous ne pouvez pas modifier individuellement les descriptions de documents lors d’une modification en bloc.
1. Effectuez les modifications suivantes avec les formulaires personnalisés :

   <table>
    <tr>
    <td><strong>Ajouter des formulaires</strong></td>
    <td>Dans la zone <strong>Ajouter un formulaire personnalisé</strong>, vous pouvez choisir parmi les formulaires joints et les formulaires à ajouter. Les formulaires joints figurent sur certains des documents sélectionnés, mais pas sur tous. Un formulaire joint à tous les documents sélectionnés s’affiche automatiquement dans la fenêtre d’édition.  </td>
    </tr>
    <tr>
    <td><strong>Modifier des formulaires</strong></td>
    <td>Modifiez les formulaires personnalisés joints. Les informations que vous modifiez remplacent les informations existantes dans des documents individuels. Les champs avec des valeurs différentes dans les documents s’affichent sous la forme de « Valeurs multiples ». </td>
    </tr>
    <tr>
    <td><strong>Réorganiser les formulaires</strong></td>
    <td>Cliquez sur le formulaire personnalisé et faites-le glisser pour le réorganiser.</td>
    </tr>
    </table>
1. Cliquez sur **Enregistrer**.

## Edit documents in bulk in the new documents area


Si votre entreprise utilise le stockage d’entreprise, la nouvelle zone de documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage d’entreprise, consultez [Présentation du stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Pour modifier des documents en bloc, procédez comme suit :

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Appuyez sur la touche Ctrl ou Cmd du clavier, puis sélectionnez les documents à modifier.
1. Click Edit at the bottom of the page.
   ![edit multiple documents](assets/bulk-edit-documents.png)
1. (Facultatif) Ajoutez ou modifiez la **Description**. Si la description de chaque document est différente, vous verrez _Valeurs multiples_ dans la zone de description. Vous pouvez ajouter la même description pour tous les documents, mais vous ne pouvez pas modifier individuellement les descriptions de documents lors d’une modification en bloc.
1. Effectuez les modifications suivantes avec les formulaires personnalisés :

   <table>
    <tr>
    <td><strong>Ajouter des formulaires</strong></td>
    <td>In the <strong>Custom form</strong> section, you can add a new custom form to the selected documents. Custom forms attached to all selected documents display in the <strong>Custom forms in common</strong> section.  </td>
    </tr>
    <tr>
    <td><strong>Modifier des formulaires</strong></td>
    <td>Modifiez les formulaires personnalisés joints. Les informations que vous modifiez remplacent les informations existantes dans des documents individuels. Les champs avec des valeurs différentes dans les documents s’affichent sous la forme de « Valeurs multiples ». </td>
    </tr>
    </table>
1. Cliquez sur **Enregistrer**.

## Modifier des documents en bloc dans un rapport de document

1. Accédez à un rapport de document existant.
ou
Create a document report as described in [Create a custom report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sélectionnez les documents à modifier.
1. Cliquez sur l’icône Modifier ![icône Modifier](assets/edit-icon.png).
1. (Facultatif) Ajoutez ou modifiez la **Description**. Si la description de chaque document est différente, vous verrez _Valeurs multiples_ dans la zone de description. Vous pouvez ajouter la même description pour tous les documents, mais vous ne pouvez pas modifier individuellement les descriptions de documents lors d’une modification en bloc.
1. Effectuez les modifications suivantes avec les formulaires personnalisés :

   <table>
    <tr>
    <td><strong>Ajouter des formulaires</strong></td>
    <td>Dans la zone <strong>Ajouter un formulaire personnalisé</strong>, vous pouvez choisir parmi les formulaires joints et les formulaires à ajouter. Les formulaires joints figurent sur certains des documents sélectionnés, mais pas sur tous. Un formulaire joint à tous les documents sélectionnés s’affiche automatiquement dans la fenêtre d’édition.  </td>
    </tr>
    <tr>
    <td><strong>Modifier des formulaires</strong></td>
    <td>Modifiez les formulaires personnalisés joints. Les informations que vous modifiez remplacent les informations existantes dans des documents individuels. Les champs avec des valeurs différentes dans les documents s’affichent sous la forme de « Valeurs multiples ». </td>
    </tr>
    <tr>
    <td><strong>Réorganiser les formulaires</strong></td>
    <td>Cliquez sur le formulaire personnalisé et faites-le glisser pour le réorganiser.</td>
    </tr>
    </table>
1. Cliquez sur **Enregistrer**.
