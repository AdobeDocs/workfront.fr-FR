---
user-type: administrator
product-area: system-administration;user-management
keywords: créer,groupe,sous-groupe,nouveau
navigation-topic: create-and-manage-groups
title: Créer un groupe
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer des groupes pour organiser les personnes et les projets et pour attribuer des droits d’accès dans Workfront.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1656'
ht-degree: 91%

---

# Créer un groupe

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer des groupes pour organiser les personnes et les projets et pour attribuer des droits d’accès dans Workfront. Pour plus d’informations, voir [Vue d’ensemble des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Chaque sous-groupe a besoin d’au moins un administrateur ou une administratrice de groupes. Les administrateurs et administratrices de groupes peuvent utiliser la page Groupes pour gérer leurs groupes en un seul endroit.

Si vous faites partie de l’équipe d’administration de groupes ou Workfront, vous pouvez également créer des sous-groupes au sein d’un groupe. Pour les instructions, voir [Créer un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

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

## Créer un groupe de premier niveau à partir de zéro

Ces étapes expliquent comment créer un nouveau groupe à partir de zéro. Pour plus d’informations sur la création d’un groupe ou d’un sous-groupe par copie d’un groupe ou d’un sous-groupe existant, voir [Créer un groupe de premier niveau par copie d’un groupe ou d’un sous-groupe existant](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) dans cet article.

Vous devez faire partie de l’équipe d’administration de Workfront pour créer un groupe de premier niveau.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

1. Au-dessus de la liste des groupes, cliquez sur **Nouveau groupe**.

   >[!TIP]
   >
   >Au bas de la liste des groupes, vous pouvez également cliquer sur **Ajouter plus de groupes** pour ajouter un groupe en ligne, puis cliquez sur **Entrée** lorsque vous avez terminé d’ajouter les informations relatives au groupe.

1. Dans la boîte **Nouveau groupe** qui s’affiche, saisissez un nom pour le groupe.
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
      <td>Saisissez une description pour le groupe. Vous pouvez saisir jusqu’à 512 caractères.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Est active</td> 
      <td> <p>(Activé par défaut) Active le groupe dans votre instance Workfront.</p> <p>Dans les champs à remplissage automatique comme celui illustré ci-dessous, lorsque des utilisateurs et utilisatrices ordinaires recherchent un groupe pour le joindre à un objet ou pour partager un objet avec celui-ci, seuls les groupes actifs s’affichent dans la liste.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Pour simplifier cette opération pour vos utilisateurs et utilisatrices, vous pouvez désactiver l’option Est actif pour les groupes qui ne sont pas actuellement utilisés.</p> <p>Vous pouvez facilement afficher, filtrer et regrouper la liste des groupes en fonction de l’état actif ou inactif à l’aide de ce champ. Pour plus d’informations sur l’utilisation des vues, des filtres et des regroupements dans les listes, consultez <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Éléments de création de rapports : filtres, vues et regroupements</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendre ce groupe et ses sous-groupes publics</td> 
      <td> <p>(Disponible uniquement si vous affichez les détails d’un groupe de niveau supérieur, et non d’un sous-groupe.) Activez cette option pour permettre aux utilisateurs du groupe disposant d’un accès utilisateur en modification (qui ne sont pas administrateurs du groupe) d’ajouter ce groupe et ses sous-groupes au profil utilisateur d’autres utilisateurs.</p> <p>Pour un groupe public, toute personne (faisant partie ou non du groupe) disposant d’un accès d’édition peut ajouter le groupe au profil d’autres utilisateurs et utilisatrices. Cette personne ne peut pas effectuer cette action pour un groupe privé.</p> <p>Vous ne pouvez modifier cette option que pour le groupe parent situé au niveau le plus haut d’une hiérarchie de groupes à plusieurs niveaux. Tous les sous-groupes du groupe parent héritent de ce paramètre.</p> <p><b>NOTE</b> :  
        <ul> 
         <li>Vous ne pouvez pas rendre public un sous-groupe seul, mais vous pouvez rendre public son groupe parent de niveau supérieur, ce qui a pour effet de rendre également publics tous les sous-groupes du groupe parent.</li> 
         <li>Un sous-groupe appartenant à un groupe public est public par défaut. Par conséquent, toute personne disposant d’un accès en modification peut également ajouter le sous-groupe à d’autres utilisateurs et utilisatrices.</li> 
        </ul> </p> <p>Si vous avez besoin d’informations sur l’accès nécessaire pour modifier les personnes, reportez-vous à la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux personnes</a>. Pour plus d’informations sur la modification des personnes, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifier le profil d’une personne</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chef d’entreprise </td> 
      <td> <p>Vous pouvez désigner un utilisateur ou une utilisatrice responsable commercial d’un groupe que vous gérez. La ou le responsable commercial est la personne qui prend des décisions commerciales pour le groupe. Pour plus d’informations, voir l’article <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Vue d’ensemble des responsables commerciaux</a><span>.</span></p> <p>Si la personne n’est pas encore membre du groupe, l’ajout de son nom dans ce champ l’ajoute également au groupe.</p> <p><b>NOTE</b> :  
        <ul> 
         <li>avant de pouvoir retirer la ou le responsable commercial d’un groupe, vous devez supprimer son nom du champ Responsable commercial.</li> 
         <li>Si vous supprimez le nom du champ Responsable commercial, cette personne reste membre du groupe à moins que vous ne l’en retiriez. Pour savoir comment retirer une personne d’un groupe, voir la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Gérer les membres d’un groupe</a> dans l’article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Gérer un groupe</a>.</li> 
        </ul> </p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Vue d‘ensemble du rôle de chef d’entreprise</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membres du groupe et administrateurs de groupe</td> 
      <td>
        <p>Pour ajouter des membres à un groupe, commencez par taper le nom de la personne ou du groupe existant à ajouter, puis sélectionnez le nom lorsqu’il apparaît.</p> 
        <p>Les personnes et les groupes que vous ajoutez ont accès à tous les objets partagés avec le groupe.</p>
        <p>Un groupe de premier niveau doit avoir au moins un administrateur ou une administratrice de groupe. </p>
     </tr> 
     <tr> 
      <td role="rowheader">Rechercher des personnes et des groupes dans la liste</td> 
      <td> Si vous devez trouver un utilisateur, une utilisatrice ou un groupe déjà affecté à ce groupe, vous pouvez taper son nom ici et le sélectionner lorsqu’il apparaît.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Créer un groupe**.

## Créer un groupe de premier niveau en copiant un groupe ou un sous-groupe existant {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

En tant qu’administrateur ou administratrice Workfront, vous pouvez créer un nouveau groupe de premier niveau en copiant un groupe ou un sous-groupe existant.

Pour ce faire, gardez à l’esprit les éléments suivants :

* Tous les membres et tous les sous-groupes appartenant au groupe existant sont copiés dans le nouveau groupe de premier niveau.
* Les membres du groupe copié conservent les affectations qu’ils avaient dans le groupe d’origine. Par conséquent, l’équipe d’administration du groupe d’origine est également désignée comme équipe d’administration de groupe dans le groupe copié.

Pour créer un nouveau groupe de premier niveau en copiant un groupe ou un sous-groupe, procédez comme suit :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![groupes](assets/groups-icon.png).

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Sélectionnez le groupe à copier, puis cliquez sur l’icône Copier ![icône Copier](assets/copy-icon.png).
1. Dans la zone **Copier le groupe** qui s’affiche, saisissez un **Nom de groupe** pour le groupe copié.

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
      <td>Saisissez une description pour le groupe. Vous pouvez saisir jusqu’à 512 caractères.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Est active</td> 
      <td> <p>(Activé par défaut) Active le groupe dans votre instance Workfront.</p> <p>Dans les champs à remplissage automatique comme celui illustré ci-dessous, lorsque des utilisateurs et utilisatrices ordinaires recherchent un groupe pour le joindre à un objet ou pour partager un objet avec celui-ci, seuls les groupes actifs s’affichent dans la liste.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Pour simplifier cette opération pour vos utilisateurs et utilisatrices, vous pouvez désactiver l’option Est actif pour les groupes qui ne sont pas actuellement utilisés.</p> <p>Vous pouvez facilement afficher, filtrer et regrouper la liste des groupes en fonction de l’état actif ou inactif à l’aide de ce champ. Pour plus d’informations sur l’utilisation des vues, des filtres et des regroupements dans les listes, consultez <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Éléments de création de rapports : filtres, vues et regroupements</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rendre ce groupe et ses sous-groupes publics</td> 
      <td> <p>(Disponible uniquement si vous affichez les détails d’un groupe de niveau supérieur, et non d’un sous-groupe.) Activez cette option pour permettre aux utilisateurs du groupe disposant d’un accès utilisateur en modification (qui ne sont pas administrateurs du groupe) d’ajouter ce groupe et ses sous-groupes au profil utilisateur d’autres utilisateurs.</p> <p>Pour un groupe public, toute personne (faisant partie ou non du groupe) disposant d’un accès d’édition peut ajouter le groupe au profil d’autres utilisateurs et utilisatrices. Cette personne ne peut pas effectuer cette action pour un groupe privé.</p> <p>Vous ne pouvez modifier cette option que pour le groupe parent situé au niveau le plus haut d’une hiérarchie de groupes à plusieurs niveaux. Tous les sous-groupes du groupe parent héritent de ce paramètre.</p> <p><b>REMARQUE</b> :  
        <ul> 
         <li>Vous ne pouvez pas rendre public un sous-groupe seul, mais vous pouvez rendre public son groupe parent de niveau supérieur, ce qui a pour effet de rendre également publics tous les sous-groupes du groupe parent.</li> 
         <li>Un sous-groupe appartenant à un groupe public est public par défaut. Par conséquent, toute personne disposant d’un accès d’édition peut également ajouter le sous-groupe à d’autres utilisateurs et utilisatrices.</li> 
        </ul> </p> <p>Si vous avez besoin d’informations sur l’accès nécessaire pour modifier les personnes, reportez-vous à la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Accorder l’accès aux personnes</a>. Pour plus d’informations sur la modification des personnes, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Modifier le profil d’une personne</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chef d’entreprise </td> 
      <td> <p>Vous pouvez désigner un utilisateur ou une utilisatrice responsable commercial d’un groupe que vous gérez. La ou le responsable commercial est la personne qui prend des décisions commerciales pour le groupe. Pour plus d’informations, voir l’article <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Vue d’ensemble des responsables commerciaux</a><span>.</span></p> <p>Si la personne n’est pas encore membre du groupe, l’ajout de son nom dans ce champ l’ajoute également au groupe.</p> <p><b>NOTE</b> :  
        <ul> 
         <li>avant de pouvoir retirer la ou le responsable commercial d’un groupe, vous devez supprimer son nom du champ Responsable commercial.</li> 
         <li>Si vous supprimez le nom du champ Responsable commercial, cette personne reste membre du groupe à moins que vous ne l’en retiriez. Pour savoir comment retirer une personne d’un groupe, voir la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gérer les membres d’un groupe</a> dans l’article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Gérer un groupe</a>.</li> 
        </ul> </p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Vue d‘ensemble du rôle de chef d’entreprise</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membres du groupe et administrateurs de groupe</td> 
      <td> 
       <ul> 
        <li> <p>Membres du groupe : pour ajouter des personnes et des groupes au groupe, commencez à taper le nom d’une personne ou d’un groupe existant que vous souhaitez ajouter, puis sélectionnez le nom lorsqu’il apparaît.</p> <p>Les personnes et les groupes que vous ajoutez ont accès à tous les objets partagés avec le groupe.</p> </li> 
        <li> <p>Administrateurs et administratrices de groupe : les administrateurs et administratrices du groupe d’origine sont également désignés administrateurs et administratrices de groupe dans le groupe copié. Vous pouvez attribuer à une personne du groupe les droits d’administration de groupes à l’aide du menu déroulant situé à droite du nom de la personne.</p> <p>Un groupe de premier niveau doit avoir au moins un administrateur ou une administratrice de groupe.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rechercher des personnes et des groupes dans la liste</td> 
      <td> Si vous devez trouver un utilisateur, une utilisatrice ou un groupe déjà affecté à ce groupe, vous pouvez taper son nom ici et le sélectionner lorsqu’il apparaît.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Si le groupe d’origine comporte des sous-groupes, ceux-ci sont ajoutés au nouveau groupe et leur nom est, par défaut, « Nom du sous-groupe d’origine (Copie) ».
   >* Vous pouvez retirer une personne ou un sous-groupe du groupe d’origine en cliquant sur le X à droite de son nom.

1. Cliquez sur **Créer un groupe**.
