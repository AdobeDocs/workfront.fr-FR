---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Affectez un travail à l’équilibreur de charge de travail en le faisant glisser et en le déposant
description: Vous pouvez affecter des tâches à l’aide de l’équilibreur de charge de travail Adobe Workfront en les faisant glisser et en les déposant sur les utilisateurs appropriés.
author: Alina
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: a1ffec0d8a50ff7f025ff23370afa746cf0d6d3f
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 1%

---

# Affectez un travail à l’équilibreur de charge de travail en le faisant glisser et en le déposant

<!--remove production and preview preferences at release-->

Vous pouvez affecter des tâches à l’aide de l’équilibreur de charge de travail Adobe Workfront en les faisant glisser et en les déposant sur les utilisateurs appropriés.

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

## Attribuer un élément en le faisant glisser et en le déposant

Vous pouvez affecter un élément de la zone de travail non attribué à un utilisateur ou réaffecter un élément déjà affecté à un autre utilisateur de la zone de travail attribué.

1. Accédez à l’équilibreur de charge de travail où vous souhaitez affecter le travail.

   Vous pouvez affecter du travail aux utilisateurs à l’aide de l’équilibreur de charge de travail dans la zone Ressource, au niveau du projet ou au niveau de l’équipe. Pour plus d’informations sur l’emplacement de l’équilibreur de charge de travail dans Workfront, voir [Localisation de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Facultatif) Accédez au **Travail non attribué** et appliquez un filtre pour afficher les tâches et les problèmes qui ne sont pas affectés aux utilisateurs.

   Ou

   Accédez au **Travail attribué** et développez le nom d’un utilisateur pour afficher les tâches qui lui sont affectées, si vous souhaitez réaffecter ses éléments.

1. (Conditionnel) Dans l’équilibreur de charge de travail d’un projet, cliquez sur le bouton **Afficher tous les utilisateurs** icon ![](assets/show-all-users-icon-project-workload-balancer.png) pour afficher tous les utilisateurs de Workfront.

   Cette option affiche tous les utilisateurs auxquels vous avez accès.

   Les utilisateurs qui font également partie de l’équipe de projet et qui sont déjà affectés à des éléments du projet disposent de l’icône de projet à droite de leur nom dans la zone Travail attribué .

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* L’option Afficher tous les utilisateurs est disponible uniquement dans l’équilibreur de charge de travail d’un projet.
   >* Utilisez des filtres pour n’afficher que les utilisateurs qui vous intéressent. Par exemple, utilisez un filtre pour afficher uniquement les utilisateurs de vos équipes ou groupes.




1. Cliquez sur la barre d’un élément de travail qui indique la chronologie planifiée ou projetée et faites-la glisser sur le nom d’un utilisateur dans la variable **Attribué** zone.

   L’utilisateur sur lequel vous passez le curseur pour déposer l’élément de travail est mis en surbrillance.

   >[!TIP]
   >
   >Les Heures planifiées de l’utilisateur que vous survolez en temps réel avec la mise à jour du nombre d’heures planifiées quotidiennes de l’élément de travail, afin d’indiquer l’impact de l’ajout d’un nouvel élément sur leur allocation globale.

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. Lorsque vous êtes prêt, déposez l’élément de travail sélectionné dans la même ligne que le nom de l’utilisateur dans la zone affectée. L’élément est attribué et les heures planifiées allouées sont mises à jour pour l’utilisateur avec les nouvelles heures de l’élément de travail.

   Si l’élément a été attribué à un rôle de tâche que l’utilisateur ne peut pas remplir, il s’affiche sous le nom de l’utilisateur dans la zone de travail Affecté et il reste également dans la zone de travail Non affecté pour indiquer que le rôle de tâche qui lui est associé n’a pas encore été remplacé par un utilisateur.

   >[!TIP]
   >
   >* Si vous avez activé l’option Groupe par projet dans la zone Paramètres , la tâche affectée s’affiche sous le projet correspondant. Si le paramètre est désactivé, la tâche affectée s’affiche dans la zone utilisateur.
      >
      >
      >     L’élément s’affiche en fonction des critères de l’équilibreur de charge de travail pour le tri des tâches. Pour plus d’informations, voir [Navigation dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* Si vous avez activé l’option Afficher tous les utilisateurs dans l’équilibreur de charge de travail d’un projet et affecté des éléments à des utilisateurs qui n’avaient pas été auparavant affectés à des éléments du projet, les utilisateurs sont ajoutés à l’équipe de projet. Pour plus d’informations, voir [Gérer l’équipe de projet](../../manage-work/projects/planning-a-project/manage-project-team.md).



1. (Facultatif) Cliquez sur la barre d’un élément de travail sous le nom d’un utilisateur dans la zone de travail Affecté et faites-le glisser sur la zone de travail Non affecté pour l’annuler. L’élément n’est pas attribué à l’utilisateur, mais il peut toujours être affecté à un rôle de tâche, auquel cas il s’affiche dans la zone de travail non attribué. Si l’élément est attribué à un autre utilisateur, il reste dans la zone de travail attribué sous le nom de l’utilisateur qui est toujours affecté.
1. (Facultatif) Cliquez sur le **Icône Afficher les attributions** ![](assets/show-allocations-icon-small.png), puis cliquez sur le bouton **Plus de menu** ![](assets/qs-more-menu.png) > **Modifier les attributions**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   Ou

   Double-cliquez sur une allocation quotidienne ou hebdomadaire pour modifier la durée pendant laquelle l’utilisateur est affecté à l’élément de travail.

   Pour plus d’informations sur la modification des affectations d’utilisateurs dans l’équilibreur de charge de travail, voir la section &quot;Modifier les affectations d’utilisateurs&quot; de l’article. [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Pour plus d’informations sur la suppression d’affectations d’un élément de travail à l’aide de l’équilibreur de charge de travail, voir [Annulation de l’affectation du travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

