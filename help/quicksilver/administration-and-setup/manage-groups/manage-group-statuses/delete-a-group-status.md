---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Suppression d’un état de groupe
description: En tant qu’administrateur de groupe, vous pouvez supprimer l’état d’un groupe que vous gérez s’il n’est pas configuré comme obligatoire ou verrouillé au niveau du système ou pour un groupe supérieur dans la hiérarchie.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 18%

---

# Supprimer le statut d’un groupe

En tant qu’administrateur de groupe, vous pouvez supprimer l’état d’un groupe que vous gérez s’il n’est pas configuré comme obligatoire ou verrouillé au niveau du système ou pour un groupe supérieur dans la hiérarchie.

S’il existe des groupes au-dessus du groupe que vous gérez, leur équipe d’administration peut également le faire pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

>[!NOTE]
>
>Vous ne pouvez pas supprimer les éléments suivants :
>
>* Les états intégrés Planification, Actuel et Terminé. Vous pouvez mettre à jour leurs noms, modifier leurs couleurs, les verrouiller ou les déverrouiller, mais ils ne peuvent pas être supprimés.
>* États dont l’état est en attente de validation pour au moins un objet associé au groupe ou à l’un de ses sous-groupes.

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

## Supprimer le statut d’un groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**.
1. Cliquez sur le nom du groupe de niveau supérieur.
1. Dans le panneau de gauche, cliquez sur **États**.
1. Dans la liste des états qui s’affiche, passez la souris sur l’état que vous souhaitez supprimer, puis cliquez sur **Supprimer** lorsqu’il s’affiche à l’extrême droite.

   ![](assets/hover-click-delete.jpg)

1. Dans la zone qui s’affiche, sélectionnez un état pour désigner un état de remplacement pour les objets (projets, tâches, problèmes et processus d’approbation) qui utilisaient l’état que vous supprimez.

   Seuls les états correspondant au statut que vous supprimez sont disponibles. Par exemple, si vous supprimez un état qui correspond à Actuel, vous ne pouvez afficher que les états qui correspondent à Actuel.

   En outre, les états qui s’affichent dépendent du déverrouillage ou du verrouillage de l’état que vous supprimez :

   * **S’il est déverrouillé** : les états verrouillés et déverrouillés non masqués sont disponibles.

     Outre les états créés pour le sous-groupe, les états hérités des groupes de niveau système et supérieur sont inclus.

   * **S’il est verrouillé** : l’une des conditions suivantes est vraie :

      * S’il existe d’autres états verrouillés et non masqués, seuls ces états sont disponibles.
      * S’il n’existe aucun état verrouillé non masqué, l’état Workfront par défaut est disponible, même s’il est masqué ou déverrouillé.

        Pour plus d’informations sur les états Workfront par défaut, voir [Accès à la liste des états du projet système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [Accès à la liste des états des tâches système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md) et les informations sur les 4 états des problèmes requis dans [Accès à la liste des états des problèmes système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Cliquez sur **Supprimer l’état**.

   Si le statut supprimé était le statut par défaut de ce type dans le groupe, le statut de remplacement prend sa place.

   Si l’état supprimé a été défini comme état par défaut du projet dans les préférences du projet, la préférence est désormais définie sur le statut de remplacement.

## Lorsqu’un groupe est supprimé

Lorsqu’un groupe est supprimé et remplacé par un autre groupe, tous les états uniques du groupe supprimé sont ajoutés aux états du groupe de remplacement. Pour plus d’informations, voir [Statuts personnalisés dans un groupe qui est déplacé ou supprimé](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
