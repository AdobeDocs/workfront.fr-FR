---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Affectation manuelle du travail à l’aide de l’équilibreur de charge
description: Vous pouvez affecter manuellement des tâches aux utilisateurs à l’aide de l’équilibreur de charge de travail Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 2%

---

# Affectation manuelle du travail à l’aide de l’équilibreur de charge

Vous pouvez affecter manuellement des tâches aux utilisateurs à l’aide de l’équilibreur de charge de travail Adobe Workfront.

Pour obtenir des informations générales sur l’affectation de travail aux utilisateurs à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’affectation de travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Planifiez l’utilisation de l’équilibreur de charge de travail pour une équipe ou dans la zone de ressources </p>
   <p>Fonctionnement lors de l’utilisation de l’équilibreur de charge de travail d’un projet </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Modifiez l’accès aux éléments suivants :</p> 
    <ul> 
     <li> <p>Gestion des ressources</p> </li> 
     <li> <p>Projets</p> </li> 
     <li> <p>Tâches</p> </li> 
     <li> <p>Événements</p> </li> 
    </ul> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Attribuez des autorisations ou des autorisations supérieures aux projets, tâches et problèmes qui incluent l’attribution des affectations.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Affectation manuelle du travail dans l’équilibreur de charge

Vous pouvez affecter des tâches qui n’ont pas encore été affectées à un utilisateur ou réaffecter des éléments qui ont été affectés à des utilisateurs dans l’équilibreur de charge de travail.

1. Accédez à l’équilibreur de charge de travail où vous souhaitez affecter le travail.

   Vous pouvez affecter du travail aux utilisateurs à l’aide de l’équilibreur de charge de travail dans la zone Ressource, au niveau du projet ou au niveau de l’équipe. Pour plus d’informations sur l’emplacement de l’équilibreur de charge de travail dans Workfront, voir [Localisation de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Facultatif) Accédez au **Travail non attribué** et appliquer un filtre pour afficher les tâches ou les problèmes ;

   Ou

   Accédez au **Travail attribué** et développez le nom d’un utilisateur pour afficher les tâches qui lui sont affectées, si vous souhaitez réaffecter ses éléments.

1. Cliquez sur le bouton **Plus de menu** ![](assets/qs-more-menu.png) à gauche du nom d’un élément de travail, puis cliquez sur **Attribuez-le à**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >Vous pouvez également utiliser les raccourcis suivants pour affecter des tâches ou des problèmes :
   >
   >* Sous Windows : CTRL+clic sur la barre de tâche ou de problème.
   >* Dans Mac : CMD+cliquez sur la barre de tâche ou de problème.


1. Utilisez l’une des méthodes suivantes :

   * Commencez à saisir le nom d’un utilisateur, d’un rôle de tâche ou d’une équipe que vous souhaitez affecter à l’élément dans la variable **Recherche de personnes, de rôles ou d’équipes** , sélectionnez-le lorsqu’il s’affiche dans la liste, puis cliquez sur **Enregistrer**.
   >[!TIP]
   >
   >Lors de l’ajout d’un utilisateur, notez l’avatar, le rôle Principal de l’utilisateur et son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques. Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher à mesure que vous les ajoutez.

   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Si l’administrateur de Workfront ou de groupe a activé les délégations dans votre environnement, utilisez l’onglet Affectations pour affecter des utilisateurs à la tâche ou au problème. Utilisez l’onglet Délégations pour afficher les utilisateurs qui sont délégués à l’élément de travail. Pour plus d’informations sur la délégation de travail, voir [Gérer la délégation des tâches et des problèmes](../../manage-work/delegate-work/how-to-delegate-work.md).


   Cela affecte ou réaffecte l’élément de travail aux personnes désignées.

   Si vous attribuez un élément à une seule équipe ou à un rôle de tâche, l’élément s’affiche uniquement dans la zone de travail Non affecté . Vous devez affecter des tâches aux utilisateurs afin de les afficher dans la zone de travail affectée de l’équilibreur de charge de travail.

   >[!TIP]
   >
   >Vous pouvez affecter plusieurs utilisateurs, rôles de tâche ou équipes. Vous ne pouvez affecter que des utilisateurs, des rôles de tâche et des équipes principaux.
   >
   >
   >Si un utilisateur, un rôle de tâche ou une équipe a été affecté avant d’être désactivé, il reste attribué à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
   >
   >   
   >   
   >   * Réaffectez l’élément de travail aux principales ressources.
   >   * Associez les utilisateurs d’une équipe désactivée à une équipe principale et réaffectez l’élément de travail à l’équipe principale.


   * Cliquez sur **Avancé** pour accéder aux affectations avancées.

      Pour plus d’informations sur la création d’affectations avancées, voir [Création d’affectations avancées](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).


1. (Facultatif) Cliquez sur le **Icône Afficher les attributions** ![](assets/show-allocations-icon-small.png), puis cliquez sur le bouton **Plus de menu** ![](assets/qs-more-menu.png) > **Modifier les attributions**.

   Ou

   Double-cliquez sur une allocation quotidienne ou hebdomadaire pour modifier la durée pendant laquelle l’utilisateur est affecté à l’élément de travail.

   Pour plus d’informations sur la modification des affectations d’utilisateurs dans l’équilibreur de charge de travail, voir la section &quot;Modifier les affectations d’utilisateurs&quot; de l’article. [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Pour plus d’informations sur la suppression d’affectations d’un élément de travail à l’aide de l’équilibreur de charge de travail, voir [Annulation de l’affectation du travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
