---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Verrouillage ou déverrouillage d’un projet, d’une tâche ou d’une préférence de problème pour les sous-groupes
description: En tant qu’administrateur ou administratrice de groupes, vous pouvez configurer puis verrouiller une préférence de projet, de tâche ou de problème si un administrateur ou une administratrice Workfront l’a déverrouillée au niveau du système.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 95%

---

# Verrouiller ou déverrouiller une préférence de projet, de tâche ou de problème pour les sous-groupes

En tant qu’administrateur ou administratrice de groupes, vous pouvez configurer puis verrouiller une préférence de projet, de tâche ou de problème si un administrateur ou une administratrice Workfront l’a déverrouillée au niveau du système.

Le verrouillage d’une préférence de projet, de tâche ou de problème que vous avez configurée à ce niveau garantit que toutes les personnes membres de votre groupe et de ses sous-groupes utilisent le même paramètre pour cette préférence. Bien que vous puissiez toujours reconfigurer une préférence que vous verrouillez pour votre groupe, les administrateurs et administratrices de groupes ne peuvent pas la reconfigurer pour les groupes.

À l’inverse, le déverrouillage d’une préférence de projet, de tâche ou de problème permet aux administrateurs et administratrices de groupe de gérer avec plus de souplesse la manière dont leurs groupes utilisent ces éléments. Lorsqu’une préférence est déverrouillée, les administrateurs et administratrices de groupes peuvent la reconfigurer pour ces sous-groupes.

De même, les administrateurs et administratrices de Workfront doivent verrouiller ou déverrouiller une préférence pour toutes les personnes du système.

Pour plus d’informations sur la façon dont un administrateur ou administratrice Workfront peut verrouiller ou déverrouiller une préférence pour tous les groupes du système, voir [Verrouiller ou déverrouiller des préférences de projet pour tous les groupes du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* La configuration d’une préférence déverrouillée pour un groupe n’affecte pas cette préférence pour les sous-groupes situés sous le groupe.
>
>  Cependant, lorsqu’un nouveau sous-groupe est créé, il hérite des paramètres de la préférence et du statut verrouillé ou déverrouillé du groupe situé immédiatement au-dessus.
>
>* Si vous déplacez un groupe sous un groupe ayant une préférence verrouillée, le groupe déplacé hérite de cette préférence et elle est verrouillée pour le groupe déplacé.
>* Si vous déplacez un groupe sous un groupe avec une préférence déverrouillée, le groupe déplacé n’est pas affecté par cette préférence.
>
>  Si la préférence du groupe déplacé est verrouillée au moment du déplacement, son statut n’est pas modifié, mais l’administrateur ou l’administratrice du groupe peut à présent déverrouiller cette préférence, car elle est déverrouillée pour le groupe parent.

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

## Verrouiller ou déverrouiller une préférence de projet, de tâche ou de problème de groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**.
1. Cliquez sur le nom du groupe dans lequel vous souhaitez verrouiller ou déverrouiller une préférence de projet.
1. Dans le panneau de gauche, cliquez sur **Préférences de projet** ou **Préférences de tâches et de problèmes**.

1. Sur la page qui s’affiche, effectuez l’une des opérations suivantes pour une préférence déverrouillée au niveau du système ou pour un groupe supérieur au vôtre :

   * Si vous souhaitez que les administrateurs et administratrices des groupes situés sous votre groupe puissent configurer une préférence pour leurs groupes, déverrouillez-la ![](assets/unlock-toggle-button.png).
   * Si vous souhaitez que tous les groupes inférieurs au vôtre utilisent votre configuration pour une préférence, assurez-vous qu’elle est verrouillée ![](assets/lock-toggle-button.png).

     >[!IMPORTANT]
     >
     >Il est important de communiquer avec les administrateurs et administratrices et les utilisateurs et utilisatrices des groupes situés sous les vôtres pour vous assurer que votre configuration pour la préférence verrouillée répond aux besoins de tous. Lorsque vous verrouillez une préférence, tous les sous-groupes situés en dessous héritent de sa configuration. Notez également que si la préférence a été déverrouillée pendant une période quelconque, votre configuration remplace celles effectuées par les administrateurs et administratrices de groupe des sous-groupes situés en dessous.

1. Cliquer sur **Enregistrer**.
