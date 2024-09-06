---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Annulation de l’affectation du travail dans l’équilibreur de charge de travail
description: Vous pouvez annuler l’affectation de personnes à des tâches dans la zone de travail affecté de l’équilibreur de charge de travail Adobe Workfront ou réaffecter ces tâches à d’autres personnes, rôles ou équipes.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 196d0aa4ed67cf564c823625515ef49d811e0e06
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 93%

---

# Annuler l’affectation de travaux dans l’équilibreur de charge de travail

Vous pouvez annuler l’affectation de personnes à des tâches dans la zone de travail affecté de l’équilibreur de charge de travail Adobe Workfront ou réaffecter ces tâches à d’autres personnes, rôles ou équipes.

Vous pouvez manuellement annuler l’affectation de tâches à des personnes en les faisant glisser et en les déposant, ou en bloc. Cet article décrit comment annuler manuellement l’affectation d’utilisateurs et utilisatrices.

Pour plus d’informations sur l’annulation de l’affectation des personnes par glisser-déposer, voir [Affecter un travail dans l’équilibreur de charge de travail en le faisant glisser et en le déposant](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Pour plus d’informations sur l’annulation de l’affectation de personnes en bloc, voir [Affecter du travail en bloc à l’aide de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

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
       <p>Actuel : planifiez, lors de l’utilisation de l’équilibreur de charge de travail dans la zone Ressource ;</br>
       Fonctionnement lors de l’utilisation de l’équilibreur de charge de travail d’une équipe ou d’un projet</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifiez l’accès aux éléments suivants :</p> 
    <ul> 
     <li>Gestion des ressources</li> 
     <li>Projets</li> 
     <li>Tâches</li> 
     <li>Problèmes</li> 
    </ul></td>
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Autorisations Contribuer ou supérieures aux projets, tâches et problèmes qui incluent la création d’affectations.</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Annuler l’affectation d’éléments de travail dans l’équilibreur de charge de travail

Vous pouvez soit annuler l’affectation d’éléments à des personnes et les déplacer vers la zone de travail non affecté, soit les réaffecter à d’autres personnes.

Pour annuler l’affectation d’éléments de travail à des personnes :

1. Dans l’équilibreur de charge de travail, accédez à la zone de **Travail affecté** et développez un utilisateur ou une utilisatrice.
1. Utilisez l’une des méthodes suivantes :

   * Recherchez l’élément dont vous souhaitez annuler l’affectation dans la zone d’un utilisateur ou d’une utilisatrice, cliquez dessus, puis faites-le glisser et déposez-le dans la zone Non affecté ou dans la zone d’un autre utilisateur ou d’une autre utilisatrice.
   * Cliquez sur l’icône **Plus** ![](assets/more-icon-task-list.png) à droite du nom d’un élément de travail, cliquez sur **Affecter ceci à**, supprimez ensuite le nom des entités affectées à l’élément de travail ou saisissez un autre nom, puis cliquez sur **Enregistrer**.

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   L’élément s’affiche dans la zone de travail non affecté s’il correspond aux critères de filtrage de cette zone et qu’il n’est affecté à aucune autre personne, ou s’il s’affiche dans la zone de l’utilisateur ou de l’utilisatrice s’il est affecté à une autre personne.

   Pour plus d’informations sur le filtrage des informations dans l’équilibreur de charge de travail, voir [Filtrer des informations dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
