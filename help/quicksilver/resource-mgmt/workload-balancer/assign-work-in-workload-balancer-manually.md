---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Affectation manuelle du travail à l’aide de l’équilibreur de charge
description: Vous pouvez affecter manuellement des tâches aux utilisateurs et aux utilisatrices à l’aide de l’équilibreur de charge de travail d’Adobe Workfront.
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 94%

---

# Affecter manuellement du travail à l’aide de l’équilibreur de charge de travail

Vous pouvez affecter manuellement des tâches aux utilisateurs et aux utilisatrices à l’aide de l’équilibreur de charge de travail d’Adobe Workfront.

Pour des informations générales sur l’attribution de travail aux utilisateurs et utilisatrices à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’attribution de travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Autorisations Contribuer ou supérieures aux projets, tâches et problèmes qui incluent la création d’affectations.</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Affecter du travail dans l’équilibreur de charge de travail

Vous pouvez affecter des tâches qui n’ont pas encore été attribuées à un utilisateur ou à une utilisatrice ou réaffecter des tâches qui ont été attribuées à des utilisateurs et utilisatrices dans l’équilibreur de charge de travail.

1. Accédez à l’équilibreur de charge de travail auquel vous souhaitez attribuer du travail.

   Vous pouvez attribuer du travail aux utilisateurs et utilisatrices à l’aide de l’équilibreur de charge de travail dans la zone Ressources, au niveau du projet ou de l’équipe. Pour plus d’informations sur l’emplacement de l’équilibreur de charge de travail dans Workfront, voir [Localiser l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Facultatif) Accédez à la zone **Travail non affecté** et appliquez un filtre pour afficher les tâches ou les problèmes.

   Ou

   Accédez à la zone **Travail affecté** et développez le nom d’un utilisateur ou d’une utilisatrice pour afficher les éléments de travail qui lui ont été affectés, si vous souhaitez réaffecter ses éléments.

1. Cliquez sur le **menu Plus** ![](assets/qs-more-menu.png) à gauche du nom d’un élément de travail, puis cliquez sur **Affecter cet élément à**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >Vous pouvez également utiliser les raccourcis suivants pour affecter des tâches ou des problèmes :
   >
   >* Sous Windows : cliquez sur la barre des tâches ou des problèmes en maintenant la touche CTRL enfoncée.
   >* Sur Mac : cliquez sur la barre des tâches ou des problèmes en maintenant la touche CMD enfoncée.

1. Utilisez l’une des méthodes suivantes :

   * Commencez à saisir le nom d’un utilisateur ou d’une utilisatrice, d’une fonction ou d’une équipe que vous souhaitez affecter à l’élément dans le champ **Rechercher des personnes, des rôles ou des équipes**, sélectionnez-le lorsqu’il s’affiche dans la liste, puis cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Lors de l’ajout d’un utilisateur ou d’une utilisatrice, faites attention à l’avatar, au rôle principal de l’utilisateur ou de l’utilisatrice et à son adresse e-mail afin de distinguer les utilisateurs et les utilisatrices ayant des noms identiques.
   >
   >Les utilisateurs et utilisatrices doivent être associés à au moins une fonction pour l’afficher à mesure que vous les ajoutez.
   >
   > Pour que les utilisateurs et utilisatrices puissent afficher les e-mails de leurs utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, consultez la section [Accorder l’accès aux utilisateurs et aux utilisatrices](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Si la fonction de délégation a été activée par l’équipe d’administration de Workfront ou de groupes dans votre environnement, utilisez l’onglet des affectations pour affecter des utilisateurs et des utilisatrices à la tâche ou au problème. L’onglet « Délégations » permet d’afficher les utilisateurs et les utilisatrices qui sont délégués à l’élément de travail. Pour plus d’informations sur la délégation de travail, voir [Délégation de tâches et de problèmes](../../manage-work/delegate-work/how-to-delegate-work.md).


   Cette opération permet d’attribuer ou de réattribuer l’élément de travail aux destinataires spécifiés.

   Si vous n’affectez un élément qu’à une équipe ou à une fonction, l’élément ne s’affiche que dans la zone du travail non affecté. Vous devez assigner des éléments de travail aux utilisateurs et aux utilisatrices afin de les afficher dans la zone du travail affecté de l’équilibreur de charge de travail.

   >[!TIP]
   >
   >Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
   >
   >
   >Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
   >
   >   
   >   
   >   * Réaffectez la tâche aux ressources actives.
   >   * Associez les utilisateurs et utilisatrices d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.
   >   
   >

   * Cliquez sur **Avancé** pour accéder aux affectations avancées.

     Pour plus d’informations sur les affectations avancées, consultez la section [Créer des affectations avancées](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. (Facultatif) Cliquez sur l’icône **Afficher les affectations** ![](assets/show-allocations-icon-small.png), puis cliquez sur le menu **Plus** ![](assets/qs-more-menu.png) > **Modifier les affectations**.

   Ou

   Double-cliquez sur une allocation quotidienne ou hebdomadaire pour modifier le temps alloué à l’utilisateur ou à l’utilisatrice pour cet élément de travail.

   Pour plus d’informations sur la modification des affectations d’utilisateurs ou d’utilisatrices dans l’équilibreur de charge de travail, consultez la section « Modifier les affectations d’utilisateurs ou d’utilisatrices » dans l’article [Gérer les affectations d’utilisateurs ou d’utilisatrices dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Pour plus d’informations sur la suppression des affectations d’un élément de travail à l’aide de l’équilibreur de charge de charge de travail, consultez la section [Annuler l’affectation de travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
