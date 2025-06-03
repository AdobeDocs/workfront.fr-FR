---
product-area: projects
navigation-topic: use-predecessors
title: Créer une relation d’antériorité dans la liste des tâches
description: Vous pouvez utiliser des tâches antérieures (ou plus simplement des prédécesseurs) pour lier des tâches dont le démarrage ou l’achèvement dépend d’autres tâches. Par exemple, vous ne souhaiteriez pas organiser une fête (tâche dépendante) avant d’avoir envoyé les invitations (tâche antérieure).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 70%

---

# Créer une relation d’antériorité dans la liste des tâches

<!-- Audited: 5/2025 -->

Vous pouvez utiliser des tâches antérieures (ou plus simplement des prédécesseurs) pour lier des tâches dont le démarrage ou l’achèvement dépend d’autres tâches. Par exemple, vous ne souhaiteriez pas organiser une fête (tâche dépendante) avant d’avoir envoyé les invitations (tâche antérieure).

Cet article vous explique comment créer des tâches antérieures sur la liste des tâches.

Vous pouvez afficher les tâches antérieures de tâches dans les zones suivantes d’Adobe Workfront :

* Dans la liste des tâches de la colonne Tâches antérieures.
* Dans le graphique de Gantt.
* Dans la section Prédécesseurs d&#39;une tâche dépendante.

Pour plus d’informations, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard </p><p>Actuel : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur les tâches et le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une tâche antérieure

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. Dans la liste déroulante **Vues**, sélectionnez une vue qui affiche la colonne **Prédécesseur** ou ajoutez-la à votre vue actuelle.

1. Sélectionnez la tâche que vous souhaitez désigner comme tâche dépendante.
1. Cliquez dans la colonne **Prédécesseurs** de la tâche.
1. Tapez le numéro de tâche que vous souhaitez désigner comme prédécesseur de la tâche sélectionnée, puis appuyez sur **Entrée**.

   >[!TIP]
   >
   >Pour ajouter un projet transversal antérieur, procédez comme suit :
   >
   >1. Cliquez sur l’icône **Mode Plan** et choisissez **Enregistrement automatique**.
   >
   >1. Tapez le Numéro de référence du projet du prédécesseur suivi du signe deux-points et du numéro de la tâche. Par exemple, la saisie de *765021:12* indique que le numéro de référence du projet du prédécesseur est 765021 et que le prédécesseur est la tâche numéro 12 du projet.
   >
   >1. Ajoutez le type de dépendance de cette tâche antérieure. Pour plus d’informations, voir [Créer des projets transversaux antérieurs](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >1. Appuyez sur **Entrée**.
   >
   >**IMPORTANT**
   >
   >Vous ne pouvez pas ajouter un projet transversal antérieur lorsque la liste des tâches s’affiche en mode d’enregistrement manuel.

   L’icône de la tâche antérieure devient verte lorsque la tâche antérieure est marquée comme terminée. Cela indique que la tâche dépendante est prête à être exécutée.

   Pour plus d’informations sur les types de relation disponibles dans la colonne Prédécesseurs, voir [Présentation des prédécesseurs de tâche](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Afficher les détails de la tâche antérieure

Vous pouvez afficher rapidement les détails de la tâche antérieure dans la liste des tâches.

1. Dans la liste des tâches, pointez sur le numéro du prédécesseur dans la colonne **Prédécesseurs**. Une zone contenant les détails du prédécesseur s’affiche.

   ![Détails de la tâche antérieure](assets/predecessor-details-in-task-list.png)

   Les détails suivants sont affichés :

   **Nom de la tâche antérieure :** nom de la tâche antérieure référencée. Le numéro de la tâche antérieure est inclus. Cliquez sur le nom de la tâche pour l’ouvrir.

   **Nom du projet :** nom du projet dans lequel se trouve la tâche antérieure. Le projet est identifié comme le projet en cours si la tâche antérieure appartient aux mêmes projets que la tâche, ou comme un projet transversal, si la tâche antérieure appartient à un autre projet. Pour plus d’informations sur les projets transversaux antérieurs, voir [Créer des projets transversaux antérieurs](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Vous pouvez développer les détails du projet pour afficher les dates de début et de fin prévues du projet, la condition, le statut, le pourcentage terminé et la personne propriétaire. Pour un projet transversal, vous pouvez ensuite cliquer sur **Afficher le projet** pour ouvrir le projet.

   **ID :** numéro de référence du projet dans lequel se trouve la tâche antérieure.

   **Date de début prévue :** date de début planifiée de la tâche antérieure.

   **Date de fin prévue :** date d’achèvement prévue de la tâche antérieure.

   **Nombre de prédécesseurs :** nombre de prédécesseurs pour le prédécesseur référencé.

   **Nombre de successeurs :** nombre de tâches du successeur (ou dépendantes) pour le prédécesseur référencé.
