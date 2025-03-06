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
source-git-commit: f9ebf647c7672a9d471288806cf596d103007613
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 20%

---

# Modifier des documents en bloc

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Cette option n’est disponible que dans l’environnement de prévisualisation de sandbox.</span>

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

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td><p> Nouvelle : contributeur ou contributrice ou supérieure</p> 
   <p> Actuelle : demande ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer l’accès aux documents</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

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

<span class="preview">

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

</span>