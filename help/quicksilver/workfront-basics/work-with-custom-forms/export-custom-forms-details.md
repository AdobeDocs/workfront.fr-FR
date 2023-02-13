---
title: Exportation de formulaires personnalisés et de détails d’objet
description: Exportation de formulaires personnalisés et de détails d’objet
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1670edf153e57152e51adcfbda052eb74541d931
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 1%

---

# Exportation de formulaires personnalisés et de détails d’objet

Vous pouvez exporter l’ Aperçu et les informations de formulaire personnalisées de la section Détails d’un objet vers un fichier de PDF. Vous pouvez ensuite imprimer ou partager le PDF avec d’autres utilisateurs.

Cette fonctionnalité est prise en charge pour les objets suivants :

* Projets
* Tâches
* Événements
* Portfolio
* Programmes

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>Les champs de la section Détails que votre administrateur Workfront ou de groupe a supprimés à l’aide d’un modèle de mise en page ne s’affichent pas.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Formule Adobe Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licence Adobe Workfront*</p> </td> 
   <td> <p>Demande ou version ultérieure pour les problèmes</p> <p>Révision ou version ultérieure pour les projets et les tâches</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong> </td> 
   <td> <p>Affichage ou version ultérieure pour les projets, tâches et problèmes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorisations d’objet</p> </td> 
   <td> <p>Afficher ou des autorisations supérieures pour le projet, la tâche ou le formulaire dont vous souhaitez exporter le formulaire</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de commencer, vous devez disposer des éléments suivants :

1. Créez un formulaire personnalisé pour un objet spécifique à partir duquel vous souhaitez l’exporter.
1. Associer le formulaire personnalisé à l’objet

   Ou

   Disposez des droits d’accès appropriés pour joindre un formulaire personnalisé et modifier les informations contenues dans le formulaire.

Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

Pour plus d’informations sur l’association de formulaires à des objets, voir [Ajout d’un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Informations sur l’export dans la section Détails

L’export d’informations depuis la section Détails d’un objet est identique pour tous les objets dans lesquels il est pris en charge.

1. Accédez à un projet, une tâche, un portefeuille, un programme ou un problème pour lequel vous disposez au moins des autorisations Afficher .
1. Cliquez sur le bouton **Elément &quot;Détails&quot;** dans le panneau de gauche, par exemple **Détails de la tâche**.
1. (Facultatif) Si aucun formulaire personnalisé n’est associé à l’objet, commencez à saisir le nom d’un formulaire personnalisé dans la variable **Ajouter un champ de formulaire personnalisé**, puis cliquez dessus lorsqu’il apparaît dans la liste.

   Vous pouvez ajouter jusqu’à 10 formulaires.

1. (Facultatif) Mettez à jour les informations dans la section Détails, puis cliquez sur **Enregistrer les modifications**.
1. Cliquez sur le bouton **Exporter** dans le menu déroulant du coin supérieur droit, sélectionnez **Présentation** ou les formulaires à exporter, puis cliquez sur **Exporter**.

   Vous pouvez également sélectionner **Tout sélectionner** si vous souhaitez exporter la zone Aperçu et tous les formulaires personnalisés.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Les scénarios suivants peuvent exister :
   >
   >   
   >   
   >   * Lorsque votre administrateur de groupe ou Workfront désélectionne tous les champs de la zone Overview et que des formulaires personnalisés sont associés à l’objet, la section Overview ne s’affiche pas.
   >   * Lorsque votre administrateur de groupe ou Workfront désélectionne tous les champs de la zone Overview et que l’objet ne comporte aucun formulaire personnalisé associé, le menu déroulant Export n’est pas visible.
   >   * Si aucun formulaire personnalisé n’est associé à l’objet, vous pouvez exporter uniquement la zone Overview .
   >   * Les champs personnalisés qui se trouvent derrière la logique et ne sont pas visibles sur le formulaire ne sont pas exportés. Pour plus d’informations sur l’ajout d’une logique à un formulaire personnalisé, voir [Ajouter une logique d’affichage et ignorer une logique dans un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md).


   Un fichier de PDF est produit et téléchargé sur votre ordinateur. Le fichier du PDF contient les informations suivantes :

   * Nom de l’objet auquel le formulaire est associé
   * Nom de l’utilisateur qui a exporté le PDF
   * Date et heure auxquelles le PDF a été produit
   * Nom des formulaires que vous avez exportés
   * Informations des champs renseignés sur le formulaire
