---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Statuts personnalisés dans un groupe déplacé ou supprimé
description: Cet article explique ce qu’il advient des états personnalisés de groupe lorsque vous déplacez ou supprimez un groupe.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Statuts personnalisés dans un groupe déplacé ou supprimé

Cet article explique ce qu’il advient des états personnalisés de groupe lorsque vous déplacez ou supprimez un groupe.

## Statuts personnalisés dans un groupe déplacé

Tenez compte des scénarios suivants qui décrivent ce qu’il advient des états personnalisés d’un groupe lorsque vous le déplacez vers un nouvel emplacement sous un autre groupe.

Pour plus d’informations sur le déplacement d’un groupe, voir [Déplacer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Lorsque vous déplacez un groupe sous un autre groupe </td> 
   <td> <p>Tous les statuts du groupe déplacé restent inchangés. Ils ne sont pas ajoutés aux états du nouveau groupe parent du groupe.</p> <p>Mais le groupe déplacé hérite des états verrouillés du groupe ou des groupes qui sont désormais plus élevés dans sa hiérarchie. Désormais, si un administrateur verrouille un état plus haut dans la hiérarchie, le groupe déplacé hérite de cet état.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Lorsqu’un état dans les deux groupes possède les mêmes attributs clés mais différents</td> 
   <td> <p>Supposons que deux sous-groupes différents héritent du même état déverrouillé d’un groupe parent. Les administrateurs de groupe des deux groupes personnalisent ensuite l’état de leurs groupes de différentes manières.</p> <p>Par la suite, l’un des deux groupes est déplacé sous l’autre. Maintenant, ils ont tous deux un statut avec la même clé, mais il a des attributs différents dans les deux groupes.</p> <p>Dans ce cas, l’une des conditions suivantes est vraie :</p> 
    <ul> 
     <li>Si l’état du nouveau groupe parent est déverrouillé, l’état du groupe déplacé conserve ses attributs, sans être affecté par le déplacement.</li> 
     <li>Si l’état du nouveau groupe parent est verrouillé, les attributs du statut dans le groupe parent remplacent ceux du statut dans le groupe déplacé.</li> 
    </ul> <p>Pour plus d’informations sur les clés d’état, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Création ou modification d’un état</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Lorsqu’un groupe déplacé a des états hérités de son groupe parent précédent </td> 
   <td> <p>Tous les états personnalisés hérités du groupe parent précédent sont fournis avec le groupe déplacé et deviennent ses propres états personnalisés. Ils ne sont plus connectés au groupe parent précédent.</p> 
    <ul> 
     <li>Si le groupe parent précédent modifie un état personnalisé verrouillé après le déplacement, les modifications n’affectent pas l’état du sous-groupe déplacé.</li> 
     <li>Si le groupe parent précédent verrouille un état personnalisé qui était déverrouillé lors du déplacement du groupe, l’état du sous-groupe déplacé n’est pas verrouillé.</li> 
     <li>Le groupe déplacé peut désormais déverrouiller les états qui étaient verrouillés lorsqu’il les héritait du groupe parent précédent.</li> 
    </ul> 
     <p><b>EXEMPLE :</b><p> 
     <p>Olivia, l’administrateur du groupe Marketing, crée deux états pour le groupe. Elle cite une première critique, avec la clé ABC, et la verrouille. Elle désigne l’autre révision finale, avec la clé XYZ, et ne la verrouille pas.</p> 
     <p>Elle crée également un sous-groupe sous le groupe Marketing appelé Marketing des produits. Au moment de sa création, il hérite automatiquement de la Première révision et de la Révision finale du groupe Marketing.</p> 
     <p>Ultérieurement, Olivia déplace le sous-groupe Marketing produit sous le groupe Produit . Première révision et Révision finale : le groupe Marketing produit se trouve à son nouvel emplacement sous le groupe Produit .</p> 
     <p>Bien que la Première révision ait été verrouillée avant le déplacement, l’administrateur du groupe Marketing produit peut la modifier maintenant car il n’est plus un état hérité contrôlé par le groupe parent dont il provient.</p> 
     <p>La révision finale est déverrouillée et modifiable comme elle l’a toujours été.</p> 
     <p>Pour le groupe Marketing, Olivia change les couleurs Première révision et Révision finale et les renomme Première révision - Modifiée et Révision finale - Modifiée. Elle verrouille également Final Review-Edited. Pendant ce temps, dans le groupe Marketing des produits, les couleurs et les noms des états Première révision et Révision finale ne changent pas.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Statuts personnalisés dans un groupe supprimé

Lorsque vous supprimez un groupe ou un sous-groupe, vous réaffectez les informations qui lui sont associées, y compris ses statuts personnalisés, à un autre groupe ou sous-groupe. Les états du groupe supprimé sont ajoutés à ceux du groupe de destination.

Si l’un des statuts du groupe supprimé était également utilisé par le groupe de destination (l’état des deux groupes a la même clé) et que le groupe de destination a personnalisé l’état de différentes manières, les paramètres de la version du groupe de destination remplacent les paramètres de la version du groupe déplacé.

>[!INFO]
>
>**EXEMPLE :**
>
>L’administrateur du groupe A renomme un état de niveau système déverrouillé pour son groupe. L’administrateur de groupe d’un groupe B renomme également cet état pour son groupe. Bien que l’état porte des noms différents dans les deux groupes, il comporte la même clé.
>
>Par la suite, le groupe A est supprimé et toutes ses informations sont réaffectées au groupe B.
>
>* Le nom de la version Groupe B de l’état remplace celui de la version Groupe A.
>* Si l’état a été appliqué à un objet par une personne du groupe A avant la suppression de ce groupe, le nom de l’état sur l’objet est mis à jour par rapport au nom du statut utilisé par le groupe B.
>
>Pour plus d’informations sur la clé d’un état, reportez-vous au tableau de cet article sous [Créer ou modifier un état personnalisé](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [Créer ou modifier un état pour un groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>Pour plus d&#39;informations sur la suppression d&#39;un groupe, voir [Suppression d&#39;un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
