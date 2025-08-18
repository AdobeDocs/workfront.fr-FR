---
user-type: administrator
product-area: system-administration;user-management
keywords: ajouter,utilisateurs,utilisatrices,groupe,ajouter,autre,attribuer,administrateur,administratrice,supprimer,utilisateur,utilisatrice,afficher,rôles,membres,exporter,appartenance,données
navigation-topic: create-and-manage-groups
title: Afficher et gérer les adhésions d'un groupe
description: En tant qu’administrateur ou administratrice d’Adobe Workfront, vous pouvez afficher, ajouter, supprimer, exporter, activer et désactiver les personnes membres des groupes que vous gérez. Vous pouvez également modifier leur profil, ajouter des mises à jour à leur profil et les affecter en tant qu’administrateurs ou administratrices de groupes supplémentaires pour le groupe.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: 2096cfa0fd4d0e7eeb85dbf00668dc1dd7fb1d99
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 91%

---

# Consulter et gérer les appartenances à un groupe

En tant qu’administrateur ou administratrice d’Adobe Workfront, vous pouvez afficher, ajouter, supprimer, exporter, activer et désactiver les personnes membres des groupes que vous gérez. Vous pouvez également modifier leur profil, ajouter des mises à jour à leur profil et les affecter en tant qu’administrateurs ou administratrices de groupes supplémentaires pour le groupe.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs et administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

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

## Consulter et gérer les appartenances à un groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**.

   Dans la liste qui s’affiche, les administrateurs et administratrices de Workfront peuvent voir tous les groupes et sous-groupes. Les administrateurs et administratrices de groupes peuvent afficher uniquement les groupes et les sous-groupes qu’ils gèrent.

1. Cliquez sur le nom du groupe que vous souhaitez modifier.
1. Sur la page qui s’affiche, avec **Membres du groupe** sélectionné dans le menu de gauche, effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ajouter un utilisateur ou une utilisatrice au groupe</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Cliquez sur <strong>Ajouter des membres</strong> <img src="assets/add-icon-plus-in-circle.png">, commencez à saisir le nom de l’utilisateur ou de l’utilisatrice, puis sélectionnez-le lorsqu’il apparaît.</li> 
        <li value="2"> <p>Répétez cette opération pour les autres utilisateurs et utilisatrices que vous souhaitez ajouter.</p> <p>Vous pouvez cliquer sur le X situé à droite d’un nom si vous décidez de ne pas ajouter cet utilisateur ou cette utilisatrice.</p> </li> 
        <li value="3">Cliquez sur <strong>Terminé</strong> lorsque vous avez terminé.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer un utilisateur ou une utilisatrice du groupe</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Sélectionnez un ou plusieurs noms d’utilisateur ou d’utilisatrice, puis cliquez sur <strong>Supprimer une personne membre</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Cliquez sur <strong>Supprimer</strong> dans le message d’avertissement qui s’affiche.</p> <p>Vous pouvez trouver un utilisateur ou une utilisatrice à supprimer de la liste en cliquant sur <strong>Rechercher des personnes et des groupes dans la liste</strong>. Saisissez alors son nom dans la zone, puis sélectionnez-le lorsqu’il apparaît.</p> <p><b>REMARQUE</b> :  
          <ul> 
           <li>Si ce groupe est le groupe principal d’un utilisateur ou d’une utilisatrice que vous souhaitez supprimer, vous devez d’abord attribuer un autre groupe principal dans le profil de cette personne. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Vue d’ensemble des groupes principaux</a> et <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifier le profil d’un utilisateur ou d’une utilisatrice</a>.</li> 
           <li>Si le groupe n’a qu’un seul administrateur ou une seule administratrice de groupes et que vous devez le ou la supprimer du groupe, vous devez d’abord affecter un autre administrateur ou administratrice au groupe.</li> 
           <li>Un utilisateur ou une utilisatrice peut appartenir à un sous-groupe ainsi qu’au groupe parent. Lorsque vous supprimez une personne d’un sous-groupe, elle fait toujours partie du groupe parent. De même, lorsque vous la supprimez du groupe parent, elle reste membre du sous-groupe. Si vous ne souhaitez pas que l’accès soit autorisé à un utilisateur ou une utilisatrice pour le groupe parent, vous devez supprimer la personne des deux sous-groupes ainsi que du groupe parent, si elle est répertoriée aux deux endroits individuellement.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifier les informations de profil d’un utilisateur ou d’une utilisatrice</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Sélectionnez un ou plusieurs noms d’utilisateur, puis cliquez sur le <strong> </strong>Modifier<img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>Modifiez les informations de profil de l’utilisateur ou l’utilisatrice.</p> <p>Pour plus d’informations sur les modifications que vous pouvez apporter, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifier le profil d’un utilisateur ou d’une utilisatrice</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exporter les données d’appartenance de l’utilisateur ou l’utilisatrice</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Sélectionnez un ou plusieurs noms d’utilisateur, puis cliquez sur <strong>Exporter</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Exportez les données sous la forme d’un fichier PDF, Excel ou délimité par des tabulations.</p> <p>Pour plus d’informations sur l’exportation de données, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exporter des données</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher et modifier les rôles de groupe des membres</td> 
      <td> <p>La colonne <strong>Rôle du groupe</strong> répertorie le rôle de chaque personne membre. En tant qu’administrateur ou administratrice de groupes, vous pouvez double-cliquer sur le rôle d’une personne membre pour le modifier.</p> <p>Pour les membres du groupe qui ne sont pas des administrateurs ou administratrices de groupes, cette colonne n’est pas modifiable.</p> <p>Les administrateurs et les administratrices de groupes se trouvent toujours en haut de la liste.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envoyer un commentaire à des membres du groupe</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Sélectionnez au moins un membre du groupe, puis cliquez sur <strong>Envoyer la mise à jour à l’utilisateur</strong> dans la barre d’outils.</li> 
        <li value="2"><p>Saisissez le commentaire à envoyer aux personnes et à la zone Mises à jour de leurs profils.</p>
        <p>Pour plus d’informations, voir <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">Envoi de messages directs à d’autres utilisateurs</a>.</p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activer un utilisateur ou une utilisatrice dans Workfront</td> 
      <td>Sélectionnez une ou plusieurs personnes inactives, puis cliquez sur <strong>Activer l’utilisateur ou l’utilisatrice</strong> pour l’activer dans Workfront. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Désactiver un utilisateur ou une utilisatrice dans Workfront</td> 
      <td>Sélectionnez une ou plusieurs personnes actives, puis cliquez sur <strong>Désactiver l’utilisateur ou l’utilisatrice</strong><img src="assets/deactivate-user.png"> pour la désactiver dans Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Trier par colonne</td> 
      <td>Cliquez sur l’en-tête d’une colonne pour trier la liste en fonction du contenu de cette colonne.</td> 
     </tr> 
    </tbody> 
   </table>
