---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Modifier des documents en bloc
description: Vous pouvez modifier plusieurs documents à la fois dans la zone Documents .
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: e8badce6-86f5-416c-a238-f9b7f19cdd2d
source-git-commit: 4a0448583cbcfd1f1df10d6474fdf4e77e7bff3e
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 10%

---

# Modifier des documents en bloc

Vous pouvez modifier la description, ajouter des formulaires personnalisés et modifier simultanément des formulaires personnalisés dans plusieurs documents.

## Remarques concernant la modification des formulaires personnalisés

Tenez compte des points suivants lors de la modification en bloc de formulaires personnalisés de document :

* Les informations que vous modifiez sur tous les documents sélectionnés remplacent les informations existantes sur des documents individuels.
* Lorsque vous sélectionnez des documents dont les valeurs du champ sont différentes, le champ affiche un indicateur « Valeurs multiples ». L’indicateur « Plusieurs valeurs » s’affiche en regard des champs qui sont des cases à cocher, des cases d’option et des boutons bascules.
* Lorsque vous mettez à jour une option dans un champ à options multiples (par exemple un champ qui s’affiche sous la forme d’un ensemble de bascules ou de cases à cocher), toutes les autres options doivent correspondre entre les documents sélectionnés.

>[!BEGINSHADEBOX]

**Exemple**
Vous pouvez avoir un formulaire personnalisé avec un champ de case à cocher avec trois cases à cocher (Option1, Option 2 et Option 3) et l&#39;Option 1 est décochée pour tous les documents sélectionnés, et les Options 2 et 3 sont cochées pour certains et décochées pour d&#39;autres documents que vous avez sélectionnés. Si vous souhaitez cocher l&#39;option 1 pour tous les documents, vous devez également faire correspondre les options 2 et 3 pour tous les projets sélectionnés avant de pouvoir enregistrer vos modifications. Vous devez donc les sélectionner ou les désélectionner afin qu’ils correspondent à tous les projets sélectionnés. Si vous ne modifiez aucune des options, vous pouvez enregistrer le champ tel quel et les documents conservent leur sélection actuelle pour toutes les options.

>[!ENDSHADEBOX]

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td><p>Contributeur ou version ultérieure</p> 
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

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier des documents en bloc

Pour modifier des documents en bloc :

1. Accédez à l’onglet Documents d’un projet ou à la zone Documents à partir du menu principal.
1. Appuyez sur la touche Ctrl ou Cmd du clavier, puis sélectionnez les documents à modifier.
1. Cliquez sur l’icône Modifier ![icône Modifier](assets/edit-icon.png).
   ![modifier l’emplacement de l’icône sur la page](assets/edit-multiple-documents.png)
1. (Facultatif) Ajoutez ou modifiez la **Description**. Si la description de chaque document est différente, vous verrez _Valeurs multiples_ dans la zone de description. Vous pouvez ajouter la même description pour tous les documents, mais vous ne pouvez pas modifier individuellement les descriptions de documents lors d&#39;une modification en bloc.
1. Effectuez les modifications suivantes avec les formulaires personnalisés :

   <table>
    <tr>
    <td><strong>Ajouter des formulaires</strong></td>
    <td>Dans la zone <strong>Ajouter un formulaire personnalisé</strong>, vous pouvez choisir parmi les formulaires joints et les formulaires à ajouter. Les formulaires joints figurent sur certains des documents sélectionnés, mais pas sur tous. Un formulaire joint à tous les documents sélectionnés s'affiche automatiquement dans la fenêtre d'édition.  </td>
    </tr>
    <tr>
    <td><strong>Modification de formulaires</strong></td>
    <td>Modifiez les formulaires personnalisés joints. Les informations que vous modifiez remplacent les informations existantes dans des documents individuels. Les champs avec des valeurs différentes dans les documents s’affichent sous la forme de « valeurs multiples ». </td>
    </tr>
    <tr>
    <td><strong>Réorganiser les formulaires</strong></td>
    <td>Cliquez sur le formulaire personnalisé et faites-le glisser pour le réorganiser.</td>
    </tr>
    </table>
1. Cliquer sur **Enregistrer**.


## Modifier des documents en bloc dans un rapport de document

1. Accédez à un rapport de document existant.
ou
Créez un rapport de document comme décrit dans la section [Créer un rapport personnalisé](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Sélectionnez les documents à modifier.
1. Cliquez sur l’icône Modifier ![icône Modifier](assets/edit-icon.png).
   ![modifier l’emplacement de l’icône sur la page](assets/edit-multiple-documents.png)
1. (Facultatif) Ajoutez ou modifiez la **Description**. Si la description de chaque document est différente, vous verrez _Valeurs multiples_ dans la zone de description. Vous pouvez ajouter la même description pour tous les documents, mais vous ne pouvez pas modifier individuellement les descriptions de documents lors d&#39;une modification en bloc.
1. Effectuez les modifications suivantes avec les formulaires personnalisés :

   <table>
    <tr>
    <td><strong>Ajouter des formulaires</strong></td>
    <td>Dans la zone <strong>Ajouter un formulaire personnalisé</strong>, vous pouvez choisir parmi les formulaires joints et les formulaires à ajouter. Les formulaires joints figurent sur certains des documents sélectionnés, mais pas sur tous. Un formulaire joint à tous les documents sélectionnés s'affiche automatiquement dans la fenêtre d'édition.  </td>
    </tr>
    <tr>
    <td><strong>Modification de formulaires</strong></td>
    <td>Modifiez les formulaires personnalisés joints. Les informations que vous modifiez remplacent les informations existantes dans des documents individuels. Les champs avec des valeurs différentes dans les documents s’affichent sous la forme de « valeurs multiples ». </td>
    </tr>
    <tr>
    <td><strong>Réorganiser les formulaires</strong></td>
    <td>Cliquez sur le formulaire personnalisé et faites-le glisser pour le réorganiser.</td>
    </tr>
    </table>
1. Cliquer sur **Enregistrer**.
