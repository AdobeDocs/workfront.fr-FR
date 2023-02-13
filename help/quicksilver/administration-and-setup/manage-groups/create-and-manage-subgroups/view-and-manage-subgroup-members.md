---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Affichage et gestion des membres de sous-groupe
description: Lorsque vous affichez un groupe que vous gérez, vous pouvez afficher et gérer tous les utilisateurs des sous-groupes du groupe.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Affichage et gestion des membres de sous-groupe

Lorsque vous affichez un groupe que vous gérez, vous pouvez afficher et gérer tous les utilisateurs des sous-groupes du groupe.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

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
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Éditer l’accès des utilisateurs, avec l’option Administration utilisateur (tous les utilisateurs) sélectionnée</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur Workfront.

## Afficher et gérer les membres des sous-groupes sous un groupe

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Groupes**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils possèdent. Les administrateurs Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe pour lequel vous souhaitez afficher ou gérer les membres du sous-groupe.
1. Dans le panneau de gauche, cliquez sur **Membres du sous-groupe**.

   Cet élément de panneau de gauche n’est disponible que si le groupe comporte des sous-groupes.

1. Effectuez l’une des opérations suivantes :

   * Sélectionnez un membre dans la liste, puis cliquez sur Modifier . ![](assets/edit-icon.png) pour modifier le profil utilisateur de cette personne.

      Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) ou [Modification en masse des profils utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * Sélectionnez un nombre quelconque de membres dans la liste, puis cliquez sur Mettre à jour . ![](assets/comment-icon.png) pour ajouter un commentaire à leurs profils utilisateur.

      L’utilisateur ou les utilisateurs reçoivent une notification intégrée (in-app) ainsi qu’une notification par e-mail avec votre commentaire. Le commentaire s’affiche dans la zone Mises à jour du profil de l’utilisateur.

   * Sélectionnez un nombre quelconque de membres dans la liste, puis cliquez sur Désactiver . ![](assets/deactivate-user.png) ou Activer ![](assets/activate-user.png).

      Pour plus d’informations, voir [Désactivation ou réactivation d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Exporter ![](assets/export.png) la liste des membres.
