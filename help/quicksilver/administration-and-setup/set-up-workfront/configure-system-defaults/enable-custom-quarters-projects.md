---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Activation des trimestres personnalisés pour les projets
description: À des fins de création de rapports, vous pouvez créer des trimestres personnalisés si les trimestres de votre entreprise sont basés sur des critères spécifiques autres que des dates calendaires (par exemple, jours ouvrables ou jours d’achats).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Activation des trimestres personnalisés pour les projets

À des fins de création de rapports, vous pouvez créer des trimestres personnalisés si les trimestres de votre entreprise sont basés sur des critères spécifiques autres que des dates calendaires (par exemple, jours ouvrables ou jours d’achats).

Vous pouvez configurer jusqu’à huit trimestres personnalisés pour votre [!DNL Adobe Workfront] système.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td> <p>Vous devez être un [!DNL Workfront] administrateur.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurez des quartiers personnalisés pour vos [!DNL Workfront] system

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Projets].**

1. Dans le **[!UICONTROL Chronologies]** , sélectionnez **[!UICONTROL Activation des trimestres personnalisés]**.

1. Saisissez un nom pour le trimestre personnalisé, par exemple &quot;1er trimestre 2021 fiscal&quot;.
1. Sélectionnez les dates de début et de fin pour le trimestre personnalisé.

   ![](assets/custom-quarters-nwe.png)

1. (Facultatif) Cliquez sur **[!UICONTROL Ajout d’un trimestre personnalisé]** pour ajouter des trimestres personnalisés supplémentaires au système.
1. (Facultatif) Créez un élément de rapport qui fait référence aux trimestres fiscaux.

   **Exemple :** Création d’un filtre pour un [!UICONTROL project] répertorie et inclut la date d’achèvement planifiée d’un projet référençant les trimestres personnalisés.

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   Les références à &quot;Ce trimestre&quot;, &quot;Suivant trimestre&quot; et &quot;Dernier trimestre&quot; sont remplacées par de nouvelles références aux trimestres personnalisés.

   Pour plus d’informations sur les éléments de création de rapports, voir [Éléments de reporting : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Pour plus d’informations sur la création de filtres, voir [Création ou modification de filtres dans [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
