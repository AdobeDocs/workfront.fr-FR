---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Verrouillage ou déverrouillage d’une feuille de temps et d’heure de groupe
description: Si vous êtes administrateur de groupe, vous pouvez configurer, puis verrouiller une préférence de feuille de temps et d’heure pour votre groupe après qu’un administrateur Workfront l’ait déverrouillée au niveau du système.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 11%

---

# Verrouillage ou déverrouillage d’une feuille de temps et d’une préférence d’heure de groupe

Si vous êtes administrateur de groupe, vous pouvez configurer, puis verrouiller une préférence de feuille de temps et d’heure pour votre groupe après qu’un administrateur Workfront l’ait déverrouillée au niveau du système.

Le verrouillage d’une préférence Adobe Workfront garantit que toutes les personnes de votre groupe et de ses sous-groupes utilisent le même paramètre pour cette préférence. Bien que vous puissiez toujours reconfigurer une préférence que vous verrouillez, les administrateurs de groupe ne peuvent pas le faire pour les sous-groupes inférieurs.

Inversement, le déverrouillage d’une préférence au niveau du groupe offre aux administrateurs de sous-groupes plus de flexibilité pour gérer la manière dont leurs groupes fonctionnent avec ces éléments. Lorsqu’une préférence est déverrouillée, les administrateurs de groupe peuvent la reconfigurer pour ces sous-groupes.

Cela est parallèle à la possibilité qu’un administrateur de Workfront doit verrouiller ou déverrouiller une préférence pour tous les utilisateurs du système.

Pour plus d’informations sur la façon dont un administrateur Workfront peut verrouiller ou déverrouiller une feuille de temps et des préférences horaires pour tous les groupes du système, voir [Configuration des préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Pour plus d’informations sur la configuration des préférences de feuille de temps et d’heure pour un groupe, voir [Configuration des préférences de feuille de temps et d’heure pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

## Verrouillage ou déverrouillage d’une feuille de temps et d’une préférence d’heure de groupe

>[!TIP]
>
>Si vous êtes administrateur de Workfront, vous pouvez ignorer les étapes 1 à 4 en accédant à Configuration > Frise chronologique et heures > Préférences, puis en recherchant le nom du groupe dans la zone située en haut de la page.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**.
1. Cliquez sur le nom du groupe dans lequel vous souhaitez verrouiller ou déverrouiller une feuille de temps et une préférence d’heures.
1. Dans le panneau de gauche, cliquez sur **Préférences Fiches horaires et Heures**.

1. Sur la page qui s’affiche, effectuez l’une des opérations suivantes :

   * Si vous souhaitez que les administrateurs de groupes situés sous votre groupe puissent configurer une préférence pour leurs groupes, déverrouillez-la ![](assets/unlock-toggle-button.png).
   * Si vous souhaitez que tous les groupes situés sous le vôtre utilisent votre configuration pour une préférence, assurez-vous qu’elle est verrouillée ![](assets/lock-toggle-button.png) (il s’agit de la valeur par défaut).

     >[!IMPORTANT]
     >
     >Il est important de communiquer avec les administrateurs et les utilisateurs des groupes situés sous les vôtres pour vous assurer que tous les besoins sont pris en compte dans la configuration d’une préférence verrouillée. Lorsque vous la verrouillez, votre configuration pour elle est héritée par tous les sous-groupes ci-dessous. Et si la préférence a été déverrouillée pendant une période quelconque, votre configuration remplace celles que les administrateurs de groupe dans les sous-groupes inférieurs ont pu faire.

1. Cliquer sur **Enregistrer**.
