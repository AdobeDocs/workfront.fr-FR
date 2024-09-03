---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 14 de l’API
description: Adobe Workfront a publié la version 14 de l’API le 9 septembre 2021. La version 14 de l’API présente les changements suivants par rapport à la version 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 100%

---

# Nouveautés de la version 14 de l’API

Adobe Workfront a publié la version 14 de l’API le 9 septembre 2021. La version 14 de l’API présente les changements suivants par rapport à la version 14.

## Ressources ajoutées

Aucune ressource n’a été ajoutée pour la version 14 de l’API.

## Ressources supprimées

Aucune ressource n’a été supprimée pour la version 14 de l’API.

## Ressources modifiées

Les ressources suivantes ont été modifiées pour la version 14 de l’API.

* [BillingRecord (BILL)](#billingrecord-bill)
* [Category (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [Customer (CUST)](#customer-cust)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [Group (GROUP)](#group-group)
* [NoteTag (NTAG)](#notetag-ntag)
* [Project (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [Resource Allocation (RSALLO)](#resource-allocation-rsallo)
* [Role (ROLE)](#role-role)
* [Template (TMPL)](#template-tmpl)
* [Timesheet (TSHET)](#timesheet-tshet)

### BillingRecord (BILL) {#billingrecord-bill}

Un objet BillingRecord enregistre les revenus, les heures ou les dépenses qui peuvent être facturées. Ces informations peuvent être utilisées pour créer des factures dans un système comptable externe.

Pour plus d’informations sur les enregistrements de facturation, voir [Créer des enregistrements de facturation](../../manage-work/projects/project-finances/create-billing-records.md).

L’objet BillingRecord a ajouté l’indicateur **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Champs directs</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>Ajouté. Une catégorie est un formulaire personnalisé. Ce paramètre a été ajouté pour permettre d’ajouter des formulaires personnalisés aux objets BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Champs de référence</td> 
   <td> 
    <ul> 
     <li> <p><b>category</b> </p> <p>Ajouté. Une catégorie est un formulaire personnalisé. Ce paramètre a été ajouté pour permettre d’ajouter des formulaires personnalisés aux objets BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Champs de collection</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>Ajouté. Il s’agit d’une collection de catégories (formulaires personnalisés) associées à l’objet BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>Ajouté. Cette action recalcule les expressions dans les champs des formulaires personnalisés.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Catégorie (CTGY) {#category-ctgy}

Un objet Category est un formulaire personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>Ajout de la valeur possible :</p> 
      <ul> 
       <li> <p> BILL (BillingRecord)</p> </li> 
      </ul> <p>Cette valeur a été ajoutée pour permettre d’ajouter des formulaires personnalisés aux objets BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>Cette action prend les paramètres objID et objCode et renvoie un booléen.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

L’objet CustomEnum permet de convertir les codes de statut en texte lisible par une personne.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Requêtes</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>Ajouté. Cette requête permet de créer et de gérer des statuts pour les groupes et les sous-groupes. </p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Gérer les statuts des groupes</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Customer (CUST) {#customer-cust}

Un objet Customer représente une organisation qui utilise une instance de Workfront.

Il s’agit d’un objet interne.

### CustomerPreferences (CUSTPR) {#customerpreferences-custpr}

Un objet CustomerPreferences représente l’ensemble des préférences définies par un client ou une cliente pour son instance de Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>Ajout de la valeur possible :</p> 
      <ul> 
       <li> <p>Permettre aux personnes d’ajouter des images dans les mises à jour (updates:images.toggle)</p> </li> 
      </ul> <p>Ce paramètre permet d’ajouter des images dans les mises à jour des éléments de travail. </p> <p>Pour plus d’informations, voir <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mettre à jour le travail</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

Un objet DocumentVersion représente une version spécifique d’un fichier (comme du contenu écrit, des images ou d’autres formes d’informations).

Pour plus d’informations sur les versions des documents, voir [Charger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>Ajouté. Ce champ enregistre la date et l’heure du dernier rappel de Workfront Proof, si la version est associée à une épreuve.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Groupe (GROUP) {#group-group}

Un objet Group représente un ensemble d’utilisateurs et utilisatrices et d’équipes. Les groupes représentent souvent la structure des services.

Pour plus d’informations sur les groupes, voir [Groupes et équipes dans Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>Ajouté. Cette action prend un tableau d’identifiants de groupes et ajoute ces groupes en tant que sous-groupes au groupe spécifié.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag (NTAG) {#notetag-ntag}

Un objet NoteTag représente l’action de marquer une personne ou une équipe dans une mise à jour d’un élément de travail.

Pour plus d’informations sur le marquage dans les mises à jour, voir [Marquer d’autres personnes sur les mises à jour](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Opérations</td> 
   <td> <p>Les opérations suivantes ont été ajoutées à l’objet NoteTag :</p> 
    <ul> 
     <li> <p><b>COUNT</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>REPORT</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projet (PROJ) {#project-proj}

Les projets sont des éléments de travail dans Workfront et sont un bloc de création essentiel de la façon dont Workfront aide les personnes à travailler. Un objet Projet représente un groupe de tâches avec un objectif commun et spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>Ajout.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

Un objet QueueDef représente une file d’attente, qui est un projet qui a été publié dans la zone Centre d’assistance pour permettre aux utilisateurs et utilisatrices de lui soumettre des problèmes.

Pour plus d’informations sur les files d’attente des demandes, voir [Créer une file d’attente des demandes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>Ajouté. Cette action permet de trouver des demandes en utilisant le chemin d’accès à la file d’attente des demandes et aux groupes de rubriques.</p> <p>Pour plus d’informations sur la recherche de files d’attente des demandes par chemin d’accès, voir <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Créer des demandes et générer des brouillons dans l’application web Workfront</a> dans <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Créer et soumettre des demandes Adobe Workfront</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Allocation des ressources (RSALLO) {#resource-allocation-rsallo}

Un objet Allocation des ressources représente l’estimation des ressources nécessaires pour un projet donné. Cet objet n’est utilisé que dans le planificateur de ressources hérité. Pour le champ correspondant dans le nouveau planificateur de ressources, utilisez l’heure budgétée (BGHR).

L&#39;objet Allocation des ressources a supprimé l’indicateur **REPORTABLE**.

### Rôle (ROLE) {#role-role}

Un objet Rôle (fonction) représente une capacité fonctionnelle ou un ensemble de compétences qu’un utilisateur ou une utilisateur peut remplir, tel que Designer ou Chef ou Cheffe de produits.

Pour plus d’informations sur les fonctions, voir [Vue d’ensemble des fonctions](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ajouté. Il s’agit d’un paramètre booléen qui a la valeur true si un objet est actif et false s’il ne l’est pas. Les objets définis comme actifs apparaissent dans les menus déroulants et les champs de saisie et peuvent être attachés à d’autres objets.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Champs par défaut</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ajouté(e)(s)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Modèle (TMPL) {#template-tmpl}

Un objet Template représente un modèle de projet. Les projets peuvent être créés à partir de modèles pour gagner du temps. Un modèle contient une équipe et des tâches qui seront copiées dans tout projet créé à partir du modèle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Ajouté. Ce champ a été ajouté pour permettre d’associer des groupes à des modèles.</p> <p style="font-weight: normal;">Pour plus d’informations, voir <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Modifier les modèles de projet</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupe</p> <p style="font-weight: normal;">Ajouté. Ce champ a été ajouté pour permettre d’associer des groupes à des modèles.</p> <p style="font-weight: normal;">Pour plus d’informations, voir <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Modifier les modèles de projet</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->
