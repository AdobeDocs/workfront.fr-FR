---
title: Définir une condition personnalisée comme valeur par défaut pour les projets
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Si le type de condition d’un projet est défini sur Statut de la progression au lieu de Manuel, Adobe Workfront affiche automatiquement l’une des trois conditions par défaut intégrées au projet (Dans les temps, À risque ou En difficulté) au fur et à mesure de sa progression, comme expliqué dans Vue d’ensemble de la condition du projet et du type de condition.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 96%

---

# Définir une condition personnalisée par défaut pour les projets

Si le type de condition d’un projet est défini sur Statut de la progression au lieu de Manuel, Adobe Workfront affiche automatiquement l’une des trois conditions par défaut intégrées au projet (Dans les temps, À risque ou En difficulté) au fur et à mesure de sa progression, comme expliqué dans [Vue d’ensemble de la condition du projet et du type de condition](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![Condition dans l’en-tête du projet](assets/condition-in-project-header-nwe.png)

Vous pouvez définir vos conditions personnalisées comme conditions par défaut au lieu d’utiliser ces trois conditions par défaut intégrées. Par exemple, vous pouvez modifier la condition par défaut Dans les temps pour qu’elle s’affiche comme Bon suivi dans tous les projets.

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

## Définir une condition personnalisée comme condition par défaut pour tous les projets :

{{step-1-to-setup}}

1. Cliquez sur **Préférences du projet** > **Conditions**.

1. Cliquez sur l’onglet **Projet**.
1. Cliquez sur **Définir les conditions par défaut**.
1. Dans le menu déroulant en regard de la condition par défaut que vous souhaitez modifier, cliquez sur la condition personnalisée que vous souhaitez utiliser à la place.
1. Répétez l’étape précédente pour toute autre condition par défaut que vous souhaitez modifier.
1. Cliquer sur **Enregistrer**.

Pour plus d’informations sur la définition d’une condition personnalisée comme condition par défaut pour les tâches et les problèmes, voir [Définir une condition personnalisée par défaut pour les tâches et les problèmes](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Pour plus d’informations sur la configuration d’un projet afin que les utilisateurs et utilisatrices puissent mettre à jour manuellement sa condition, voir [Mettre à jour une condition pour les tâches et les problèmes](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).

Pour plus d’informations sur les conditions personnalisées, voir [Conditions personnalisées](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
