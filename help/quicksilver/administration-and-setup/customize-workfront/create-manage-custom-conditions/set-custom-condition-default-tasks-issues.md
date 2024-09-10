---
title: Définition d’une condition personnalisée comme valeur par défaut pour les tâches et les problèmes
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Lorsqu’une personne clique sur Travailler sur ce projet ou ajoute un commentaire de mise à jour à une nouvelle tâche qui lui a été assignée (sans définir manuellement une condition pour la tâche), Adobe Workfront affiche la condition par défaut pour les tâches, qui est configurée dans Configuration. Il en est de même pour les problèmes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 97%

---

# Définir une condition personnalisée comme condition par défaut pour les tâches et les problèmes

Lorsqu’une personne clique sur Travailler sur ce projet ou ajoute un commentaire de mise à jour à une nouvelle tâche qui lui a été assignée (sans définir manuellement une condition pour la tâche), Adobe Workfront affiche la condition par défaut pour les tâches, qui est configurée dans Configuration. Il en est de même pour les problèmes.

Workfront utilise la condition intégrée « Tout est en ordre » comme condition par défaut pour les tâches et, séparément, pour les problèmes. En tant qu’administrateur ou administratrice Workfront, vous pouvez remplacer la condition par défaut de ces deux types d’objets par une condition personnalisée que vous avez créée.

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

## Définissez une condition personnalisée comme condition par défaut pour les tâches ou les problèmes :

{{step-1-to-setup}}

1. Cliquez sur **Préférences du projet** > **Conditions**.

1. Cliquez sur l’onglet **Tâches** ou **Problèmes**.

1. Cliquez sur **Définir les conditions par défaut**.
1. Dans le menu déroulant, cliquez sur la condition personnalisée que vous souhaitez utiliser comme condition par défaut pour les tâches (ou les problèmes).
1. Cliquer sur **Enregistrer**.

>[!NOTE]
>
>* Une personne assignée à une tâche ou à un problème, ou qui dispose des droits de gestion pour cette tâche ou ce problème, peut modifier sa condition manuellement. Pour plus d’informations, voir [Mettre à jour la condition pour les tâches et les problèmes](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* Les trois conditions par défaut pour les tâches et les problèmes qui sont fournies avec Workfront sont : Tout est en ordre, Quelques inquiétudes et Obstacles majeurs. Vous ne pouvez pas masquer ou supprimer ces conditions, mais vous pouvez modifier leurs noms et leurs couleurs. Vous pouvez également créer de nouvelles conditions pour remplacer les précédentes, tel que décrit dans [Créer ou modifier une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
>

Pour plus d’informations sur la configuration d’une condition personnalisée comme condition par défaut pour les projets, voir [Définir une condition personnalisée comme condition par défaut pour les projets](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Pour plus d’informations sur les conditions personnalisées, voir [Conditions personnalisées](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
