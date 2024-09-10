---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Modifier et créer des types de risque
description: Vous pouvez ajouter des risques à un projet au cours de la phase de planification afin d’identifier les obstacles potentiels avant l’approbation de tout travail. Les risques sont des événements possibles qui pourraient empêcher l’achèvement du projet dans les délais ou dans le respect du budget.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 98%

---

# Modifier et créer des types de risques

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Vous pouvez ajouter des risques à un projet au cours de la phase de planification afin d’identifier les obstacles potentiels avant l’approbation de tout travail. Les risques sont des événements possibles qui pourraient empêcher l’achèvement du projet dans les délais ou dans le respect du budget.

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

## Types de risques

Les types de risques sont des libellés que vous pouvez utiliser pour classer vos risques à des fins de reporting. Ils sont créés dans la zone **[!UICONTROL Configurer]** par l’administrateur ou l’administratrice [!DNL Adobe Workfront]. Une fois les types de risque établis dans votre zone **[!UICONTROL Configurer]**, ils s’appliquent à l’ensemble de votre système. Toutes les personnes propriétaires de projet peuvent utiliser les mêmes types de risques pour leurs projets.

## Modifier et créer des types de risques

Certains types de risques sont déjà présents par défaut dans [!DNL Workfront]. Pour répondre aux besoins de votre organisation, vous pouvez soit modifier les types de risques existants, soit en créer.

* [Modifier les types de risques existants](#edit-existing-risk-types)
* [Créer des types de risques](#create-new-risk-types)

### Modifier les types de risques existants {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Types de risques]**.
1. Sélectionnez le type de risque à modifier.
1. Cliquez sur **[!UICONTROL Modifier]**.
1. (Facultatif) Modifiez le nom et la description du type de risque.

   Les champs **[!UICONTROL Nom]** et **[!UICONTROL Description]** sont limités à 50 caractères.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications].**

### Créer des types de risques {#create-new-risk-types}

Vous pouvez créer des types de risques, en plus des types par défaut, afin de répondre aux besoins de votre organisation.

Pour créer un type de risque, procédez comme suit :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Types de risques]**.
1. Cliquez sur **[!UICONTROL Nouveau type de risque]**.
1. Saisissez un **[!UICONTROL Nom]** (obligatoire) et une **[!UICONTROL Description]** (facultative) pour le type de risque.

   Les champs **[!UICONTROL Nom]** et **[!UICONTROL Description]** sont limités à 50 caractères.

1. Cliquez sur **[!UICONTROL Créer un type de risque]**. Si vous avez utilisé la modification en ligne pour ajouter votre type de risque, cliquez sur **[!UICONTROL Entrée]** lorsque vous avez terminé.

   >[!NOTE]
   >
   >Si vous devez modifier un type de risque personnalisé, reportez-vous à la section [[!UICONTROL Modifier les types de risque existants]](#edit-existing-risk-types) de cet article.

## Attacher des risques à des types de risques sur les projets

Les types de risques peuvent être utilisés pour étiqueter les risques ajoutés à vos projets. Pour plus d’informations sur la manière d’ajouter des risques aux projets, voir la section [Créer et modifier des risques sur des projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
