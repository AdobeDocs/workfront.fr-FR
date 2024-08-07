---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Affecter manuellement du travail à l’aide de l’équilibreur de charge de travail
description: Vous pouvez affecter manuellement des tâches aux utilisateurs à l’aide de l’équilibreur de charge de travail Adobe Workfront.
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 30%

---

# Affecter manuellement du travail à l’aide de l’équilibreur de charge de travail

Vous pouvez affecter manuellement des tâches aux utilisateurs à l’aide de l’équilibreur de charge de travail Adobe Workfront.

Pour des informations générales sur l’affectation de travail aux utilisateurs à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’affectation de travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Modifiez l’accès aux éléments suivants :</p> 
    <ul> 
     <li> <p>Gestion des ressources</p> </li> 
     <li> <p>Projets</p> </li> 
     <li> <p>Tâches</p> </li> 
     <li> <p>Problèmes</p> </li> 
    </ul> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribute ou supérieures aux projets, tâches et problèmes qui incluent l’attribution des tâches</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Affectation manuelle du travail dans l’équilibreur de charge

Vous pouvez affecter des tâches qui n’ont pas encore été affectées à un utilisateur ou réaffecter des éléments qui ont été affectés à des utilisateurs dans l’équilibreur de charge de travail.

1. Accédez à l’équilibreur de charge de travail où vous souhaitez affecter le travail.

   Vous pouvez affecter du travail aux utilisateurs à l’aide de l’équilibreur de charge de travail dans la zone Ressource, au niveau du projet ou au niveau de l’équipe. Pour plus d’informations sur l’emplacement de l’équilibreur de charge de travail dans Workfront, voir [Localisation de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Facultatif) Accédez à la zone **Travail non attribué** et appliquez un filtre pour afficher les tâches ou les problèmes.

   Ou

   Accédez à la zone **Travail attribué** et développez le nom d’un utilisateur pour afficher les tâches qui lui sont affectées, si vous souhaitez réaffecter ses éléments.

1. Cliquez sur le menu **Plus** ![](assets/qs-more-menu.png) situé à gauche du nom d’un élément de travail, puis cliquez sur **Attribuer ceci à**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >Vous pouvez également utiliser les raccourcis suivants pour affecter des tâches ou des problèmes :
   >
   >* Sous Windows : cliquez sur la barre de tâches ou de problèmes tout en maintenant la touche Ctrl enfoncée.
   >* Dans Mac : cliquez sur la barre de tâches ou de problèmes tout en maintenant la touche CMD.

1. Utilisez l’une des méthodes suivantes :

   * Commencez à saisir le nom d’un utilisateur, d’un rôle de tâche ou d’une équipe que vous souhaitez affecter à l’élément dans le champ **Rechercher des personnes, un rôle ou des équipes**, sélectionnez-le lorsqu’il s’affiche dans la liste, puis cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Lors de l’ajout d’un utilisateur, notez l’avatar, le rôle de Principal de l’utilisateur et son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques.
   >
   >Les personnes doivent être associées à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
   >
   > Pour pouvoir voir les adresses e-mail des utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, consultez [Accorder l’accès aux utilisateurs et utilisatrices](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Si l’administrateur de Workfront ou de groupe a activé les délégations dans votre environnement, utilisez l’onglet Affectations pour affecter des utilisateurs à la tâche ou au problème. Utilisez l’onglet Délégations pour afficher les utilisateurs qui sont délégués à l’élément de travail. Pour plus d’informations sur la délégation de travail, voir [Gérer la tâche et la délégation de problème](../../manage-work/delegate-work/how-to-delegate-work.md).


   Cela affecte ou réaffecte l’élément de travail aux personnes désignées.

   Si vous attribuez un élément à une seule équipe ou à un rôle de tâche, l’élément s’affiche uniquement dans la zone de travail Non affecté . Vous devez affecter des tâches aux utilisateurs afin de les afficher dans la zone de travail affectée de l’équilibreur de charge de travail.

   >[!TIP]
   >
   >Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
   >
   >
   >Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
   >
   >   
   >   
   >   * Réaffectez l’élément de travail aux ressources actives.
   >   * Associez les personnes d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.
   >   
   >

   * Cliquez sur **Avancé** pour accéder aux affectations avancées.

     Pour plus d’informations sur la création d’affectations avancées, voir [Création d’affectations avancées](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. (Facultatif) Cliquez sur l’icône **Afficher les attributions** ![](assets/show-allocations-icon-small.png), puis sur le **menu Plus** ![](assets/qs-more-menu.png) > **Modifier les attributions**.

   Ou

   Double-cliquez sur une allocation quotidienne ou hebdomadaire pour modifier la durée pendant laquelle l’utilisateur est affecté à l’élément de travail.

   Pour plus d’informations sur la modification des affectations utilisateur dans l’équilibreur de charge de travail, voir la section &quot;Modifier les affectations utilisateur&quot; dans l’article [Gérer les affectations utilisateur dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Pour plus d’informations sur la suppression d’affectations d’un élément de travail à l’aide de l’équilibreur de charge de travail, voir [Annuler l’affectation d’un travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
