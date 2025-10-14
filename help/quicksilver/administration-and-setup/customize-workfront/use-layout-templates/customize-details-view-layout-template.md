---
title: Personnalisation de la vue Détails à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En tant qu’administrateur ou administratrice Workfront, vous pouvez utiliser un modèle de mise en page pour déterminer les informations qui s’affichent lorsqu’une personne sélectionne la section Détails dans le panneau de gauche lors de l’affichage d’une tâche, d’un problème, d’un document, d’un programme ou d’un portfolio.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 74%

---

# Personnaliser la vue Détails à l’aide d’un modèle de mise en page

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un modèle de mise en page pour déterminer les informations qui s’affichent lorsqu’un utilisateur clique sur l’icône Détails ![icône Détails](assets/project-details-icon.png) dans le panneau de gauche lors de l’affichage d’une tâche, d’un événement, d’un document, d’un programme ou d’un portfolio.

<!--
or billing record
-->

Vous pouvez également modifier l’ordre dans lequel ces informations apparaissent. Par exemple, pour toutes les tâches que vos utilisateurs et utilisatrices voient, vous pouvez déplacer les informations sur les formulaires personnalisés en haut de la vue Détails.

Pour plus d’informations sur la création de modèles de mise en page, voir [Créer et gérer des modèles de mise en page](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de disposition pour les groupes, voir [Créer et modifier des modèles de disposition d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de mise en page, vous devez l’affecter aux utilisateurs et utilisatrices pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de mise en page aux utilisateurs et utilisatrices, voir [Attribuer des utilisateurs et utilisatrices à un modèle de mise en page](../use-layout-templates/assign-users-to-layout-template.md).

Les modifications apportées à la vue Détails d’un objet déterminent également la disponibilité et l’ordre des champs visibles par les utilisateurs et utilisatrices dans les zones suivantes :


* Zones « Créer un objet », telles que Créer une tâche

  ![&#x200B; Boîte de dialogue Nouvelle tâche &#x200B;](assets/new-task-dialog.png)


* Écrans « Modifier un objet » lors de la modification d’un objet, tels que Modifier une tâche, Modifier un problème et Modifier un projet

  ![Écran Modifier la tâche](assets/edit-task-screen.png)


* Écrans « Modifier des objets » lors de la modification d’objets en masse. Actuellement, cette fonctionnalité est prise en charge pour la modification en masse de projets.

  ![Personnaliser la modification de projets](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* Panneau Résumé ![panneau Résumé](assets/summary-panel-icon.png) pour les listes de tâches et d’événements

  ![Zone Résumé](assets/summary-area.png)

  >[!NOTE]
  >
  >Les modifications apportées aux modèles de mise en page affectent l’ordre et la disponibilité des champs du panneau Résumé uniquement pour les tâches et les problèmes affectés à la personne connectée.

* Zones de conversion, telles que les zones Convertir le problème en tâche ou Convertir le problème en projet.

  ![Zone Convertir le problème en tâche](assets/convert-issue-to-task-box.png)

Pour plus d’informations sur les modèles de mise en page pour les groupes, voir [Créer et modifier des modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td><p>Nouveau : Standard</p>
  <p> Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.
Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personnaliser ce que voient les utilisateurs et utilisatrices dans la vue Détails.

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans la section [Créet et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Cliquez sur la flèche vers le bas ![Flèche vers le bas](assets/dropdown-arrow-12x12.png) sous **Personnaliser ce que voient les utilisateurs**, puis cliquez sur **Projet**, **Tâche**, **Problème**, **Program** ou **Portfolio.**
<!--
, or billing record
-->

1. Dans la section **Détails**, pour personnaliser ce que voient les utilisateurs et utilisatrices dans la vue Détails, effectuez l’une des opérations suivantes :

   * Faites glisser les en-têtes de section ![icône Déplacer](assets/move-icon---dots.png) pour modifier leur ordre.
   * Activez ou désactivez les options dans les différentes zones (telles que **Présentation**, **Finance** et **Forms personnalisé**) pour les afficher ou les masquer.

     Si vous masquez tous les champs de l’une de ces sections, la section entière est masquée.

     Tous les champs sont activés par défaut. Vous pouvez cocher ou décocher la case **Tout sélectionner** dans une zone pour afficher ou masquer tous les champs de cette zone.

   ![Vue Détails dans le modèle de mise en page](assets/layout-template-details-view.png)

1. Poursuivez la personnalisation du modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Vous pouvez cliquer à tout moment sur Enregistrer pour enregistrer votre progression, puis continuer à modifier le modèle ultérieurement.
