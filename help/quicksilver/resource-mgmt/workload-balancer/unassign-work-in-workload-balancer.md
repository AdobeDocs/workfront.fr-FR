---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Annulation de l’affectation du travail dans l’équilibreur de charge de travail
description: Vous pouvez annuler l’affectation d’utilisateurs à des tâches dans la zone de travail affectée de l’équilibreur de charge de travail Adobe Workfront ou les réaffecter à d’autres utilisateurs, rôles ou équipes.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 2%

---

# Annulation de l’affectation du travail dans l’équilibreur de charge de travail

Vous pouvez annuler l’affectation d’utilisateurs à des tâches dans la zone de travail affectée de l’équilibreur de charge de travail Adobe Workfront ou les réaffecter à d’autres utilisateurs, rôles ou équipes.

Vous pouvez annuler l’affectation manuelle des utilisateurs des tâches en les faisant glisser et en les déposant, ou en bloc. Cet article décrit comment annuler manuellement l’affectation d’utilisateurs.

Pour plus d’informations sur l’annulation de l’attribution des utilisateurs par glisser-déposer, voir [Affectez un travail à l’équilibreur de charge de travail en le faisant glisser et en le déposant](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Pour plus d’informations sur l’annulation de l’attribution des utilisateurs en bloc, voir [Affectation du travail en masse à l’aide de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Planifiez l’utilisation de l’équilibreur de charge de travail dans la zone Ressource .</p>
   <p>Fonctionnement lors de l’utilisation de l’équilibreur de charge de travail d’une équipe ou d’un projet</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifiez l’accès aux éléments suivants :</p> 
    <ul> 
     <li> <p>Gestion des ressources</p> </li> 
     <li> <p>Projets</p> </li> 
     <li> <p>Tâches</p> </li> 
     <li> <p>Problèmes</p> </li> 
    </ul> <p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Attribuez des autorisations ou des autorisations supérieures aux projets, tâches et problèmes qui incluent l’attribution des affectations.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

 

## Annulation de l’affectation des tâches dans l’équilibreur de charge de travail

Vous pouvez soit annuler l’affectation d’éléments à des utilisateurs et les déplacer vers la zone de travail non affectée, soit les réaffecter à d’autres utilisateurs.

Pour annuler l’affectation d’éléments de travail à des utilisateurs :

1. Dans l’équilibreur de charge de travail, accédez au **Travail assigné** et développez un utilisateur.
1. Utilisez l’une des méthodes suivantes :

   * Recherchez l’élément que vous souhaitez annuler l’affectation dans la zone d’un utilisateur, cliquez dessus, puis faites-le glisser et déposez-le dans la zone Non affecté ou dans la zone d’un autre utilisateur.
   * Cliquez sur le bouton **Plus** icon ![](assets/more-icon-task-list.png) à droite du nom d’une tâche, cliquez sur **Attribuez-le à**, supprimez ensuite le nom des entités affectées à l’élément de travail ou saisissez un autre nom, puis cliquez sur **Enregistrer**.

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   L’élément s’affiche dans la zone de travail non attribué s’il correspond aux critères de filtrage de cette zone et qu’il n’est attribué à aucun autre utilisateur, ou s’il s’affiche dans la zone utilisateur s’il est attribué à un autre utilisateur.

   Pour plus d’informations sur le filtrage des informations dans l’équilibreur de charge de travail, voir [Filtrage des informations dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
