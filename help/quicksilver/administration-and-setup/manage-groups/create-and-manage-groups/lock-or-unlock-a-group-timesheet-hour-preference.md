---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Verrouillage ou déverrouillage d’une feuille de temps et d’heure de groupe
description: Si vous êtes administrateur ou administratrice de groupes, vous pouvez configurer et verrouiller les préférences en matière de feuilles de temps et d’heures pour votre groupe après qu’un administrateur ou une administratrice Workfront a déverrouillé cette fonctionnalité au niveau du système.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 98%

---

# Verrouiller ou déverrouiller les préférences en matière de feuilles de temps et d’heures pour les groupes

Si vous êtes administrateur ou administratrice de groupes, vous pouvez configurer et verrouiller les préférences en matière de feuilles de temps et d’heures pour votre groupe après qu’un administrateur ou une administratrice Workfront a déverrouillé cette fonctionnalité au niveau du système.

Le verrouillage de préférences Adobe Workfront garantit des paramètres uniformes pour toutes les personnes de votre groupe et de ses sous-groupes. Bien que vous puissiez configurer ultérieurement une préférence que vous verrouillez, les administrateurs et administratrices de groupes ne peuvent pas le faire pour les sous-groupes inférieurs.

Inversement, le déverrouillage d’une préférence au niveau du groupe offre aux administrateurs et administratrices de sous-groupes plus de flexibilité pour gérer la manière dont leurs groupes fonctionnent avec ces éléments. Lorsqu’une préférence est déverrouillée, les administrateurs et administratrices de groupes peuvent la reconfigurer pour ces sous-groupes.

De même, les administrateurs et administratrices de Workfront doivent verrouiller ou déverrouiller une préférence pour toutes les personnes du système.

Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut verrouiller ou déverrouiller une préférence en matière de feuilles de temps et d’heures pour tous les groupes du système, voir [Configurer les préférences en matière de feuilles de temps et d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Pour plus d’informations sur la configuration d’une préférence en matière de feuilles de temps et d’heures pour un groupe, voir [Configurer les préférence en matière de feuilles de temps et d’heures pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez faire partie de l’équipe d’administration de groupe pour le groupe ou de l’équipe d’administration Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif complet à un utilisateur ou une utilisatrice</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez connaître le plan ou le type de licence que vous possédez, contactez votre administrateur ou administratrice Workfront.

+++

## Verrouiller ou déverrouiller les préférences en matière de feuilles de temps et d’heures pour les groupes

>[!TIP]
>
>Si vous êtes administrateur ou administratrice de Workfront, ignorez les étapes 1 à 4 en accédant à Configuration > Feuille de temps et heures > Préférences, puis en recherchant le nom du groupe dans la zone située en haut de la page.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**.
1. Cliquez sur le nom du groupe dans lequel vous souhaitez verrouiller ou déverrouiller une préférence en matière de feuilles de temps et d’heures.
1. Dans le panneau de gauche, cliquez sur **Préférences en matière de feuilles de temps et d’heures**.

1. Sur la page qui s’affiche, effectuez l’une des opérations suivantes :

   * Si vous souhaitez que les administrateurs et administratrices des groupes situés sous votre groupe puissent configurer une préférence pour leurs groupes, déverrouillez-la ![](assets/unlock-toggle-button.png).
   * Si vous souhaitez que tous les groupes situés sous le vôtre adoptent la même configuration pour une préférence, assurez-vous qu’elle est verrouillée ![](assets/lock-toggle-button.png) (il s’agit du statut par défaut).

     >[!IMPORTANT]
     >
     >Il est important de communiquer avec les administrateurs et administratrices et les utilisateurs et utilisatrices des groupes situés sous les vôtres pour vous assurer que votre configuration pour la préférence verrouillée répond aux besoins de tous. Lorsque vous verrouillez une préférence, tous les sous-groupes situés en dessous héritent de sa configuration. Notez également que si la préférence a été déverrouillée pendant une période quelconque, votre configuration remplace celles effectuées par les administrateurs et administratrices de groupe des sous-groupes situés en dessous.

1. Cliquer sur **Enregistrer**.
