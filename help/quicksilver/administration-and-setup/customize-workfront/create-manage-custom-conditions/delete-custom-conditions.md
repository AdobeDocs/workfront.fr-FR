---
title: Suppression d’une condition personnalisée
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Vous pouvez supprimer une condition personnalisée.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 93%

---

# Supprimer une condition personnalisée

Vous pouvez supprimer une condition personnalisée si elle n’est plus nécessaire.

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
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Supprimer une condition personnalisée

{{step-1-to-setup}}

1. Cliquez sur **Préférences du projet** > **Conditions**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Sélectionnez l’onglet du type d’objet (**Projet**, **Tâche**, ou **Problème**) dans lequel se trouve la condition à supprimer.

1. Pointez sur la condition que vous souhaitez supprimer, puis cliquez sur l’icône **Supprimer** ![](assets/delete.png) qui apparaît tout à droite.
1. Dans le message de confirmation qui s’affiche, cliquez sur **Supprimer la condition**.

1. Dans la boîte **Supprimer la condition** qui apparaît, sélectionnez une nouvelle condition dans la liste déroulante pour tous les projets qui utilisaient la condition que vous supprimez.

   Les conditions personnalisées ne sont disponibles dans la liste déroulante que si elles correspondent à la même condition intégrée que celle que vous supprimez. Par exemple, si vous supprimez une condition qui équivaut à À risque, seules les conditions personnalisées qui équivalent également à À risque peuvent être sélectionnées.

1. Cliquez sur **Supprimer la condition**.

>[!NOTE]
>
>Vous ne pouvez pas supprimer les conditions intégrées, qui sont Ciblé, À risque et À problème. Toutefois, vous pouvez modifier leurs noms et leurs couleurs.

Pour plus d’informations sur les conditions personnalisées, voir [Conditions personnalisées](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
