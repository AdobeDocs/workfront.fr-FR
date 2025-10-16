---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configuration des nouveaux calculs de chronologie pour les projets
description: Recalculer les chronologies permet aux personnes gestionnaires de voir comment des forces extérieures au projet affectent la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévisionnelles pour le projet.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 90%

---

# Configurer les recalculs de chronologies pour les projets

Recalculer les chronologies permet aux personnes gestionnaires de voir comment des forces extérieures au projet affectent la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévisionnelles pour le projet.

En tant qu’administrateur ou administratrice [!DNL Adobe Workfront], vous pouvez recalculer manuellement les chronologies pour tous les projets du système. Les personnes propriétaires de projet peuvent également recalculer manuellement les chronologies des projets individuels. Pour plus d’informations, voir [Recalculer les chronologies des projets](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Cet article décrit comment vous, en tant qu’administrateur ou administratrice [!DNL Workfront], pouvez déterminer comment et quand [!DNL Workfront] calcule automatiquement les chronologies de projet en configurant les préférences du projet dans la zone [!UICONTROL Configuration].

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer des recalculs automatiques

En tant qu’administrateur ou administratrice [!DNL Adobe Workfront], vous pouvez configurer quand [!DNL Workfront] recalcule automatiquement les chronologies du projet. [!DNL Workfront] peut recalculer les chronologies du projet chaque nuit ou lorsque l’étendue du projet change, ou les deux.

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Projets].**

1. Dans la section **[!UICONTROL Chronologies]**, activez ou désactivez l’un des paramètres ci-dessous, ou les deux. Par défaut, les deux paramètres sont activés.

   * **Tous les soirs :** [!DNL Workfront&#x200B;&#x200B;&#x200B;] recalcule les chronologies une fois toutes les 24 heures, la nuit, uniquement pour les projets dont le statut est [!UICONTROL En cours] et qui ont été mis à jour au cours des trois derniers mois. Selon la charge du système et d’autres facteurs, le temps de recalcul peut être retardé de plus de 24 heures.

     Dans ce cas, [!DNL Workfront] recalcule la chronologie de tous les projets dont le [!UICONTROL Type de mise à jour] est [!UICONTROL Automatique] ou [!UICONTROL Automatique et En cas de modification].

   * **Lorsque l’étendue d’un projet change** : pour plus d’informations sur ce qui constitue un changement d’étendue d’un projet, voir [Recalculer les chronologies des projets](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     Dans ce cas, [!DNL Workfront] recalcule la chronologie de tous les projets dont le Type de mise à jour est [!UICONTROL Automatique et En cas de modification] ou [!UICONTROL En cas de modification uniquement].
Pour plus d’informations sur les types de mise à jour de projet, voir [Vue d’ensemble du type de mise à jour d’un projet](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   La chronologie de tous les projets du système est recalculée automatiquement en fonction du type de mise à jour de chaque projet.

>[!IMPORTANT]
>
>Pour les environnements Sandbox de prévisualisation et d’actualisation personnalisée, le recalcul nocturne est désactivé et les chronologies de projet ne sont pas recalculées automatiquement. Vous devez recalculer manuellement la chronologie du projet pour les environnements de prévisualisation et de sandbox d’actualisation personnalisée. Pour plus d’informations, voir [Recalculer la chronologie du projet](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Recalculer les chronologies pour l’ensemble de l’instance [!DNL Workfront]

Vous pouvez exécuter le diagnostic [!UICONTROL Recalculer la chronologie] pour recalculer manuellement toutes les chronologies du système [!DNL Workfront]. Cela permet à toutes les personnes gestionnaires de projet de voir immédiatement l’influence des modifications externes sur les dates prévues et prévisionnelles. Pour plus d’informations, voir [Utiliser les diagnostics pour déclencher des processus automatisés](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
