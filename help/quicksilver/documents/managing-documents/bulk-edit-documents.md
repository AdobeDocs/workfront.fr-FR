---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Modifier des documents en masse
description: Vous pouvez modifier plusieurs documents à la fois dans la zone Documents .
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: 8c1f829eb29d8cd13524814d98ed353add15e881
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 26%

---


# Modifier des documents en masse

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Cette option n’est disponible que dans l’environnement de prévisualisation de sandbox.</span>

Vous pouvez modifier la description, ajouter des formulaires personnalisés et modifier des formulaires personnalisés sur plusieurs documents à la fois.

## Remarques concernant la modification de formulaires personnalisés

Tenez compte des points suivants lors de la modification en masse de formulaires personnalisés de document :

* Les informations que vous modifiez sur tous les documents sélectionnés remplacent les informations existantes sur les documents individuels.
* Lorsque vous sélectionnez des documents dont les valeurs du même champ sont différentes, le champ affiche un indicateur &quot;Plusieurs valeurs&quot;. L’indicateur « Plusieurs valeurs » s’affiche en regard des champs qui sont des cases à cocher, des cases d’option et des boutons bascules.
* Lorsque vous mettez à jour une option dans un champ à plusieurs options (un champ qui s’affiche sous la forme d’un ensemble de bascules ou de cases à cocher, par exemple), toutes les autres options doivent correspondre entre les documents sélectionnés.

>[!BEGINSHADEBOX]

**Exemple**
Il se peut que vous ayez un formulaire personnalisé avec un champ de case à cocher comportant trois cases à cocher (Option 1, Option 2 et Option 3). L’option 1 n’est pas cochée pour tous les documents sélectionnés. Les options 2 et 3 sont cochées pour certains documents et décochées pour d’autres documents que vous avez sélectionnés. Si vous souhaitez vérifier l’option 1 pour tous les documents, vous devez également faire correspondre les options 2 et 3 pour tous les projets sélectionnés avant de pouvoir enregistrer vos modifications. Vous devez donc les sélectionner ou les désélectionner afin qu’ils puissent correspondre à tous les projets sélectionnés. Si vous ne modifiez aucune des options, vous pouvez enregistrer le champ tel quel et les documents conservent leur sélection actuelle pour toutes les options.

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

## Modifier des documents en masse

Pour modifier des documents en bloc :

1. Accédez à l’onglet Documents d’un projet ou à la zone Documents à partir du menu principal.
1. Appuyez sur ctrl ou cmd sur votre clavier, puis sélectionnez les documents à modifier.
1. Cliquez sur l&#39;icône Modifier ![icône de modification](assets/edit-icon.png).
   ![Modifier l’emplacement de l’icône sur la page](assets/edit-multiple-documents.png)
1. (Facultatif) Ajoutez ou modifiez la **description**. Si la description de chaque document est différente, vous verrez _Plusieurs valeurs_ dans la zone de description. Vous pouvez ajouter la même description pour tous les documents, mais vous ne pouvez pas modifier les descriptions de documents individuels lors de la modification en bloc.
1. Apportez les modifications suivantes aux formulaires personnalisés :

   <table>
    <tr>
    <td><strong>Ajouter des formulaires</strong></td>
    <td>Dans la <strong> zone Ajouter un formulaire personnalisé</strong>, vous pouvez choisir parmi Formulaires joints et formulaires à ajouter. Les formulaires attachés se trouvent sur certains des documents sélectionnés, mais pas tous. Un formulaire joint à tous les documents sélectionnés s’affiche automatiquement dans la fenêtre d’édition.  </td>
    </tr>
    <tr>
    <td><strong>Modifier les formulaires</strong></td>
    <td>Modifiez tous les formulaires personnalisés joints. Les informations que vous modifiez remplacent les informations existantes sur les documents individuels. Les champs avec des valeurs différentes dans les documents s’affichent sous la forme "Plusieurs valeurs". </td>
    </tr>
    <tr>
    <td><strong>Réorganiser les formulaires</strong></td>
    <td>Cliquez sur le formulaire personnalisé et faites-le glisser pour le réorganiser.</td>
    </tr>
    </table>
1. Cliquer sur **Enregistrer**.


