---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Annuler l’affectation de travail dans l’équilibreur de charge de travail
description: Vous pouvez annuler l’affectation d’utilisateurs à des tâches dans la zone de travail affectée de l’équilibreur de charge de travail Adobe Workfront ou les réaffecter à d’autres utilisateurs, rôles ou équipes.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 27%

---

# Annuler l’affectation de travail dans l’équilibreur de charge de travail

Vous pouvez annuler l’affectation d’utilisateurs à des tâches dans la zone de travail affectée de l’équilibreur de charge de travail Adobe Workfront ou les réaffecter à d’autres utilisateurs, rôles ou équipes.

Vous pouvez annuler l’affectation manuelle des utilisateurs des tâches en les faisant glisser et en les déposant, ou en bloc. Cet article décrit comment annuler manuellement l’affectation d’utilisateurs.

Pour plus d’informations sur l’annulation de l’affectation des utilisateurs en les faisant glisser et en les déposant, voir [Affectation d’un travail dans l’équilibreur de charge de travail par glisser-déposer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Pour plus d’informations sur l’annulation de l’affectation des utilisateurs en bloc, voir [Affecter du travail en masse à l’aide de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Planifiez l’utilisation de l’équilibreur de charge de travail dans la zone Ressource .</p>
   <p>Fonctionnement lors de l’utilisation de l’équilibreur de charge de travail d’une équipe ou d’un projet</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux éléments suivants :</p> 
    <ul> 
     <li> <p>Gestion des ressources</p> </li> 
     <li> <p>Projets</p> </li> 
     <li> <p>Tâches</p> </li> 
     <li> <p>Problèmes</p> </li> 
    </ul> <p>Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribute ou supérieures aux projets, tâches et problèmes qui incluent l’attribution des tâches</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

 

## Annulation de l’affectation des tâches dans l’équilibreur de charge de travail

Vous pouvez soit annuler l’affectation d’éléments à des utilisateurs et les déplacer vers la zone de travail non affectée, soit les réaffecter à d’autres utilisateurs.

Pour annuler l’affectation d’éléments de travail à des utilisateurs :

1. Dans l’équilibreur de charge de travail, accédez à la zone **Travail affecté** et développez un utilisateur.
1. Utilisez l’une des méthodes suivantes :

   * Recherchez l’élément que vous souhaitez annuler l’affectation dans la zone d’un utilisateur, cliquez dessus, puis faites-le glisser et déposez-le dans la zone Non affecté ou dans la zone d’un autre utilisateur.
   * Cliquez sur l’icône **Plus** ![](assets/more-icon-task-list.png) à droite du nom d’un élément de travail, cliquez sur **Attribuer ceci à**, puis supprimez le nom des entités affectées à l’élément de travail ou saisissez un autre nom, puis cliquez sur **Enregistrer**.

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   L’élément s’affiche dans la zone de travail non attribué s’il correspond aux critères de filtrage de cette zone et qu’il n’est attribué à aucun autre utilisateur, ou s’il s’affiche dans la zone utilisateur s’il est attribué à un autre utilisateur.

   Pour plus d’informations sur le filtrage dans l’équilibreur de charge de travail, voir [Filtrage des informations dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
