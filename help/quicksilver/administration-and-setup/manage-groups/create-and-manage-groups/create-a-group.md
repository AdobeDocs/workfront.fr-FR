---
user-type: administrator
product-area: system-administration;user-management
keywords: create,group,subgroup,new
navigation-topic: create-and-manage-groups
title: Création d’un groupe
description: En tant qu’administrateur Adobe Workfront, vous pouvez créer des groupes pour organiser les utilisateurs et les projets et attribuer des droits d’accès dans Workfront.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '1658'
ht-degree: 8%

---

# Créer un groupe

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

En tant qu’administrateur Adobe Workfront, vous pouvez créer des groupes pour organiser les utilisateurs et les projets et attribuer des droits d’accès dans Workfront. Pour plus d’informations, voir [Présentation des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Chaque sous-groupe a besoin d’au moins un administrateur de groupe. Les administrateurs de groupe peuvent utiliser la page Groupes pour gérer leurs groupes au même endroit.

Si vous êtes administrateur de groupe ou administrateur Workfront, vous pouvez également créer des sous-groupes sous un groupe. Pour obtenir des instructions, voir [Création d’un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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

+++

## Création d’un groupe de niveau supérieur à partir de zéro

Ces étapes expliquent comment créer un nouveau groupe à partir de zéro. Pour plus d’informations sur la création d’un groupe ou d’un sous-groupe en copiant un groupe existant, voir [Création d’un groupe de niveau supérieur en copiant un groupe ou sous-groupe existant](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) dans cet article.

Pour créer un groupe de niveau supérieur, vous devez être un administrateur Workfront.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Au-dessus de la liste des groupes, cliquez sur **Nouveau groupe**.

   >[!TIP]
   >
   >Au bas de la liste des groupes, vous pouvez également cliquer sur **Ajouter d’autres groupes** pour ajouter un groupe en ligne, puis sur **Entrée** lorsque vous avez terminé d’ajouter les informations du groupe.

1. Dans la zone **New Group** qui s’affiche, saisissez le nom du groupe.
1. Indiquez les informations suivantes :

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
      <td>Saisissez une description pour le groupe. Vous pouvez saisir jusqu’à 512 caractères.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">En activité</td> 
      <td> <p>(Activé par défaut) Active le groupe dans votre instance Workfront.</p> <p>Dans des champs de type anticipé comme celui illustré ci-dessous, lorsque des utilisateurs ordinaires recherchent un groupe pour le joindre à un objet ou pour le partager avec lui, seuls les groupes actifs s’affichent dans la liste.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Pour rationaliser cette opération pour vos utilisateurs, vous pouvez désactiver l’option Est active pour les groupes qui ne sont pas actuellement utilisés.</p> <p>Vous pouvez facilement afficher, filtrer et regrouper la liste Groupes en fonction de l’état actif ou inactif à l’aide de ce champ. Pour plus d’informations sur l’utilisation des vues, des filtres et des regroupements dans des listes, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Éléments de reporting : filtres, vues et regroupements</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendre ce groupe et ses sous-groupes publics</td> 
      <td> <p>(Disponible uniquement si vous affichez les détails d’un groupe de niveau supérieur et non d’un sous-groupe.) Activez cette option pour permettre aux utilisateurs du groupe ayant un accès utilisateur d’édition (qui ne sont pas administrateurs du groupe) d’ajouter ce groupe et ses sous-groupes au profil utilisateur des autres utilisateurs.</p> <p>Pour un groupe public, tout utilisateur (dans ou hors du groupe) disposant d’un accès utilisateur d’édition peut ajouter le groupe au profil d’autres utilisateurs. Ils ne peuvent pas le faire pour un groupe privé.</p> <p>Vous ne pouvez modifier cette option que sur le groupe parent supérieur d’une hiérarchie de groupes comportant plusieurs niveaux. Tous les sous-groupes du groupe parent héritent de son paramètre.</p> <p><b>NOTE</b> :  
        <ul> 
         <li>Vous ne pouvez pas rendre un sous-groupe public en lui-même, mais vous pouvez rendre son groupe parent de niveau supérieur public, ce qui rend également tous les sous-groupes du parent public.</li> 
         <li>Un sous-groupe appartenant à un groupe public est public par défaut. Par conséquent, tout utilisateur disposant d’un accès utilisateur de modification peut également ajouter le sous-groupe à d’autres utilisateurs.</li> 
        </ul> </p> <p>Si vous avez besoin d’informations sur l’accès nécessaire pour modifier les utilisateurs, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Octroi de l’accès aux utilisateurs</a>. Pour plus d’informations sur la modification des utilisateurs, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chef d’entreprise </td> 
      <td> <p>Vous pouvez affecter un utilisateur en tant que chef d’entreprise à un groupe que vous gérez. Un chef d’entreprise est quelqu’un qui prend des décisions commerciales pour le groupe. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Présentation du chef d’entreprise</a><span>.</span></p> <p>Si la personne n’est pas déjà membre du groupe, l’ajout de son nom à ce champ les ajoute également au groupe.</p> <p><b>NOTE</b> :  
        <ul> 
         <li>Avant de pouvoir supprimer le chef d’entreprise d’un groupe, vous devez supprimer son nom du champ Chef d’entreprise .</li> 
         <li>Si vous supprimez le nom du champ Business Leader , cet utilisateur reste membre du groupe, sauf si vous le supprimez. Pour plus d’informations sur la suppression d’une personne d’un groupe, reportez-vous à la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Gestion des appartenances à un groupe</a> de l’article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Gérer un groupe</a>.</li> 
        </ul> </p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Présentation du chef de l’entreprise</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membres du groupe et administrateurs de groupe</td> 
      <td>
        <p>Pour ajouter des membres de groupe, commencez à saisir le nom d’un utilisateur ou d’un groupe que vous souhaitez ajouter, puis sélectionnez le nom qui s’affiche.</p> 
        <p>Les utilisateurs et les groupes que vous ajoutez ont accès à tous les objets partagés avec le groupe.</p>
        <p>Un groupe de niveau supérieur doit avoir au moins un administrateur de groupe. </p>
     </tr> 
     <tr> 
      <td role="rowheader">Rechercher des personnes et des groupes dans la liste</td> 
      <td> Si vous devez trouver un utilisateur ou un groupe déjà affecté à ce groupe, vous pouvez saisir son nom ici et le sélectionner lorsqu’il apparaîtra.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Créer un groupe**.

## Créer un groupe de niveau supérieur en copiant un groupe ou un sous-groupe existant {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

En tant qu’administrateur Workfront, vous pouvez créer un groupe de niveau supérieur en copiant un groupe ou un sous-groupe existant.

Gardez les éléments suivants à l’esprit lorsque vous souhaitez effectuer cette opération :

* Tous les membres et tous les sous-groupes appartenant au groupe existant sont copiés dans le nouveau groupe de niveau supérieur.
* Les membres du groupe copié conservent les affectations qu’ils avaient dans le groupe d’origine. Par conséquent, les administrateurs de groupe du groupe d’origine sont également désignés comme administrateurs de groupe dans le groupe copié.

Pour créer un groupe de niveau supérieur en copiant un groupe ou un sous-groupe :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils possèdent. Les administrateurs Adobe Workfront peuvent voir tous les groupes.

1. Sélectionnez le groupe à copier, puis cliquez sur l’icône Copier ![](assets/copy-icon.png).
1. Dans la zone **Copier le groupe** qui s’affiche, saisissez un **nom de groupe** pour le groupe copié.

1. Indiquez les informations suivantes :

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
      <td>Saisissez une description pour le groupe. Vous pouvez saisir jusqu’à 512 caractères.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">En activité</td> 
      <td> <p>(Activé par défaut) Active le groupe dans votre instance Workfront.</p> <p>Dans des champs de type anticipé comme celui illustré ci-dessous, lorsque des utilisateurs ordinaires recherchent un groupe pour le joindre à un objet ou pour le partager avec lui, seuls les groupes actifs s’affichent dans la liste.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Pour rationaliser cette opération pour vos utilisateurs, vous pouvez désactiver l’option Est active pour les groupes qui ne sont pas actuellement utilisés.</p> <p>Vous pouvez facilement afficher, filtrer et regrouper la liste Groupes en fonction de l’état actif ou inactif à l’aide de ce champ. Pour plus d’informations sur l’utilisation des vues, des filtres et des regroupements dans des listes, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Éléments de reporting : filtres, vues et regroupements</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendre ce groupe et ses sous-groupes publics</td> 
      <td> <p>(Disponible uniquement si vous affichez les détails d’un groupe de niveau supérieur et non d’un sous-groupe.) Activez cette option pour permettre aux utilisateurs du groupe ayant un accès utilisateur d’édition (qui ne sont pas administrateurs du groupe) d’ajouter ce groupe et ses sous-groupes au profil utilisateur des autres utilisateurs.</p> <p>Pour un groupe public, tout utilisateur (dans ou hors du groupe) disposant d’un accès utilisateur d’édition peut ajouter le groupe au profil d’autres utilisateurs. Ils ne peuvent pas le faire pour un groupe privé.</p> <p>Vous ne pouvez modifier cette option que sur le groupe parent supérieur d’une hiérarchie de groupes comportant plusieurs niveaux. Tous les sous-groupes du groupe parent héritent de son paramètre.</p> <p><b>NOTE</b> :  
        <ul> 
         <li>Vous ne pouvez pas rendre un sous-groupe public en lui-même, mais vous pouvez le rendre public en tant que groupe parent de niveau supérieur, ce qui rend également tous les sous-groupes du parent public.</li> 
         <li>Un sous-groupe appartenant à un groupe public est public par défaut. Par conséquent, tout utilisateur disposant d’un accès utilisateur de modification peut également ajouter le sous-groupe à d’autres utilisateurs.</li> 
        </ul> </p> <p>Si vous avez besoin d’informations sur l’accès nécessaire pour modifier les utilisateurs, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Octroi de l’accès aux utilisateurs</a>. Pour plus d’informations sur la modification des utilisateurs, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Modification du profil d’un utilisateur</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chef d’entreprise </td> 
      <td> <p>Vous pouvez affecter un utilisateur en tant que chef d’entreprise à un groupe que vous gérez. Un chef d’entreprise est quelqu’un qui prend des décisions commerciales pour le groupe. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Présentation du chef d’entreprise</a><span>.</span></p> <p>Si la personne n’est pas déjà membre du groupe, l’ajout de son nom à ce champ les ajoute également au groupe.</p> <p><b>NOTE</b> :  
        <ul> 
         <li>Avant de pouvoir supprimer le chef d’entreprise d’un groupe, vous devez supprimer son nom du champ Chef d’entreprise .</li> 
         <li>Si vous supprimez le nom du champ Business Leader , cet utilisateur reste membre du groupe, sauf si vous le supprimez. Pour plus d’informations sur la suppression d’une personne d’un groupe, reportez-vous à la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gestion des appartenances à un groupe</a> de l’article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Gérer un groupe</a>.</li> 
        </ul> </p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Présentation du chef de l’entreprise</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membres du groupe et administrateurs de groupe</td> 
      <td> 
       <ul> 
        <li> <p>Membres du groupe : pour ajouter des utilisateurs et des groupes au groupe, commencez à saisir le nom d’un utilisateur ou d’un groupe que vous souhaitez ajouter, puis sélectionnez le nom qui s’affiche.</p> <p>Les utilisateurs et les groupes que vous ajoutez ont accès à tous les objets partagés avec le groupe.</p> </li> 
        <li> <p>Administrateurs de groupe : tous les administrateurs de groupe du groupe d’origine sont également désignés comme administrateurs de groupe dans le groupe copié. Vous pouvez affecter un membre du groupe en tant qu’administrateur du groupe à l’aide du menu déroulant situé à droite du nom de l’utilisateur.</p> <p>Un groupe de niveau supérieur doit avoir au moins un administrateur de groupe.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rechercher des personnes et des groupes dans la liste</td> 
      <td> Si vous devez trouver un utilisateur ou un groupe déjà affecté à ce groupe, vous pouvez saisir son nom ici et le sélectionner lorsqu’il apparaîtra.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Si le groupe d’origine comporte des sous-groupes, ceux-ci sont ajoutés au nouveau groupe et leurs noms sont, par défaut, &quot;Nom du sous-groupe d’origine (Copier)&quot;.
   >* Vous pouvez éliminer n’importe quel utilisateur ou sous-groupe du groupe d’origine en cliquant sur le X situé à droite du nom de l’utilisateur ou du sous-groupe.

1. Cliquez sur **Créer un groupe**.
