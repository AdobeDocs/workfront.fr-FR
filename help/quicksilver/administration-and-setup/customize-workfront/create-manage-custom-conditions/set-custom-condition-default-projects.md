---
title: Définir une condition personnalisée comme condition par défaut pour les projets
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Si le type de condition d’un projet est défini sur État de progression au lieu de Manuel, Adobe Workfront affiche automatiquement l’une des trois conditions par défaut intégrées au projet (Sur la cible, À risque ou En danger) au fur et à mesure de sa progression, comme expliqué dans Aperçu de la condition et du type de condition du projet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 25%

---

# Définir une condition personnalisée comme condition par défaut pour les projets

Si le type de condition d’un projet est défini sur État de progression au lieu de Manuel, Adobe Workfront affiche automatiquement l’une des trois conditions par défaut intégrées au projet (Sur la cible, À risque ou En danger) au fur et à mesure de sa progression, comme expliqué dans la section [Présentation de la condition du projet et du type de condition](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![](assets/condition-in-project-header-nwe.png)

Vous pouvez définir vos conditions personnalisées comme conditions par défaut au lieu d’utiliser ces trois conditions par défaut intégrées. Par exemple, vous pouvez modifier la condition Par défaut Sur la cible pour qu’elle s’affiche comme Tracking Well dans tous les projets.

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

## Définissez une condition personnalisée comme condition par défaut pour tous les projets :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Préférences du projet** > **Conditions**.

1. Cliquez sur l’onglet **Projet** .
1. Cliquez sur **Définir les conditions par défaut**.
1. Dans le menu déroulant en regard de la condition par défaut que vous souhaitez modifier, cliquez sur la condition personnalisée que vous souhaitez utiliser à la place.
1. Répétez l’étape précédente pour toute autre condition par défaut que vous souhaitez modifier.
1. Cliquer sur **Enregistrer**.

Pour plus d’informations sur la définition d’une condition personnalisée comme condition par défaut pour les tâches et les problèmes, voir [Définition d’une condition personnalisée comme condition par défaut pour les tâches et les problèmes](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Pour plus d’informations sur la configuration d’un projet afin que les utilisateurs puissent mettre à jour manuellement sa condition, voir [Mise à jour de la condition pour les tâches et les problèmes](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).

Pour plus d’informations sur les conditions personnalisées, voir [Conditions personnalisées](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
