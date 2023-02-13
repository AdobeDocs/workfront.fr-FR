---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de l’API version 14
description: Adobe Workfront a publié l’API version 14 le 9 septembre 2021. L’API version 14 comprend les modifications suivantes à partir de la version 14.
author: John
feature: Workfront API
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 1%

---

# Nouveautés de l’API version 14

Adobe Workfront a publié l’API version 14 le 9 septembre 2021. L’API version 14 comprend les modifications suivantes à partir de la version 14.

## Ressources ajoutées

Aucune ressource n’a été ajoutée pour l’API version 14.

## Ressources supprimées

Aucune ressource n’a été supprimée pour l’API version 14.

## Ressources modifiées

Les ressources suivantes ont été modifiées pour l’API version 14.

* [BillingRecord (BILL)](#billingrecord-bill)
* [Catégorie (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [Client (CUST)](#customer-cust)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [Groupe (GROUP)](#group-group)
* [RemarqueTag (NTAG)](#notetag-ntag)
* [Projet (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [Affectation de ressources (RSALLO)](#resource-allocation-rsallo)
* [Rôle (RÔLE)](#role-role)
* [Modèle (TMPL)](#template-tmpl)
* [Feuille de calcul (TSHET)](#timesheet-tshet)

### BillingRecord (BILL) {#billingrecord-bill}

Un objet BillingRecord enregistre les recettes, les heures ou les dépenses qui peuvent être facturées. Ces informations peuvent être utilisées pour créer des factures dans un système comptable externe.

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
     <li> <p><b>categoryID</b> </p> <p>Ajout de . Une catégorie est un formulaire personnalisé. Ce paramètre a été ajouté pour prendre en charge la possibilité d’ajouter des Forms personnalisées aux objets BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Champs de référence</td> 
   <td> 
    <ul> 
     <li> <p><b>category</b> </p> <p>Ajout de . Une catégorie est un formulaire personnalisé. Ce paramètre a été ajouté pour prendre en charge la possibilité d’ajouter des formulaires personnalisés aux objets BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Champs de collection</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>Ajout de . Il s’agit d’un ensemble de catégories (formulaires personnalisés) associés à l’objet BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>Ajout de . Cette action recalcule les expressions dans les champs de formulaire personnalisés.</p> </li> 
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
     <li> <p><b>catObjCode</b> </p> <p>Ajout de la valeur possible :</p> 
      <ul> 
       <li> <p> BILL (BillingRecord)</p> </li> 
      </ul> <p>Cette valeur a été ajoutée pour prendre en charge la possibilité d’ajouter des formulaires personnalisés aux objets BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>Cette action utilise les paramètres objID et objCode et renvoie une valeur booléenne.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

L’objet CustomEnum permet de convertir des codes d’état en texte lisible.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Requêtes</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>Ajout de . Cette requête permet de créer et de gérer des états pour les groupes et les sous-groupes. </p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Gestion des états d’un groupe</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Client (CUST) {#customer-cust}

Un objet client représente une organisation qui utilise une instance de Workfront.

C&#39;est un objet interne.

### CustomerPreferences (CUSTPR) {#customerpreferences-custpr}

Un objet CustomerPreferences représente l’ensemble des préférences définies par un client pour son instance de Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>Ajout de la valeur possible :</p> 
      <ul> 
       <li> <p>Autoriser les utilisateurs à ajouter des images dans les mises à jour (mises à jour:images.toggle)</p> </li> 
      </ul> <p>Ce paramètre prend en charge la possibilité d’ajouter des images aux mises à jour des éléments de travail. </p> <p>Pour plus d’informations, voir <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mise à jour du travail</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

Un objet DocumentVersion représente une version spécifique d’un fichier (comme du matériel écrit, des images ou d’autres formes d’informations).

Pour plus d’informations sur les versions de document, voir [Télécharger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>Ajout de . Ce champ enregistre la date et l’heure du dernier rappel à partir du BAT Workfront, si la version est associée à un BAT.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Groupe (GROUP) {#group-group}

Un objet Group représente un ensemble d’utilisateurs et d’équipes. Les groupes représentent souvent la structure du Ministère.

Pour plus d’informations sur les groupes, voir [Groupes par rapport aux équipes dans Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>Ajout de . Cette action utilise un tableau de groupID et ajoute ces groupes en tant que sous-groupes au groupe spécifié.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RemarqueTag (NTAG) {#notetag-ntag}

Un objet NoteTag représente l’acte de balisage d’un utilisateur ou d’une équipe lors d’une mise à jour d’un élément de travail.

Pour plus d’informations sur le balisage dans les mises à jour, voir [Balisage des autres sur les mises à jour](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Opérations</td> 
   <td> <p>Les opérations suivantes ont été ajoutées à l’objet NoteTag :</p> 
    <ul> 
     <li> <p><b>COUNT</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>RAPPORT</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projet (PROJ) {#project-proj}

Les projets sont des éléments de travail dans Workfront et sont une composante essentielle de la façon dont Workfront aide les personnes à travailler. Un objet Projet représente un groupe de tâches avec un objectif commun et spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>Ajout de .</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

Un objet QueueDef représente une file d’attente, qui est un projet qui a été publié dans la zone Aide Desk pour permettre aux utilisateurs de lui envoyer des problèmes.

Pour plus d’informations sur les files d’attente de requête, voir [Création d’une file d’attente de requête](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>Ajout de . Cette action prend en charge la possibilité de rechercher des requêtes à l’aide du chemin d’accès par le biais de la file d’attente des requêtes et des groupes de rubriques.</p> <p>Pour plus d’informations sur la recherche de files d’attente de requêtes par chemin d’accès, voir <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Création de requêtes et génération de brouillons dans l’application web Workfront</a> in <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Création et envoi de requêtes Adobe Workfront</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Affectation de ressources (RSALLO) {#resource-allocation-rsallo}

Un objet d’allocation de ressources représente l’estimation des ressources nécessaires pour un projet donné. Cet objet est utilisé uniquement dans l’ancien planificateur de ressources. Pour le champ correspondant dans le nouveau planificateur de ressources, utilisez l’option Heure budgétaire (BGHR).

L’objet Resource Attribution a supprimé l’indicateur **REPORTABLE**.

### Rôle (RÔLE) {#role-role}

Un objet Rôle (rôle de tâche) représente une capacité fonctionnelle ou un ensemble de compétences qu’un utilisateur peut remplir, tel que Designer ou Gestionnaire de produits.

Pour plus d’informations sur les rôles de tâche, voir [Présentation des rôles de tâche](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Ajout de . Il s’agit d’un paramètre booléen dont la valeur est true si un objet est Principal et false dans le cas contraire. Les objets définis sur Principal apparaissent dans les menus déroulants et les champs de type avant et peuvent être associés à d’autres objets.</p> </li> 
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

Un objet Template représente un modèle pour un projet. Les projets peuvent être créés à partir de modèles pour gagner du temps. Un modèle contient une équipe et des tâches qui seront copiées dans tout projet créé à partir du modèle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Champs directs</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Ajout de . Ce champ a été ajouté pour prendre en charge la possibilité d’associer des groupes à des modèles.</p> <p style="font-weight: normal;">Pour plus d’informations, voir <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Modifier des modèles de projet</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Champs de référence</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupe</p> <p style="font-weight: normal;">Ajout de . Ce champ a été ajouté pour prendre en charge la possibilité d’associer des groupes à des modèles.</p> <p style="font-weight: normal;">Pour plus d’informations, voir <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Modifier des modèles de projet</a>.</p> </li> 
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
