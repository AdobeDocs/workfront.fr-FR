---
title: Définir une condition personnalisée comme valeur par défaut pour les projets
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Si le type de condition d’un projet est défini sur Statut de la progression au lieu de Manuel, Adobe Workfront affiche automatiquement l’une des trois conditions par défaut intégrées au projet (Dans les temps, À risque ou En difficulté) au fur et à mesure de sa progression, comme expliqué dans Vue d’ensemble de la condition du projet et du type de condition.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
TQID: https://experienceleague.adobe.com/4DNiEZ7cIWavM-3anuC3IU3fQ93y9hsokS31ZL-FSaQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 302
ht-degree: 77%

---

# Définir une condition personnalisée par défaut pour les projets

Si le type de condition d’un projet est défini sur Statut de la progression au lieu de Manuel, Adobe Workfront affiche automatiquement l’une des trois conditions par défaut intégrées au projet (Dans les temps, À risque ou En difficulté) au fur et à mesure de sa progression, comme expliqué dans [Vue d’ensemble de la condition du projet et du type de condition](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![Condition dans l’en-tête et les détails du projet ](assets/condition-of-project-0825.png)

Vous pouvez définir vos conditions personnalisées comme conditions par défaut au lieu d’utiliser ces trois conditions par défaut intégrées. Par exemple, vous pouvez modifier la condition par défaut Dans les temps pour qu’elle s’affiche comme Bon suivi dans tous les projets.

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

## Définir une condition personnalisée comme condition par défaut pour tous les projets :

{{step-1-to-setup}}

1. Cliquez sur **Préférences du projet** > **Conditions**.

1. Cliquez sur l’onglet **Projets**.
1. Cliquez sur **Définir les conditions par défaut**.
1. Dans le menu déroulant de la condition par défaut que vous souhaitez modifier, cliquez sur la condition personnalisée que vous souhaitez utiliser à la place.
1. Répétez l’étape précédente pour toute autre condition par défaut que vous souhaitez modifier.
1. Cliquer sur **Enregistrer**.

Pour plus d’informations sur la définition d’une condition personnalisée comme condition par défaut pour les tâches et les problèmes, voir [Définir une condition personnalisée par défaut pour les tâches et les problèmes](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Pour plus d&#39;informations sur la configuration d&#39;un projet afin que les utilisateurs puissent mettre à jour manuellement sa condition, voir [Mettre à jour la condition pour les tâches et les événements](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
