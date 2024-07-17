---
title: Définir une condition personnalisée comme condition par défaut pour les tâches et les problèmes
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Lorsqu’un utilisateur clique sur Travailler dessus ou ajoute un commentaire de mise à jour à une nouvelle tâche à laquelle il a été affecté (sans définir manuellement une condition pour la tâche), Adobe Workfront affiche la condition par défaut pour les tâches, qui est configurée dans Configuration. Il en va de même pour les problèmes.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 21%

---

# Définir une condition personnalisée comme condition par défaut pour les tâches et les problèmes

Lorsqu’un utilisateur clique sur Travailler dessus ou ajoute un commentaire de mise à jour à une nouvelle tâche à laquelle il a été affecté (sans définir manuellement une condition pour la tâche), Adobe Workfront affiche la condition par défaut pour les tâches, qui est configurée dans Configuration. Il en va de même pour les problèmes.

Workfront utilise la condition intégrée Going Smoothly comme condition par défaut pour les tâches et, séparément, pour les problèmes. En tant qu’administrateur Workfront, vous pouvez définir la condition par défaut de ces deux types d’objets sur une condition personnalisée que vous avez créée.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Définissez une condition personnalisée comme condition par défaut pour les tâches ou pour les problèmes :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Préférences du projet** > **Conditions**.

1. Cliquez sur l’onglet **Tâches** ou **Problèmes** .

1. Cliquez sur **Définir les conditions par défaut**.
1. Dans le menu déroulant, cliquez sur la condition personnalisée que vous souhaitez utiliser comme condition par défaut pour les tâches (ou problèmes).
1. Cliquer sur **Enregistrer**.

>[!NOTE]
>
>* Un utilisateur affecté à une tâche ou à un problème, ou disposant des autorisations Manage (Gérer), peut modifier sa condition manuellement. Pour plus d’informations, voir [Mise à jour de la condition pour les tâches et les problèmes](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* Les trois conditions par défaut pour les tâches et les problèmes fournis avec Workfront se présentent comme suit : En douceur, Quelques préoccupations et Blocs de route majeurs. Vous ne pouvez pas masquer ni supprimer ces conditions, mais vous pouvez modifier leurs noms et leurs couleurs. Vous pouvez également en créer de nouveaux à utiliser à la place, comme décrit dans [Création ou modification d’une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
>

Pour plus d’informations sur la configuration d’une condition personnalisée comme condition par défaut pour les projets, voir [Définition d’une condition personnalisée comme condition par défaut pour les projets](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Pour plus d’informations sur les conditions personnalisées, voir [Conditions personnalisées](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
