---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Activer les trimestres personnalisés
description: À des fins de création de rapports, vous pouvez créer des trimestres personnalisés si les trimestres de votre organisation sont basés sur des critères spécifiques autres que les dates du calendrier (tels que les jours ouvrables ou les jours d’achats).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/8kRfZ17zcgN0-hlc16wh328YGRjTlzuI3LAe-Yjj25s
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 85c9f757134bc84e4b5038e4001f9a9fe1430f2a
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 56%

---

# Activer les trimestres personnalisés

<!--Audited: 03/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

À des fins de création de rapports, vous pouvez créer des trimestres personnalisés si les trimestres de votre organisation sont basés sur des critères spécifiques autres que les dates du calendrier (tels que les jours ouvrables ou les jours d’achats).

Selon les produits achetés par votre société, vous pouvez configurer le nombre de trimestres suivant dans la zone Configuration de Workfront :

* Les clients qui ont acheté [!DNL Workfront] uniquement peuvent configurer jusqu’à huit trimestres personnalisés pour leur système [!DNL Adobe Workfront].
* Les clients qui ont acheté [!DNL Workfront] et [!DNL Workfront Planning] peuvent configurer jusqu’à 100 trimestres pour leur système [!DNL Workfront], également disponible dans [!DNL Planning].

<!--
<div class="preview">
* Customers who purchased [!DNL Workfront] and [!DNL Workfront Planning], can configure custom weeks for each custom quarter which are visible in the [!DNL Planning] timeline views. 
</div>
-->


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
   <td><p>Licence [!UICONTROL Workflow Standard] ou [!UICONTROL Workfront Plan]</p>
       <p></p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
When we release fiscal weeks, replace the table above with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>Any Workfront or Workflow package</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>Any Planning package, including Planning as a standalone product</p>
   </div>
   </li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>
   
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>[!UICONTROL Workflow Standard] or [!UICONTROL Workfront Plan] license</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>A [!UICONTROL Planning Standard] license, in addition to a Workfront or a Workflow license</p>
   </div>
   </li>
   </ul>
    </td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

-->


## Configurer des trimestres personnalisés pour votre système [!DNL Workfront]

<!--
Setting up custom quarters differs depending on which environment you use. 

### Set up custom quarters for your [!DNL Workfront] system in the Production environment
-->

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Trimestres personnalisés]**.

1. Sélectionnez **[!UICONTROL Activer les trimestres personnalisés]**.

1. Saisissez un nom pour le trimestre personnalisé, par exemple « T1 exercice 2021 ».
1. Sélectionnez les dates de début et de fin du trimestre personnalisé.

   ![Trimestres personnalisés](assets/custom-quarters-nwe.png)

1. (Facultatif) Cliquez sur **[!UICONTROL Ajouter un trimestre personnalisé]** pour ajouter d’autres trimestres personnalisés au système.

   >[!IMPORTANT]
   >
   > Si votre société a acheté des [!DNL Workfront Planning], vous ne pouvez pas enregistrer vos trimestres personnalisés en cas d’écart ou de chevauchement entre les trimestres.
   >![Trimestres personnalisés avec avertissement de chevauchement](assets/custom-quarters-with-overlap-warning.png)
   >Les écarts et les chevauchements entre les trimestres ne sont autorisés que pour les clients [!DNL Workfront].

1. (Facultatif et conditionnel) Si votre société a acheté uniquement des [!DNL Workfront], sans [!DNL Workfront Planning], créez un élément de reporting qui fait référence aux trimestres fiscaux.

   **Exemple :** créez un filtre pour une liste de [!UICONTROL projets] et incluez la date d’achèvement prévue d’un projet faisant référence aux trimestres personnalisés.

   ![Filtre de projet avec trimestres personnalisés](assets/example-of-project-filter-with-custom-quarters.png)

   Les références à « Ce trimestre », « Trimestre prochain » et « Trimestre dernier » sont remplacées par de nouvelles références aux trimestres personnalisés.

   Pour plus d’informations sur les éléments de création de rapports, voir [Éléments de création de rapports : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Pour plus d’informations sur la création de filtres, voir [Créer ou modifier des filtres dans  [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Facultatif et conditionnel) Si votre société a acheté Workfront Planning et que vous avez accès à [!DNL Workfront Planning], accédez à une page de type d’enregistrement et affichez une vue chronologique. La vue affiche les nouveaux trimestres personnalisés.
Pour plus d’informations, consultez [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).

<!--
<div class="preview">

### Set up custom quarters for your [!DNL Workfront] system in the Preview environment

>[!NOTE]
>
>If your organization purchased a Planning package in addition to a Workflow package, or if they purchased  Workfront Planning as a standalone package, you can configure custom weeks, in addition to custom quarters. 
> 
>Custom weeks are not available for Workfront reports and lists. 

{{step-1-to-setup}}

1. Click **[!UICONTROL Custom Quarters]**.

1. Select **[!UICONTROL Enable Custom Quarters]**.

1. Type a name for the custom quarter. For example, "Fiscal Q1 2021."
1. Select start and end dates for the custom quarter.

1. (Optional) Select the **Starts a new custom week sequence** option. 

    When selected, this option sets the start of the custom quarter as the start of the first custom week of the quarter in the Planning timeline view. 
1. (Optional) In the **Custom week label format** area, choose the **Format** for the custom week labels. Choose from the following options:

    * **W1, W2, W3 ...** . This is the default format.
    * **FW1, FW2, FW3 ...**
    * **Week1, Week 2, Week 3, ...**
    * **Custom**

1. (Conditional) If you selected **Custom** for the **Format** field, type a **Custom label** to identify the custom weeks.  

    Custom weeks display in Planning timeline views. 

    >[!TIP]
    >
    >When adding a custom label, you can type up to 100 characters. 
    >
    >You may indicate the name of the first week, and the following weeks will use the same label followed by a sequential number. 
    >
    >For example, a **Custom label** of "Fiscal week" will add the labels of "Fiscal week 1, Fiscal week 2, Fiscal week 3 ..." to the rest of the weeks in the sequence. 

1. (Optional) Click **[!UICONTROL Add Custom Quarter]** to add additional custom quarters to the system.

      >[!IMPORTANT]
      >
      > If your company purchased [!DNL Workfront Planning], you cannot save your custom quarters if there are gaps or overlaps between the quarters. 
      >![Custom quarters with overlap warning](assets/custom-quarters-with-overlap-warning-red-outline.png)
      >Gaps and overlaps between the quarters are allowed for [!DNL Workfront] only customers. 

1. (Optional and conditional) To view the custom quarters in Workfront, create a reporting element that refers to the custom quarters.

   **Example:** Create a filter for a [!UICONTROL project] list and include the Planned Completion Date of a project referencing the custom quarters.

   ![Project filter with custom quarters](assets/example-of-project-filter-with-custom-quarters.png)

   The references to "This Quarter", "Next Quarter", and "Last Quarter" are replaced with new references to the custom quarters.

   For information about reporting elements, see [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   For information about creating filters, see [Create or edit filters in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Optional and conditional) To view custom quarters and weeks in Workfront Planning, go to a record type page and open a timeline view. The view displays the new custom quarters and weeks. 

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 

</div>
-->