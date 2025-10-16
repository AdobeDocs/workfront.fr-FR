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
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 60%

---

# Activer les trimestres personnalisés

<!--Audited: 11/2024-->

À des fins de création de rapports, vous pouvez créer des trimestres personnalisés si les trimestres de votre organisation sont basés sur des critères spécifiques autres que les dates du calendrier (tels que les jours ouvrables ou les jours d’achats).

Selon les produits achetés par votre société, vous pouvez configurer le nombre de trimestres suivant dans la zone Configuration de Workfront :

* Les clients qui ont acheté [!DNL Workfront] uniquement peuvent configurer jusqu’à huit trimestres personnalisés pour leur système [!DNL Adobe Workfront].
* Les clients qui ont acheté [!DNL Workfront] et [!DNL Workfront Planning] peuvent configurer jusqu’à 100 trimestres pour leur système [!DNL Workfront], également disponible dans [!DNL Planning].

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

## Configurer des trimestres personnalisés pour votre système [!DNL Workfront]

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Projets].**

1. Dans la section **[!UICONTROL Chronologies]**, sélectionnez **[!UICONTROL Activer les trimestres personnalisés]**.

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
1. (Facultatif et conditionnel) Si vous avez accès à [!DNL Workfront Planning], accédez à une page de type enregistrement et ouvrez une vue chronologique. La vue affiche les nouveaux trimestres personnalisés.
Pour plus d’informations, consultez [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).
