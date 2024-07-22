---
product-area: projects
navigation-topic: use-predecessors
title: Créer les projets transversaux antérieurs
description: Une tâche antérieure multi-projet est une tâche dont dépend une autre tâche (appelée tâche ultérieure) dans un autre projet. La tâche antérieure a la priorité sur la tâche dépendante (ultérieure). Par exemple, vous pouvez créer une dépendance qui nécessite que la tâche antérieure soit marquée comme Terminé avant que la tâche dépendante ne puisse commencer.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 96%

---

# Créer les projets transversaux antérieurs

<!--Audited: 12/2023-->

Une tâche antérieure multi-projet est une tâche dont dépend une autre tâche (appelée tâche ultérieure) dans un autre projet. La tâche antérieure a la priorité sur la tâche dépendante (ultérieure). Par exemple, vous pouvez créer une dépendance qui nécessite que la tâche antérieure soit marquée comme Terminé avant que la tâche dépendante ne puisse commencer.

Adobe Workfront permet aux tâches de dépendre des tâches d’autres projets, tout comme les tâches antérieures sont autorisées dans un seul projet.

>[!INFO]
>
>Par exemple, une entreprise d’excavation n’a qu’une seule pelleteuse et deux projets ont des tâches qui nécessitent l’utilisation de la pelleteuse. La personne en charge du projet peut définir la tâche du premier projet comme une tâche antérieure à la tâche du deuxième projet. Cela montre que le deuxième projet peut commencer à utiliser la pelleteuse lorsque le premier projet est terminé.

Lors de la liaison de projets par le biais de tâches antérieures multi-projets, les dates du projet principal (celui qui a la tâche antérieure) auront un impact sur le projet secondaire (celui qui a la tâche ultérieure).

>[!TIP]
>
>Vous devez recalculer les chronologies des projets afin d’afficher les dates mises à jour pour le projet secondaire. Pour plus d’informations sur le nouveau calcul des chronologies, voir [Configurer des nouveaux calculs de chronologie pour les projets](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Pour plus d’informations sur les relations des tâches antérieures, voir [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td> <p>Nouvelle : standard </p> 
   Ou
   <p>Actuelle : formule </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Accès en modification aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations pour les tâches et les projets</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations sur les informations contenues dans ce tableau, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une tâche antérieure multi-projets

1. Accédez à votre tâche ultérieure (tâche dépendante).
1. Cliquez sur **Tâches antérieures** dans le panneau de gauche.
1. Cliquez sur **Ajouter une tâche antérieure**.
1. Dans le champ **Projet parent**, commencez à saisir le nom du projet qui contient la tâche antérieure à la tâche en cours.
1. Cliquez sur le nom qui apparaîtra dans la liste déroulante.
1. Dans le champ **Tâche**, commencez à saisir le nom de la tâche antérieure à la tâche en cours.
1. Indiquez les informations suivantes pour définir la relation entre la tâche antérieure et la tâche dépendante :

   * **Type de dépendance :** sélectionnez la relation que vous souhaitez que la tâche antérieure ait avec la tâche dépendante. La relation par défaut est « Terminer-Démarrer », ce qui signifie que la tâche antérieure doit se terminer avant que la tâche dépendante ne puisse commencer. Pour plus d’informations sur les différents types de dépendance, voir [Vue d’ensemble des types de dépendance des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * **Décalage :** spécifiez le temps qui doit s’écouler entre la fin d’une tâche antérieure appliquée et le début de la tâche dépendante. Pour plus d’informations sur les différents types de décalage, voir [Vue d’ensemble des types de décalage](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Appliqué :** lorsque cette option est sélectionnée, la relation de dépendance entre les deux tâches ne peut pas être contournée par les personnes qui commencent les tâches tôt. Par exemple, si vous appliquez une relation entre la tâche A et la tâche B, la tâche B ne peut pas être lancée tant que la tâche A n’est pas terminée. Pour plus d’informations sur l’application des tâches antérieures, voir [Applquer les tâches antérieures](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Lorsque cette option n’est pas sélectionnée, la dépendance est traitée comme une suggestion aux personnes. Par exemple, les personnes peuvent démarrer la tâche B avant que la tâche A ne soit terminée.

1. Cliquer sur **Enregistrer**.

   Les tâches qui ont une tâche antérieure multi-projets affichent le numéro de référence du projet auquel appartient la tâche antérieure et le numéro de la tâche, séparé par un signe deux-points, dans la colonne Tâches antérieures d’une liste de tâches.

   ![Tâche antérieure multi-projets](assets/cross-project-predecessor-in-list-view.png)

   L’icône de la tâche antérieure devient verte lorsque la tâche antérieure est marquée comme terminée. Cela indique que la tâche dépendante est prête à être exécutée.

   Pointez sur cette valeur pour obtenir plus d’informations sur la tâche antérieure, le projet et les dates. Cliquez sur la tâche antérieure multi-projets dans la zone Détails pour ouvrir la tâche.

   Cliquez près de la partie supérieure de la fenêtre de survol pour afficher plus d’informations sur le projet de la tâche antérieure.

   Cliquez sur **Voir Projet** pour ouvrir le projet de la tâche antérieure.

   ![Détails de la tâche antérieure multi-projets](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   L’option **Voir Projet** s’affiche uniquement lors de l’affichage d’une tâche antérieure multi-projets.

