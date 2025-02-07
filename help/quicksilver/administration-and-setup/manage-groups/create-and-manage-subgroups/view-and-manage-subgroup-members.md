---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Afficher et gérer les membres des sous-groupes
description: Lorsque vous affichez un groupe que vous gérez, vous pouvez afficher et gérer tous les utilisateurs et utilisatrices des sous-groupes du groupe.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 75%

---

# Afficher et gérer des membres de sous-groupe

Lorsque vous affichez un groupe que vous gérez, vous pouvez afficher et gérer tous les utilisateurs et utilisatrices des sous-groupes du groupe.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

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
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès de l’administrateur système. </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-settings.png">. </p> <p>De ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher et gérer les membres des sous-groupes sous un groupe

{{step-1-to-setup}}

1. Cliquez sur **Groupes**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe pour lequel vous souhaitez afficher ou gérer les membres du sous-groupe.
1. Dans le panneau de gauche, cliquez sur **Membres du sous-groupe**.

   Cet élément du panneau de gauche n’est disponible que si le groupe comporte des sous-groupes.

1. Effectuez l’une des opérations suivantes :

   * Sélectionnez un membre dans la liste, puis cliquez sur Modifier ![icône Modifier](assets/edit-icon.png) pour modifier le profil utilisateur de cette personne.

     Pour plus d’informations, voir [Modifier le profil utilisateur/utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) ou [Modifier des profils utilisateur/utilisatrice en bloc](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * Sélectionnez un nombre illimité de membres dans la liste, puis cliquez sur Mettre à jour ![icône de commentaire](assets/comment-icon.png) pour ajouter un commentaire à leurs profils utilisateur.

     Les personnes reçoivent une notification in-app ainsi qu’une notification par e-mail avec votre commentaire. Le commentaire s’affiche dans la zone Mises à jour du profil de l’utilisateur ou de l’utilisatrice.

   * Sélectionnez un nombre quelconque de membres dans la liste, puis cliquez sur Désactiver ![Désactiver l’utilisateur](assets/deactivate-user.png) ou Activer ![Activer l’utilisateur](assets/activate-user.png).

     Pour plus d’informations, voir [Désactiver ou réactiver un utilisateur ou une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Exportez ![Exporter](assets/export.png) la liste des membres.
