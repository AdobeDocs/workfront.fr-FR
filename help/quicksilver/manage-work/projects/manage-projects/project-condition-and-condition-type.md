---
title: Vue d’ensemble de la condition du projet et du type de condition
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: La condition du projet est une représentation visuelle de l’avancement du projet. Il s’agit d’une variable à déclarer déterminée par la relation entre les dates prévues, prévues et estimées du projet.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: e4de185f172b173dcc3ad966afa69ffb3bc479eb
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 8%

---

# Vue d’ensemble de la condition du projet et du type de condition

<!-- Audited: 12/2023 -->

La condition du projet est une représentation visuelle de l’avancement du projet. Il s’agit d’une variable à déclarer déterminée par la relation entre les dates prévues, prévues et estimées du projet.

## Présentation de la condition de projet

Tenez compte des points suivants lors de la compréhension de la condition d’un projet :

* En tant que propriétaire du projet, vous pouvez décider si la condition d’un projet est définie manuellement ou automatiquement. La condition d’un projet peut être définie comme suit :

   * Manuellement par les utilisateurs qui ont accès à la fonction Gérer le projet et lorsque le type de condition du projet est défini sur Manuel.
   * Automatiquement par Adobe Workfront, lorsque le type de condition du projet est défini sur État de progression. L’état d’avancement du projet est déterminé par la progression des tâches sur le projet. Pour plus d’informations sur l’état d’avancement du projet, consultez la [présentation de l’état d’avancement du projet](../../../manage-work/projects/planning-a-project/project-progress-status.md).

  Pour plus d’informations sur la mise à jour du type de condition du projet, voir [Définition du type de condition d’un projet](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* Lorsque vous autorisez Workfront à estimer automatiquement la condition du projet, nous vous recommandons d’utiliser les prédécesseurs sur vos tâches afin que la progression de la tâche se reflète dans la progression réelle et l’état de progression du projet.
* En tant que propriétaire de projet, vous pouvez modifier le projet afin d’utiliser un type de condition manuel au lieu d’utiliser l’état de progression en passant du type de condition État de progression à Manuel.

  >[!NOTE]
  >
  >Les projets qui se trouvent dans l’un des états suivants sont toujours marqués comme Sur Target, quelles que soient les dates des tâches et leur progression :
  >
  >* Idée
  >* Demandé
  >* Approuvé
  >* Rejeté

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Comment Workfront met à jour la condition du projet en fonction de l’état de progression

Lorsque le type de condition du projet est défini sur Manuel, vous pouvez déterminer la condition du projet indépendamment de l’état de progression du projet.

Cependant, nous vous recommandons de définir le type de condition du projet sur État de progression afin que vous puissiez avoir une indication claire de la véritable progression du projet, en fonction de la progression de vos tâches. Pour plus d’informations sur la façon dont Workfront calcule l’état de progression des projets, consultez la [présentation de l’état de progression du projet](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Dans ce cas, les valeurs de la condition de projet peuvent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Statut du projet</strong></td> 
   <td><strong>État d’avancement du projet</strong></td> 
   <td><strong>Indicateur de condition Workfront</strong></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dans les temps</td> 
   <td>Lorsque l’état d’avancement du projet de l’heure d’activation, la condition du projet est <strong>Sur Target</strong>. </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>En danger</td> 
   <td>Lorsque l’état d’avancement du projet est <strong>Derrière</strong> ou <strong>En danger</strong>, la condition du projet est <strong>En danger</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>En difficulté</td> 
   <td>Lorsque l’état de progression du projet est <strong>En retard</strong>, la condition du projet est <strong>En problème</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Les conditions peuvent être personnalisées pour votre environnement. Vous pouvez donc trouver plus de trois options pour la condition dans votre environnement. Les noms des conditions peuvent être différents de ceux répertoriés ci-dessus. Pour plus d’informations sur la personnalisation des conditions dans , voir l’article [Création ou modification d’une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Rapport sur la condition du projet, la mise à jour de la condition du projet et la note de la dernière condition

Dans l’affichage d’un rapport de projet, vous pouvez afficher les champs suivants liés à la condition du projet :

* **Condition du projet :** affiche la condition actuelle du projet.
* **Mise à jour de la condition du projet** : affiche la mise à jour la plus récente fournie par le propriétaire du projet dans le flux de mise à jour du projet, ainsi que la nouvelle condition.\
  Les commentaires effectués sur les mises à jour de condition ne sont pas affichés dans la colonne **Mise à jour de condition** ; seule la mise à jour principale s’affiche.

* **Remarque sur la dernière condition** : affiche la dernière mise à jour entrée sur un objet par le propriétaire de l’objet. Ce champ est utile pour afficher l’activité ou l’interaction la plus récente du propriétaire sur un objet.\
  La colonne **Dernière condition note** est vide si le texte de la dernière note d’un objet a été supprimé. Lorsqu’une nouvelle note est saisie sur l’objet, elle devient la dernière note et s’affiche à nouveau dans la colonne.

Pour plus d’informations sur la création d’un rapport, reportez-vous à l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
