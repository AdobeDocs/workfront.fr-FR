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
source-git-commit: 6f64c3e6ebb8407c38ad3a1d46b2fc63b534879e
workflow-type: tm+mt
source-wordcount: 902
ht-degree: 36%

---

# Activer les trimestres personnalisés

<!--Audited: 03/2026-->

<!--remove Production and Preview references at release-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


À des fins de création de rapports, vous pouvez créer des trimestres personnalisés si les trimestres de votre organisation sont basés sur des critères spécifiques autres que les dates du calendrier (tels que les jours ouvrables ou les jours d’achats).

Selon les produits achetés par votre société, vous pouvez configurer le nombre de trimestres suivant dans la zone Configuration de Workfront :

* Les clients qui ont acheté [!DNL Workfront] uniquement peuvent configurer jusqu’à huit trimestres personnalisés pour leur système [!DNL Adobe Workfront].
* Les clients qui ont acheté [!DNL Workfront] et [!DNL Workfront Planning] peuvent configurer jusqu’à 100 trimestres pour leur système [!DNL Workfront], également disponible dans [!DNL Planning].

<div class="preview">

* Les clients qui ont acheté des [!DNL Workfront] et des [!DNL Workfront Planning] peuvent configurer des semaines personnalisées pour chaque trimestre personnalisé. Les semaines personnalisées sont visibles dans les vues chronologiques [!DNL Planning].

</div>

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

La configuration des trimestres personnalisés diffère selon l’environnement utilisé.

### Configuration de trimestres personnalisés pour votre système [!DNL Workfront] dans l’environnement de production

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

<div class="preview">

### Configurer des trimestres personnalisés pour votre système [!DNL Workfront] dans l’environnement de prévisualisation

>[!NOTE]
>
>Si votre entreprise a acheté un package Planning en plus d’un package Workflow ou si elle a acheté Workfront Planning sous la forme d’un package autonome, vous pouvez configurer des semaines personnalisées, en plus des trimestres personnalisés.
> 
>Les semaines personnalisées ne sont pas disponibles pour les rapports et les listes Workfront.

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Trimestres personnalisés]**.

1. Sélectionnez **[!UICONTROL Activer les trimestres personnalisés]**.

1. Saisissez un nom pour le trimestre personnalisé. Par exemple, « Exercice T1 2021 ».
1. Sélectionnez les dates de début et de fin du trimestre personnalisé.

1. (Facultatif) Sélectionnez l’option **Démarre une nouvelle séquence de semaines personnalisée**.

   Lorsque cette option est sélectionnée, le début du trimestre personnalisé est le début de la première semaine personnalisée du trimestre dans la vue chronologique Planification .
1. (Facultatif) Dans la zone **Format personnalisé des libellés de semaine**, choisissez le **Format** pour les libellés de semaine personnalisés. Choisissez l’une des options suivantes :

   * **W1, W2, W3...** . Il s’agit du format par défaut.
   * **FW1, FW2, FW3 ...**
   * **Semaine 1, Semaine 2, Semaine 3, ...**
   * **Personnalisé**

1. (Conditionnel) Si vous avez sélectionné **Personnalisé** pour le champ **Format**, saisissez un **Libellé personnalisé** pour identifier les semaines personnalisées.

   Les semaines personnalisées s&#39;affichent dans les vues chronologiques Planning.

   >[!TIP]
   >
   >Lors de l’ajout d’un libellé personnalisé, vous pouvez saisir jusqu’à 100 caractères.
   >
   >Vous pouvez indiquer le nom de la première semaine et les semaines suivantes utiliseront le même libellé suivi d’un numéro séquentiel.
   >
   >Par exemple, un **libellé personnalisé** de « Semaine fiscale » ajoute les libellés de « Semaine fiscale 1, Semaine fiscale 2, Semaine fiscale 3 ... » au reste des semaines de la séquence.

1. (Facultatif) Cliquez sur **[!UICONTROL Ajouter un trimestre personnalisé]** pour ajouter d’autres trimestres personnalisés au système.

   >[!IMPORTANT]
   >
   > Si votre société a acheté des [!DNL Workfront Planning], vous ne pouvez pas enregistrer vos trimestres personnalisés en cas d’écart ou de chevauchement entre les trimestres.
   >![Trimestres personnalisés avec avertissement de chevauchement](assets/custom-quarters-with-overlap-warning-red-outline.png)
   >Les écarts et les chevauchements entre les trimestres ne sont autorisés que pour les clients [!DNL Workfront].

1. (Facultatif et conditionnel) Pour afficher les trimestres personnalisés dans Workfront, créez un élément de rapport qui fait référence aux trimestres personnalisés.

   **Exemple :** créez un filtre pour une liste de [!UICONTROL projets] et incluez la date d’achèvement prévue d’un projet faisant référence aux trimestres personnalisés.

   ![Filtre de projet avec trimestres personnalisés](assets/example-of-project-filter-with-custom-quarters.png)

   Les références à « Ce trimestre », « Trimestre prochain » et « Trimestre dernier » sont remplacées par de nouvelles références aux trimestres personnalisés.

   Pour plus d’informations sur les éléments de création de rapports, voir [Éléments de création de rapports : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Pour plus d’informations sur la création de filtres, voir [Créer ou modifier des filtres dans  [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Facultatif et conditionnel) Pour afficher les trimestres et les semaines personnalisés dans Workfront Planning, accédez à une page de type d’enregistrement et ouvrez une vue chronologique. La vue affiche les nouveaux trimestres et semaines personnalisés.

Pour plus d’informations, consultez [Gérer la vue chronologique](/help/quicksilver/planning/views/manage-the-timeline-view.md).

</div>
