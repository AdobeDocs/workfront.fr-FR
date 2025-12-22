---
title: Création et personnalisation de priorités
description: Vous pouvez contrôler les priorités des projets, des tâches et des problèmes dans la zone Configuration de Workfront. Les priorités donnent de l’importance à vos projets, tâches ou problèmes dans Adobe Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 45%

---

# Créer et personnaliser les priorités

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Vous pouvez contrôler les priorités des projets, des tâches et des problèmes dans la zone Configuration de Workfront. Les priorités donnent de l’importance à vos projets, tâches ou problèmes dans Adobe Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Administrateur ou administratrice système</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personnaliser les priorités existantes

En tant qu’administrateur ou administratrice Workfront, vous pouvez apporter les modifications suivantes aux priorités par défaut fournies dans Workfront :

* Renommer les priorités.
* Réorganiser les priorités.

  Pour plus d’informations sur la réorganisation des priorités, voir [Créer une priorité pour un projet, une tâche ou un événement](#create-a-priority-for-a-project-task-or-issue).

* Modifier la priorité par défaut.

  Pour plus d’informations sur la fonctionnalité de modification de la priorité par défaut, voir [Créer une priorité pour un projet, une tâche ou un événement](#create-a-priority-for-a-project-task-or-issue).

* Modifier la description des priorités.
* Définir une couleur pour chaque priorité.

  La couleur de la priorité est utilisée dans les rapports sous forme de graphique, lorsque vous regroupez vos résultats par **Priorité**.

  Pour plus d’informations sur les rapports sous forme de graphique, voir [Ajouter un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Supprimer les priorités.

  Lorsque vous supprimez une priorité existante, vous devez sélectionner une priorité de remplacement.

* Masquer les priorités.

  Pour plus d’informations sur la fonctionnalité de masquage des priorités, voir [Création d’une priorité pour un projet, une tâche ou un événement](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Vous devez avoir au moins une priorité dans votre compte Workfront pour chaque objet.

Les priorités fournies par défaut pour chaque type d’objet (projet, tâche et problème) sont identiques :

* Aucun
* Faible
* Normal
* Élevé
* Urgent

## Créer une priorité pour un projet, une tâche ou un événement {#create-a-priority-for-a-project-task-or-issue}

En plus des priorités par défaut fournies dans Workfront, vous pouvez ajouter vos propres priorités pour refléter les besoins de votre organisation.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Préferences du projet** > **Priorités**.

1. Cliquez sur l’onglet correspondant au type d’objet pour lequel vous souhaitez créer une priorité (**Projet**, **Tâche** ou **Problème**).
1. Cliquez sur **Nouvelle ligne** au bas du tableau.
1. Configurez les options suivantes pour la priorité :

   * **Nom de la priorité** : saisissez un nom pour la priorité.
   * **Importance** : Lors de l’ajout d’une nouvelle priorité, un nombre lui est attribué par défaut. Modifiez ce numéro s’il ne correspond pas à vos besoins.

     Le numéro d’importance de chaque priorité doit être unique. Le numéro de la priorité reflète l&#39;importance du projet, de la tâche ou de l&#39;événement : le numéro le plus élevé correspond à la priorité la plus élevée.

     Vous ne pouvez pas modifier ce nombre après avoir enregistré la priorité.

   * **Couleur** : choisissez une couleur pour la priorité.

     La couleur de la priorité est utilisée dans les rapports sous forme de graphique et dans les paramètres de l’équipe Agile. Pour plus d&#39;informations sur les rapports graphiques, voir [Ajouter un graphique à un rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md). Pour plus d&#39;informations sur les paramètres d&#39;équipe Agile, voir [Créer une équipe Agile](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

   * **Priorité par défaut** : sélectionnez la priorité que Workfront doit appliquer automatiquement à tous les nouveaux projets, tâches ou événements.

     **Normal** est la priorité par défaut pour tous les objets dans Workfront.

     Vous ne pouvez pas définir une priorité masquée comme priorité par défaut.

     La priorité par défaut est indiquée par une icône ![Icône de priorité par défaut](assets/default-icon.png). Pour choisir une nouvelle valeur par défaut, effectuez l’une des opérations suivantes :

      * Cochez la case en regard du nom de la priorité et sélectionnez **Rendre par défaut** dans la barre d’actions située en bas de l’écran.
      * Passez la souris sur le nom de la priorité et cliquez sur le menu **Plus** qui s’affiche. Sélectionnez ensuite **Rendre par défaut**.

        La nouvelle priorité par défaut est étiquetée avec l’icône .

   * **Description** : saisissez une description de la priorité pour expliquer sa fonction.
   * **Masquer le choix** : sélectionnez **Oui** pour masquer une priorité qui n’est plus nécessaire.

     Une priorité masquée ne s’affiche nulle part dans Workfront. Les utilisateurs ne peuvent donc pas la choisir pour leurs projets, tâches ou événements.

     >[!IMPORTANT]
     >
     >Au lieu de supprimer des priorités que vous ne souhaitez plus utiliser, nous vous suggérons de les masquer. De cette façon, vous conservez toutes vos données historiques sur les objets déjà terminés avec la priorité, tout en empêchant les personnes d’utiliser la priorité à l’avenir.

1. (Facultatif) Modifiez l’ordre des listes de vos priorités en les faisant glisser et en les déposant dans l’ordre souhaité.

   Cela modifie l&#39;ordre dans lequel ils s&#39;affichent pour les projets, les tâches ou les événements. Cela ne modifie pas le numéro d’**Importance**.

1. Cliquer sur **Enregistrer**.

Pour savoir comment appliquer des priorités aux projets, aux tâches et aux problèmes, voir les articles suivants :

* [Comprendre et mettre à jour les priorités du projet](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Mettre à jour la priorité de la tâche](../../../manage-work/tasks/task-information/task-priority.md)
* [Mettre à jour la priorité du problème](../../../manage-work/issues/issue-information/update-issue-priority.md)
