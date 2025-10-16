---
product-area: resource-management
keywords: travail,équipe,personnel,ressources
navigation-topic: the-workload-balancer
title: Localiser l’équilibreur de charge de travail
description: L’équilibreur de charge de travail est disponible pour plusieurs projets dans la zone Ressource, pour une équipe, pour un projet et pour un utilisateur.
author: Lisa
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: 18c39c5b1959c31b6fd0018476b48643b4b15021
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 62%

---

# Localiser l’équilibreur de charge de travail

{{preview-fast-release-general}}

Utilisez l’équilibreur de charge de travail pour planifier le travail des ressources ou vérifier leur disponibilité et affectations actuelles.

Vous pouvez accéder à l’équilibreur de charge de travail de différentes façons :

* Dans plusieurs zones prédéfinies par Adobe Workfront
* En l’ajoutant au panneau de gauche sous forme de tableau de bord

Cet article décrit les zones à partir desquelles vous pouvez accéder à l’équilibreur de charge de travail.

>[!NOTE]
>
>Quelle que soit la méthode utilisée pour accéder à l’équilibreur de charge de travail, l’expérience de navigation et de gestion des ressources est identique.
>
>Pour plus d’informations sur l’équilibreur de charge de travail et sur son utilisation pour gérer et planifier le travail de vos ressources, consultez les articles suivants :
>
>* [Vue d’ensemble de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [Parcourir l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [Vue d’ensemble de l’affectation de travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [Gérer les affectations de personnes dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td>
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan, lors de l’utilisation de l’équilibreur de charge de travail dans la zone Ressource ; Travail, lors de l’utilisation de l’équilibreur de charge de travail d’une équipe ou d’un projet</p>
       <p><span class="preview">Remarque : tous les utilisateurs peuvent accéder à l’équilibreur de charge de travail dans leurs propres profils utilisateur, sans aucune exigence de licence.</span></p></td>
  </tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès Affichage ou niveau supérieur aux éléments suivants :</p> 
    <ul> 
     <li>Gestion des ressources</li> 
     <li>Projets</li> 
     <li>Tâches</li> 
     <li>Problèmes</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Autorisations d’affichage ou supérieures aux projets, tâches et problèmes</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Accéder à l’équilibreur de charge de travail dans les zones prédéfinies

Les sections suivantes illustrent les endroits où vous pouvez accéder à l’équilibreur de charge de travail dans Workfront.

### Accéder à l’équilibreur de charge de travail pour plusieurs projets dans la zone Ressources

{{step1-to-resourcing}}

1. Cliquez sur **Équilibreur de charge de travail** dans le panneau de gauche.

   ![Équilibreur de charge de travail](assets/nwe-balancer-global.png)

   L’équilibreur de charge de travail affiche par défaut les informations suivantes dans la zone Ressources :

   * **Travail non affecté** : aucun élément de travail non affecté.
   * **Travail affecté** : toutes les personnes actives du système.

     Il est recommandé d’utiliser des filtres lors de l’affichage des personnes dans la zone Travail affecté. Pour plus d’informations, consultez la section [Filtrer les informations dans l’équilibreur de charge de travail](../workload-balancer/filter-information-workload-balancer.md).

### Accéder à l’équilibreur de charge de travail d’une équipe

Pour plus d’informations sur les équipes dans Workfront, voir [Présentation des équipes](/help/quicksilver/people-teams-and-groups/create-and-manage-teams/teams-overview.md).

{{step1-to-team}}

La page de votre équipe interne s’affiche.

1. Cliquez sur **Équilibreur de charge de travail** dans le panneau de gauche.

   ![Équilibreur de charge de travail pour l’équipe](assets/nwe-balancer-team-350x172.png)

   L’équilibreur de charge de travail d’une équipe affiche par défaut les informations suivantes :

   * **Travail non affecté** : éléments affectés à l’équipe et non affectés aux utilisateurs et utilisatrices.
   * **Travail assigné** : toutes les personnes membres de l’équipe avec toutes leurs affectations.

     >[!TIP]
     >
     >Les personnes membres de l’équipe peuvent être affectées à un travail également attribué à l’équipe ou à un travail affecté à d’autres équipes ou rôles.

### Accéder à l’équilibreur de charge de travail pour un projet

{{step1-to-projects}}

1. Cliquez sur le nom d’un projet pour ouvrir la page du projet.
1. Cliquez sur **Équilibreur de charge de travail** dans le panneau de gauche.

   L’équilibreur de charge de travail pour le projet s’affiche.

   ![Équilibreur de charge de travail pour le projet](assets/nwe-balancer-project-350x152.png)

   L’équilibreur de charge de travail d’un projet affiche les informations suivantes par défaut :

   * **Travail non affecté** : éléments du projet qui sont affectés à des fonctions ou à des équipes et qui ne sont pas affectés aux utilisateurs et aux utilisatrices.
   * **Travail assigné** : utilisateurs et utilisatrices affectés aux éléments du projet.

     >[!TIP]
     >
     >Vous pouvez afficher tous les utilisateurs et utilisatrices du système au lieu d’afficher uniquement ceux du projet (dans la zone de travail attribuée) en activant l’option Afficher tous les utilisateurs et utilisatrices. Pour plus d’informations, voir [Naviguer dans l’équilibreur de charge de travail](../workload-balancer/navigate-the-workload-balancer.md).

<div class="preview">

### Accès à l’équilibreur de charge de travail pour un utilisateur

Tous les utilisateurs ont accès à l’équilibreur de charge de travail sur leurs propres profils. Les données de l’équilibreur de charge de travail d’un utilisateur sont en lecture seule. Vous ne pouvez pas affecter de travail, annuler l’affectation d’un travail ou ajuster les allocations au niveau de l’utilisateur.

Tous les paramètres d’affichage sont disponibles pour l’équilibreur de charge de travail pour un utilisateur ou une utilisatrice. Pour plus d’informations, voir [Naviguer dans l’équilibreur de charge de travail](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

{{step1-click-profile-pic}}

1. Cliquez sur **Équilibreur de charge de travail** dans le panneau de gauche.

   L’équilibreur de charge de travail de l’utilisateur s’affiche.

   ![Équilbreur de charge de travail pour un utilisateur](assets/workload-balancer-user.png)

   L’équilibreur de charge de travail d’un utilisateur affiche les informations suivantes par défaut :

   * **Travail affecté** : tâches et événements affectés à l’utilisateur spécifique.

</div>

## Ajoutez l’équilibreur de charge de travail au panneau de gauche sous forme de tableau de bord

Vous pouvez ajouter l’équilibreur de charge de travail sous forme de tableau de bord au panneau de gauche des objets permettant la personnalisation.

La plupart des personnalisations que vous avez déjà appliquées à l’équilibreur de charge de travail sont conservées lors de son ajout au panneau de gauche.

1. Accédez à l’équilibreur de charge de travail en vous rendant dans l’une des zones suivantes :

   * Zone Ressources
   * Équipe
   * Un projet

1. Obtenez un lien partageable et copiez-le dans le presse-papiers, comme décrit dans [Partager l’équilibreur de charge de travail avec un lien](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
1. Créez un tableau de bord avec une page externe, comme décrit dans [Incorporer une page web externe dans un tableau de bord](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Utilisez le lien partageable obtenu à l’étape 2 pour la page externe.

   <!--
      (NOTE: ensure this stays correct)
      -->

1. Ajoutez un tableau de bord au panneau de navigation de gauche d’un objet, comme décrit dans la section [Ajouter un tableau de bord dans le panneau de gauche d’un objet ou d’une zone Workfront](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) pour placer le tableau de bord sur l’onglet personnalisé.

   Lors de l’accès à l’équilibreur de charge de travail à partir du tableau de bord, vous pouvez l’afficher comme si vous y accédiez directement à partir de l’une de ses zones d’origine répertoriées à l’étape 1.

   <!--
      (NOTE: ensure this stays correct)
     -->

1. (Facultatif) Partagez le tableau de bord dans un modèle de mise en page comme décrit dans [Personnaliser le panneau de gauche à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md) .


<!--
For a team:

* From the Workload Balancer section of a team.

  You can adjust allocations and review or assign work from multiple projects to individual team members.

For a project:

  You can do the following when you use the Workload Balancer within a project:

   * Assign work on the project to users already assigned other work on the project.
   * Assign work to any user that might not be on the project.

   * View additional work that users are assigned to on other projects.
   * Adjust user allocations to work items.-->
