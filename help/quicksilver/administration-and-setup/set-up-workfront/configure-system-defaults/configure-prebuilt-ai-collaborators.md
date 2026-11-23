---
user-type: administrator
product-area: system-administration;setup
title: Configuration des collaborateurs d’IA préconfigurés
description: En tant qu’administrateur Adobe Workfront, vous pouvez configurer des collaborateurs d’IA préconfigurés à partir d’Adobe, tels que le coordinateur d’entrée, en tant qu’agents de travail que les utilisateurs peuvent affecter à des tâches et à des événements.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 71c1855166c2f950509cc8b7dc63792eabb6de16
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 10%
---
# Configuration des collaborateurs d’IA préconfigurés

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Une fois la version à prévisualiser, les mêmes fonctionnalités sont également disponibles tous les mois dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activer ou désactiver les versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

## Vue d’ensemble

Les collaborateurs IA préconfigurés sont des agents de travail prêts à l’emploi Adobe configurés pour effectuer une tâche spécifique, comme vérifier les demandes d’informations manquantes. Ils sont disponibles en tant qu’agents de travail natifs Adobe. Vous n’avez donc pas besoin de configurer un agent dans une plateforme externe ni de fournir les informations d’identification de plateforme externe.

Lorsque vous configurez un agent de travail, vous sélectionnez un collaborateur prédéfini comme source de l&#39;agent. Vous pouvez ensuite nommer l’agent de travail, définir son niveau d’accès et choisir les actions qu’il peut entreprendre. Les utilisateurs affectent l’agent de travail configuré aux tâches ou aux événements de la même manière qu’ils affectent tout autre agent de travail. Les utilisateurs n&#39;ont pas besoin de savoir que l&#39;agent est un collaborateur préconfiguré.

Pour plus d’informations sur les agents de travail et les autres types de collaborateurs AI, consultez [Configurer des collaborateurs AI](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Select, Prime ou Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>[!UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator] ou Administrateur de groupe</td> 
  </tr> 
  </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Adobe CX Coworker doit être activé pour votre organisation. Pour plus d’informations, consultez [Présentation de CX Enterprise Coworker dans Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

## Configuration d’un collaborateur d’IA préconfiguré

Vous configurez un collaborateur IA préconfiguré lorsque vous configurez un agent de travail. Dans la zone **Choisir l&#39;origine de l&#39;agent**, sélectionnez **Adobe Native**, puis sélectionnez le collaborateur préconfiguré que vous souhaitez utiliser dans la liste ci-dessous.

Pour les étapes complètes, voir [Configurer un agent de travail dans Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent-in-workfront).

Une fois le collaborateur configuré, les utilisateurs peuvent l&#39;affecter à des tâches ou à des événements. Pour plus d&#39;informations, voir [Utiliser des agents de travail](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

## Collaborateurs IA préconfigurés disponibles

### CX Enterprise Coworker {#cx-enterprise-coworker}

Un agent CX Enterprise Coworker optimisé par Adobe Agent Orchestrator.

Pour plus d’informations, consultez [Présentation de CX Enterprise Coworker dans Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

### Coordinateur d’admission {#intake-coordinator}

Le coordinateur d’admission vérifie les détails, les formulaires personnalisés et les pièces jointes des demandes pour rechercher des informations manquantes, peu claires ou incohérentes. Il publie des commentaires ou apporte des modifications avec l’approbation de l’utilisateur.

<!--
### Context Carrier {#context-carrier}

The Context Carrier keeps brief information flowing downstream so that context doesn't get scattered. It helps campaign managers and project managers keep the project team current without writing reports.

Requirements: A Workfront project and a Workfront Planning project must be connected to a Planning record. The Context Carrier must be triggered to run.

Steps to be added.

### Production Specialist {#production-specialist}

The Production Specialist produces images in every size you need, so designers don't have to resize them manually.

Requirement: Users must assign the Production Specialist to a task or issue.

Steps to be added.

### Version Comparer {#version-comparer}

The Version Comparer compares versions of a document so project teams can move content faster instead of spotting differences by hand.

Requirement: The document must have more than one version.

Steps to be added.

### Metadata Manager {#metadata-manager}

The Metadata Manager helps marketing teams find, tag, and label documents while work is in progress instead of later in the process.

Requirement: The Metadata Manager is available when you upload a document. Users must trigger it from the toolbar.

Steps to be added.

### Resource PTO Detector {#resource-pto-detector}

The Resource PTO Detector helps project teams make sure delivery isn't affected by time off, by identifying tasks assigned to people who are out of office.

Requirements: Tasks must be assigned, and PTO must be logged in Workfront.

Steps to be added.

### Campaign Summarizer {#campaign-summarizer}

Description and steps to be added.
-->
