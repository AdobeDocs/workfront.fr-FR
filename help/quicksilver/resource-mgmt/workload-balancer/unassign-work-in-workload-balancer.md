---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Annuler l’affectation de travaux dans l’équilibreur de charge de travail
description: Vous pouvez annuler l’affectation de personnes à des tâches dans la zone de travail affecté de l’équilibreur de charge de travail Adobe Workfront ou réaffecter ces tâches à d’autres personnes, rôles ou équipes.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 100%

---

# Annuler l’affectation de travaux dans l’équilibreur de charge de travail

Vous pouvez annuler l’affectation de personnes à des tâches dans la zone de travail affecté de l’équilibreur de charge de travail Adobe Workfront ou réaffecter ces tâches à d’autres personnes, rôles ou équipes.

Vous pouvez manuellement annuler l’affectation de tâches à des personnes en les faisant glisser et en les déposant, ou en bloc. Cet article décrit comment annuler manuellement l’affectation d’utilisateurs et utilisatrices.

Pour plus d’informations sur l’annulation de l’affectation des personnes par glisser-déposer, voir [Affecter un travail dans l’équilibreur de charge de travail en le faisant glisser et en le déposant](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Pour plus d’informations sur l’annulation de l’affectation de personnes en bloc, voir [Affecter du travail en bloc à l’aide de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan, pour l’utilisation de l’équilibreur de charge de travail dans la zone Ressources.</p>
   <p>Travail, pour l’utilisation de l’équilibreur de charge de travail d’une équipe ou d’un projet.</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifiez l’accès aux éléments suivants :</p> 
    <ul> 
     <li> <p>Gestion des ressources</p> </li> 
     <li> <p>Projets</p> </li> 
     <li> <p>Tâches</p> </li> 
     <li> <p>Problèmes</p> </li> 
    </ul> <p>Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribuer ou supérieures aux projets, tâches et problèmes qui incluent la création d’affectations.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

 

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
