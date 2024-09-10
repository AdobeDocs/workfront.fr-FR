---
title: Création et personnalisation des priorités
description: Vous pouvez contrôler les priorités des projets, des tâches et des problèmes dans la zone Configuration de Workfront. Les priorités donnent de l’importance à vos projets, tâches ou problèmes dans Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 99%

---

# Créer et personnaliser les priorités

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Vous pouvez contrôler les priorités des projets, des tâches et des problèmes dans la zone Configuration de Workfront. Les priorités donnent de l’importance à vos projets, tâches ou problèmes dans Adobe Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
     <p>Nouveau : Standard</p>
     <p>ou</p>
     <p>Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personnaliser les priorités existantes

En tant qu’administrateur ou administratrice Workfront, vous pouvez apporter les modifications suivantes aux priorités par défaut fournies dans Workfront :

* Renommer les priorités.
* Réorganiser les priorités.

  Pour plus d’informations sur la réorganisation des priorités, voir [Créer une priorité pour un projet, une tâche ou un problème](#create-a-priority-for-a-project-task-or-issue).

* Modifier la priorité par défaut.

  Pour plus d’informations sur la fonctionnalité de modification de la priorité par défaut, voir [Créer une priorité pour un projet, une tâche ou un problème](#create-a-priority-for-a-project-task-or-issue).

* Modifier la description des priorités.
* Définir une couleur pour chaque priorité.

  La couleur de la priorité est utilisée dans les rapports sous forme de graphique, lorsque vous regroupez vos résultats par **Priorité**.

  Pour plus d’informations sur les rapports sous forme de graphique, voir [Ajouter un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Supprimer les priorités.

  Lorsque vous supprimez une priorité existante, vous devez sélectionner une priorité de remplacement.

* Masquer les priorités.

  Pour plus d’informations sur la fonctionnalité de masquage des priorités, voir [Créer une priorité pour un projet, une tâche ou un problème](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Vous devez avoir au moins une priorité dans votre compte Workfront pour chaque objet.

Les priorités fournies par défaut pour chaque type d’objet (projet, tâche et problème) sont identiques :

* Aucun
* Faible
* Normal
* Élevé
* Urgent

## Créer une priorité pour un projet, une tâche ou un problème {#create-a-priority-for-a-project-task-or-issue}

En plus des priorités par défaut fournies dans Workfront, vous pouvez ajouter vos propres priorités pour refléter les besoins de votre organisation.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Préferences du projet** > **Priorités**.

1. Cliquez sur l’onglet correspondant au type d’objet pour lequel vous souhaitez créer une priorité (**Projet**, **Tâche** ou **Problème**).
1. Cliquez sur **Ajouter une nouvelle priorité**.
1. Spécifiez les informations suivantes pour la nouvelle priorité :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom de la priorité</td> 
      <td>Saisissez le nom de votre priorité.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Importance</td> 
      <td> <p>Lors de l’ajout d’une nouvelle priorité, un numéro lui est attribué par défaut. Modifiez ce numéro s’il ne correspond pas à vos besoins.</p> <p>Le numéro d’<strong>importance</strong> de chaque priorité doit être unique pour l’objet que vous avez sélectionné.<br>Le numéro de la priorité reflète l’importance du projet, de la tâche ou du problème : le numéro le plus élevé correspond à la plus haute priorité.</p> <p><b>NOTE</b> : vous ne pouvez pas modifier le numéro d’importance après avoir enregistré la priorité. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Couleur</td> 
      <td> <p>Choisissez une couleur pour votre priorité.</p> <p>La couleur de la priorité est utilisée dans les rapports sous forme de graphique et dans les paramètres de l’équipe Agile. Pour plus d’informations sur les rapports sous forme de graphique, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Ajouter un graphique à un rapport</a>.</p> <p>Pour plus d’informations sur les paramètres de l’équipe Agile, voir dans .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorité par défaut</td> 
      <td> <p>Décidez s’il s’agit d’une priorité par défaut ou non, en sélectionnant la case d’option.</p> <p>Si une priorité est désignée comme la <strong>priorité par défaut</strong>, elle est automatiquement choisie pour tous les projets, tâches ou problèmes dans Workfront. <strong>Normal</strong> est la priorité par défaut pour tous les objets dans Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Ajoutez une description de votre priorité pour expliquer sa fonction.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Masquer</td> 
      <td> <p>Cochez cette case si vous souhaitez masquer la priorité.</p><p>Lorsque vous sélectionnez l’option <b>Masquer</b>, la priorité ne s’affiche nulle part dans Workfront et les utilisateurs et utilisatrices ne peuvent pas la choisir pour leurs projets, tâches et problèmes.</p> 
      <p><b>IMPORTANT</b> : nous vous recommandons de masquer les priorités que vous ne souhaitez plus utiliser, plutôt que de les supprimer. En les masquant, vous conservez toutes vos données historiques et celles des objets qui ont été achevés avec cette priorité, tout en empêchant d’autres personnes de choisir cette priorité à l’avenir. </p>
      <p>Vous pouvez éventuellement modifier l’ordre de liste de vos priorités en les faisant glisser et en les déposant dans l’ordre souhaité. Cette fonction modifie l’ordre dans lequel elles sont affichées pour les projets, les tâches et les problèmes. Cela ne modifie pas le numéro d’<b>importance</b>. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

Pour savoir comment appliquer des priorités aux projets, aux tâches et aux problèmes, voir les articles suivants :

* [Comprendre et mettre à jour les priorités du projet](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Mettre à jour la priorité de la tâche](../../../manage-work/tasks/task-information/task-priority.md)
* [Mettre à jour la priorité du problème](../../../manage-work/issues/issue-information/update-issue-priority.md)
