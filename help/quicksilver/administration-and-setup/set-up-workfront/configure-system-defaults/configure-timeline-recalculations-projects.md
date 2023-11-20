---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configuration de nouveaux calculs de chronologie pour les projets
description: Recalculer les chronologies permet aux gestionnaires de voir comment les forces en dehors du projet affectent la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévues pour le projet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 4705c3fc76c1544f8c71e70a773432f164282abb
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Configuration de nouveaux calculs de chronologie pour les projets

Recalculer les chronologies permet aux gestionnaires de voir comment les forces en dehors du projet affectent la chronologie du projet. La chronologie d’un projet fait référence aux dates prévues et prévues pour le projet.

Comme [!DNL Adobe Workfront] , vous pouvez recalculer manuellement les chronologies pour tous les projets du système. Les propriétaires de projet peuvent également recalculer manuellement les échéances des projets individuels. Pour plus d’informations, voir [Recalculer les calendriers du projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Cet article décrit comment vous, en tant que [!DNL Workfront] administrateur, peut déterminer comment et quand [!DNL Workfront] calcule automatiquement les chronologies de projet en configurant les préférences du projet dans la variable [!UICONTROL Configuration] zone.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Niveau d’accès administrateur système</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurer des recalculs automatiques

Comme [!DNL Adobe Workfront] administrateur, vous pouvez configurer lorsque [!DNL Workfront] recalcule automatiquement les chronologies du projet. [!DNL Workfront] Vous pouvez recalculer les calendriers du projet chaque nuit ou lorsque la portée du projet change, ou les deux.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit, ou le [!UICONTROL **Menu Principal**] icon ![](assets/lines-main-menu.png) dans le coin supérieur gauche de [!DNL Workfront], le cas échéant, cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Projets].**

1. Dans le **[!UICONTROL Chronologies]** , activez ou désactivez l’un ou les deux paramètres ci-dessous. Par défaut, les deux paramètres sont activés.

   * **Tous les soirs :** [!DNL Workfront&#x200B;&#x200B;&#x200B;] recalcule les chronologies une fois toutes les 24 heures, la nuit, uniquement pour les projets dont le statut est [!UICONTROL Actuel] et qui ont été mis à jour au cours des trois derniers mois. Selon la charge du système et d&#39;autres facteurs, le temps de recalcul peut être retardé de plus de 24 heures.

     Dans ce cas, [!DNL Workfront] recalcule la chronologie de tous les projets comportant une [!UICONTROL Type de mise à jour] de [!UICONTROL Automatique] ou [!UICONTROL Automatique et Activé].

   * **Lorsque la portée d’un projet change**: pour plus d’informations sur ce qui constitue un changement de portée d’un projet, voir [Recalculer les calendriers du projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     Dans ce cas, [!DNL Workfront] recalcule la chronologie de tous les projets dont le type de mise à jour est [!UICONTROL Automatique et Activé] ou [!UICONTROL En cas de modification uniquement].
Pour plus d’informations sur les types de mise à jour de projet, voir [Présentation du type de mise à jour de projet](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   La chronologie de tous les projets du système est recalculée automatiquement en fonction du type de mise à jour de chaque projet.

## Recalculer les chronologies pour l’ensemble de la [!DNL Workfront] instance

Vous pouvez exécuter la variable [!UICONTROL Recalculer la chronologie] pour recalculer manuellement toutes les chronologies dans la variable [!DNL Workfront] système. Cela permet à tous les chefs de projet de voir immédiatement l’influence des modifications externes sur les dates prévues et prévues. Pour plus d’informations, voir [Utiliser les diagnostics pour déclencher des processus automatisés](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
