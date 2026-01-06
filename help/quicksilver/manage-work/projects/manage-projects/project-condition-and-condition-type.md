---
title: Vue d’ensemble de la condition du projet et du type de condition
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: La condition du projet est une représentation visuelle de la progression du projet. Il s’agit d’une variable faisant l’objet d’un rapport déterminée par la relation entre les dates prévues, prévisionnelles et estimées du projet.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 100%

---

# Vue d’ensemble de la condition du projet et du type de condition

<!-- Audited: 12/2023 -->

La condition du projet est une représentation visuelle de la progression du projet. Il s’agit d’une variable faisant l’objet d’un rapport déterminée par la relation entre les dates prévues, prévisionnelles et estimées du projet.

## Vue d’ensemble de la condition du projet

Pour comprendre la condition d’un projet, il faut tenir compte des éléments suivants :

* En tant que personne propriétaire du projet, vous pouvez décider si la condition d’un projet est définie manuellement ou automatiquement. La condition d’un projet peut être définie des manières suivantes :

   * Manuellement par les personnes qui ont accès à la gestion du projet et lorsque le type de condition du projet est défini sur Manuel.
   * Automatiquement par Workfront lorsque le type de condition du projet est défini sur Statut de la progression. Le statut de la progression du projet est déterminé par la progression des tâches du projet. Pour plus d’informations sur le statut de la progression du projet, voir [Vue d’ensemble du statut de la progression du projet](../../../manage-work/projects/planning-a-project/project-progress-status.md).

  Pour plus d’informations sur la manière de mettre à jour le type de condition du projet, voir [Définir le type de condition d’un projet](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* Lorsque vous permettez à Workfront d’estimer automatiquement la condition du projet, nous vous recommandons d’utiliser des prédécesseurs sur vos tâches afin que la progression des tâches se reflète dans la progression réelle et le statut de la progression du projet.
* En tant que personne propriétaire du projet, vous pouvez modifier le projet pour utiliser un type de condition manuel au lieu du statut de la progression en changeant le type de condition de Statut de la progression à Manuel.

  >[!NOTE]
  >
  >Les projets qui se trouvent dans l’un des statuts suivants sont toujours marqués comme Dans les temps, quelles que soient les dates des tâches et leur progression :
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

## Mise à jour par Workfront de la condition du projet en fonction du statut de la progression

Lorsque le type de condition du projet est défini sur Manuel, vous pouvez déterminer la condition du projet indépendamment du statut de la progression du projet.

Toutefois, nous vous recommandons de définir le type de condition du projet sur Statut de la progression afin que vous ayez une indication claire de la progression réelle du projet en fonction de la progression de vos tâches. Pour plus d’informations sur la façon dont Workfront calcule le statut de la progression des projets, voir [Vue d’ensemble du statut de la progression des projets](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Dans ce cas, les valeurs de la condition du projet peuvent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Statut du projet</strong></td> 
   <td><strong>Statut de la progression du projet</strong></td> 
   <td><strong>Indicateur de condition Workfront</strong></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dans les temps</td> 
   <td>Lorsque le statut de la progression du projet est « À l’heure », la condition du projet est <strong>Dans les temps</strong>. </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>En danger</td> 
   <td>Lorsque le statut de la progression du projet est <strong>En retard</strong> ou <strong>À risque</strong>, la condition du projet est <strong>À risque</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>En difficulté</td> 
   <td>Lorsque le statut de la progression du projet est <strong>En retard</strong>, la condition du projet est <strong>En difficulté</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Les conditions peuvent être personnalisées en fonction de votre environnement. Il est donc possible que vous trouviez plus de trois options pour les conditions dans votre environnement. Les noms des conditions peuvent être différents de ceux énumérés ci-dessus. Pour plus d’informations sur la personnalisation des conditions, voir l’article [Créer ou modifier une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Rapport sur la condition du projet, mise à jour de la condition du projet et dernière note sur la condition du projet

Dans la vue d’un rapport de projet, vous pouvez afficher les champs suivants relatifs à la condition du projet :

* **Condition du projet :** affiche la condition actuelle du projet.
* **Mise à jour de la condition du projet** : affiche la mise à jour la plus récente que la personne propriétaire du projet a fournie dans le flux de mise à jour du projet, ainsi que la nouvelle condition.\
  Les commentaires sur les mises à jour des conditions ne sont pas affichés dans la colonne **Mise à jour des conditions** ; seule la mise à jour principale est affichée.

* **Dernière note sur la condition** : affiche la dernière mise à jour entrée sur un objet par la personne propriétaire de l’objet. Ce champ est utile pour afficher l’activité ou l’interaction la plus récente de la personne propriétaire sur un objet.\
  La colonne **Dernière note sur la condition** est vide si le texte de la dernière note d’un objet a été supprimé. Lorsqu’une nouvelle note est saisie sur l’objet, elle devient la dernière note et s’affiche à nouveau dans la colonne.

Pour plus d’informations sur la création d’un rapport, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
