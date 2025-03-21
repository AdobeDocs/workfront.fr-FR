---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Modifier et créer des types de risques
description: Vous pouvez ajouter des risques à un projet au cours de la phase de planification afin d’identifier les obstacles potentiels avant l’approbation de tout travail. Les risques sont des événements possibles qui pourraient empêcher l’achèvement du projet dans les délais ou dans le respect du budget.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 39%

---

# Modifier et créer des types de risques

<!--Audited: 03/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Adobe Workfront dispose de plusieurs types de risques par défaut que vous pouvez associer aux projets au cours de la phase de planification afin d’identifier les obstacles potentiels avant l’approbation de tout travail.

Les risques sont des événements possibles qui pourraient empêcher l’achèvement du projet dans les délais ou dans le respect du budget.

Outre les types de risques par défaut, vous pouvez ajouter un nouveau type de risque pour refléter les besoins de votre entreprise.

Vous pouvez associer des types de risques aux risques du projet afin d&#39;identifier le type de risque qu&#39;un projet peut rencontrer.

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
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
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

* Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Types de risques

Les types de risques sont des libellés que vous pouvez utiliser pour classer les risques à des fins de création de rapports.

En tant qu&#39;administrateur [!DNL Workfront], vous pouvez créer des [!UICONTROL types de risques] dans la zone [!UICONTROL **Configuration**].

Après avoir configuré les types de risques, ils sont universels à votre système.

Toutes les personnes propriétaires de projet peuvent utiliser les mêmes types de risques pour leurs projets.

## Modifier et créer des types de risques

Par défaut, certains types de risques sont déjà en [!DNL Workfront].


Pour augmenter le nombre de types de risques dans votre instance Workfront, procédez comme suit :

* [Modifier les types de risques existants](#edit-existing-risk-types)
* [Créer des types de risques](#create-risk-types)

### Modifier les types de risques existants {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Types de risques]**.
1. Sélectionnez le type de risque à modifier.
1. Cliquez sur l’icône **[!UICONTROL Modifier]** ![Modifier](assets/edit-icon.png).

   La boîte de dialogue [!UICONTROL **Modifier le type de risque**] s&#39;ouvre. <!--add screen shot-->

   >[!TIP]
   >
   >   Vous pouvez modifier les informations sur le type de risque en ligne, lorsque vous double-cliquez sur le Nom ou la Description d&#39;un type de risque dans une liste de types de risque.

1. (Facultatif) Modifiez le nom et la description du type de risque.

   Les champs **[!UICONTROL Nom]** et **[!UICONTROL Description]** sont limités à 50 caractères.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications].**

1. (Facultatif) Pour supprimer un type de risque, sélectionnez-le dans la liste, cliquez sur l&#39;icône [!UICONTROL **Supprimer**] ![Icône Supprimer](assets/delete.png), puis cliquez sur [!UICONTROL **Oui, supprimer**]. Le type de risque est supprimé et ne peut pas être récupéré.

1. (Facultatif) Pour exporter une liste de types de risques, cliquez sur l’icône [!UICONTROL **Exporter**] ![Icône Exporter](assets/export-icon.png). Vous pouvez exporter des vers les types de fichiers suivants :

   * PDF
   * Excel
   * Excel (xlsx)
   * Délimité par des tabulations

   >[!TIP]
   >
   >   Vous pouvez d&#39;abord sélectionner un nombre limité de types de risques, puis les exporter pour une liste plus réduite.


### Créer des types de risques {#create-risk-types}

Vous pouvez créer des types de risques, en plus de ceux par défaut.

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Types de risques]**.
1. Cliquez sur **[!UICONTROL Nouveau type de risque]** pour ouvrir la boîte de dialogue [!UICONTROL **Nouveau type de risque**]

   Ou

   Cliquez sur [!UICONTROL **Ajouter d&#39;autres types de risques**] dans le coin inférieur gauche de la liste des types de risques pour ajouter des types de risques intégrés. <!--add screen shot-->
1. Ajoutez un **[!UICONTROL Nom]** (obligatoire) et un **[!UICONTROL Description]** (facultatif) pour le type de risque.

   Les champs **[!UICONTROL Nom]** et **[!UICONTROL Description]** sont limités à 50 caractères.

1. Cliquez sur **[!UICONTROL Créer un type de risque]**,

   Ou, si vous avez utilisé la modification en ligne pour ajouter votre type de risque, cliquez sur **[!UICONTROL Entrée]** lorsque vous avez terminé.

   >[!TIP]
   >
   >Pour modifier un type de risque personnalisé, consultez la section [[!UICONTROL Modifier les types de risques existants] dans cet article](#edit-existing-risk-types).

## Attacher des risques à des types de risques sur les projets

Vous pouvez utiliser des types de risques pour libeller les risques ajoutés à vos projets.

Pour plus d’informations sur la manière d’ajouter des risques aux projets, voir la section [Créer et modifier des risques sur des projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
