---
title: Personnalisation de la vue Détails à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En tant qu’administrateur de Workfront, vous pouvez utiliser un modèle de mise en page pour déterminer les informations qui s’affichent lorsqu’un utilisateur sélectionne la section Détails dans le panneau de gauche lors de l’affichage d’une tâche, d’un problème, d’un document, d’un programme ou d’un portfolio.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 7c624eff8931d206285b6c4d91083f4bf09a88b0
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 31%

---

# Personnalisation de la vue Détails à l’aide d’un modèle de mise en page

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un modèle de mise en page pour déterminer les informations qui s’affichent lorsqu’un utilisateur clique sur l’icône Détails ![](assets/project-details-icon.png) dans le panneau de gauche lors de l’affichage d’une tâche, d’un problème, d’un document, d’un programme ou d’un portfolio.

<!--
or billing record
-->

Vous pouvez également modifier l’ordre des informations dans lequel ces informations apparaissent. Par exemple, pour toutes les tâches que vos utilisateurs voient, vous pouvez déplacer les informations Forms personnalisées en haut de la vue Détails pour toutes les tâches que vos utilisateurs voient.

Pour plus d’informations sur la création de modèles de disposition, voir [Créer et gérer des modèles de disposition](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de disposition pour les groupes, voir [Créer et modifier des modèles de disposition d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de disposition, vous devez l’attribuer à des utilisateurs et utilisatricess pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de disposition à des utilisateurs et utilisatrices, voir [Attribuer un modèle de disposition à des utilisateurs et utilisatrices](../use-layout-templates/assign-users-to-layout-template.md).

Les modifications apportées à la vue Détails d’un objet déterminent également la disponibilité et l’ordre des champs visibles par les utilisateurs dans les zones suivantes :


* Boîtes &quot;Créer un objet&quot;, telles que Créer une tâche

  ![](assets/new-task-dialog.png)


* Écrans &quot;Modifier l’objet&quot; lors de la modification d’un objet, tels que Modifier la tâche, Modifier le problème et Modifier le projet

  ![](assets/edit-task-screen.png)


* Ecrans &quot;Modifier des objets&quot; lors de l’édition d’objets en bloc. Actuellement, cette fonctionnalité est prise en charge pour la modification en masse de projets.

  ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* Panneau de résumé ![](assets/summary-panel-icon.png) pour les listes de tâches et de problèmes

  ![](assets/summary-area.png)

  >[!NOTE]
  >
  >Les modifications apportées aux modèles de mise en page affectent l’ordre et la disponibilité des champs du panneau Résumé uniquement pour les tâches et les problèmes affectés à l’utilisateur connecté.

* Boîtes de conversion, telles que Convertir le problème en tâche ou Convertir le problème en zones de projet.

  ![Convertir le problème en zone de tâche](assets/convert-issue-to-task-box.png)

Pour plus d’informations sur les modèles de disposition pour les groupes, voir [Créer et modifier des modèles de disposition d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.
Pour les exécuter pour un groupe, vous devez être un responsable de ce groupe.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnaliser ce que voient les utilisateurs dans la vue Détails

1. Commencez à travailler sur un modèle de disposition, comme décrit dans la section [Créer et gérer des modèles de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Cliquez sur la flèche vers le bas ![](assets/dropdown-arrow-12x12.png) sous **Personnaliser ce que les utilisateurs voient**, puis cliquez sur **Projet**, **Tâche**, **Problème**, **Programme** ou **Portfolio.**
<!--
, or billing record
-->

1. Dans la section **Détails** , effectuez l’une des opérations suivantes pour personnaliser ce que les utilisateurs voient dans la vue Détails :

   * Faites glisser les en-têtes de section ![](assets/move-icon---dots.png) pour modifier leur ordre.
   * Activez ou désactivez des options sous **Aperçu** et **Forms personnalisé** pour les afficher ou les masquer.

     Si vous masquez tous les champs de l’une de ces sections, la section entière est masquée.

     Tous les champs sont activés par défaut.

1. Poursuivez la personnalisation du modèle de disposition.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Vous pouvez cliquer à tout moment sur Enregistrer pour enregistrer votre progression, puis continuer à modifier le modèle ultérieurement.
