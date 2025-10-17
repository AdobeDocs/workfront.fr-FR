---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Créer un sous-groupe
description: Vous pouvez créer un sous-groupe en dessous d’un groupe que vous gérez afin d’organiser les utilisateurs et utilisatrices et les projets et pour attribuer des droits d’accès dans Adobe Workfront. En règle générale, les administrateurs et administratrices de groupes gèrent les groupes et les sous-groupes. Ceux-ci peuvent utiliser la page Groupes pour gérer leurs groupes et leurs sous-groupes au même endroit.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 60%

---

# Créer un sous-groupe

Vous pouvez créer un sous-groupe en dessous d’un groupe que vous gérez afin d’organiser les utilisateurs et utilisatrices et les projets et pour attribuer des droits d’accès dans Adobe Workfront.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

Toutefois, en règle générale, les administrateurs et administratrices de groupes gèrent les groupes et les sous-groupes. Ceux-ci peuvent utiliser la page Groupes pour gérer leurs groupes et leurs sous-groupes au même endroit. Pour plus d’informations sur le fonctionnement des groupes et des sous-groupes dans Workfront, consultez [Vue d’ensemble des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md) et [Vue d’ensemble des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter un sous-groupe

{{step-1-to-setup}}

1. Cliquez sur **Groupes**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Sélectionnez le groupe ou le sous-groupe existant auquel vous souhaitez ajouter un nouveau sous-groupe.
1. Cliquez sur **Nouveau sous-groupe**.
1. Dans la zone **Nouveau sous-groupe** qui s’affiche, saisissez un **nom du groupe** pour le sous-groupe.
1. (Facultatif) Saisissez l’une des informations suivantes :

   * **Description** : saisissez une description pour le sous-groupe. Vous pouvez saisir jusqu’à 512 caractères.
   * **Est actif** : cette option est activée par défaut et rend le groupe actif dans votre instance Workfront.

     Dans les champs de saisie semi-automatique comme celui illustré ci-dessous, lorsque les utilisateurs réguliers recherchent un groupe pour le joindre à un objet ou partager un objet avec celui-ci, seuls les groupes actifs s’affichent dans la liste.

     ![Champ de saisie semi-automatique pour un groupe](assets/typeahead-for-group.png)

     Pour simplifier cette opération pour vos utilisateurs, vous pouvez désactiver l’option **Est actif** pour les groupes qui ne sont pas utilisés actuellement.

     Vous pouvez facilement afficher, filtrer et regrouper la liste des groupes en fonction de l’état actif ou inactif à l’aide de ce champ. Pour plus d’informations sur l’utilisation des vues, des filtres et des regroupements dans les listes, consultez [Éléments de création de rapports : filtres, vues et regroupements](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   * **Chef d’entreprise** : vous pouvez affecter un utilisateur en tant que chef d’entreprise à un sous-groupe que vous gérez. La personne disposant du rôle de chef d’entreprise prend des décisions commerciales pour le sous-groupe. Pour plus d’informations, voir [Vue d‘ensemble du rôle de chef ou cheffe d’entreprise](/help/quicksilver/administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

     Si la personne n’est pas déjà membre du sous-groupe, l’ajout de son nom à ce champ l’ajoute également au groupe.

     >[!NOTE]
     >
     >* Avant de pouvoir supprimer la personne disposant du rôle de chef d’entreprise d’un sous-groupe, vous devez supprimer son nom du champ Chef d’entreprise.
     >* Si vous supprimez le nom du champ Chef d’entreprise, cette personne reste membre du sous-groupe, sauf si vous la supprimez du sous-groupe. Pour obtenir des instructions sur la suppression d’une personne d’un groupe, voir [Afficher et gérer les appartenances à un groupe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

   * **Membres du groupe et administrateurs de groupe**: pour ajouter des utilisateurs et des groupes en tant que membres du sous-groupe, commencez à saisir le nom d’un utilisateur ou d’un groupe existant que vous souhaitez ajouter, puis sélectionnez le nom lorsqu’il apparaît.

     Les personnes et les groupes que vous ajoutez ont accès à tous les objets partagés avec le groupe.

     Un sous-groupe hérite des administrateurs de groupe du groupe situé au-dessus. Par conséquent, la spécification d’un utilisateur en tant qu’administrateur de groupe pour un sous-groupe est facultative. Vous pouvez attribuer à une personne du groupe les droits d’administration de groupes à l’aide du menu déroulant situé à droite du nom de la personne.

   * **Rechercher des personnes et des groupes dans la liste** : si vous devez trouver un utilisateur ou un groupe déjà affecté à ce sous-groupe, vous pouvez saisir son nom ici et le sélectionner lorsqu&#39;il apparaît.

1. Cliquer sur **Enregistrer**.
