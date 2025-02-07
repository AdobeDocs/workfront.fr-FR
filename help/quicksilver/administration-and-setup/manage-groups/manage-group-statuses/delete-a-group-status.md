---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Supprimer un statut de groupe
description: En tant qu’administrateur ou administratrice de groupe, vous pouvez supprimer le statut d’un groupe que vous gérez s’il n’est pas configuré comme obligatoire ou verrouillé au niveau du système ou pour un groupe supérieur dans la hiérarchie.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 96%

---

# Supprimer le statut d’un groupe

En tant qu’administrateur ou administratrice de groupe, vous pouvez supprimer le statut d’un groupe que vous gérez s’il n’est pas configuré comme obligatoire ou verrouillé au niveau du système ou pour un groupe supérieur dans la hiérarchie.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

>[!NOTE]
>
>Vous ne pouvez pas supprimer les éléments suivants :
>
>* Les statuts intégrés Planification, Actif et Terminé. Vous pouvez mettre à jour leurs noms, modifier leurs couleurs, les verrouiller ou les déverrouiller, mais ils ne peuvent pas être supprimés.
>* Statuts qui sont en cours d’approbation pour au moins un objet associé au groupe ou à l’un de ses sous-groupes.

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

## Supprimer le statut d’un groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**.
1. Cliquez sur le nom du groupe de niveau supérieur.
1. Dans le panneau de gauche, cliquez sur **Statuts**.
1. Dans la liste des statuts qui s’affiche, pointez sur le statit que vous souhaitez supprimer, puis cliquez sur **Supprimer** quand il apparaît à l’extrême droite.

   ![Supprimer](assets/hover-click-delete.jpg)

1. Dans la boîte qui s’affiche, sélectionnez un statut pour désigner un statut de remplacement pour les objets (projets, tâches, problèmes et processus d’approbation) qui utilisaient le statut que vous supprimez.

   Seuls les statuts correspondant au statut que vous supprimez sont disponibles. Par exemple, si vous supprimez un statut qui correspond à Actif, vous ne pouvez afficher que les statuts qui correspondent à Actif.

   En outre, les statuts qui s’affichent dépendent du déverrouillage ou du verrouillage du statut que vous supprimez :

   * **S’il est déverrouillé** : les statuts verrouillés et déverrouillés non masqués sont disponibles.

     Outre les statuts créés pour le sous-groupe, les statuts hérités des groupes de niveau système et de niveau supérieur sont inclus.

   * **S’il est verrouillé** : l’une des conditions suivantes est vraie :

      * S’il existe d’autres statuts verrouillés et non masqués, seuls ces statuts sont disponibles.
      * S’il n’existe aucun statut verrouillé non masqué, le statut Workfront par défaut est disponible, même s’il est masqué ou déverrouillé.

        Pour plus d’informations sur les statuts Workfront par défaut, voir [Accéder à la liste des statuts des projets système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [Accéder à la liste des statuts des tâches système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)et les informations sur les 4 statuts de problème requis dans [Accéder à la liste des statuts des problèmes système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Cliquez sur **Supprimer un statut**.

   Si le statut supprimé était le statut par défaut de ce type dans le groupe, le statut de remplacement prend sa place.

   Si le statut supprimé a été défini comme statut par défaut du projet dans les préférences du projet, la préférence est désormais définie sur le statut de remplacement.

## Lorsqu’un groupe est supprimé

Lorsqu’un groupe est supprimé et remplacé par un autre groupe, tous les statuts uniques du groupe supprimé sont ajoutés aux statuts du groupe de remplacement. Pour plus d’informations, voir [Personnaliser les statuts dans un groupe déplacé ou supprimé](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
