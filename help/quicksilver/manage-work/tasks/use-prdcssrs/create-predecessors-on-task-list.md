---
product-area: projects
navigation-topic: use-predecessors
title: Créer une relation d’antériorité dans la liste des tâches
description: Vous pouvez utiliser des tâches antérieures (ou plus simplement des prédécesseurs) pour lier des tâches dont le démarrage ou l’achèvement dépend d’autres tâches. Par exemple, vous ne souhaiteriez pas organiser une fête (tâche dépendante) avant d’avoir envoyé les invitations (tâche antérieure).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 100%

---

# Créer une relation d’antériorité dans la liste des tâches

Vous pouvez utiliser des tâches antérieures (ou plus simplement des prédécesseurs) pour lier des tâches dont le démarrage ou l’achèvement dépend d’autres tâches. Par exemple, vous ne souhaiteriez pas organiser une fête (tâche dépendante) avant d’avoir envoyé les invitations (tâche antérieure).

Cet article vous explique comment créer des tâches antérieures sur la liste des tâches.

Vous pouvez afficher les tâches antérieures de tâches dans les zones suivantes d’Adobe Workfront :

* Dans la liste des tâches de la colonne Tâches antérieures.
* Dans le graphique de Gantt.
* Dans la section Tâches antérieures d’une tâche dépendante.

Pour plus d’informations, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard </p><p>Actuel : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur les tâches et le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront. Pour plus d’informations sur les exigences d’accès, consultez l’article [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Créer une tâche antérieure

1. Accédez à un projet.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. Assurez-vous que votre affichage actuel comporte la colonne **Tâches antérieures**.

   Si l’affichage ne comporte pas la colonne Tâches antérieures, modifiez l’affichage ou ajoutez-y la colonne.

1. Sélectionnez la tâche que vous souhaitez désigner comme tâche dépendante.
1. Cliquez dans la colonne **Tâches antérieures**.
1. Saisissez le numéro de la tâche que vous souhaitez désigner comme tâche antérieure de la tâche sélectionnée, puis appuyez sur **Entrée**.

   >[!TIP]
   >
   >Pour ajouter un projet transversal antérieur, procédez comme suit :
   >
   >1. Cliquez sur l’icône **Mode Plan** et choisissez **Enregistrement automatique**.
   >
   >1. Saisissez le numéro de référence du projet de la tâche antérieure, suivi de deux points et du numéro de la tâche. Par exemple, saisissez : 765021:12. Cette saisie indique que le numéro de référence du projet de la tâche antérieure est 765021 et que la tâche antérieure est la tâche numéro 12 du projet.
   >
   >1. Ajoutez le type de dépendance de cette tâche antérieure. Pour plus d’informations, voir [Créer des projets transversaux antérieurs](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >Appuyez sur **Entrée**.
   >
   >**IMPORTANT**
   >
   >Vous ne pouvez pas ajouter de projet transversal antérieur lorsque la liste des tâches s’affiche en mode Enregistrement manuel.

   L’icône de la tâche antérieure devient verte lorsque la tâche antérieure est marquée comme terminée. Cela indique que la tâche dépendante est prête à être exécutée.

   Pour plus d’informations sur les types de relations disponibles dans la colonne Tâches antérieures, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) dans [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Afficher les détails de la tâche antérieure

Vous pouvez afficher rapidement les détails de la tâche antérieure dans la liste des tâches.

1. Dans la liste des tâches, placez la souris sur le numéro de la tâche antérieure de la colonne **Tâches antérieures**.

   Une zone contenant les détails de la tâche antérieure s’affiche.

   ![Détails de la tâche antérieure](assets/predecessor-details-in-task-list.png)

   Les détails suivants sont affichés :

   **Nom de la tâche antérieure :** nom de la tâche antérieure référencée. Le numéro de la tâche antérieure est inclus. Cliquez sur le nom de la tâche pour l’ouvrir. Dans l’exemple ci-dessus, la tâche antérieure est Production/Exécution/Diffusion.

   **Nom du projet :** nom du projet dans lequel se trouve la tâche antérieure. Le projet est identifié comme le projet en cours si la tâche antérieure appartient aux mêmes projets que la tâche, ou comme un projet transversal, si la tâche antérieure appartient à un autre projet. Dans l’exemple ci-dessus, le nom du projet est Production de ressources numériques (intégrée) - Projet. Pour plus d’informations sur les projets transversaux antérieurs, voir [Créer des projets transversaux antérieurs](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Vous pouvez développer les détails du projet pour afficher les dates de début et de fin prévues du projet, la condition, le statut, le pourcentage terminé et la personne propriétaire. Pour un projet transversal, vous pouvez ensuite cliquer sur **Afficher le projet** pour ouvrir le projet.

   **ID :** numéro de référence du projet dans lequel se trouve la tâche antérieure.

   **Date de début prévue :** date de début planifiée de la tâche antérieure.

   **Date de fin prévue :** date d’achèvement prévue de la tâche antérieure.

   **Nombre de tâches antérieures :** nombre de tâches antérieures pour la tâche antérieure référencée. Dans l’exemple ci-dessus, la tâche antérieure référencée a 1 tâche antérieure.

   **Nombre de tâches antérieures :** nombre de tâches antérieures (ou dépendantes) pour la tâche antérieure référencée. Dans l’exemple ci-dessus, la tâche antérieure référencée a 1 tâche antérieure.
