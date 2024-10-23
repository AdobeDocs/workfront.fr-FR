---
title: Exporter les formulaires personnalisés et les détails des objets
description: Exporter les formulaires personnalisés et les détails des objets
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 94%

---

# Exporter les formulaires personnalisés et les détails des objets

Vous pouvez exporter la vue d’ensemble et les informations sur les formulaires personnalisés depuis la section Détails d’un objet vers un fichier PDF. Vous pouvez ensuite imprimer ou partager le PDF avec d’autres utilisateurs et utilisatrices.

Cette fonctionnalité est prise en charge pour les objets suivants :

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
>Les champs de la section Détails que votre administrateur ou administratrice Workfront ou de groupes a supprimés à l’aide d’un modèle de disposition ne s’affichent pas.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Formule Adobe Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licence Adobe Workfront*</p> </td> 
   <td> <p>Demande ou niveau supérieur pour les problèmes</p> <p>Révision ou niveau supérieur pour les projets et les tâches</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès*</strong> </td> 
   <td> <p>Affichage ou niveau supérieur pour les projets, les tâches et les événements</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorisations d’objet</p> </td> 
   <td> <p>Autorisations d’affichage ou supérieures pour le projet, la tâche ou le problème dont vous souhaitez exporter le formulaire</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Avant de commencer :

1. Un formulaire personnalisé doit avoir été créé pour un objet spécifique à partir duquel vous souhaitez l’exporter.
1. Le formulaire personnalisé doit être joint à l’objet.

   Ou

   Vous devez disposer des droits d’accès appropriés pour joindre un formulaire personnalisé et modifier les informations contenues dans le formulaire.

Pour plus d’informations sur la création de formulaires personnalisés, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Pour plus d’informations sur l’association de formulaires à des objets, consultez [Ajouter un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Exporter des informations depuis la section Détails

L’exportation d’informations depuis la section Détails d’un objet est identique pour tous les objets dans lesquels cette fonctionnalité est prise en charge.

1. Accédez à un projet, une tâche, un portfolio, un programme ou un problème pour lequel vous disposez au moins des autorisations Affichage.
1. Cliquez sur l’**élément « Détails »** dans le panneau de gauche, par exemple **Détails de la tâche**.
1. (Facultatif) Si aucun formulaire personnalisé n’est joint à l’objet, commencez à saisir le nom d’un formulaire personnalisé dans le champ **Ajouter un formulaire personnalisé**, puis cliquez dessus lorsqu’il apparaît dans la liste.

   Vous pouvez ajouter jusqu’à 10 formulaires.

1. (Facultatif) Mettez à jour les informations dans la section Détails, puis cliquez sur **Enregistrer les modifications**.
1. Cliquez sur le menu déroulant **Exporter** dans le coin supérieur droit, sélectionnez **Vue d’ensemble** ou les formulaires à exporter, puis cliquez sur **Exporter**.

   Vous pouvez également sélectionner **Tout sélectionner** si vous souhaitez exporter la zone Vue d’ensemble et tous les formulaires personnalisés.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Les scénarios suivants sont possibles :
   >
   >   
   >   
   >   * Lorsque votre administrateur ou administratrice de groupes ou Workfront désélectionne tous les champs de la zone Vue d’ensemble et que des formulaires personnalisés sont joints à l’objet, la section Vue d’ensemble ne s’affiche pas.
   >   * Lorsque votre administrateur ou administratrice de groupes ou Workfront désélectionne tous les champs de la zone Vue d’ensemble et qu’aucun formulaire personnalisé n’est joint à l’objet, le menu déroulant Exporter n’est pas visible.
   >   * Si aucun formulaire personnalisé n’est joint à l’objet, vous pouvez uniquement exporter la zone Vue d’ensemble.
   >   * Les champs personnalisés qui se trouvent derrière une logique et ne sont pas visibles sur le formulaire ne sont pas exportés. Pour plus d’informations sur l’ajout d’une logique à un formulaire personnalisé, voir [Ajout d’une logique d’affichage et saut de la logique à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
   >   
   >

   Un fichier PDF est produit et téléchargé sur votre ordinateur. Le fichier PDF contient les informations suivantes :

   * Le nom de l’objet auquel le formulaire est associé.
   * Le nom de l’utilisateur ou de l’utilisatrice qui a exporté le PDF.
   * La date et l’heure de production du PDF.
   * Le nom des formulaires que vous avez exportés.
   * Les informations des champs renseignés sur le formulaire.
