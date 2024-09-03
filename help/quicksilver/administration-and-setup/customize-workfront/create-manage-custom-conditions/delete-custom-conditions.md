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
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 94%

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
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
