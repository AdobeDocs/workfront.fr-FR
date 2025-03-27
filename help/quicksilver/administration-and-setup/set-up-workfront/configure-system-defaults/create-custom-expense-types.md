---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Créer des types de dépenses personnalisés
description: En tant qu’administrateur ou administratrice  [!DNL Adobe Workfront] , vous pouvez créer des types de dépenses personnalisés pour définir et suivre les dépenses associées à vos tâches et projets. Les dépenses sont des coûts non liés à la main-d’œuvre qui peuvent être associés à des tâches ou à des projets.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: ff4a9b317bd75b298a7a39814b4ae265c92c6d2a
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 84%

---

# Créer des types de dépenses personnalisés

{{highlighted-preview}}

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

En tant qu’administrateur ou administratrice [!DNL Adobe Workfront], vous pouvez créer des types de dépenses personnalisés pour définir et suivre les dépenses associées à vos tâches et projets. Les dépenses sont des coûts non liés à la main-d’œuvre qui peuvent être associés à des tâches ou à des projets.

Vous pouvez modifier ou supprimer les types de dépenses que vous créez. Vous ne pouvez pas supprimer ni modifier les types de dépenses [!DNL Workfront] intégrés.

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
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   Ou
   <p>Actuelle : [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr>
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Types de dépense par défaut

Les types de dépenses par défaut dans [!DNL Workfront] qui ne peuvent pas être supprimés ou modifiés sont les suivants :

* [!UICONTROL Publicité]
* [!UICONTROL Conseils]
* [!UICONTROL Loisirs]
* [!UICONTROL Général]
* [!UICONTROL Matériaux]
* [!UICONTROL Déplacements]

## Créer des types de dépenses personnalisés

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Types de dépenses]**.
1. Cliquez sur **[!UICONTROL Nouveau type de dépense]**.
1. Dans la boîte de dialogue **[!UICONTROL Nouveau type de dépense]**, spécifiez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Attribuez un nom à la dépense.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Indiquez une description de la dépense.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Calculated Unit]</td> 
      <td> <p>Sélectionnez l’unité de mesure de votre type de dépense dans la liste déroulante.</p> <p>Les unités de mesure disponibles sont les suivantes :</p> 
       <ul> 
        <li>Mile</li> 
        <li>Kilomètre</li> 
        <li>Kilogramme</li> 
        <li>Dollar</li> 
        <li>Dollar</li> 
        <li>Jour</li> 
        <li>Autre - Lorsque vous sélectionnez cette option, vous devez nommer votre unité de mesure et la définir comme quelque chose de familier à votre organisation.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taux</td> 
      <td> <p>Indiquez le prix unitaire. Il s’agit d’un champ au format monétaire qui représente le coût de chaque unité définie dans le champ <strong>[!UICONTROL Calculated Unit]</strong>. </p> <p>Le taux peut contenir une valeur numérique allant jusqu’à 4 chiffres après la virgule. Par exemple, 1,0375.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Créer un type de dépense** <span class="preview">ou **[!UICONTROL Enregistrer]**.</span>

   Le type de dépense est désormais disponible pour que les utilisateurs et utlisatrices puissent l’associer à leurs dépenses sur les projets et les tâches.

## Modifier les types de dépenses personnalisés

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Types de dépenses]**.
1. Sélectionnez le type de dépense à modifier, puis cliquez sur **[!UICONTROL Modifier]**.

   La boîte de dialogue **[!UICONTROL Modifier le type de dépense]** s&#39;affiche.

1. Apportez les modifications souhaitées, puis cliquez sur **Enregistrer les modifications** <span class="preview">ou **[!UICONTROL Enregistrer]**.</span>

   Le type de dépense est désormais disponible pour que les utilisateurs et utlisatrices puissent l’associer à leurs dépenses sur les projets et les tâches.

Pour plus d’informations sur l’utilisation des dépenses et sur leur impact sur le coût d’un projet, consultez l’article [Gérer les dépenses de projet](../../../manage-work/projects/project-finances/manage-project-expenses.md).
