---
product-area: templates
navigation-topic: templates-navigation-topic
title: Création d’un modèle de projet
description: Vous pouvez créer et supprimer des modèles dans la zone Modèles . Lors de la création d’un modèle, vous pouvez saisir les informations pour toutes les tâches et toutes les informations pour les futurs paramètres du projet. Ces informations seront ensuite transférées vers le projet, lorsque vous le créerez à partir du modèle.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Création d’un modèle de projet

Vous pouvez créer et supprimer des modèles dans la zone Modèles . Lors de la création d’un modèle, vous pouvez saisir les informations pour toutes les tâches et toutes les informations pour les futurs paramètres du projet. Ces informations seront ensuite transférées vers le projet, lorsque vous le créerez à partir du modèle.

Vous pouvez créer un modèle de la manière suivante :

* À partir de zéro, comme décrit dans cet article.
* À partir de projets existants, en enregistrant un projet en tant que modèle.

   Pour plus d’informations sur la création de modèles à partir de projets existants, voir [Enregistrement d’un projet en tant que modèle](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* En la copiant à partir d’un autre modèle.

   Pour plus d’informations sur la copie d’un modèle existant, voir [Copier un modèle de projet](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Si vous êtes administrateur de Workfront, vous pouvez créer des modèles en important des plans directeurs. Pour plus d’informations, voir [Configuration d’un plan directeur](../../../administration-and-setup/blueprints/configure-template-package.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Administrateur système pour l’importation de modèles à partir de plans directeurs</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux modèles</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Par défaut, vous disposez des autorisations de gestion des modèles que vous créez.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Créer un modèle

1. Dans la **Menu Principal** ![](assets/main-menu-icon.png) click **Modèles**.

1. Cliquez sur **Nouveau modèle**.

   Le modèle est sans titre.

   ![Nouveau modèle](assets/create-template-nwe-2022-350x102.png)

1. Indiquez un nom pour le nouveau modèle dans l’en-tête du modèle, puis appuyez sur **Saisissez .**
1. Cliquez sur le bouton **Tâches de modèle** dans le panneau de gauche.
1. Cliquez sur **Commencer à ajouter des tâches de modèle**.

   Ou

   Cliquez sur **Nouvelle tâche de modèle** pour commencer à ajouter des tâches à votre modèle.

   L’ajout de tâches de modèle à un modèle est identique à l’ajout de tâches à un projet.

   Pour plus d’informations sur l’ajout de tâches à un projet, voir [Création de tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Vous ne pouvez pas ajouter de tâches récurrentes à un modèle.

1. (Facultatif) Cliquez sur le **Graphique Gantt** dans le coin supérieur droit de la liste des tâches pour afficher une représentation visuelle de la liste des tâches du modèle.

   >[!TIP]
   >
   >Vous ne pouvez pas modifier les tâches directement à partir de ce diagramme de Gantt.

1. Pour ajouter des informations à votre nouveau modèle, cliquez sur le bouton **Plus** menu ![](assets/more-icon.png), puis cliquez sur **Modifier**.

   Pour plus d’informations sur la modification d’un modèle, voir [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Cliquez sur **Enregistrer les modifications**.
1. (Facultatif) Si vous souhaitez ajouter des éléments supplémentaires au modèle, reportez-vous à la section [Ajouter des éléments supplémentaires à un modèle](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) dans l’article [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Paramètres de modèle déterminés par l’association de groupe

L’association d’un modèle de projet à un groupe (ou son absence) affecte la manière dont les préférences de projet, de tâche et d’émission déterminent certains paramètres du modèle. Pour plus d’informations, voir la section [Création et modification de modèles de projet d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) dans l’article [Création et modification de modèles de projet d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
