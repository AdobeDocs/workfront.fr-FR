---
title: Créer et personnaliser les priorités
description: Vous pouvez contrôler les priorités des projets, des tâches et des problèmes dans la zone Configuration de Workfront. Les priorités accordent de l’importance à vos projets, tâches ou problèmes dans Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 15%

---

# Créer et personnaliser les priorités

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Vous pouvez contrôler les priorités des projets, des tâches et des problèmes dans la zone Configuration de Workfront. Les priorités accordent de l’importance à vos projets, tâches ou problèmes dans Adobe Workfront.

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
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnalisation des priorités existantes

En tant qu’administrateur Workfront, vous pouvez apporter les modifications suivantes aux priorités par défaut fournies dans Workfront :

* Renommez les priorités.
* Réorganisez les priorités.

  Pour plus d’informations sur la façon de réorganiser les priorités, voir [Création d’une priorité pour une tâche de projet, ou problème](#create-a-priority-for-a-project-task-or-issue).

* Modifiez la priorité par défaut.

  Pour plus d’informations sur la fonctionnalité de modification de la priorité par défaut, voir [Création d’une priorité pour une tâche de projet, ou problème](#create-a-priority-for-a-project-task-or-issue).

* Modifiez la description des priorités.
* Définissez une couleur pour chaque priorité.

  La couleur de la priorité est utilisée dans les rapports graphiques lorsque vous regroupez vos résultats par **Priorité**.

  Pour plus d’informations sur les rapports de graphique, voir [Ajout d’un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Supprimer les priorités.

  Lorsque vous supprimez une priorité existante, vous devez la sélectionner.

* Masquer les priorités.

  Pour plus d’informations sur la fonctionnalité de masquage des priorités, voir [Création d’une priorité pour une tâche de projet ou problème](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >Vous devez avoir au moins une priorité dans votre compte Workfront pour chaque objet.

Les priorités fournies par défaut pour chaque type d’objet (projet, tâche et problème) sont identiques :

* Aucun
* Faible
* Normal
* Élevé
* Urgent

## Création d’une priorité pour une tâche de projet ou un problème {#create-a-priority-for-a-project-task-or-issue}

Outre les priorités par défaut fournies dans Workfront, vous pouvez ajouter vos propres priorités afin de tenir compte des besoins de votre organisation.

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Préférences du projet** > **Priorités**.

1. Cliquez sur l’onglet correspondant au type d’objet pour lequel vous souhaitez créer une priorité (**Projet**, **Tâche** ou **Problème**).
1. Cliquez sur **Ajouter une nouvelle priorité**.
1. Indiquez les informations suivantes pour la nouvelle priorité :

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
      <td> <p>Lors de l’ajout d’une nouvelle priorité, un nombre lui est attribué par défaut. Modifiez ce nombre s’il ne correspond pas à vos besoins.</p> <p>Le nombre <strong>Importance</strong> pour chaque priorité doit être unique pour l’objet que vous avez sélectionné.<br>Le nombre de priorités reflète l'importance du projet, de la tâche ou du problème : le nombre le plus élevé correspond à la priorité la plus élevée.</p> <p><b>REMARQUE</b> : vous ne pouvez pas modifier le numéro d’importance après avoir enregistré la priorité. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Couleur</td> 
      <td> <p>Choisissez une couleur pour votre priorité.</p> <p>La couleur de la priorité est utilisée dans les rapports graphiques et dans les paramètres d’équipe agile. Pour plus d’informations sur les rapports de graphique, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Ajout d’un graphique à un rapport</a>.</p> <p>Pour plus d’informations sur les paramètres d’équipe mobile, voir dans .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorité par défaut</td> 
      <td> <p>Choisissez s’il doit s’agir d’une priorité par défaut, en sélectionnant le bouton radio.</p> <p>Si une priorité est désignée comme <strong>Priorité par défaut</strong>, elle est automatiquement sélectionnée pour tous les projets, tâches ou problèmes dans Workfront. <strong>Normal</strong> est la priorité par défaut de tous les objets dans Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Ajoutez une description de votre priorité pour expliquer sa fonction.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Masquer</td> 
      <td> <p>Cochez cette case si vous souhaitez masquer la priorité.</p><p>Lorsque vous sélectionnez l’option <b>Masquer</b>, la priorité ne s’affiche nulle part dans Workfront et les utilisateurs ne sont pas en mesure de la choisir pour leurs projets, tâches et problèmes.</p> 
      <p><b>IMPORTANT</b> : nous vous recommandons de masquer les priorités que vous ne souhaitez plus utiliser plutôt que de les supprimer. En les cachant, vous conservez toujours toutes vos données historiques, des objets qui ont été remplis avec cette priorité, tout en empêchant les gens de choisir cette priorité à l'avenir. </p>
      <p>Vous pouvez éventuellement modifier l’ordre de liste de vos priorités en les faisant glisser et en les déposant dans l’ordre souhaité. Cela modifie l’ordre dans lequel ils s’affichent pour les projets, les tâches et les problèmes. Cela ne modifie pas le nombre <b>Importance</b>. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

Pour obtenir des instructions sur l’application des priorités aux projets, tâches et problématiques, reportez-vous aux articles suivants :

* [Comprendre et mettre à jour les priorités de projet](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Mise à jour de la priorité des tâches](../../../manage-work/tasks/task-information/task-priority.md)
* [Mettre à jour la priorité du problème](../../../manage-work/issues/issue-information/update-issue-priority.md)
