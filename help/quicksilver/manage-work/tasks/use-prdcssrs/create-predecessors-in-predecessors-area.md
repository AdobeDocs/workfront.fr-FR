---
product-area: projects
navigation-topic: use-predecessors
title: Créer une relation de prédécesseur à l’aide de la zone Prédécesseurs
description: Vous pouvez utiliser des tâches antérieures (ou plus simplement des prédécesseurs) pour lier des tâches dont le démarrage ou l’achèvement dépend d’autres tâches.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
TQID: https://experienceleague.adobe.com/BOZkyUl3TKCzpbjbLnUcMQZjM-1laW-TSsVptvBP-0U
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 422
ht-degree: 44%

---

# Créer une relation d’antériorité à l’aide de la zone Tâches antérieures

<!-- Audited: 5/2025 -->

Vous pouvez utiliser des tâches antérieures (ou plus simplement des prédécesseurs) pour lier des tâches dont le démarrage ou l’achèvement dépend d’autres tâches. Par exemple, vous ne voudriez pas héberger une partie (tâche dépendante) avant d&#39;envoyer les invitations (tâche antérieure).

Cet article montre comment vous pouvez définir des tâches antérieures à l’aide de l’onglet Tâches antérieures dans une tâche.

Pour plus d’informations sur la définition de tâches antérieures dans une liste de tâches, voir [Créer une relation d’antériorité dans la liste des tâches](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Vous pouvez afficher les tâches antérieures de tâches dans les zones suivantes d’Adobe Workfront :

* Dans la section Tâches antérieures des tâches dépendantes
* Dans le graphique de Gantt.
* Dans la liste des tâches, dans la colonne Tâches antérieures

Pour plus d’informations sur les tâches antérieures, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur les tâches et le projet</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une tâche antérieure pour une tâche

La création d’un prédécesseur pour une tâche de projet à l’aide de la zone Prédécesseurs est similaire à la création de prédécesseurs pour une tâche de modèle sur un modèle.

Pour créer une tâche antérieure pour une tâche de projet :

1. Accédez à la tâche que vous souhaitez désigner comme tâche dépendante.

1. Dans le panneau de gauche, cliquez sur **Prédécesseurs**.

1. Dans la section **Prédécesseurs**, cliquez sur **Ajouter un prédécesseur**. La boîte de dialogue **Ajouter un prédécesseur** s’ouvre.

1. (Facultatif) Pour ajouter un projet transversal antérieur, remplacez le nom du projet dans le champ **Projet parent** par un autre projet.

   Pour plus d’informations, voir [Création de projets transversaux antérieurs](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

   >[!TIP]
   >
   >Vous ne pouvez pas créer de prédécesseurs sur plusieurs modèles pour les tâches de modèle.


1. Dans le champ **Tâches**, saisissez le nom de la ou des tâches que vous souhaitez désigner comme prédécesseurs, puis sélectionnez-les lorsqu’elles s’affichent dans la liste déroulante.

1. Sélectionnez un **Type de dépendance**.

   Pour plus d&#39;informations, voir [Présentation des types de dépendance de tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Saisissez un montant **Décalage**.

   &#x200B; Pour plus d’informations, voir Présentation [ types décalage](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   ![Boîte de dialogue Ajouter le prédécesseur](assets/add-predecessor-dialog-box.png)

1. Cochez la case **Appliquée** si vous souhaitez appliquer la relation de prédécesseur entre les deux tâches.

   Pour plus d’informations, voir [Appliquer les prédécesseurs](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Cliquer sur **Enregistrer**.

1. (Facultatif) Pour supprimer un prédécesseur, sélectionnez-le dans la liste des prédécesseurs, puis cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/remove-or-delete-icon.png).

   La tâche antérieure est supprimée de la liste. La tâche antérieure n’est pas supprimée de son projet.
