---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Présentation de la date de début réelle du projet
description: Les projets, tâches et problèmes ont une date de début réelle dans Adobe Workfront. Pour les tâches et les problèmes, il s’agit de la date à laquelle ils ont été marqués comme En cours. Pour les projets, il s’agit de la date à laquelle la première tâche du projet est marquée comme En cours ou est terminée.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Présentation de la date de début réelle du projet

Les projets, tâches et problèmes ont une date de début réelle dans Adobe Workfront. Pour les tâches et les problèmes, il s’agit de la date à laquelle ils ont été marqués comme En cours. Pour les projets, il s’agit de la date à laquelle la première tâche du projet est marquée comme En cours ou est terminée.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage ou accès supérieur à la console Projets</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures d’un projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Considérations sur les dates de début réelles dans Workfront

* La date de début réelle se trouve dans la section Détails des projets, tâches et problèmes. 
* La date de début réelle d’un projet, d’une tâche ou d’un problème n’est pas renseignée lors de la création de ces éléments.
* La date de début réelle est renseignée lorsque le travail commence réellement sur le projet, la tâche ou le problème.
* La date de début réelle ne s’affiche pas dans l’onglet Détails du projet si le travail sur le projet n’a pas encore commencé.

   La Date de début réelle s’affiche vide dans les onglets Tâche et Détails du problème si le travail n’a pas encore commencé sur ces onglets.

* Vous pouvez modifier manuellement la date de début réelle d’une tâche ou d’un problème, mais vous ne pouvez pas modifier la date de début réelle d’un projet.

## Observations sur les dates de début réelles des projets

* Workfront définit automatiquement la date réelle d’un projet lorsque l’un des événements suivants se produit :

   * Une tâche affectée modifie l’état d’une tâche à partir de *Nouveau* à tout autre état qui n’équivaut pas à *Nouveau*.

   * Une tâche affectée modifie le pourcentage d’achèvement d’une tâche.

      >[!IMPORTANT]
      >
      >La date de début réelle du projet n’est pas renseignée lorsque le projet est marqué comme actif. Le travail réel doit commencer sur les tâches du projet avant que la Date de début réelle du projet ne soit remplie.

      Dans ce cas, la date de début réelle du projet est définie sur la date et l’heure auxquelles ces actions se sont produites pour la première tâche du projet. Cela indique que le projet a réellement commencé à cette date et cette heure.

## Localisation de la date de début réelle d’un projet

Vous pouvez localiser la date de début réelle d’un projet dans les zones suivantes :

* Dans la section Détails d’un projet.
* Dans un rapport ou une vue de projet, lorsque vous ajoutez la Date de début réelle de l’objet Projet dans le rapport.

   Pour plus d’informations sur la création de rapports, voir l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour localiser la date de début réelle dans la section Détails du projet :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **Projets**.
1. Cliquez sur le projet pour lequel vous souhaitez afficher la Date de début réelle.
1. Cliquez sur **Détails du projet** dans le panneau de gauche, puis accédez au **Présentation** .

   La date de début réelle s’affiche avec les autres dates du projet .

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
