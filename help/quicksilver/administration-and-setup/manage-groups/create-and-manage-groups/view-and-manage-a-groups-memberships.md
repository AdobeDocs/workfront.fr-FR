---
user-type: administrator
product-area: system-administration;user-management
keywords: add,users,group,add,another,assign,administrator,remove,user,view,rôles,membres,export,membership,data
navigation-topic: create-and-manage-groups
title: Affichage et gestion des adhésions d’un groupe
description: En tant qu’administrateur Adobe Workfront, vous pouvez afficher, ajouter, supprimer, exporter, activer et désactiver les membres de n’importe quel groupe que vous gérez. Vous pouvez également modifier leurs profils, ajouter des mises à jour à leurs profils et les affecter en tant qu’administrateurs de groupe supplémentaires au groupe.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 16%

---

# Consulter et gérer les appartenances à un groupe

En tant qu’administrateur Adobe Workfront, vous pouvez afficher, ajouter, supprimer, exporter, activer et désactiver les membres de n’importe quel groupe que vous gérez. Vous pouvez également modifier leurs profils, ajouter des mises à jour à leurs profils et les affecter en tant qu’administrateurs de groupe supplémentaires au groupe.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs ou administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

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

## Consulter et gérer les appartenances à un groupe

{{step-1-to-setup}}

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
        <li value="1">Sélectionnez un ou plusieurs noms d’utilisateur, puis cliquez sur <strong>Supprimer le membre</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Cliquez sur <strong>Supprimer</strong> dans le message d’avertissement qui s’affiche.</p> <p>Vous pouvez trouver un utilisateur que vous souhaitez supprimer de la liste en cliquant sur <strong>Rechercher des personnes et des groupes dans la liste</strong>, en saisissant leur nom dans la zone, puis en cliquant sur le nom lorsqu’il s’affiche.</p> <p><b>NOTE</b> :  
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
        <li value="2"> <p>Modifiez les informations de profil de l’utilisateur.</p> <p>Pour plus d'informations sur les modifications que vous pouvez apporter, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d'un utilisateur</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportation des données d’adhésion des utilisateurs</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Sélectionnez un ou plusieurs noms d’utilisateur, puis cliquez sur <strong>Export</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Exportez les données sous la forme d’un fichier délimité par des PDF, Excel ou des tabulations.</p> <p>Pour plus d'informations sur l'export de données, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Export de données</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Affichage et modification des rôles de groupe des membres</td> 
      <td> <p>La colonne <strong>Rôle de groupe</strong> répertorie le rôle de chaque membre. En tant qu’administrateur de groupe, vous pouvez double-cliquer sur le rôle d’un membre pour le modifier.</p> <p>Pour les membres du groupe qui ne sont pas des administrateurs de groupe, cette colonne n’est pas modifiable.</p> <p>Les administrateurs de groupe se trouvent toujours en haut de la liste.</p> </td> 
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
      <td>Sélectionnez un ou plusieurs utilisateurs actifs, puis cliquez sur <strong>Désactiver l’utilisateur</strong><img src="assets/deactivate-user.png"> pour les désactiver dans Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tri par colonne</td> 
      <td>Cliquez sur l’en-tête d’une colonne pour trier la liste en fonction du contenu de cette colonne.</td> 
     </tr> 
    </tbody> 
   </table>
