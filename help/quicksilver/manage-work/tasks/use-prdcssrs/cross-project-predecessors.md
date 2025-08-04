---
product-area: projects
navigation-topic: use-predecessors
title: Créer des projets transversaux antérieurs
description: Un projet transversal antérieur est une tâche dont dépend une autre tâche (appelée tâche ultérieure) dans un autre projet. La tâche antérieure est la tâche qui a la priorité sur la tâche dépendante (tâche ultérieure). Par exemple, vous pouvez créer une dépendance qui exige que la tâche antérieure soit marquée comme étant terminée avant que la tâche dépendante ne puisse démarrer.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 94%

---

# Créer les projets transversaux antérieurs

<!--Audited: 12/2024-->

Un projet transversal antérieur est une tâche dont dépend une autre tâche (appelée tâche ultérieure) dans un autre projet. La tâche antérieure est la tâche qui a la priorité sur la tâche dépendante (tâche ultérieure). Par exemple, vous pouvez créer une dépendance qui exige que la tâche antérieure soit marquée comme étant terminée avant que la tâche dépendante ne puisse démarrer.

Adobe Workfront permet aux tâches de dépendre de tâches d’autres projets, tout comme il permet la présence de tâches antérieures dans un même projet.

>[!INFO]
>
>Par exemple, une entreprise d’excavation ne possède qu’une seule pelleteuse, et deux projets comportent des tâches nécessitant l’utilisation de la pelleteuse. La personne chargée de la gestion de projets peut définir la tâche du premier projet comme étant une tâche antérieure à celle du second projet. Cela indique que le deuxième projet pourra commencer à utiliser la pelleteuse lorsque le premier projet ne l’utilisera plus.

Lorsque des projets sont liés par des projets transversaux antérieurs, les dates du projet principal (celui qui comporte la tâche antérieure) auront un impact sur le projet secondaire (celui qui comporte la tâche ultérieure).

>[!TIP]
>
>Vous devez recalculer la chronologie des projets afin de visualiser les dates mises à jour du projet secondaire. Pour plus d’informations sur le recalcul des chronologies, consultez la section [Configurer le recalcul de la chronologie des projets](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Pour plus d’informations sur les relations entre les tâches antérieures, consultez la section [Vue d’ensemble des tâches antérieures](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

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
   <td> <p>Standard </p>

<p>Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion pour les tâches et les projets</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un projet transversal antérieur

>[!TIP]
>
>Bien que la création de prédécesseurs de tâches de modèle soit similaire à la création de prédécesseurs de tâches de projet, vous ne pouvez pas créer de prédécesseurs intermodèles pour les tâches de modèle.


1. Accédez à la tâche qui sera votre tâche ultérieure (tâche dépendante).
1. Cliquez sur **Tâches antérieures** dans le panneau de gauche.

   >[!TIP]
   >
   >   Votre administrateur Workfront ou de groupe peut supprimer la section **Prédécesseurs** ou d’autres sections du panneau de gauche.

1. Cliquez sur **Ajouter antérieur.**
1. Dans le champ **Projet parent**, commencez à saisir le nom du projet qui contient la tâche que vous voulez définir comme étant la tâche antérieure de votre tâche actuelle.
1. Cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.
1. Dans le champ **Tâches**, commencez à saisir le nom de la tâche que vous voulez définir comme étant la tâche antérieure de votre tâche actuelle.
1. Spécifiez les informations suivantes pour définir la relation entre la tâche antérieure et la tâche dépendante :


   * **Type de dépendance :** sélectionnez la relation entre la tâche antérieure et la tâche dépendante. La relation par défaut est « Terminer-Démarrer », ce qui signifie que la tâche antérieure doit se terminer avant que la tâche dépendante ne puisse commencer. Pour plus d’informations sur les différents types de dépendance, voir [Vue d’ensemble des types de dépendance des tâches](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * **Décalage :** spécifiez le temps qui doit s’écouler entre la fin d’une tâche antérieure appliquée et le début de la tâche dépendante. Pour plus d’informations sur les différents types de décalage, consultez la section [Vue d’ensemble des types de décalage](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Forcée :** lorsque cette option est sélectionnée, la relation de dépendance entre les deux tâches ne peut être contournée par les personnes qui commencent les tâches plus tôt. Par exemple, si vous appliquez une relation entre la tâche A et la tâche B, la tâche B ne peut être lancée tant que la tâche A n’est pas terminée. Pour plus d’informations sur l’application des tâches antérieures, consultez la section [Appliquer les tâches antérieures](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Lorsque cette option n’est pas sélectionnée, la relation de dépendance est suggérée aux utilisateurs et utilisatrices. Par exemple, il leur est possible de démarrer la tâche B avant que la tâche A ne soit terminée.

1. Cliquer sur **Enregistrer**.

   Les tâches qui comportent un projet transversal antérieur affichent le numéro de référence du projet auquel appartiennent les tâches antérieures, ainsi que le numéro de la tâche, séparés par deux points, dans la colonne Tâches antérieures d’une liste de tâches.

   ![Projet transversal anterieur](assets/cross-project-predecessor-in-list-view.png)

   L’icône de la tâche antérieure devient verte lorsque la tâche antérieure est marquée comme terminée. Cela indique que la tâche dépendante est prête à être exécutée.

   Pointez sur cette valeur pour obtenir plus d’informations sur la tâche antérieure, le projet et les dates. Cliquez sur le projet transversal antérieur dans la zone de détails pour ouvrir la tâche.

   Cliquez en haut de la fenêtre de pointage pour obtenir plus d’informations sur le projet de la tâche antérieure.

   Cliquez sur **Afficher le projet** pour ouvrir le projet de la tâche antérieure.

   ![Détails du projet transversal antérieur](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   L’option **Afficher le projet** ne s’affiche que lors de la visualisation d’un projet transversal antérieur.

