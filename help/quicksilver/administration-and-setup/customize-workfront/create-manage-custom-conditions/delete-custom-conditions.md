---
title: Suppression d’une condition personnalisée
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Vous pouvez supprimer une condition personnalisée.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
TQID: 'https://experienceleague.adobe.com/jHR0a3-MzkRRrlZ-h-X9f0n5HQbO9nDhWSxqy8KnWa8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 00c44bda4c719c94bd974cca133a0d8faf47612a
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 62%
---
# Supprimer une condition personnalisée

Vous pouvez supprimer une condition personnalisée si elle n’est plus nécessaire.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Administrateur ou administratrice système</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Supprimer une condition personnalisée

{{step-1-to-setup}}

1. Cliquez sur **Préférences du projet** > **Conditions**.
1. Sélectionnez l’onglet du type d’objet (**Projet**, **Tâche**, ou **Problème**) dans lequel se trouve la condition à supprimer.
1. Cochez la case en regard du nom de la condition à supprimer, puis cliquez sur **Supprimer** dans la barre d’actions située en bas de l’écran.
1. Dans la zone **Supprimer la condition** qui s’affiche, sélectionnez une nouvelle condition dans la liste déroulante pour tous les projets, tâches ou événements qui utilisaient la condition que vous supprimez.

   Les conditions personnalisées ne sont disponibles dans la liste déroulante que si elles correspondent à la même condition intégrée que celle que vous supprimez. Par exemple, si vous supprimez une condition qui équivaut à À risque, seules les conditions personnalisées qui équivalent également à À risque peuvent être sélectionnées.

1. Cliquez sur **Supprimer la condition**.

>[!NOTE]
>
>Vous ne pouvez pas supprimer les conditions intégrées, qui sont Ciblé, À risque et À problème. Toutefois, vous pouvez modifier leurs noms et leurs couleurs.
>
>Pour plus d’informations sur la modification des conditions personnalisées, voir [Créer ou modifier une condition personnalisée](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
