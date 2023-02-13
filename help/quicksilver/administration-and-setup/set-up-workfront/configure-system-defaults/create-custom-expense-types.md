---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Création de types de dépenses personnalisés
description: En tant que [!DNL Adobe Workfront] administrateur, vous pouvez créer des types de dépenses personnalisés pour définir et suivre les dépenses associées à vos tâches et projets. Les dépenses sont des coûts hors travail qui peuvent être associés à des tâches ou à des projets.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 3%

---

# Création de types de dépenses personnalisés

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

En tant que [!DNL Adobe Workfront] administrateur, vous pouvez créer des types de dépenses personnalisés pour définir et suivre les dépenses associées à vos tâches et projets. Les dépenses sont des coûts hors travail qui peuvent être associés à des tâches ou à des projets.

Vous pouvez modifier ou supprimer les types de dépenses que vous créez. Vous ne pouvez pas supprimer ni modifier le [!DNL Workfront] types de dépenses.

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

## Types de dépenses par défaut

Les types de dépenses qui se trouvent dans [!DNL Workfront] par défaut, ne peut pas être supprimé ou modifié :

* [!UICONTROL Publicité]
* [!UICONTROL Conseils]
* [!UICONTROL Loisirs]
* [!UICONTROL Général]
* [!UICONTROL Matériaux]
* [!UICONTROL Voyage]

## Création de types de dépenses personnalisés

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront].
1. Cliquez sur **[!UICONTROL Types de dépenses]**.
1. Cliquez sur **[!UICONTROL Nouveau type de dépense]**.
1. Dans le **[!UICONTROL Nouveau type de dépense]** qui s’affiche, indiquez les informations suivantes :

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
      <td role="rowheader">[!UICONTROL Unité calculée]</td> 
      <td> <p>Sélectionnez l'unité de mesure de votre type de dépense dans la liste déroulante.</p> <p>Les unités de mesure disponibles sont les suivantes :</p> 
       <ul> 
        <li>Mile</li> 
        <li>Kilomètre</li> 
        <li>Kilogramme</li> 
        <li>Dollar</li> 
        <li>Dollar</li> 
        <li>Jour</li> 
        <li>Autre - Lorsque vous sélectionnez cette option, vous devez nommer votre unité de mesure et définir cette unité comme quelque chose de familier à votre organisation.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taux</td> 
      <td> <p>Indiquez le prix unitaire. Il s’agit d’un champ au format monétaire qui représente le coût de chaque unité définie dans la variable <strong>[!UICONTROL Unité calculée]</strong> champ . </p> <p>Le taux peut contenir une valeur numérique allant jusqu’à 4 chiffres après la décimale. Par exemple, 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Créer un type de dépense]**.\
   Le type de dépense est désormais disponible pour que les utilisateurs puissent l’associer à leurs dépenses sur les projets et tâches.

## Modification des types de dépenses personnalisés

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront].
1. Cliquez sur **[!UICONTROL Types de dépenses]**.
1. Sélectionnez le type de dépense à modifier, puis cliquez sur **[!UICONTROL Modifier]**.

   Le **[!UICONTROL Modifier le type de dépense]** s’affiche.

1. Effectuez les modifications souhaitées, puis cliquez sur **[!UICONTROL Enregistrer les modifications]**.\
   Le type de dépense est désormais disponible pour que les utilisateurs puissent l’associer à leurs dépenses sur les projets et tâches.

Pour plus d’informations sur l’utilisation des dépenses et sur leur impact sur le coût d’un projet, consultez l’article [Gestion des dépenses de projet](../../../manage-work/projects/project-finances/manage-project-expenses.md).
