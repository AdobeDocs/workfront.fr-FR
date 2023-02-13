---
title: Suppression d’une condition personnalisée
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Vous pouvez supprimer une condition personnalisée.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Suppression d’une condition personnalisée

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Suppression d’une condition personnalisée

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Préférences du projet** > **Conditions**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Sélectionnez l’onglet du type d’objet (**Projet**, **Tâche** ou **Problème**) où se trouve la condition que vous souhaitez supprimer.

1. Pointez sur la condition à supprimer, puis cliquez sur le **Supprimer** icon ![](assets/delete.png) qui apparaît à l&#39;extrême droite.
1. Dans le message de confirmation qui s’affiche, cliquez sur **Condition de suppression**.

1. Dans le **Condition de suppression** qui s’affiche, sélectionnez une nouvelle condition dans la liste déroulante pour tous les projets qui utilisaient la condition que vous supprimez.

   Les conditions personnalisées ne sont disponibles dans la liste déroulante que si elles correspondent à la même condition intégrée que celle que vous supprimez. Par exemple, si vous supprimez une condition qui correspond à &quot;En danger&quot;, seules les conditions personnalisées qui correspondent également à &quot;En risque&quot; peuvent être sélectionnées.

1. Cliquez sur **Condition de suppression**.

>[!NOTE]
>
>Vous ne pouvez pas supprimer les conditions intégrées, qui sont Sur Target, À risque et En problème. Vous pouvez toutefois modifier leurs noms et leurs couleurs.

Pour plus d’informations sur les conditions personnalisées, voir [Conditions personnalisées](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
