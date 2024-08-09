---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Modifier et créer des types de risque
description: Vous pouvez ajouter des risques à un projet lors de la phase de planification afin d’identifier les obstacles potentiels avant l’approbation de tout travail. Les risques sont des événements possibles qui pourraient empêcher la réalisation du projet à temps ou dans les limites du budget.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 15%

---

# Modifier et créer des types de risque

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Vous pouvez ajouter des risques à un projet lors de la phase de planification afin d’identifier les obstacles potentiels avant l’approbation de tout travail. Les risques sont des événements possibles qui pourraient empêcher la réalisation du projet à temps ou dans les limites du budget.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Types de risques

Les types de risque sont des étiquettes que vous pouvez utiliser pour vos risques afin de les classer à des fins de création de rapports. Ils sont créés dans la zone **[!UICONTROL Setup]** par l’administrateur [!DNL Adobe Workfront]. Une fois les types de risque définis dans votre zone de **[!UICONTROL configuration]**, ils sont universels à votre système. Tous les propriétaires de projet peuvent utiliser les mêmes types de risque pour leurs projets.

## Modifier et créer des types de risque

Certains types de risque sont déjà présents dans [!DNL Workfront], par défaut. Pour répondre aux besoins de votre entreprise, vous pouvez modifier les types de risque existants ou créer de nouveaux types de risque.

* [Modifier les types de risque existants](#edit-existing-risk-types)
* [Créer de nouveaux types de risque](#create-new-risk-types)

### Modifier les types de risque existants {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Types de risque]**.
1. Sélectionnez le type de risque à modifier.
1. Cliquez sur **[!UICONTROL Modifier]**.
1. (Facultatif) Modifiez le nom et la description du type de risque.

   Il existe une limite de caractères de 50 caractères pour les champs **[!UICONTROL Nom]** et **[!UICONTROL Description]** .

1. Cliquez sur **[!UICONTROL Enregistrer les modifications].**

### Créer de nouveaux types de risque {#create-new-risk-types}

Vous pouvez créer de nouveaux types de risque, en plus des types par défaut, pour répondre aux besoins de votre entreprise.

Pour créer un nouveau type de risque :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Types de risque]**.
1. Cliquez sur **[!UICONTROL New Risk Type]**.
1. Saisissez un **[!UICONTROL Nom]** (obligatoire) et une **[!UICONTROL Description]** (facultatif) pour le type de risque.

   Il existe une limite de caractères de 50 caractères pour les champs **[!UICONTROL Nom]** et **[!UICONTROL Description]** .

1. Cliquez sur **[!UICONTROL Créer un type de risque]**. Si vous avez utilisé la modification en ligne pour ajouter votre type de risque, cliquez sur **[!UICONTROL Entrée]** lorsque vous avez terminé.

   >[!NOTE]
   >
   >Si vous devez modifier un type de risque personnalisé, reportez-vous à la section [[!UICONTROL Modification des types de risque ] existants](#edit-existing-risk-types) de cet article.

## Ajout des risques aux types de risque sur les projets

Les types de risque peuvent être utilisés pour étiqueter les risques ajoutés à vos projets. Pour plus d’informations sur l’ajout de risques aux projets, voir [Créer et modifier des risques sur les projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
