---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Verrouillage ou déverrouillage d’un projet, d’une tâche ou d’une préférence d’émission pour les sous-groupes
description: En tant qu’administrateur de groupe, vous pouvez configurer, puis verrouiller un projet, une tâche ou une préférence d’émission si un administrateur Workfront l’a déverrouillé au niveau du système.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Verrouillage ou déverrouillage d’un projet, d’une tâche ou d’une préférence d’émission pour les sous-groupes

En tant qu’administrateur de groupe, vous pouvez configurer, puis verrouiller un projet, une tâche ou une préférence d’émission si un administrateur Workfront l’a déverrouillé au niveau du système.

Le verrouillage d’un projet, d’une tâche ou d’une préférence d’émission que vous avez configurée au niveau garantit que tous les membres de votre groupe et de ses sous-groupes utilisent le même paramètre pour cette préférence. Bien que vous puissiez toujours reconfigurer une préférence que vous verrouillez pour votre groupe, les administrateurs de groupe ne peuvent pas la reconfigurer pour les groupes.

Inversement, le déverrouillage d’un projet, d’une tâche ou d’une préférence de problème offre aux administrateurs de groupe une plus grande flexibilité pour gérer la manière dont leurs groupes fonctionnent avec ces éléments. Lorsqu’une préférence est déverrouillée, les administrateurs de groupe peuvent la reconfigurer pour ces sous-groupes.

Cela est parallèle à la possibilité qu’un administrateur de Workfront doit verrouiller ou déverrouiller une préférence pour tous les utilisateurs du système.

Pour plus d’informations sur la façon dont un administrateur Workfront peut verrouiller ou déverrouiller une préférence pour tous les groupes du système, voir [Verrouillage ou déverrouillage des préférences de projet pour tous les groupes du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* La configuration d’une préférence déverrouillée pour un groupe n’affecte pas cette préférence pour les sous-groupes situés sous le groupe.
>
>  Cependant, lorsqu’un nouveau sous-groupe est créé, il hérite des paramètres de préférence et de l’état verrouillé ou déverrouillé du groupe immédiatement au-dessus.
>
>* Si vous déplacez un groupe sous un groupe ayant une préférence verrouillée, le groupe déplacé hérite de cette préférence et elle est verrouillée pour le groupe déplacé.
>* Si vous déplacez un groupe sous un groupe avec une préférence déverrouillée, le groupe déplacé n’est pas affecté par cette préférence.
>
>  Si la préférence du groupe déplacé est verrouillée au moment du déplacement, elle l’est toujours, mais l’administrateur du groupe peut la déverrouiller maintenant car elle est déverrouillée pour le groupe parent.

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

## Verrouillage ou déverrouillage d’un projet de groupe, d’une tâche ou d’une préférence d’émission

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes**.
1. Cliquez sur le nom du groupe dans lequel vous souhaitez verrouiller ou déverrouiller une préférence de projet.
1. Dans le panneau de gauche, cliquez sur **Préférences du projet** ou **Tâches et préférences relatives aux problèmes**.

1. Sur la page qui s’affiche, effectuez l’une des opérations suivantes pour une préférence déverrouillée au niveau du système ou pour un groupe situé au-dessus de votre groupe :

   * Si vous souhaitez que les administrateurs des groupes situés sous votre groupe puissent configurer une préférence pour leurs groupes, déverrouillez-la. ![](assets/unlock-toggle-button.png).
   * Si vous souhaitez que tous les groupes situés sous le vôtre utilisent votre configuration pour une préférence, assurez-vous qu’elle est verrouillée. ![](assets/lock-toggle-button.png).

      >[!IMPORTANT]
      >
      >Il est important de communiquer avec les administrateurs et les utilisateurs des groupes situés sous les vôtres pour vous assurer que tous les besoins sont pris en compte dans la configuration d’une préférence verrouillée. Lorsque vous la verrouillez, votre configuration pour elle est héritée par tous les sous-groupes ci-dessous. Et si la préférence a été déverrouillée pendant une période quelconque, votre configuration remplace celles que les administrateurs de groupe dans les sous-groupes inférieurs ont pu faire.

1. Cliquer sur **Enregistrer**.
