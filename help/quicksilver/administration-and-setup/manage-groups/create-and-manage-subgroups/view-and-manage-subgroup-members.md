---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Affichage et gestion des membres de sous-groupe
description: Lorsque vous affichez un groupe que vous gérez, vous pouvez afficher et gérer tous les utilisateurs des sous-groupes du groupe.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 32%

---

# Afficher et gérer les personnes membres d’un sous-groupe

Lorsque vous affichez un groupe que vous gérez, vous pouvez afficher et gérer tous les utilisateurs des sous-groupes du groupe.

S’il existe des groupes au-dessus du groupe que vous gérez, leur équipe d’administration peut également le faire pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

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
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Éditer l’accès des utilisateurs, avec l’option Administration utilisateur (tous les utilisateurs) sélectionnée</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur Workfront.

+++

## Afficher et gérer les membres des sous-groupes sous un groupe

{{step-1-to-setup}}

1. Cliquez sur **Groups**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils possèdent. Les administrateurs Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe pour lequel vous souhaitez afficher ou gérer les membres du sous-groupe.
1. Dans le panneau de gauche, cliquez sur **Subgroup Members**.

   Cet élément de panneau de gauche n’est disponible que si le groupe comporte des sous-groupes.

1. Effectuez l’une des opérations suivantes :

   * Sélectionnez un membre dans la liste, puis cliquez sur Modifier ![](assets/edit-icon.png) pour modifier le profil utilisateur de cette personne.

     Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) ou [Modification des profils utilisateur en masse](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * Sélectionnez un nombre quelconque de membres dans la liste, puis cliquez sur Mettre à jour ![](assets/comment-icon.png) pour ajouter un commentaire à leurs profils utilisateur.

     L’utilisateur ou les utilisateurs reçoivent une notification intégrée (in-app) ainsi qu’une notification par e-mail avec votre commentaire. Le commentaire s’affiche dans la zone Mises à jour du profil de l’utilisateur.

   * Sélectionnez un nombre quelconque de membres dans la liste, puis cliquez sur Désactiver ![](assets/deactivate-user.png) ou sur Activer ![](assets/activate-user.png).

     Pour plus d’informations, voir [Désactivation ou réactivation d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Exportez ![](assets/export.png) la liste des membres.
