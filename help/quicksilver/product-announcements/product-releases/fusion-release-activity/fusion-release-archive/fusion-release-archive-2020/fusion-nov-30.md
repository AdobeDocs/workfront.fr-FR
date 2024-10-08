---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
keywords: Fusion
navigation-topic: fusion-release-activity
title: '« Activité Version de Workfront Fusion : semaine du 30  novembre 2020 »'
description: Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion la semaine du 30 novembre 2020.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 9621683b-735d-40a6-8d7c-b5bd167cbdd2
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 100%

---

# Activité Version de Workfront Fusion : semaine du 30 novembre 2020

Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion la semaine du 30 novembre 2020.

Pour obtenir la liste de toutes les modifications récentes, voir [Activité de publication d’Adobe Workfront Fusion](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Pour obtenir la liste des correctifs récents dans Workfront Fusion, reportez-vous à la page [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) et recherchez toutes les mises à jour intitulées Mise à jour de maintenance de Workfront Fusion.

## Limite de taux pour les webhooks Workfront Fusion 2.0.

Nous avons introduit une nouvelle sécurisation des performances pour Workfront Fusion 2.0. Désormais, les webhooks ont une limite de taux de 100 demandes par seconde. Lorsque cette limite est atteinte, Workfront Fusion 2.0 envoie un statut 429 (Too many requests).

Auparavant, les demandes webhook n’étaient pas limitées.

Pour plus d’informations, voir [Sécurisation des performances d’Adobe Workfront Fusion](../../../../../workfront-fusion/get-started/fusion-performance-guardrails.md).

## Ajouter un formulaire personnalisé à un objet Workfront dans Workfront Fusion 2.0

Pour que vous puissiez ajouter des formulaires personnalisés à des objets dans Workfront Fusion 2.0, nous avons ajouté une action AssignCategories à Workfront > Divers. Module d’action.

Auparavant, il n’était pas possible d’utiliser un module Workfront Fusion 2.0 pour ajouter un formulaire personnalisé à un objet dans Workfront.

Pour plus d’informations sur le module d’action Workfront > Divers, voir [Modules Adobe Workfront](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Jira Server connector and modules now available</h2>
<p>We've added a Jira Server connector to Workfront Fusion. The Jira Server connector offers the same functionality as the current Jira Cloud connector. </p>
<p>With Jira Server modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, modified, or deleted</p> </li>
<li> <p>Create, read, update, or delete a record</p> </li>
<li> <p>List or search records</p> </li>
<li> <p>Download an attachment</p> </li>
<li> <p>Add an issue to a sprint</p> </li>
<li> <p>Make a custom API call</p> </li>
</ul>
<p>Previously, Jira modules were available only for Jira Cloud.</p>
<p>For more information on available Jira modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref" xrefformat="{para}">Jira Software modules</a>.</p>
<h2>Azure DevOps connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Azure DevOps applications. With the Azure DevOps modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, updated, or deleted.</p> </li>
<li> <p>Create or update records.</p> </li>
<li> <p>Get data from existing records.</p> </li>
<li> <p>Download or upload attachments.</p> </li>
<li> <p>Link work items together.</p> </li>
<li> <p>Retrieve a list of work items.</p> </li>
<li> <p>Perform a custom API call.</p> </li>
</ul>
<p>For more information see <a href="../../../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref" xrefformat="{para}">Azure DevOps modules</a>.</p>
<h2>Microsoft Dynamics 365 connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Microsoft Dynamics 365 account. With the Microsoft Dynamics 365 modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when records are added or updated in Microsoft Dynamics 365</p> </li>
<li> <p>Create, read, update, or delete a Microsoft Dynamics 365record</p> </li>
<li> <p>Perform a custom API call</p> </li>
</ul>
<p>For information about available Microsoft Dynamics 365 modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref" xrefformat="{para}">Microsoft Dynamics 365 modules</a>.</p>
</div>
-->
