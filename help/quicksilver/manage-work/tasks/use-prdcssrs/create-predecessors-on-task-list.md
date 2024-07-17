---
product-area: projects
navigation-topic: use-predecessors
title: Créer une relation d’antériorité dans la liste des tâches
description: Vous pouvez utiliser les tâches précédentes (ou simplement les prédécesseurs) pour lier des tâches qui dépendent d’autres tâches à démarrer ou à terminer. Par exemple, vous ne souhaitez pas héberger une partie (tâche dépendante) avant d’envoyer les invitations (tâche prédécesseur).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 14%

---

# Créer une relation d’antériorité dans la liste des tâches

Vous pouvez utiliser les tâches précédentes (ou simplement les prédécesseurs) pour lier des tâches qui dépendent d’autres tâches à démarrer ou à terminer. Par exemple, vous ne souhaitez pas héberger une partie (tâche dépendante) avant d’envoyer les invitations (tâche prédécesseur).

Cet article vous explique comment créer des prédécesseurs sur la liste des tâches.

Vous pouvez afficher les prédécesseurs des tâches dans les zones suivantes d’Adobe Workfront :

* Dans la liste des tâches de la colonne Prédécesseurs .
* Dans le diagramme de Gantt
* Dans la section Prédécesseurs d’une tâche dépendante

Pour plus d’informations, voir [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouvelle : standard </p><p>Actuelle : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux tâches et aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion sur les tâches et le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. Pour plus d’informations sur les exigences d’accès, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Création d’un prédécesseur

1. Accédez à un projet.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. Assurez-vous que la vue actuelle affiche la colonne **Predecessor**.

   Si la vue n’affiche pas la colonne Prédécesseurs, modifiez la vue ou ajoutez la colonne à votre vue.

1. Sélectionnez la tâche que vous souhaitez désigner comme tâche dépendante.
1. Cliquez dans la colonne **Prédécesseurs** .
1. Saisissez le numéro de la tâche que vous souhaitez désigner comme prédécesseur de la tâche sélectionnée, puis appuyez sur **Entrée**.

   >[!TIP]
   >
   >Pour ajouter un prédécesseur multi-projet, procédez comme suit :
   >
   >1. Cliquez sur l’icône **Mode Plan** et sélectionnez **Enregistrement automatique**.
   >
   >1. Saisissez le Numéro de référence du projet du prédécesseur, suivi du signe deux-points et du numéro de la tâche. Par exemple, saisissez : 765021:12. Cela indique que le numéro de référence du projet du prédécesseur est 765021 et que le prédécesseur est la tâche numéro 12 sur le projet.
   >
   >1. Ajoutez le type de dépendance de ce prédécesseur. Pour plus d’informations, voir [Création de prédécesseurs multi-projets](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >Appuyez sur **Entrée**.
   >
   >**IMPORTANT**
   >
   >Vous ne pouvez pas ajouter de prédécesseur de projet croisé lorsque la liste des tâches s’affiche en mode d’enregistrement manuel.

   L’icône de la tâche antérieure devient verte lorsque la tâche antérieure est marquée comme terminée. Cela indique que la tâche dépendante est prête à être exécutée.

   Pour plus d’informations sur les types de relations disponibles dans la colonne Prédécesseurs, voir [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) dans [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Afficher les détails du prédécesseur

Vous pouvez afficher rapidement les détails du prédécesseur dans la liste des tâches.

1. Dans la liste des tâches, passez la souris sur le numéro du prédécesseur dans la colonne **Prédécesseurs**.

   Une zone contenant les détails du prédécesseur s’affiche.

   ![Détails du prédécesseur](assets/predecessor-details-in-task-list.png)

   Les détails suivants s’affichent :

   **Nom du prédécesseur :** nom du prédécesseur référencé. Le numéro de la tâche du prédécesseur est inclus. Cliquez sur le nom de la tâche pour l’ouvrir. Dans l’exemple ci-dessus, le prédécesseur est Production/Exécution/Diffusion.

   **Nom du projet :** nom du projet dans lequel réside le prédécesseur. Le projet est identifié comme le projet en cours si le prédécesseur appartient aux mêmes projets que la tâche, ou comme un projet interprojet, si le prédécesseur appartient à un projet différent. Dans l’exemple ci-dessus, le nom du projet est Production de ressources numériques (intégré) - Projet. Pour plus d’informations sur les prédécesseurs sur plusieurs projets, voir [Création de prédécesseurs sur plusieurs projets](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Vous pouvez développer les détails du projet pour afficher les dates de début et de fin prévues du projet, la condition, l’état, le pourcentage terminé et le propriétaire. Pour un projet interprojet, vous pouvez ensuite cliquer sur **Voir Projet** pour ouvrir le projet.

   **ID :** Numéro de référence du projet dans lequel se trouve le prédécesseur.

   **Début planifié :** Date de début planifiée de la tâche précédente.

   **Fin planifiée :** Date d’achèvement prévue de la tâche précédente.

   **Nombre de prédécesseurs :** Nombre de prédécesseurs pour le prédécesseur référencé. Dans l’exemple ci-dessus, le prédécesseur référencé a 1 prédécesseur.

   **Nombre de successeurs :** Nombre de tâches de successeur (ou dépendantes) pour le prédécesseur référencé. Dans l’exemple ci-dessus, le prédécesseur référencé a 1 successeur.
