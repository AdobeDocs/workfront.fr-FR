---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Statuts personnalisés dans un groupe déplacé ou supprimé
description: Cet article explique ce qu’il advient des statuts personnalisés des groupes lorsque vous déplacez ou supprimez un groupe.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 98%

---

# Statuts personnalisés dans un groupe déplacé ou supprimé

Cet article explique ce qu’il advient des statuts personnalisés des groupes lorsque vous déplacez ou supprimez un groupe.

## Statuts personnalisés dans un groupe déplacé

Les scénarios suivants décrivent ce qu’il advient des statuts personnalisés des groupes lorsque vous déplacez un groupe vers un nouvel emplacement sous un autre groupe.

Pour plus d’informations sur le déplacement d’un groupe, voir [Déplacer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Lorsque vous déplacez un groupe sous un autre groupe </td> 
   <td> <p>Tous les statuts du groupe déplacé sont conservés. Ils ne sont pas ajoutés aux statuts du nouveau groupe parent du groupe.</p> <p>Mais le groupe déplacé hérite de tous les statuts verrouillés dans le ou les groupes qui se trouvent désormais à un niveau supérieur dans sa hiérarchie. Désormais, si un administrateur ou une administratrice verrouille un statut plus haut dans la hiérarchie, le groupe déplacé hérite de ce statut.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Lorsqu’un statut dans les deux groupes a la même clé mais des attributs différents</td> 
   <td> <p>Supposons que deux sous-groupes différents héritent du même statut non verrouillé d’un groupe parent. Les administrateurs et administratrices des deux groupes personnalisent ensuite le statut de leur groupe de différentes manières.</p> <p>Plus tard, l’un des deux groupes est déplacé sous l’autre. Ils ont maintenant tous les deux un statut avec la même clé, mais il y a des attributs différents dans les deux groupes.</p> <p>Dans ce cas, l’une des affimations suivantes est vraie :</p> 
    <ul> 
     <li>Si le statut du nouveau groupe parent est déverrouillé, le statut du groupe déplacé conserve ses attributs, sans être affecté par le déplacement.</li> 
     <li>Si le statut du nouveau groupe parent est verrouillé, les attributs du statut du groupe parent remplacent ceux du statut du groupe déplacé.</li> 
    </ul> <p>Pour plus d’informations sur les clés de satut, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Créer ou modifier un statut</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Lorsqu’un groupe déplacé a des statuts hérités de son ancien groupe parent </td> 
   <td> <p>Tous les statuts personnalisés hérités du groupe parent précédent sont intégrés au groupe déplacé et deviennent ses propres statuts personnalisés. Ils ne sont plus liés à l’ancien groupe parent.</p> 
    <ul> 
     <li>Si le groupe parent précédent modifie un statut personnalisé verrouillé après le déplacement, les modifications n’affectent pas le statut du sous-groupe déplacé.</li> 
     <li>Si le groupe parent précédent verrouille un statut personnalisé qui a été déverrouillé lors du déplacement du groupe, le statut du sous-groupe déplacé n’est pas verrouillé.</li> 
     <li>Le groupe déplacé peut désormais déverrouiller les statuts qui étaient verrouillés lorsqu’il les a hérités du groupe parent précédent.</li> 
    </ul> 
     <p><b>EXEMPLE</b><p> 
     <p>Olivia, l’administratrice du groupe Marketing, crée deux statuts pour le groupe. Elle en nomme un Première révision, avec la clé ABC, et le verrouille. Elle nomme l’autre Révision finale, avec la clé XYZ, et ne le verrouille pas.</p> 
     <p>Elle crée également un sous-groupe dans le groupe Marketing, appelé Marketing produit. Au moment où il est créé, il hérite automatiquement à la fois des statuts Première révision et Révision finale du groupe Marketing.</p> 
     <p>Plus tard, Olivia déplace le sous-groupe Marketing produit sous le groupe Produit. Les satuts Première révision et Révision finale accompagnent le groupe Marketing produit dans son nouvel emplacement dans le groupe Produit.</p> 
     <p>Bien que le statut Première révision ait été verrouillé avant le transfert, l’administrateur ou administratrice du groupe Marketing produit peut désormais le modifier, car il ne s’agit plus d’un statut hérité contrôlé par le groupe parent dont il est issu.</p> 
     <p>Le statut Révision finale est déverrouillé et modifiable comme il l’a toujours été.</p> 
     <p>Pour le groupe Marketing, Olivia modifie les couleurs des statuts Première révision et Révision finale et renomme ces derniers Première révision-modifiée et Révision finale-modifiée. Elle verrouille également Révision finale-modifiée. En revanche, dans le groupe Marketing produit, les couleurs et les noms des statuts Première révision et Révision finale ne changent pas.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Statuts personnalisés dans un groupe supprimé

Lorsque vous supprimez un groupe ou un sous-groupe, vous réaffectez les informations qui lui sont associées, y compris ses statuts personnalisés, à un autre groupe ou sous-groupe. Les statuts du groupe supprimé sont ajoutés à ceux du groupe de destination.

Si l’un des statuts du groupe supprimé était également utilisé par le groupe de destination (le statut dans les deux groupes a la même clé) et que le groupe de destination a personnalisé le statut de différentes manières, les paramètres de la version du groupe de destination remplacent les paramètres de la version du groupe déplacé.

>[!INFO]
>
>**EXEMPLE :**
>
>L’administrateur ou administratrice du groupe A renomme un statut de niveau système déverrouillé pour son groupe. L’administrateur ou administratrice d’un groupe B renomme également ce statut pour son groupe. Bien que le statut porte des noms différents dans les deux groupes, il a la même clé.
>
>Plus tard, le groupe A est supprimé et toutes ses informations sont réaffectées au groupe B.
>
>* Le nom de la version du groupe B du statut prévaut sur le nom de la version du groupe A.
>* Si le statut a été appliqué à un objet par un membre du groupe A avant que ce groupe ne soit supprimé, le nom du statut de l’objet est remplacé par le nom du statut utilisé par le groupe B.
>
>Pour plus d’informations sur la clé d’un statut, voir le tableau de cet article sous [Créer ou modifier un statut personnalisé](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [Créer ou modifier un statut pour un groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>Pour plus d’informations sur la suppression d’un groupe, voir [Supprimer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
