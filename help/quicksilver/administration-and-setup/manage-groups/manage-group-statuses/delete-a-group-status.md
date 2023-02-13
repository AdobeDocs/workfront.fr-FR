---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Suppression d’un état de groupe
description: En tant qu’administrateur de groupe, vous pouvez supprimer l’état d’un groupe que vous gérez s’il n’est pas configuré comme obligatoire ou verrouillé au niveau du système ou pour un groupe supérieur dans la hiérarchie.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Suppression d’un état de groupe

En tant qu’administrateur de groupe, vous pouvez supprimer l’état d’un groupe que vous gérez s’il n’est pas configuré comme obligatoire ou verrouillé au niveau du système ou pour un groupe supérieur dans la hiérarchie.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

>[!NOTE]
>
>Vous ne pouvez pas supprimer les éléments suivants :
>
>* Les états intégrés Planification, Actuel et Terminé. Vous pouvez mettre à jour leurs noms, modifier leurs couleurs, les verrouiller ou les déverrouiller, mais ils ne peuvent pas être supprimés.
>* États dont l’état est en attente de validation pour au moins un objet associé au groupe ou à l’un de ses sous-groupes.


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

## Suppression d’un état de groupe

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes**.
1. Cliquez sur le nom du groupe de niveau supérieur.
1. Dans le panneau de gauche, cliquez sur **Statuts**.
1. Dans la liste des statuts qui s’affiche, passez la souris sur l’état que vous souhaitez supprimer, puis cliquez sur **Supprimer** quand il apparaît à l&#39;extrême droite.

   ![](assets/hover-click-delete.jpg)

1. Dans la zone qui s’affiche, sélectionnez un état pour désigner un état de remplacement pour les objets (projets, tâches, problèmes et processus d’approbation) qui utilisaient l’état que vous supprimez.

   Seuls les états correspondant au statut que vous supprimez sont disponibles. Par exemple, si vous supprimez un état qui correspond à Actuel, vous ne pouvez afficher que les états qui correspondent à Actuel.

   En outre, les états qui s’affichent dépendent du déverrouillage ou du verrouillage de l’état que vous supprimez :

   * **S’il est déverrouillé**: Les états verrouillés et déverrouillés non masqués sont disponibles.

      Outre les états créés pour le sous-groupe, les états hérités des groupes de niveau système et supérieur sont inclus.

   * **Si c&#39;est verrouillé**: L’une des conditions suivantes est vraie :

      * S’il existe d’autres états verrouillés et non masqués, seuls ces états sont disponibles.
      * S’il n’existe aucun état verrouillé non masqué, l’état Workfront par défaut est disponible, même s’il est masqué ou déverrouillé.

         Pour plus d’informations sur les états Workfront par défaut, voir [Accéder à la liste des états du projet système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [Accéder à la liste des états des tâches système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)et les informations sur les 4 états de problème requis dans [Accéder à la liste des statuts des problèmes système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Cliquez sur **État de la suppression**.

   Si le statut supprimé était le statut par défaut de ce type dans le groupe, le statut de remplacement prend sa place.

   Si l’état supprimé a été défini comme état par défaut du projet dans les préférences du projet, la préférence est désormais définie sur le statut de remplacement.

## Lorsqu’un groupe est supprimé

Lorsqu’un groupe est supprimé et remplacé par un autre groupe, tous les états uniques du groupe supprimé sont ajoutés aux états du groupe de remplacement. Pour plus d’informations, voir [Statuts personnalisés dans un groupe déplacé ou supprimé](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
