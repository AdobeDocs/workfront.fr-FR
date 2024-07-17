---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Créer un sous-groupe
description: Vous pouvez créer un sous-groupe sous un groupe afin d’organiser les utilisateurs et les projets et d’attribuer des droits d’accès dans Adobe Workfront. En règle générale, les administrateurs de groupe gèrent les groupes et les sous-groupes. Ils peuvent utiliser la page Groupes pour gérer leurs groupes et sous-groupes au même endroit.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 16%

---

# Créer un sous-groupe

Vous pouvez créer un sous-groupe sous un groupe afin d’organiser les utilisateurs et les projets et d’attribuer des droits d’accès dans Adobe Workfront.

S’il existe des groupes au-dessus du groupe que vous gérez, leur équipe d’administration peut également le faire pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

Cependant, en règle générale, les administrateurs de groupe gèrent les groupes et les sous-groupes. Ils peuvent utiliser la page Groupes pour gérer leurs groupes et sous-groupes au même endroit. Pour plus d’informations sur le fonctionnement des groupes et des sous-groupes dans Workfront, voir [Présentation des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md) et [Présentation des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan Workfront*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur ou une administratrice de groupe pour le groupe ou un administrateur ou une administratrice de Workfront. Pour plus d’informations, consultez les sections <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à une personne</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir votre plan ou type de licence, contactez l’administration de Workfront.

## Ajouter un sous-groupe

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Groups**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils possèdent. Les administrateurs Adobe Workfront peuvent voir tous les groupes.

1. Sélectionnez le groupe ou le sous-groupe existant dans lequel vous souhaitez ajouter un nouveau sous-groupe.
1. Cliquez sur **Nouveau sous-groupe**.
1. Dans la zone **New Subgroup** qui s’affiche, saisissez un **nom de groupe** pour le sous-groupe.
1. (Facultatif) indiquez l’une des informations suivantes :

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
      <td>Saisissez une description pour le sous-groupe. Vous pouvez saisir jusqu’à 512 caractères.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Est actif</td> 
      <td> <p>(Activé par défaut) Active le groupe dans votre instance Workfront.</p> <p>Dans des champs de type anticipé comme celui illustré ci-dessous, lorsque des utilisateurs ordinaires recherchent un groupe pour le joindre à un objet ou pour le partager avec lui, seuls les groupes actifs s’affichent dans la liste.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Pour rationaliser cette opération pour vos utilisateurs, vous pouvez désactiver l’option Est active pour les groupes qui ne sont pas actuellement utilisés.</p> <p>Vous pouvez facilement afficher, filtrer et regrouper la liste Groupes en fonction de l’état actif ou inactif à l’aide de ce champ. Pour plus d’informations sur l’utilisation des vues, des filtres et des regroupements dans des listes, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Éléments de reporting : filtres, vues et regroupements</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendre ce groupe et ses sous-groupes publics</td> 
      <td> <p>(Disponible uniquement si vous affichez les détails d’un groupe de niveau supérieur et non d’un sous-groupe.) Activez cette option pour permettre aux utilisateurs du sous-groupe ayant un accès utilisateur d’édition (qui ne sont pas administrateurs du groupe) d’ajouter ce groupe et ses sous-groupes au profil utilisateur des autres utilisateurs.</p> <p>Pour un groupe public, tout utilisateur (dans ou hors du groupe) disposant d’un accès utilisateur d’édition peut ajouter le groupe au profil d’autres utilisateurs. Ils ne peuvent pas le faire pour un groupe privé.</p> <p>Vous ne pouvez modifier cette option que sur le groupe parent supérieur d’une hiérarchie de groupes comportant plusieurs niveaux. Tous les sous-groupes du groupe parent héritent de son paramètre.</p> <p><b>NOTE</b> :  
        <ul> 
         <li>Vous ne pouvez pas rendre un sous-groupe public en lui-même, mais vous pouvez le rendre public en tant que groupe parent de niveau supérieur, ce qui rend également tous les sous-groupes du parent public.</li> 
         <li>Un sous-groupe appartenant à un groupe public est public par défaut. Par conséquent, tout utilisateur disposant d’un accès utilisateur de modification peut également ajouter le sous-groupe à d’autres utilisateurs.</li> 
        </ul> </p> <p>Si vous avez besoin d’informations sur l’accès nécessaire pour modifier les utilisateurs, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Octroi de l’accès aux utilisateurs</a>. Pour plus d’informations sur la modification des utilisateurs, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Modification du profil d’un utilisateur</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chef d’entreprise </td> 
      <td> <p>Vous pouvez affecter un utilisateur en tant que chef d’entreprise à un sous-groupe que vous gérez. Un chef d’entreprise est une personne qui prend des décisions commerciales pour le sous-groupe. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Présentation du chef d’entreprise</a><span>.</span></p> <p>Si la personne n’est pas déjà membre du sous-groupe, l’ajout de son nom à ce champ les ajoute également au groupe.</p> <p><b>NOTE</b> :  
        <ul> 
         <li>Avant de pouvoir supprimer le chef d’entreprise d’un sous-groupe, vous devez supprimer son nom du champ Chef d’entreprise .</li> 
         <li>Si vous supprimez le nom du champ Business Leader , cet utilisateur reste membre du sous-groupe, sauf si vous le supprimez. Pour plus d’informations sur la suppression d’une personne d’un groupe, reportez-vous à la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gestion des appartenances à un groupe</a> de l’article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Gérer un groupe</a>.</li> 
        </ul> </p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Présentation du chef de l’entreprise</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membres du groupe et administrateurs de groupe</td> 
      <td> 
       <ul> 
        <li> <p>Membres du groupe : pour ajouter des utilisateurs et des groupes au sous-groupe, commencez à saisir le nom d’un utilisateur ou d’un groupe existant à ajouter, puis sélectionnez le nom qui s’affiche.</p> <p>Les utilisateurs et les groupes que vous ajoutez ont accès à tous les objets partagés avec le groupe.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">Administrateurs de groupe : un sous-groupe hérite des administrateurs de groupe du groupe situé au-dessus. Il est donc facultatif de spécifier un utilisateur en tant qu’administrateur de groupe pour un sous-groupe. Vous pouvez affecter un membre du groupe en tant qu’administrateur du groupe à l’aide du menu déroulant situé à droite du nom de l’utilisateur.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rechercher des personnes et des groupes dans la liste</td> 
      <td> Si vous devez trouver un utilisateur ou un groupe déjà affecté à ce sous-groupe, vous pouvez saisir son nom ici et le sélectionner lorsqu’il apparaîtra.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer.**
