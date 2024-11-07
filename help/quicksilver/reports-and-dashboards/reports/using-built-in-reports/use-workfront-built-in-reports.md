---
product-area: reporting
navigation-topic: using-built-in-reports
title: Utiliser les rapports intégrés d’Adobe Workfront
description: Adobe Workfront contient une liste complète de rapports natifs prêts à l’emploi. Les équipes d’administration de Workfront peuvent masquer les rapports intégrés pour que les utilisateurs et utilisatrices n’y aient pas accès.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: 0022892cabb9a44fb21e33d88148b098c937f388
workflow-type: tm+mt
source-wordcount: '2964'
ht-degree: 58%

---

# Utiliser les rapports intégrés d’Adobe Workfront

<!--Audited: 11/2024-->

Adobe Workfront dispose d’une liste étendue de rapports intégrés que vous pouvez utiliser.

Les équipes d’administration de Workfront peuvent masquer les rapports intégrés pour que les utilisateurs et utilisatrices n’y aient pas accès.

Pour plus d’informations sur la façon de masquer les rapports intégrés, voir [Masquer les rapports intégrés](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Contributeur ou version ultérieure</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Requête ou supérieure</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Affichage ou accès supérieur à Reports, Dashboard, Calendriers</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur un rapport pour ajouter ou modifier un filtre d’un rapport</p> <p>Gérer les autorisations sur un filtre pour le modifier dans une liste</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vue d’ensemble des rapports intégrés {#overview-of-built-in-reports}

Vous pouvez personnaliser un rapport intégré et l’enregistrer en tant que nouveau rapport. Pour plus d’informations sur la personnalisation des rapports intégrés, voir la section [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Les rapports suivants sont fournis avec le package Workfront. Les rapports sont disponibles pour tous les utilisateurs et toutes les utilisatrices qui disposent au moins de droits d’affichage sur les rapports intégrés dans leur niveau d’accès.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nom du rapport</strong> </th> 
   <th><strong>Description du rapport</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Coût réel du portefeuille par programme</td> 
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets. Le rapport est groupé par nom de programme, demandé par nom de portfolio, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coût réel du portefeuille par projet</td> 
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets. Le rapport est groupé par nom de projet, demandé par nom de portfolio, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu réel du portefeuille par programme</td> 
   <td>Rapport Projet qui affiche les Recettes prévues et les Recettes réelles des projets. Le rapport est groupé par nom de programme, demandé par nom de portfolio, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu réel du portefeuille par projet</td> 
   <td>Rapport Projet qui affiche les Recettes prévues et les Recettes réelles des projets. Le rapport est groupé par nom de projet, demandé par nom de portfolio, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenus réels par entreprise</td> 
   <td>Rapport Projet qui affiche les recettes réelles et la société des projets. Le rapport est groupé par nom de société et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenus réels par groupe</td> 
   <td>Rapport Projet qui affiche les recettes réelles et le groupe des projets. Le rapport est groupé par nom de groupe et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Toutes les feuilles de temps ouvertes</td> 
   <td>Rapport de feuille de temps qui affiche les feuilles de temps ouvertes. Le rapport affiche les champs suivants : la période, le nom de la personne propriétaire, le nombre total d’heures, les heures supplémentaires, le nom de l’approbateur ou de l’approbatrice et le statut des feuilles de temps.</td> 
  </tr> 
  <tr> 
   <td>Approbation des feuilles de temps (sur invite)</td> 
   <td>Rapport de feuille de temps qui affiche les feuilles de temps envoyées ou rejetées avec les approbateurs. Le rapport affiche les champs suivants : la période, la personne propriétaire, le nombre total d’heures, les heures supplémentaires, le nom de l’approbateur ou de l’approbatrice et le statut des feuilles de temps. Le rapport est ordonné par : la date de début de la feuille de temps, la date de fin de la feuille de temps, le nom de la personne chargée de l’approbation de la feuille de temps et le nom de l’utilisateur ou de l’utilisatrice.</td> 
  </tr> 
  <tr> 
   <td>Projets à risque</td> 
   <td>Rapport Projet qui affiche les projets en cours et planifiés présentant une situation de risque ou de problème. Le rapport affiche les champs suivants : la description, la date d’achèvement prévue, la date d’achèvement prévisionnelle, le pourcentage terminé, le statut et la priorité des projets. Le rapport est regroupé par nom de portfolio.</td> 
  </tr> 
  <tr> 
   <td>Facturation des revenus par entreprise</td> 
   <td>Rapport Projet qui affiche la société et les recettes de facturation des projets. Le rapport est groupé par nom de société et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Facturation des revenus par groupe</td> 
   <td>Rapport Projet qui affiche les recettes de facturation et le groupe des projets. Le rapport est groupé par nom de groupe et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Facturation des revenus par mois</td> 
   <td>Rapport d’enregistrement de facturation qui affiche le nom du projet, les recettes de facturation du projet et la date de facturation des enregistrements de facturation. Le rapport est regroupé par mois de la date de facturation des enregistrements de facturation et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Événements conclus par semaine</td> 
   <td>Rapport Problème qui affiche la date d’achèvement réelle des problèmes. Le rapport est regroupé par semaine de la date d’achèvement effective des problèmes et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Événements conclus par semaine et par utilisateur</td> 
   <td>Rapport Problème qui affiche la date d’achèvement réelle et les affectations des problèmes. Le rapport est regroupé par personne cessionnaire principale et par semaine de la date d’achèvement effective des problèmes, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets actuels</td> 
   <td>Rapport Projet qui affiche tous les projets en cours. Le rapport affiche les champs suivants : la description, la date d’achèvement prévue, la date d’achèvement prévisionnelle, le pourcentage terminé, le statut et la priorité des projets.</td> 
  </tr> 
  <tr> 
   <td>Coûts horaires par utilisateur par mois</td> 
   <td>Rapport d’heure matrice qui affiche le nombre d’heures journalisées et leur coût réel. Le rapport est regroupé par nom de propriétaire et par mois de la date d’entrée des heures.</td> 
  </tr> 
  <tr> 
   <td>Heures par utilisateur</td> 
   <td>Rapport Heure qui affiche le nombre d’heures journalisées. Le rapport est regroupé par nom de propriétaire et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Heures, par utilisateur, par semaine</td> 
   <td>Rapport Heure de matrice qui affiche le nombre d’heures enregistrées au cours des quatre dernières semaines et la date d’entrée des heures. Le rapport est présenté en fonction de la date d’entrée des heures et est regroupé par nom de propriétaire et par mois de la date d’entrée des heures.</td> 
  </tr> 
  <tr> 
   <td>Événements par statut</td> 
   <td>Rapport Problème qui affiche le statut des problèmes. Le rapport est regroupé par statut des problèmes et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Événements par statut et projet</td> 
   <td>Rapport de problèmes matrice qui affiche le statut des problèmes dans les projets en cours et le nom du projet. Le rapport est regroupé par nom de projet et par statut des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Main-d'œuvre / Coûts des dépenses par portefeuille</td> 
   <td>Rapport Projet qui affiche le coût de la main-d’oeuvre planifié, le coût de la main-d’oeuvre réel, le coût des dépenses planifiées et le coût des dépenses réelles des projets. Le rapport est regroupé par nom de portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Main-d'œuvre / Coûts des dépenses par programme</td> 
   <td>Rapport Projet qui affiche le coût de la main-d’oeuvre planifié, le coût de la main-d’oeuvre réel, le coût des dépenses planifiées et le coût des dépenses réelles des projets. Le rapport est regroupé par nom de portfolio et par nom de programme, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus/coûts réels mensuels du portefeuille par projet</td> 
   <td>Rapport de projet (données financières) matrice qui affiche la date d’allocation, le coût total prévu, le coût réel total et l’écart total des coûts des projets. Le rapport est regroupé par nom de projet, trimestre et mois de la date d’attribution.</td> 
  </tr> 
  <tr> 
   <td>Revenus prévus/revenus réels mensuels du portefeuille par projet</td> 
   <td>Rapport Tableau de projets (données financières) qui affiche la date d’attribution, le total des recettes prévues, le total des recettes réelles et l’écart total des recettes des projets. Le rapport est regroupé par nom de projet, trimestre et mois de la date d’attribution.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus/coûts réels mensuels du projet</td> 
   <td>Rapport de projet (données financières) matrice qui affiche la date d’allocation, le coût total prévu, le coût réel total et l’écart total des coûts des projets. Le rapport est regroupé par nom de projet, par trimestre et par mois de la date d’allocation et est présenté par le nom du projet.</td> 
  </tr> 
  <tr> 
   <td>Revenus prévus/revenus réels mensuels du projet</td> 
   <td>Rapport Tableau de projets (données financières) qui affiche la date d’attribution, le total des recettes prévues, le total des recettes réelles et l’écart total des recettes des projets. Le rapport est regroupé par nom de projet, par trimestre et par mois de la date d’allocation et est présenté par le nom du projet.</td> 
  </tr> 
  <tr> 
   <td>Mes documents</td> 
   <td>Rapport Document qui affiche les documents téléchargés par l’utilisateur connecté. Le rapport affiche les champs suivants : le nom de la personne propriétaire, la date de modification, la taille, le nombre de versions, la source et le type des documents.</td> 
  </tr> 
  <tr> 
   <td>Mes favoris</td> 
   <td>Rapport Favoris qui affiche la liste des objets marqués comme favoris par l’utilisateur connecté. Le rapport affiche les champs suivants : le type d’objet et le nom des favoris.</td> 
  </tr> 
  <tr> 
   <td>Mes problèmes</td> 
   <td>Rapport Problème qui affiche les problèmes incomplets affectés à l’utilisateur connecté. Le rapport affiche les champs suivants : le nom de la source, le type de problème, la personne cessionnaire principale, la date d’entrée, le statut et la priorité des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Mes portefeuilles</td> 
   <td>Rapport Portfolio qui affiche les Portfolios actifs dans lesquels l’utilisateur connecté est le Gestionnaire de Portfolios.</td> 
  </tr> 
  <tr> 
   <td>Mes programmes</td> 
   <td>Rapport Programme qui affiche Programmes et leur Description, où l’utilisateur connecté est le Gestionnaire de programmes.</td> 
  </tr> 
  <tr> 
   <td>Mes événements ouverts dans le projet</td> 
   <td>Rapport Problème qui affiche des problèmes incomplets dans les projets dont l’équipe de projet inclut l’utilisateur connecté. Le rapport affiche les champs suivants : le nom de la source, le type de problème, la personne cessionnaire principale, la date d’entrée, le statut et la priorité des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Mes projets</td> 
   <td>Rapport Projet qui affiche les projets en cours dont l’équipe de projet inclut l’utilisateur connecté. Le rapport affiche les champs suivants : la description, la date d’achèvement prévue, la date d’achèvement prévisionnelle, le pourcentage terminé, le statut et la priorité des projets.</td> 
  </tr> 
  <tr> 
   <td>Mes problèmes soumis</td> 
   <td>Rapport de problèmes qui affiche les problèmes envoyés par l’utilisateur connecté, qui ont été fermés au cours des trois derniers mois ou qui sont actuellement ouverts. Le rapport affiche les champs suivants : le nom de la source, le type de problème, la date d’entrée, le statut et la priorité des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Mes tâches</td> 
   <td>Rapport Tâche qui affiche des tâches incomplètes dans les projets actuels affectés à l’utilisateur connecté. Le rapport affiche les champs suivants : la durée prévue, le nom du projet, la personne cessionnaire principale, la date de début prévue, la date d’achèvement prévue, le pourcentage terminé et la priorité des tâches.</td> 
  </tr> 
  <tr> 
   <td>Mes feuilles de temps</td> 
   <td>Rapport de feuille de temps qui affiche toutes les feuilles de temps de l’utilisateur connecté. Le rapport affiche les champs suivants : la période, le nom de la personne propriétaire, le nombre total d’heures, les heures supplémentaires, le nom de l’approbateur ou de l’approbatrice et le statut des feuilles de temps.</td> 
  </tr> 
  <tr> 
   <td>Mes événements non affectés</td> 
   <td>Un rapport Problème qui affiche les problèmes en cours affectés à l’un des rôles de tâche de l’utilisateur connecté et qui ne sont pas affectés à l’utilisateur. Le rapport affiche les champs suivants : le nom de la source, le type de problème, la date d’entrée, le statut et la priorité des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Mes tâches non affectées</td> 
   <td>Rapport Tâche qui affiche les tâches incomplètes affectées à l’un des rôles de tâche de l’utilisateur connecté et qui ne sont pas affectées à l’utilisateur. Le rapport affiche les champs suivants : la durée prévue, le nom du projet, la personne cessionnaire principale, la date de début prévue, la date d’achèvement prévue, le pourcentage terminé et la priorité des tâches.</td> 
  </tr> 
  <tr> 
   <td>Mes prochaines tâches</td> 
   <td>Rapport Tâche qui affiche les tâches incomplètes qui doivent commencer dans les deux semaines à venir, qui se trouvent sur les projets en cours et qui sont affectées à l’utilisateur connecté. Le rapport affiche les champs suivants : le nom du projet, la date d’achèvement prévue, la date d’achèvement prévisionnelle, le pourcentage d’achèvement et le statut des tâches.</td> 
  </tr> 
  <tr> 
   <td>Ouvrir des feuilles de temps (sur invite)</td> 
   <td>Rapport de feuille de temps qui affiche les feuilles de temps ouvertes. Le rapport affiche les champs suivants : la période, la personne propriétaire, le nombre total d’heures, les heures supplémentaires, le nom de la personne chargée de l’approbation et le statut des feuilles de temps. Le rapport est ordonné par : la date de début de la feuille de temps, la date de fin de la feuille de temps, le nom de la personne chargée de l’approbation de la feuille de temps et le nom de l’utilisateur ou de l’utilisatrice.</td> 
  </tr> 
  <tr> 
   <td>Projet dépassant le budget par portefeuille</td> 
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets. Le rapport est regroupé par nom de portfolio.</td> 
  </tr> 
  <tr> 
   <td>Coût prévu du portefeuille par programme</td> 
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets. Le rapport est déclenché par nom de portfolio, groupé par nom de programme, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coût prévu du portefeuille par projet</td> 
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets. Le rapport est ordonné par nom de portfolio, regroupé par nom de projet, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu prévu du portefeuille par programme</td> 
   <td>Rapport Projet qui affiche les recettes prévues et les recettes réelles des projets. Le rapport est déclenché par nom de portfolio, groupé par nom de programme, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu prévu du portefeuille par projet</td> 
   <td>Rapport Projet qui affiche les recettes prévues et les recettes réelles des projets. Le rapport est ordonné par nom de portfolio, regroupé par nom de projet, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus / coûts réels par portefeuille</td> 
   <td>Rapport Projet qui affiche par Portfolio le coût planifié et le coût réel des projets. Le rapport est regroupé par nom de portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus / coûts réels par programme</td> 
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets par programme. Le rapport est regroupé par nom de portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus / revenus réels par portefeuille</td> 
   <td>Rapport Projet qui affiche les Recettes prévues et les Recettes réelles des projets. Le rapport est regroupé par nom de portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts des dépenses par portefeuille revenus réels par programme</td> 
   <td>Rapport Projet qui affiche les Recettes prévues et les Recettes réelles des projets. Le rapport est regroupé par nom de programme et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts du portefeuille, regroupés par programme et par mois</td> 
   <td>Rapport Tableau de projets qui affiche le coût planifié, le coût budgété et le coût réel des projets. Le rapport est regroupé par nom de portfolio, nom de programme et mois de la date de début prévue des projets.</td> 
  </tr> 
  <tr> 
   <td>Projets du portefeuille par statut, classés par programme</td> 
   <td>Rapport Projet qui affiche le statut des projets. Le rapport est regroupé par nom de programme et par statut du projet, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets du portefeuille regroupés par statut et portefeuille</td> 
   <td>Rapport Projet qui affiche le nom du Portfolio et le statut des projets. Le rapport est regroupé en fonction du nom du portfolio et du statut des projets, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu du portefeuille par programme</td> 
   <td>Rapport Projet qui affiche le nom du Portfolio, le nom du programme, les recettes prévues et les recettes réelles des projets. Le rapport est regroupé par nom de portfolio et par nom de programme, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenus du portefeuille, regroupés par programme et par mois</td> 
   <td>Rapport de projet matrice qui affiche les Recettes prévues, les Recettes réelles, le Nom du Portfolio et le Nom du programme. Le rapport est regroupé par nom de portfolio, nom de programme et mois de la date de début prévue des projets.</td> 
  </tr> 
  <tr> 
   <td>Coûts et revenus du projet par statut de la tâche</td> 
   <td>Rapport de tâches de matrice qui affiche le coût planifié, le coût réel, les recettes planifiées, les recettes réelles et le nom du projet des tâches. Le rapport est regroupé par nom de projet et par statut des tâches.</td> 
  </tr> 
  <tr> 
   <td>Revenus du projet / revenus par portefeuille</td> 
   <td>Rapport Projet qui affiche le nom du Portfolio, le coût réel et les recettes réelles des projets. Le rapport est regroupé par nom de portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Frais du projet, par mois et par trimestre</td> 
   <td>Rapport de dépenses matrice qui affiche la date d’entrée, le montant planifié, le montant réel et le projet des dépenses. Le rapport est regroupé par nom de projet, trimestre et mois de la date d’entrée des dépenses.</td> 
  </tr> 
  <tr> 
   <td>Coûts horaire du projet, par type d'heures, par mois</td> 
   <td>Rapport Heure matriciel qui affiche les champs suivants : Heures, Date d’entrée, Coût réel des projets, Type d’heure, Nom du projet. Le rapport est regroupé par nom de projet, mois de la date d’entrée des heures et type d’heure.</td> 
  </tr> 
  <tr> 
   <td>Coûts des frais et de travail du projet, par mois et par trimestre</td> 
   <td>Rapport Tableau de projets qui affiche le coût du travail planifié, le coût réel du travail, le coût planifié des dépenses et le coût réel des dépenses des projets. Le rapport est regroupé par nom de projet et par trimestre et mois de la date de début effective des projets.</td> 
  </tr> 
  <tr> 
   <td>Performances du projet</td> 
   <td>Un rapport Projet qui affiche les champs suivants des projets en cours : Date d’échéance, IPC, IPC, experts, coûts planifiés, budget, EAC et dépenses des projets.</td> 
  </tr> 
  <tr> 
   <td>Demandes de projet</td> 
   <td>Rapport Projet qui affiche les projets demandés. Le rapport affiche les champs suivants : la description, la date d’achèvement prévue, la date d’achèvement prévisionnelle, le pourcentage terminé, le statut et la priorité des projets.</td> 
  </tr> 
  <tr> 
   <td>Projets par condition</td> 
   <td>Rapport Projet qui affiche la condition des projets. Le rapport est regroupé par statut et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets par condition, par groupe</td> 
   <td>Rapport Projet qui affiche l’état d’avancement et le groupe des projets. Le rapport est regroupé par nom de groupe et par statut de la progression, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets par priorité</td> 
   <td>Rapport Projet qui affiche la priorité des projets. Le rapport est regroupé par priorité et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets par statut de progression</td> 
   <td>Rapport Projet qui affiche l’état d’avancement des projets. Le rapport est regroupé par statut de la progression et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Tâches par statut de progression</td> 
   <td>Rapport Tâche qui affiche l’état d’avancement de toutes les tâches dans les projets en cours. Le rapport est regroupé par statut de la progression et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Tâches par statut</td> 
   <td>Un rapport Tâche qui affiche le Statut de toutes les tâches. Le rapport est regroupé par statut et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Feuilles de temps à vérifier</td> 
   <td>Rapport de feuille de temps qui affiche les feuilles de temps Envoyé et Refusé dont l’approbateur est l’utilisateur connecté. Le rapport affiche les champs suivants : Période, Personne propriétaire, Nombre total d’heures, Heures supplémentaires, Nom de l’approbateur ou de l’approbatrice et Statut des feuilles de temps.</td> 
  </tr> 
  <tr> 
   <td>Tâches problématiques</td> 
   <td>Rapport Tâche qui affiche des tâches incomplètes avec un état de progression en retard ou en arrière, une date de remise antérieure à demain et où l’utilisateur connecté fait partie de l’équipe de projet du projet sur laquelle se trouvent les tâches. Le rapport affiche les champs suivants : Durée prévue, Nom du projet, Personne cessionnaire principale, Date de début prévue, Date d’achèvement prévue, Pourcentage terminé et Priorité des tâches.</td> 
  </tr> 
  <tr> 
   <td>Connexions utilisateur</td> 
   <td>Rapport Utilisateur qui affiche les champs suivants : identifiant unique, nombre de connexions (nombre de fois où l’utilisateur s’est connecté depuis qu’il a commencé avec Workfront), date de dernière connexion des utilisateurs. Le rapport est regroupé par niveau d’accès des utilisateurs et utilisatrices.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Accéder aux rapports intégrés

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

{{step1-click-main-menu}}

1. Cliquez sur **Rapports**.
1. Cliquez sur **Tous les rapports**.
1. Développez le menu déroulant **Filtre**, puis sélectionnez **Nouveau filtre**.

1. Cliquez sur **Ajouter une règle de filtre**.
1. Dans le champ **Saisissez le nom du champ**, saisissez **ID global**.

1. Sous l’objet **Rapport**, sélectionnez **ID global**.

1. Dans le menu déroulant du modificateur de filtre, sélectionnez **N’est pas vide**.\
   ![](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Cliquez sur **Enregistrer le filtre**.\
   La liste des rapports n’affiche que les rapports intégrés.\
   Pour plus d’informations sur les rapports natifs disponibles, reportez-vous à la section [Présentation des rapports natifs](#overview-of-built-in-reports) de cet article.
