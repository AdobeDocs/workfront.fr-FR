---
product-area: projects
navigation-topic: use-predecessors
title: Créer une relation de prédécesseur sur la liste des tâches
description: Vous pouvez utiliser les tâches précédentes (ou simplement les prédécesseurs) pour lier des tâches qui dépendent d’autres tâches à démarrer ou à terminer. Par exemple, vous ne souhaitez pas héberger une partie (tâche dépendante) avant d’envoyer les invitations (tâche prédécesseur).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 420ba180dd0bfd53514c58f77ca9897ba9797320
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Créer une relation de prédécesseur sur la liste des tâches

Vous pouvez utiliser les tâches précédentes (ou simplement les prédécesseurs) pour lier des tâches qui dépendent d’autres tâches à démarrer ou à terminer. Par exemple, vous ne souhaitez pas héberger une partie (tâche dépendante) avant d’envoyer les invitations (tâche prédécesseur).

Cet article vous explique comment créer des prédécesseurs sur la liste des tâches.

Vous pouvez afficher les prédécesseurs des tâches dans les zones suivantes d’Adobe Workfront :

* Dans la liste des tâches de la colonne Prédécesseurs .
* Dans le diagramme de Gantt
* Dans la section Prédécesseurs d’une tâche dépendante

Pour plus d’informations, voir [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations pour les tâches et le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Création d’un prédécesseur

1. Accédez à un projet.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. Assurez-vous que votre vue actuelle affiche la variable **Prédécesseur** colonne .

   Si la vue n’affiche pas la colonne Prédécesseurs, modifiez la vue ou ajoutez la colonne à votre vue.

1. Sélectionnez la tâche que vous souhaitez désigner comme tâche dépendante.
1. Cliquez dans le **Prédécesseurs** colonne .
1. Saisissez le numéro de la tâche que vous souhaitez désigner comme prédécesseur de la tâche sélectionnée, puis appuyez sur **Entrée**.

   L’icône du prédécesseur devient verte lorsque la tâche du prédécesseur est marquée comme terminée. Cela indique que la tâche dépendante est prête pour le travail.

   Pour plus d’informations sur les types de relations disponibles dans la colonne Prédécesseurs, voir [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [Présentation des prédécesseurs de tâches](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Afficher les détails du prédécesseur

Vous pouvez afficher rapidement les détails du prédécesseur dans la liste des tâches.

1. Dans la liste des tâches, passez la souris sur le numéro du prédécesseur de la fonction **Prédécesseurs** colonne .

   Une zone contenant les détails du prédécesseur s’affiche.

   ![Détails du prédécesseur](assets/predecessor-details-in-task-list.png)

   Les détails suivants sont affichés :

   **Nom du prédécesseur :** Nom du prédécesseur référencé. Le numéro de la tâche du prédécesseur est inclus. Cliquez sur le nom de la tâche pour l’ouvrir. Dans l’exemple ci-dessus, le prédécesseur est Production/Exécution/Diffusion.

   **Nom du projet :** Nom du projet dans lequel se trouve le prédécesseur. Le projet est identifié comme le projet en cours si le prédécesseur appartient aux mêmes projets que la tâche, ou comme un projet interprojet, si le prédécesseur appartient à un projet différent. Dans l’exemple ci-dessus, le nom du projet est Production de ressources numériques (intégré) - Projet. Pour plus d’informations sur les prédécesseurs à plusieurs projets, voir [Création de prédécesseurs sur plusieurs projets](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Vous pouvez développer les détails du projet pour afficher les dates de début et de fin prévues du projet, la condition, l’état, le pourcentage terminé et le propriétaire. Pour un projet croisé, vous pouvez ensuite cliquer sur **Voir Projet** pour ouvrir le projet.

   **ID :** Numéro de référence du projet dans lequel se trouve le prédécesseur.

   **Démarrage planifié :** Date de début planifiée de la tâche précédente.

   **Fin planifiée :** Date d’achèvement planifiée de la tâche précédente.

   **Nombre de prédécesseurs :** Nombre de prédécesseurs pour le prédécesseur référencé. Dans l’exemple ci-dessus, le prédécesseur référencé a 1 prédécesseur.

   **Nombre de successeurs :** Nombre de tâches de remplacement (ou dépendantes) pour le prédécesseur référencé. Dans l’exemple ci-dessus, le prédécesseur référencé a 1 successeur.
