---
title: Personnalisation de la vue Détails à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En tant qu’administrateur de Workfront, vous pouvez utiliser un modèle de mise en page pour déterminer les informations qui s’affichent lorsqu’un utilisateur sélectionne la section Détails dans le panneau de gauche lors de l’affichage d’une tâche, d’un problème, d’un document, d’un programme ou d’un portfolio.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 92fb1ee0b641d2f4b527e17df272e4c37c0feaef
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Personnalisation de la vue Détails à l’aide d’un modèle de mise en page

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un modèle de mise en page pour déterminer les informations qui s’affichent lorsqu’un utilisateur clique sur l’icône Détails . ![](assets/project-details-icon.png) dans le panneau de gauche lors de l’affichage d’une tâche, d’un problème, d’un document, d’un programme ou d’un portfolio.

<!--
or billing record
-->

Vous pouvez également modifier l’ordre des informations dans lequel ces informations apparaissent. Par exemple, pour toutes les tâches que vos utilisateurs voient, vous pouvez déplacer les informations Forms personnalisées en haut de la vue Détails pour toutes les tâches que vos utilisateurs voient.

Les modifications apportées à la vue Détails d’un objet déterminent également la disponibilité et l’ordre des champs visibles par les utilisateurs dans les zones suivantes :

* Boîtes &quot;Nouvel objet&quot;, telles que Nouvelle tâche et Nouveau problème

   ![](assets/new-task-dialog.png)

* Écrans &quot;Modifier l’objet&quot;, tels que Modifier la tâche, Modifier le problème et Modifier le projet

   ![](assets/edit-task-screen.png)


* Écrans &quot;Modifier des objets&quot; lors de l’édition d’objets en bloc. Actuellement, cette fonctionnalité est prise en charge pour la modification en masse de projets.

   ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* Résumé ![](assets/summary-panel-icon.png) pour obtenir la liste des tâches et des problèmes

   ![](assets/summary-area.png)

   >[!NOTE]
   >
   >Les modifications apportées aux modèles de mise en page affectent l’ordre et la disponibilité des champs du panneau Résumé uniquement pour les tâches et les problèmes affectés à l’utilisateur connecté.

* Boîtes de conversion, telles que Convertir le problème en tâche ou Convertir le problème en zones de projet.

   ![Convertir le problème en zone de tâche](assets/convert-issue-to-task-box.png)

Pour plus d’informations sur les modèles de mise en page pour les groupes, voir [Création et modification des modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur système.
Pour les exécuter pour un groupe, vous devez être un responsable de ce groupe.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnaliser ce que voient les utilisateurs dans la vue Détails

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans la section [Création et gestion des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Cliquez sur la flèche vers le bas ![](assets/dropdown-arrow-12x12.png) under **Personnalisation des éléments affichés par les utilisateurs**, puis cliquez sur **Projet**, **Tâche**, **Problème**, **Programme** ou **Portfolio.**
<!--
, or billing record
-->

1. Dans le **Détails** pour personnaliser ce que voient les utilisateurs dans la vue Détails, effectuez l’une des opérations suivantes :

   * Faites glisser des en-têtes de section ![](assets/move-icon---dots.png) pour modifier leur ordre.
   * Activez ou désactivez des options sous **Présentation** et **Forms personnalisée** pour les afficher ou les masquer.

      Si vous masquez tous les champs de l’une de ces sections, la section entière est masquée.

      Tous les champs sont activés par défaut.

1. Continuez à personnaliser le modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Vous pouvez cliquer à tout moment sur Enregistrer pour enregistrer votre progression, puis continuer à modifier le modèle ultérieurement.
