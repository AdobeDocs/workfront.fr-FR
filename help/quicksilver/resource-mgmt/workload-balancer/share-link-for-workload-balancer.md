---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Partager l’équilibreur de charge de travail avec un lien
description: Vous pouvez partager l’équilibreur de charge de travail avec d’autres utilisateurs et utilisatrices qui ne disposent peut-être pas de la zone Ressources. Pour plus d’informations sur l’utilisation de l’équilibreur de charge de travail, voir Naviguer dans l’équilibreur de charge de travail.
author: Lisa
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 58567104d88e7e1363d4196aec8a36ee0566b95a
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 75%

---

# Partager l’équilibreur de charge de travail avec un lien

Vous pouvez partager l’équilibreur de charge de travail avec d’autres utilisateurs pour lesquels la zone Ressource n’est pas disponible dans le menu principal. Pour plus d’informations sur l’utilisation de l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuelle : planification, lors de l’utilisation de l’équilibreur de charge de travail dans la zone Ressource;</br>
       Travail, lors de l’utilisation de l’équilibreur de charge de travail d’une équipe ou d’un projet</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès Affichage ou niveau supérieur aux éléments suivants :</p> 
    <ul> 
     <li>Gestion des ressources</li> 
     <li>Projets</li> 
     <li>Tâches</li> 
     <li>Problèmes</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Autorisations en affichage ou autorisations supérieures pour les projets, les tâches et les problèmes</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informations incluses dans l’équilibreur de charge de travail lors de son affichage à partir d’un lien partagé

Lorsque vous partagez un lien vers l’équilibreur de charge de travail avec d’autres utilisateurs et utilisatrices, les informations suivantes sont incluses avec le lien partagé :

* La zone Travail affectée de l’équilibreur de charge de travail.
* Les informations sur les projets, les tâches ainsi que les utilisateurs et utilisatrices. Cela inclut les informations d’affectation des utilisateurs et utilisatrices.
* Les informations s’affichent en fonction du filtre sélectionné.

  >[!IMPORTANT]
  >
  >Si vous supprimez les filtres après avoir partagé le lien, les utilisateurs et utilisatrices qui visualisent l’équilibreur de charge de travail à partir du lien reçoivent un avertissement les informant que les filtres ont été supprimés. Tous les utilisateurs et utilisatrices dans la zone Travail affecté leur sont visibles. Il s’agit de la vue par défaut de l’équilibreur de charge de travail.

* Le nombre de semaines précédemment sélectionnées.

Les options suivantes sont disponibles pour l’utilisateur ou utilisatrice qui consulte l’équilibreur de charge de travail à partir d’un lien partagé afin de les tenir informés :

* Les sélections de chronologie suivantes :

   * Aujourd’hui
   * Icônes Précédent et Suivant
   * Sélection du calendrier

* Icônes Jour, Semaine et Mois
* Icône Paramètres
* Icône Afficher les affectations

  Pour plus d’informations sur l’utilisation de ces options, voir [Naviguer dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* Icône Afficher les affectations de rôle

  Cette option est disponible uniquement pour l’équilibreur de charge de travail d’un projet.

L’utilisateur ou utilisatrice qui reçoit le lien partagé ne peut pas effectuer les opérations suivantes dans l’équilibreur de charge de travail à partir de ce lien :

* Affecter des éléments de travail aux utilisateurs et utilisatrices
* Gérer des affectations d’utilisateur et utilisatrice
* Créer ou mettre à jour des filtres appliqués initialement

## Accès nécessaire pour afficher les informations dans l’équilibreur de charge de travail à partir d’un lien partagé

Vous avez besoin de l’accès suivant pour afficher les informations dans l’équilibreur de charge de travail à partir d’un lien partagé :

* Une licence Adobe Workfront valide et vous devez vous connecter à Workfront.
* Au moins Afficher l&#39;accès à la gestion des ressources dans votre niveau d&#39;accès. Pour plus d’informations sur l’octroi de l’accès à la gestion des ressources, voir [Accorder l’accès à la gestion des ressources](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* Les autorisations Afficher pour les projets, tâches, problèmes, utilisateurs et utilisatrices affichés dans l’équilibreur de charge de travail.

## Partager l’équilibreur de charge de travail avec d’autres utilisateurs et utilisatrices à partir d’un lien

1. Accéder à l’équilibreur de charge de travail

   Pour plus d’informations sur l’accès à l’équilibreur de charge de travail, voir [Naviguer dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. (Facultatif) Effectuez une ou plusieurs des opérations suivantes :

   * Mettez à jour la sélection de la période.
   * Cliquez sur **Jour, Semaine** ou **Mois** pour afficher des informations quotidiennes, hebdomadaires ou mensuelles.

     ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * Appliquez des filtres aux zones Travail non affecté et Travail affecté.

     Pour plus d’informations sur le filtrage des informations dans l’équilibreur de charge de travail, voir [Filtrer des informations dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. Cliquez sur l’**icône de lien** ![icône de lien](assets/wb-shearable-link-icon-small.png).

   Le lien est alors ajouté à votre presse-papiers.

1. Pour partager le lien avec d’autres personnes, effectuez l’une des opérations suivantes :

   * Collez-le dans un e-mail, un message de chat ou toute autre application, puis partagez-le avec d’autres utilisateurs et utilisatrices.
   * Ajoutez-le à un tableau de bord en tant que page externe, ajoutez le tableau de bord au profil d’un utilisateur ou à un modèle de mise en page, puis partagez le modèle de mise en page avec des utilisateurs, des équipes, des fonctions ou des groupes.

     Pour plus d’informations sur la création d’une page externe, voir [Incorporer une page web externe dans un tableau de bord](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Pour plus d’informations sur l’ajout de tableaux de bord à un modèle de mise en page, voir [Personnaliser le panneau de gauche à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

     >[!IMPORTANT]
     >
     >Lorsque vous ajoutez l’équilibreur de charge de travail sous la forme d’un tableau de bord dans le panneau de gauche d’un objet, les informations de l’équilibreur de charge de travail ne sont pas filtrées par l’objet. L’équilibreur de charge de travail affiche les informations filtrées par les filtres appliqués à l’origine.
