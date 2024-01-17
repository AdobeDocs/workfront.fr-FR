---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Partage de l’équilibreur de charge de travail avec un lien
description: Vous pouvez partager l’équilibreur de charge de travail avec d’autres utilisateurs qui ne disposent peut-être pas de la zone Ressource . Pour plus d’informations sur l’utilisation de l’équilibreur de charge de travail, voir Navigation dans l’équilibreur de charge de travail.
author: Lisa
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---

# Partage de l’équilibreur de charge de travail avec un lien

Vous pouvez partager l’équilibreur de charge de travail avec d’autres utilisateurs qui ne disposent peut-être pas de la zone Ressource . Pour plus d’informations sur l’utilisation de l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>N’importe quel plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Planifiez l’utilisation de l’équilibreur de charge de travail dans la zone Ressource .</p>
   <p>Fonctionnement lors de l’utilisation de l’équilibreur de charge de travail d’une équipe ou d’un projet</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Visualisez ou affichez un accès supérieur aux éléments suivants :</p> 
    <ul> 
     <li> <p>Gestion des ressources</p> </li> 
     <li> <p>Projets</p> </li> 
     <li> <p>Tâches</p> </li> 
     <li> <p>Problèmes</p> </li> 
    </ul> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher ou des autorisations supérieures pour les projets, les tâches et les problèmes </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Informations incluses dans l’équilibreur de charge de travail lors de son affichage à partir d’un lien partagé

Lorsque vous partagez un lien avec l’équilibreur de charge de travail avec d’autres utilisateurs, les informations suivantes sont incluses avec le lien partagé :

* La zone de travail affectée de l’équilibreur de charge de travail.
* Projet, tâche, informations sur l’utilisateur. Cela inclut les informations d’affectation des utilisateurs.
* Les informations s’affichent en fonction du filtre sélectionné.

  >[!IMPORTANT]
  >
  >Si vous supprimez les filtres après avoir partagé le lien, les utilisateurs qui visualisent l’équilibreur de charge de travail à partir du lien reçoivent un avertissement les informant que les filtres ont été supprimés. Ils affichent tous les utilisateurs dans la zone de travail affectée. Il s’agit de la vue par défaut de l’équilibreur de charge de travail.

* Nombre de semaines précédemment sélectionnées.

Les options suivantes sont disponibles pour l’utilisateur qui consulte l’équilibreur de charge de travail à partir d’un lien partagé afin de se mettre à jour :

* Sélections de chronologie suivantes :

   * Aujourd’hui
   * Icônes Précédent et Suivant
   * Sélection du calendrier

* Icônes Jour, Semaine et Mois
* Icône Paramètres
* Icône Afficher les allocations

  Pour plus d’informations sur l’utilisation de ces options, voir [Navigation dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* Icône Afficher les affectations de rôle

  Cette option est disponible uniquement pour l’équilibreur de charge de travail d’un projet.

L’utilisateur qui reçoit le lien partagé ne peut pas effectuer les opérations suivantes dans l’équilibreur de charge de travail à partir de ce lien :

* Affectation d’éléments de travail aux utilisateurs
* Gestion des affectations utilisateur
* Créer ou mettre à jour des filtres appliqués initialement

## Accès nécessaire pour afficher les informations dans l’équilibreur de charge de travail à partir d’un lien partagé

Vous avez besoin de l’accès suivant pour afficher les informations dans l’équilibreur de charge de travail à partir d’un lien partagé :

* Une licence Adobe Workfront valide et vous devez être connecté à Workfront.
* Au moins, affichez l’accès à la gestion des ressources dans votre niveau d’accès. Pour plus d’informations sur l’octroi de l’accès à Resource Management, voir [Accorder l’accès à la gestion des ressources](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* Afficher les autorisations pour les projets, tâches, problèmes et utilisateurs affichés dans l’équilibreur de charge de travail.

## Partage de l’équilibreur de charge de travail avec d’autres utilisateurs à partir d’un lien

1. Accédez à l’équilibreur de charge de travail

   Pour plus d’informations sur l’accès à l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. (Facultatif) Effectuez une ou plusieurs des opérations suivantes :

   * Mettez à jour la sélection de la période.
   * Cliquez sur **Jour, semaine**, ou **Mois** pour afficher des informations quotidiennes, hebdomadaires ou mensuelles.

     ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * Appliquez des filtres aux zones de travail non assigné et attribué.

     Pour plus d’informations sur le filtrage des informations dans l’équilibreur de charge de travail, voir [Filtrage des informations dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. Cliquez sur le bouton **icône de lien** ![](assets/wb-shearable-link-icon-small.png).

   Le lien est alors ajouté à votre presse-papiers.

1. Pour partager le lien avec d’autres personnes, effectuez l’une des opérations suivantes :

   * Collez-le dans un e-mail, un message de conversation ou toute autre application et partagez-la avec d’autres utilisateurs.
   * Ajoutez-le à une section personnalisée en tant que page externe, ajoutez-la à un profil d’utilisateur ou à un modèle de mise en page, puis partagez le modèle de mise en page avec des utilisateurs, des équipes, des rôles de tâche ou des groupes.

     Pour plus d’informations sur la création d’une page externe, voir [Incorporation d’une page web externe dans un tableau de bord](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Pour plus d’informations sur l’ajout de sections personnalisées à un modèle de mise en page, voir [Personnalisation du panneau de gauche à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

     >[!IMPORTANT]
     >
     >Lorsque vous ajoutez l’équilibreur de charge de travail à la section personnalisée d’un objet, les informations de l’équilibreur de charge de travail ne sont pas filtrées par l’objet . L’équilibreur de charge de travail affiche les informations filtrées par les filtres appliqués initialement.
