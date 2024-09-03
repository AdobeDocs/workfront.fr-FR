---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Activation des trimestres personnalisés pour les projets
description: À des fins de création de rapports, vous pouvez créer des trimestres personnalisés si les trimestres de votre organisation sont basés sur des critères spécifiques autres que les dates du calendrier (tels que les jours ouvrables ou les jours d’achats).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 98%

---

# Activer les trimestres personnalisés pour les projets

À des fins de création de rapports, vous pouvez créer des trimestres personnalisés si les trimestres de votre organisation sont basés sur des critères spécifiques autres que les dates du calendrier (tels que les jours ouvrables ou les jours d’achats).

Vous pouvez configurer jusqu’à huit trimestres personnalisés pour votre système [!DNL Adobe Workfront].

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être administrateur ou administratrice de [!DNL Workfront].</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice de [!DNL Workfront] s’il ou elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour plus d’informations sur la manière dont une équipe d’administration [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurer des trimestres personnalisés pour votre système [!DNL Workfront]

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Projets].**

1. Dans la section **[!UICONTROL Chronologies]**, sélectionnez **[!UICONTROL Activer les trimestres personnalisés]**.

1. Saisissez un nom pour le trimestre personnalisé, par exemple « T1 exercice 2021 ».
1. Sélectionnez les dates de début et de fin du trimestre personnalisé.

   ![](assets/custom-quarters-nwe.png)

1. (Facultatif) Cliquez sur **[!UICONTROL Ajouter un trimestre personnalisé]** pour ajouter d’autres trimestres personnalisés au système.
1. (Facultatif) Créez un élément de création de rapports qui se réfère aux trimestres d’exercice.

   **Exemple :** créez un filtre pour une liste de [!UICONTROL projets] et incluez la date d’achèvement prévue d’un projet faisant référence aux trimestres personnalisés.

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   Les références à « Ce trimestre », « Trimestre prochain » et « Trimestre dernier » sont remplacées par de nouvelles références aux trimestres personnalisés.

   Pour plus d’informations sur les éléments de création de rapports, voir [Éléments de création de rapports : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Pour plus d’informations sur la création de filtres, voir [Créer ou modifier des filtres dans  [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
