---
content-type: reference
product-area: resource-management
keywords: workload,balancer
navigation-topic: resource-management-overview
title: Obsolescence des outils de planification des ressources dans Adobe Workfront
description: Nous sommes en train de rendre obsolètes tous les outils de planification d’Adobe Workfront et de les remplacer par l’équilibreur de charge de travail.
author: Alina
feature: Resource Management
exl-id: 7fa644cd-cf6a-40f8-ae28-bf222bb45d3f
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Obsolescence des outils de planification des ressources dans Adobe Workfront

>[!IMPORTANT]
>  
><span class="preview">La fonctionnalité de planification décrite dans cet article a été abandonnée et supprimée d’Adobe Workfront à compter de la version 23.1 de janvier 2023.   </span>
>  
> <span class="preview"> Cet article sera également supprimé peu de temps après la version 23.1, début 2023. Pour l’instant, nous vous recommandons de mettre à jour les signets en conséquence. </span>
> 
><span class="preview"> Vous pouvez désormais utiliser l’équilibreur de charge de travail pour planifier le travail de vos ressources. </span>
>  
> <span class="preview">Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir la section [L’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--
We are currently in the process of removing all Scheduling tools from Adobe Workfront and replacing them with the Workload Balancer.

>[!IMPORTANT]
>
>We are no longer implementing new feature functionality for the current Scheduling solution and we no longer consider nor prioritize defects for a fix in this area of Adobe Workfront.

This article describes the timeline for this deprecation and it compares the functionality of the Scheduling tools and that of the Workload Balancer to indicate which Scheduling capabilities are already supported in the Workload Balancer. 

We have been announcing a more exact timeline through the Announcement Center at key milestones during the deprecation process and this article has been updated as this process continues.

>[!NOTE]
>
>The changes described in this article do not affect any other resource management tools. For example, they do not affect the [!UICONTROL Resource Planner] or the [!UICONTROL Utilization] report.
-->

## Comment préparer

Pour plus d’informations sur la préparation de la transition entre la planification et l’équilibreur de charge de travail, voir [Migration de la planification des ressources vers l’équilibreur de charge de travail](../../resource-mgmt/resource-mgmt-overview/migrate-resource-scheduling-to-workload-balancer.md).

Si vous utilisez actuellement des outils de planification, nous vous recommandons de les arrêter et de commencer à utiliser l’équilibreur de charge de travail.

![Zone de planification des ressources globale](assets/resource-scheduler-global-350x127.png)

Presque toutes les fonctionnalités précédemment disponibles dans les zones Planification sont désormais disponibles dans l’équilibreur de charge de travail. Pour plus d’informations, voir la section [Disponibilité des fonctionnalités](#feature-availability) dans cet article. Vous pouvez continuer à planifier vos ressources pour travailler exclusivement dans l’équilibreur de charge de travail.

![Zone globale de l’équilibreur de charge de travail](assets/workload-balancer-pti-350x111.png)

## Informations qui ne seront pas transférées vers l’équilibreur de charge de travail

Les informations suivantes ne seront pas transférées des outils de planification vers l’équilibreur de charge de travail :

* **Affectations quotidiennes pour les utilisateurs**: Vous ne devez pas utiliser simultanément la Planification et l’équilibreur de charge de travail pour ajuster les mêmes affectations utilisateur. Si vous avez géré les affectations d’utilisateurs dans les outils de planification, les affectations quotidiennes ajustées ne sont pas transférées à l’équilibreur de charge de travail. De même, si vous avez ajusté les allocations utilisateur dans l’équilibreur de charge de travail, il ne passe pas aux outils de planification. Nous vous encourageons vivement à vous assurer que les allocations quotidiennes sont exactes dans l’équilibreur de charge de travail pour vous préparer à cette transition. Pour plus d’informations, voir [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../workload-balancer/manage-user-allocations-workload-balancer.md).
* **Filtres**: Si vous avez enregistré des filtres dans les zones Planification , ils ne sont pas transférés vers l’équilibreur de charge de travail. Vous devez recréer les filtres dans l’équilibreur de charge de travail. Pour plus d’informations, voir [Filtrage des informations dans l’équilibreur de charge de travail](../workload-balancer/filter-information-workload-balancer.md).

## Faits saillants de la chronologie d’obsolescence

>[!IMPORTANT]
>
>Consultez cet article pour connaître la dernière frise chronologique de l’obsolescence des outils de planification. Toute mise à jour de cette chronologie sera communiquée dans cet article et dans les messages du centre d’annonce.

Vous trouverez ci-dessous une chronologie du processus d’obsolescence des outils de planification des ressources :

* [Version 2020.4 (novembre 2020)](#2020-4-release-november-2020)
* [Version 2021.4 (octobre 2021)](#2021-4-release-october-2021)
* [Versions 2022.4 - 2023.1 (Octobre 2022 - Janvier 2023)](#2022-4-2023-1-releases)

### Version 2020.4 (novembre 2020) {#2020-4-release-november-2020}

* La nouvelle fonctionnalité n’est plus mise en oeuvre pour la solution de planification.
* Seuls les défauts de gravité graves et graves graves sont prioritaires pour un correctif.
* Nouvelles fonctionnalités d’équilibreur de charge de travail ajoutées à Workfront

### Version 2021.4 (octobre 2021) {#2021-4-release-october-2021}

* L’équilibreur de charge de travail est défini par défaut pour tout nouvel utilisateur de Workfront.
* Filtres améliorés qui peuvent être partagés et inclure des champs supplémentaires

### Versions 2022.4 - 2023.1 (Octobre 2022 - Janvier 2023) {#2022-4-2023-1-releases}

* Aucun problème ne sera prioritaire pour un correctif pendant et après les versions 2022.4 ou 2023.1.
* Toutes les zones de planification sont supprimées de l’environnement de prévisualisation (**20 octobre 2022**)
* Toutes les zones de planification sont supprimées de l’environnement de production (**Janvier 2023**)
* L’équilibreur de charge de travail est le seul outil de planification des ressources disponible dans Workfront (après **Janvier 2023**)

## Disponibilité des fonctionnalités {#feature-availability}

Sauf indication contraire, toutes les fonctions de planification des ressources ont été ou seront disponibles dans l’équilibreur de charge de travail. Pour plus d’informations sur l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Outre les fonctionnalités existantes, l’équilibreur de charge de travail dispose ou aura de nouvelles fonctionnalités qui n’existaient pas dans les outils de planification des ressources, comme illustré dans le tableau suivant :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td rowspan="2"><span style="font-weight: normal;"><b>Fonctionnalités</b></span> </td> 
   <td rowspan="2"> <b>Disponibilité des fonctionnalités des outils de planification des ressources</b></td> 
   <td colspan="3"><b>Disponibilité des fonctionnalités de l’équilibreur de charge de travail</b></td> 
  </tr> 
  <tr> 
   <td><b>Disponible maintenant</b></td> 
   <td><b>Disponible bientôt</b></td> 
   <td><b>Non planifié</b></td> 
  </tr> 
  <tr> 
   <td> <p>Accès à l’outil à partir de la zone Ressource</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Zones distinctes pour les tâches non assignées et affectées</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Application et création de filtres pour les tâches non assignées et affectées</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Accès direct aux tâches à partir de l’outil</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Affectation ou annulation manuelle de tâches et de problèmes</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ajuster les allocations individuelles</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Inclure le temps de problème</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher les dates prévues </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher le travail terminé</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher les exceptions de temps d’arrêt, de week-end et de planification de l’utilisateur</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Affectez rapidement des utilisateurs en fonction de rôles*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Remplacement rapide des utilisateurs*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Annulation rapide de l’affectation des utilisateurs*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Accès à l’outil à partir d’une équipe</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Accès à l’outil à partir d’un projet</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr>
   <td>Les utilisateurs de licences de travail peuvent ajuster les affectations utilisateur lors de l’accès à l’équilibreur de charge de travail à partir d’un projet. </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td>Problèmes d’affichage dans la zone de travail non assignée</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td><span>Attribuer et annuler l’affectation de tâches et de problèmes en les faisant glisser et en les déposant*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visible par tous les utilisateurs du plan, sans avoir été désigné gestionnaire de ressources sur le projet.</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Informations de groupe par projet</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Partager l’équilibreur de charge de travail avec les utilisateurs n’ayant pas d’accès à la zone Ressource</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher et ajuster les allocations par semaine</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Accès direct des utilisateurs à partir de l’outil</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Accédez à plus d’informations sur les tâches sans quitter le panneau Résumé*</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher et ajuster l’affectation en tant que valeur de pourcentage </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher la différence entre le temps disponible et le temps alloué</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher la disponibilité des utilisateurs dans un graphique</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Éléments de travail et projets de code-couleur par état de projet</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mettre à jour automatiquement les heures planifiées lorsque vous ajustez l’affectation des utilisateurs (pour les tâches avec un type de durée simple)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Suggérer des affectations en fonction du modèle d’affectation de l’utilisateur, des affectations de rôle ou d’équipe existantes</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filtres améliorés qui peuvent être partagés et inclure des champs supplémentaires</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Effectuer des affectations avancées</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr>

<tr> 
   <td><span>Éléments de travail avec code couleur par projet et état du projet</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td>

<tr> 
   <td>Ajoutez des utilisateurs à l’équipe du projet (déplacée vers le <b>Personnes</b> onglet du projet) </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td> </td>

</tr>
   <tr> 
   <td>Affecter automatiquement des tâches et des problèmes</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr>

</tbody> 
</table>

*Ces fonctionnalités ne sont disponibles que dans la nouvelle expérience Adobe Workfront.
