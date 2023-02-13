---
user-type: administrator
product-area: system-administration;user-management
keywords: add,users,group,add,another,assign,administrator,remove,user,view,rôles,membres,export,membership,data
navigation-topic: create-and-manage-groups
title: Affichage et gestion des appartenances d’un groupe
description: En tant qu’administrateur Adobe Workfront, vous pouvez afficher, ajouter, supprimer, exporter, activer et désactiver les membres de n’importe quel groupe que vous gérez. Vous pouvez également modifier leurs profils, ajouter des mises à jour à leurs profils et les affecter en tant qu’administrateurs de groupe supplémentaires au groupe.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# Affichage et gestion des appartenances d’un groupe

En tant qu’administrateur Adobe Workfront, vous pouvez afficher, ajouter, supprimer, exporter, activer et désactiver les membres de n’importe quel groupe que vous gérez. Vous pouvez également modifier leurs profils, ajouter des mises à jour à leurs profils et les affecter en tant qu’administrateurs de groupe supplémentaires au groupe.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur de groupe du groupe ou un administrateur Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Affichage et gestion des appartenances d’un groupe

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes**.

   Dans la liste qui s’affiche, les administrateurs de Workfront peuvent voir tous les groupes et sous-groupes. Les administrateurs de groupe peuvent afficher uniquement les groupes et les sous-groupes qu’ils gèrent.

1. Cliquez sur le nom du groupe que vous souhaitez modifier.
1. Sur la page qui s’affiche, avec **Membres du groupe** sélectionné dans le menu de gauche, effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ajout d’un utilisateur au groupe</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Cliquez sur <strong>Ajouter des membres</strong> <img src="assets/add-icon-plus-in-circle.png">, commencez à saisir le nom de l’utilisateur, puis sélectionnez-le lorsqu’il apparaît.</li> 
        <li value="2"> <p>Répétez cette opération pour tous les autres utilisateurs que vous souhaitez ajouter.</p> <p>Vous pouvez cliquer sur le X situé à droite d’un nom si vous décidez de ne pas ajouter cet utilisateur.</p> </li> 
        <li value="3">Cliquez sur <strong>Terminé</strong> lorsque vous avez terminé.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suppression d’un utilisateur du groupe</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Sélectionnez un ou plusieurs noms d’utilisateur, puis cliquez sur <strong>Supprimer un membre</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Cliquez sur <strong>Supprimer</strong> dans le message d’avertissement qui s’affiche.</p> <p>Vous pouvez trouver un utilisateur que vous souhaitez supprimer de la liste en cliquant sur <strong>Recherche de personnes et de groupes dans la liste</strong>, saisissez leur nom dans la zone, puis cliquez sur le nom lorsqu’il apparaît.</p> <p><b>NOTE</b>:  
          <ul> 
           <li>Si ce groupe est le groupe d’accueil d’un utilisateur que vous souhaitez supprimer, vous devez d’abord attribuer un autre groupe d’accueil dans le profil de l’utilisateur. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Présentation des groupes d’accueil</a> et <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur</a>.</li> 
           <li>Si le groupe n’a qu’un seul administrateur de groupe et que vous devez le supprimer du groupe, vous devez d’abord affecter un autre administrateur de groupe au groupe.</li> 
           <li>Un utilisateur peut appartenir à un sous-groupe et au groupe parent. Lorsque vous supprimez une personne d’un sous-groupe, elle fait toujours partie du groupe parent. De même, lorsque vous les supprimez du groupe parent, ils restent membres du sous-groupe. Si vous ne souhaitez pas que l’accès soit autorisé à un utilisateur pour le groupe parent, vous devez supprimer l’utilisateur des deux sous-groupes ainsi que du groupe parent, s’il est répertorié aux deux endroits individuellement.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modification des informations de profil d’un utilisateur</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Sélectionnez un ou plusieurs noms d’utilisateur, puis cliquez sur <strong>Modifier</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>Modifiez les informations de profil de l’utilisateur.</p> <p>Pour plus d’informations sur les modifications que vous pouvez apporter, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportation des données d’adhésion des utilisateurs</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Sélectionnez un ou plusieurs noms d’utilisateur, puis cliquez sur <strong>Exporter</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Exportez les données sous la forme d’un fichier séparé par des tabulations, Excel ou PDF.</p> <p>Pour plus d’informations sur l’export de données, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exporter des données</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Affichage et modification des rôles de groupe des membres</td> 
      <td> <p>Le <strong>Rôle du groupe</strong> répertorie le rôle de chaque membre. En tant qu’administrateur de groupe, vous pouvez double-cliquer sur le rôle d’un membre pour le modifier.</p> <p>Pour les membres du groupe qui ne sont pas des administrateurs de groupe, cette colonne n’est pas modifiable.</p> <p>Les administrateurs de groupe se trouvent toujours en haut de la liste.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envoyer un commentaire aux membres du groupe</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Sélectionnez un ou plusieurs noms d’utilisateur, puis cliquez sur <strong>Mettre à jour</strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">Saisissez le commentaire.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activation d’un utilisateur dans Workfront</td> 
      <td>Sélectionnez un ou plusieurs utilisateurs inactifs, puis cliquez sur <strong>Activer l’utilisateur</strong> pour les activer dans Workfront. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Désactivation d’un utilisateur dans Workfront</td> 
      <td>Sélectionnez un ou plusieurs utilisateurs principaux, puis cliquez sur <strong>Désactiver l’utilisateur</strong><img src="assets/deactivate-user.png"> pour les désactiver dans Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tri par colonne</td> 
      <td>Cliquez sur l’en-tête d’une colonne pour trier la liste en fonction du contenu de cette colonne.</td> 
     </tr> 
    </tbody> 
   </table>
