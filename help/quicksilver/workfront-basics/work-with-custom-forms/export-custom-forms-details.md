---
title: Exporter les formulaires personnalisés et les détails des objets
description: Exporter les formulaires personnalisés et les détails des objets
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 19%

---

# Exporter les formulaires personnalisés et les détails des objets

Vous pouvez exporter l’ Aperçu et les informations de formulaire personnalisées de la section Détails d’un objet vers un fichier de PDF. Vous pouvez ensuite imprimer ou partager le PDF avec d’autres utilisateurs.

Cette fonctionnalité est prise en charge pour les objets suivants :

* Projets
* Tâches
* Problèmes
* Portfolio
* Programmes

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>Les champs de la section Détails que votre administrateur Workfront ou de groupe a supprimés à l’aide d’un modèle de mise en page ne s’affichent pas.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Forfait Adobe Workfront*</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licence Adobe Workfront*</p> </td> 
   <td> <p>Requête ou supérieure pour les problèmes</p> <p>Révision ou version ultérieure pour les projets et les tâches</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès*</strong> </td> 
   <td> <p>Affichage ou version ultérieure pour les projets, tâches et problèmes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorisations d’objet</p> </td> 
   <td> <p>Afficher ou des autorisations supérieures pour le projet, la tâche ou le formulaire dont vous souhaitez exporter le formulaire</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Avant de commencer, vous devez disposer des éléments suivants :

1. Créez un formulaire personnalisé pour un objet spécifique à partir duquel vous souhaitez l’exporter.
1. Associer le formulaire personnalisé à l’objet

   Ou

   disposer des droits d’accès appropriés pour joindre un formulaire personnalisé et modifier les informations contenues dans le formulaire.

Pour plus d’informations sur la création de formulaires personnalisés, voir [Concevoir un formulaire avec le concepteur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Pour plus d’informations sur l’association de formulaires à des objets, voir [Ajout d’un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Informations sur l’export dans la section Détails

L’export d’informations depuis la section Détails d’un objet est identique pour tous les objets dans lesquels il est pris en charge.

1. Accédez à un projet, une tâche, un portefeuille, un programme ou un problème pour lequel vous disposez au moins des autorisations Afficher .
1. Cliquez sur l’élément **&quot;Details&quot;** dans le panneau de gauche, par exemple **Task Details**.
1. (Facultatif) S’il n’existe aucun formulaire personnalisé associé à l’objet, commencez à saisir le nom d’un formulaire personnalisé dans le **champ Ajouter un formulaire personnalisé**, puis cliquez dessus lorsqu’il apparaît dans la liste.

   Vous pouvez ajouter jusqu’à 10 formulaires.

1. (Facultatif) Mettez à jour les informations dans la section Détails, puis cliquez sur **Enregistrer les modifications**.
1. Cliquez sur le menu déroulant **Export** dans le coin supérieur droit, sélectionnez **Overview** ou les formulaires à exporter, puis cliquez sur **Export**.

   Vous pouvez également sélectionner **Sélectionner tout** si vous souhaitez exporter la zone Aperçu et tous les formulaires personnalisés.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Les scénarios suivants peuvent exister :
   >
   >   
   >   
   >   * Lorsque votre administrateur de groupe ou Workfront désélectionne tous les champs de la zone Overview et que des formulaires personnalisés sont associés à l’objet, la section Overview ne s’affiche pas.
   >   * Lorsque votre administrateur de groupe ou Workfront désélectionne tous les champs de la zone Overview et qu’aucun formulaire personnalisé n’est associé à l’objet, le menu déroulant Export n’est pas visible.
   >   * Si aucun formulaire personnalisé n’est associé à l’objet, vous pouvez exporter uniquement la zone Overview .
   >   * Les champs personnalisés qui se trouvent derrière la logique et ne sont pas visibles sur le formulaire ne sont pas exportés. Pour plus d’informations sur l’ajout d’une logique à un formulaire personnalisé, voir [Ajout d’une logique d’affichage et saut de la logique à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
   >   
   >

   Un fichier de PDF est produit et téléchargé sur votre ordinateur. Le fichier du PDF contient les informations suivantes :

   * Nom de l’objet auquel le formulaire est associé
   * Nom de l’utilisateur qui a exporté le PDF
   * Date et heure de production du PDF
   * Nom des formulaires que vous avez exportés
   * Informations des champs renseignés sur le formulaire
