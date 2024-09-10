---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Création d’un sous-groupe
description: Vous pouvez créer un sous-groupe en dessous d’un groupe que vous gérez afin d’organiser les utilisateurs et utilisatrices et les projets et pour attribuer des droits d’accès dans Adobe Workfront. En règle générale, les administrateurs et administratrices de groupes gèrent les groupes et les sous-groupes. Ceux-ci peuvent utiliser la page Groupes pour gérer leurs groupes et leurs sous-groupes au même endroit.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 98%

---

# Créer un sous-groupe

Vous pouvez créer un sous-groupe en dessous d’un groupe que vous gérez afin d’organiser les utilisateurs et utilisatrices et les projets et pour attribuer des droits d’accès dans Adobe Workfront.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

Toutefois, en règle générale, les administrateurs et administratrices de groupes gèrent les groupes et les sous-groupes. Ceux-ci peuvent utiliser la page Groupes pour gérer leurs groupes et leurs sous-groupes au même endroit. Pour plus d’informations sur le fonctionnement des groupes et des sous-groupes dans Workfront, consultez [Vue d’ensemble des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md) et [Vue d’ensemble des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter un sous-groupe

{{step-1-to-setup}}

1. Cliquez sur **Groupes**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Sélectionnez le groupe ou le sous-groupe existant auquel vous souhaitez ajouter un nouveau sous-groupe.
1. Cliquez sur **Nouveau sous-groupe**.
1. Dans la zone **Nouveau sous-groupe** qui s’affiche, saisissez un **Nom de groupe** pour le sous-groupe.
1. (Facultatif) Indiquez l’une des informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom du groupe</td> 
      <td>Modifiez le nom du groupe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Saisissez une description pour le sous-groupe. Vous pouvez saisir jusqu’à 512 caractères.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Est active</td> 
      <td> <p>(Activé par défaut) Active le groupe dans votre instance Workfront.</p> <p>Dans les champs à remplissage automatique comme celui illustré ci-dessous, lorsque des utilisateurs et utilisatrices ordinaires recherchent un groupe pour le joindre à un objet ou pour partager un objet avec celui-ci, seuls les groupes actifs s’affichent dans la liste.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Pour simplifier cette opération pour vos utilisateurs et utilisatrices, vous pouvez désactiver l’option Est actif pour les groupes qui ne sont pas actuellement utilisés.</p> <p>Vous pouvez facilement afficher, filtrer et regrouper la liste des groupes en fonction de l’état actif ou inactif à l’aide de ce champ. Pour plus d’informations sur l’utilisation des vues, des filtres et des regroupements dans les listes, consultez <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Éléments de création de rapports : filtres, vues et regroupements</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendre ce groupe et ses sous-groupes publics</td> 
      <td> <p>(Disponible uniquement si vous consultez les détails d’un groupe de niveau supérieur et non d’un sous-groupe.) Activez cette option pour permettre aux utilisateurs et aux utilisatrices du sous-groupe disposant d’un accès d’édition (et qui ne sont pas administrateurs ou administratrices du groupe) d’ajouter ce groupe et ses sous-groupes au profil utilisateur des autres utilisateurs et utilisatrices.</p> <p>Pour un groupe public, toute personne (faisant partie ou non du groupe) disposant d’un accès d’édition peut ajouter le groupe au profil d’autres utilisateurs et utilisatrices. Cette personne ne peut pas effectuer cette action pour un groupe privé.</p> <p>Vous ne pouvez modifier cette option que pour le groupe parent situé au niveau le plus haut d’une hiérarchie de groupes à plusieurs niveaux. Tous les sous-groupes du groupe parent héritent de ce paramètre.</p> <p><b>REMARQUE</b> :  
        <ul> 
         <li>Vous ne pouvez pas rendre public un sous-groupe seul, mais vous pouvez rendre public son groupe parent de niveau supérieur, ce qui a pour effet de rendre également publics tous les sous-groupes du groupe parent.</li> 
         <li>Un sous-groupe appartenant à un groupe public est public par défaut. Par conséquent, toute personne disposant d’un accès d’édition peut également ajouter le sous-groupe à d’autres utilisateurs et utilisatrices.</li> 
        </ul> </p> <p>Si vous avez besoin d’informations sur l’accès nécessaire pour modifier les personnes, reportez-vous à la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Accorder l’accès aux personnes</a>. Pour plus d’informations sur la modification des personnes, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Modifier le profil d’une personne</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chef d’entreprise </td> 
      <td> <p>Vous pouvez attribuer une personne le rôle de chef d’entreprise à un sous-groupe que vous gérez. La personne disposant du rôle de chef d’entreprise prend des décisions commerciales pour le sous-groupe. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Vue d’ensemble du rôle de chef d’entreprise</a><span>.</span></p> <p>Si la personne n’est pas déjà membre du sous-groupe, l’ajout de son nom à ce champ l’ajoute également au groupe.</p> <p><b>REMARQUE</b> :  
        <ul> 
         <li>Avant de pouvoir supprimer la personne disposant du rôle de chef d’entreprise d’un sous-groupe, vous devez supprimer son nom du champ Chef d’entreprise.</li> 
         <li>Si vous supprimez le nom du champ Chef d’entreprise, cette personne reste membre du sous-groupe, sauf si vous la supprimez du sous-groupe. Pour obtenir des instructions sur la suppression d’une personne d’un groupe, reportez-vous à la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gérer les adhésions à un groupe</a> dans l’article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Gérer un groupe</a>.</li> 
        </ul> </p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Vue d‘ensemble du rôle de chef d’entreprise</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membres du groupe et administrateurs de groupe</td> 
      <td> 
       <ul> 
        <li> <p>Personnes membres du groupe : pour ajouter des personnes et des groupes au sous-groupe, commencez à saisir le nom d’une personne ou d’un groupe existant à ajouter, puis sélectionnez le nom qui s’affiche.</p> <p>Les personnes et les groupes que vous ajoutez ont accès à tous les objets partagés avec le groupe.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">Équipe d’administration de groupes : un sous-groupe hérite de l’équipe d’administration de groupes du groupe située au-dessus. Il est donc facultatif de spécifier les personnes faisant partie de l’équipe d’administration de groupes pour un sous-groupe. Vous pouvez attribuer à une personne du groupe les droits d’administration de groupes à l’aide du menu déroulant situé à droite du nom de la personne.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rechercher des personnes et des groupes dans la liste</td> 
      <td> Si vous devez trouver une personne ou un groupe déjà affecté(e) à ce sous-groupe, vous pouvez saisir son nom ici et la ou le sélectionner lorsqu’elle ou il apparaîtra.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer**.
