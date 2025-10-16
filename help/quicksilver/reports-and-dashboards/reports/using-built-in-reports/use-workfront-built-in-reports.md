---
product-area: reporting
navigation-topic: using-built-in-reports
title: Utiliser les rapports intégrés d’Adobe Workfront
description: Adobe Workfront dispose d’une liste exhaustive de rapports intégrés prêts à l’emploi. Les équipes d’administration de Workfront peuvent masquer les rapports intégrés pour que les utilisateurs et utilisatrices n’y aient pas accès.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '2978'
ht-degree: 56%

---

# Utiliser les rapports intégrés d’Adobe Workfront

<!--Audited: 11/2024-->

Adobe Workfront dispose d’une liste étendue de rapports intégrés que vous pouvez utiliser.

Les administrateurs et administratrices de Workfront peuvent masquer les rapports intégrés afin que les utilisateurs et utilisatrices n’y aient pas accès. Pour plus d’informations sur la façon de masquer les rapports intégrés, voir [Masquer les rapports intégrés](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
      <p>Contributeur ou version ultérieure</p>
      <p>Requête ou supérieure</p>
   </td>
  </tr>
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Accès supérieur ou égal à Rapports, Tableaux de bord, Calendriers</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur un rapport pour ajouter ou modifier un filtre d’un rapport</p> <p>Gérer les autorisations sur un filtre pour le modifier dans une liste</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vue d’ensemble des rapports intégrés {#overview-of-built-in-reports}

Vous pouvez copier un rapport intégré et l&#39;enregistrer en tant que nouveau rapport. Pour plus d’informations sur la création de copies de rapports intégrés, consultez la section [Créer une nouvelle version d’un rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#create-a-new-version-of-a-report) dans l’article [Créer une copie d’un rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

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
   <td>Rapport sur les projets qui affiche le coût prévu et le coût réel des projets. Le rapport est groupé par nom de programme, demandé par nom de portfolio, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coût réel du portefeuille par projet</td> 
   <td>Rapport sur les projets qui affiche le coût prévu et le coût réel des projets. Le rapport est groupé par nom de projet, demandé par nom de portfolio, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu réel du portefeuille par programme</td> 
   <td>Rapport sur les projets qui affiche le revenu prévu et le revenu réel des projets. Le rapport est groupé par nom de programme, demandé par nom de portfolio, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu réel du portefeuille par projet</td> 
   <td>Rapport sur les projets qui affiche le revenu prévu et le revenu réel des projets. Le rapport est groupé par nom de projet, demandé par nom de portfolio, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenus réels par entreprise</td> 
   <td>Rapport sur les projets qui affiche le revenu réel et la société des projets. Le rapport est groupé par nom de société et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenus réels par groupe</td> 
   <td>Rapport sur les projets qui affiche le revenu réel et le groupe des projets. Le rapport est groupé par nom de groupe et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Toutes les feuilles de temps ouvertes</td> 
   <td>Rapport sur les feuilles de temps qui affiche les feuilles de temps ouvertes. Le rapport affiche les champs suivants : la période, le nom de la personne propriétaire, le nombre total d’heures, les heures supplémentaires, le nom de l’approbateur ou de l’approbatrice et le statut des feuilles de temps.</td> 
  </tr> 
  <tr> 
   <td>Approbation des feuilles de temps (sur invite)</td> 
   <td>Rapport sur les feuilles de temps qui affiche les feuilles de temps soumises ou rejetées avec les approbateurs. Le rapport affiche les champs suivants : la période, la personne propriétaire, le nombre total d’heures, les heures supplémentaires, le nom de l’approbateur ou de l’approbatrice et le statut des feuilles de temps. Le rapport est ordonné par : la date de début de la feuille de temps, la date de fin de la feuille de temps, le nom de la personne chargée de l’approbation de la feuille de temps et le nom de l’utilisateur ou de l’utilisatrice.</td> 
  </tr> 
  <tr> 
   <td>Projets à risque</td> 
   <td>Rapport sur les projets qui affiche les projets actuels et prévus associés à une condition En danger ou En difficulté. Le rapport affiche les champs suivants : la description, la date d’achèvement prévue, la date d’achèvement prévisionnelle, le pourcentage terminé, le statut et la priorité des projets. Le rapport est regroupé par nom de portfolio.</td> 
  </tr> 
  <tr> 
   <td>Facturation des revenus par entreprise</td> 
   <td>Rapport sur les projets qui affiche la société et les revenus facturés des projets. Le rapport est groupé par nom de société et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Facturation des revenus par groupe</td> 
   <td>Rapport sur les projets qui affiche les revenus facturés et le groupe des projets. Le rapport est groupé par nom de groupe et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Facturation des revenus par mois</td> 
   <td>Enregistrement de facturation qui affiche le nom du projet, les revenus facturés du projet et la date de facturation des enregistrements de facturation. Le rapport est regroupé par mois de la date de facturation des enregistrements de facturation et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Événements conclus par semaine</td> 
   <td>Rapport sur les événements qui affiche la date d'achèvement effective des événements. Le rapport est regroupé par semaine de la date d’achèvement effective des problèmes et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Événements conclus par semaine et par utilisateur</td> 
   <td>Rapport sur les événements qui affiche la date d'achèvement effective et les affectations des événements. Le rapport est regroupé par personne cessionnaire principale et par semaine de la date d’achèvement effective des problèmes, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets actuels</td> 
   <td>Rapport sur les projets qui affiche tous les projets actuels. Le rapport affiche les champs suivants : la description, la date d’achèvement prévue, la date d’achèvement prévisionnelle, le pourcentage terminé, le statut et la priorité des projets.</td> 
  </tr> 
  <tr> 
   <td>Coûts horaires par utilisateur par mois</td> 
   <td>Rapport de matrice sur les heures qui affiche le nombre d'heures consignées et leur coût réel. Le rapport est regroupé par nom de propriétaire et par mois de la date d’entrée des heures.</td> 
  </tr> 
  <tr> 
   <td>Heures par utilisateur</td> 
   <td>Rapport sur les heures qui affiche le nombre d'heures consignées. Le rapport est regroupé par nom de propriétaire et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Heures, par utilisateur, par semaine</td> 
   <td>Rapport de matrice sur les heures qui affiche le nombre d'heures consignées au cours des quatre dernières semaines et la date de saisie des heures. Le rapport est présenté en fonction de la date d’entrée des heures et est regroupé par nom de propriétaire et par mois de la date d’entrée des heures.</td> 
  </tr> 
  <tr> 
   <td>Événements par statut</td> 
   <td>Rapport sur les événements qui affiche le statut des événements. Le rapport est regroupé par statut des problèmes et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Événements par statut et projet</td> 
   <td>Rapport de matrice sur les événements qui affiche le statut des événements dans les projets actuels et le nom du projet. Le rapport est regroupé par nom de projet et par statut des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Main-d'œuvre / Coûts des dépenses par portefeuille</td> 
   <td>Rapport sur les projets qui affiche le coût prévu de la main-d'œuvre, le coût réel de la main-d'œuvre, le coût prévu de dépense et le coût réel de dépense des projets. Le rapport est regroupé par nom de portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Main-d'œuvre / Coûts des dépenses par programme</td> 
   <td>Rapport sur les projets qui affiche le coût prévu de la main-d'œuvre, le coût réel de la main-d'œuvre, le coût prévu de dépense et le coût réel de dépense des projets. Le rapport est regroupé par nom de portfolio et par nom de programme, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus/coûts réels mensuels du portefeuille par projet</td> 
   <td>Rapport de matrice sur les projets (données financières) qui affiche la date d'allocation, les coûts prévus totaux, les coûts réels totaux et la variance des coûts totaux des projets. Le rapport est regroupé par nom de projet, trimestre et mois de la date d’attribution.</td> 
  </tr> 
  <tr> 
   <td>Revenus prévus/revenus réels mensuels du portefeuille par projet</td> 
   <td>Rapport de matrice sur les projets (données financières) qui affiche la date d'affectation, les revenus prévus totaux, les revenus réels totaux et la variance des revenus totaux des projets. Le rapport est regroupé par nom de projet, trimestre et mois de la date d’attribution.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus/coûts réels mensuels du projet</td> 
   <td>Rapport de matrice sur les projets (données financières) qui affiche la date d'allocation, les coûts prévus totaux, les coûts réels totaux et la variance des coûts totaux des projets. Le rapport est regroupé par nom de projet, par trimestre et par mois de la date d’allocation et est présenté par le nom du projet.</td> 
  </tr> 
  <tr> 
   <td>Revenus prévus/revenus réels mensuels du projet</td> 
   <td>Rapport de matrice sur les projets (données financières) qui affiche la date d'affectation, les revenus prévus totaux, les revenus réels totaux et la variance des revenus totaux des projets. Le rapport est regroupé par nom de projet, par trimestre et par mois de la date d’allocation et est présenté par le nom du projet.</td> 
  </tr> 
  <tr> 
   <td>Mes documents</td> 
   <td>Rapport sur les documents qui affiche les documents chargés par l'utilisateur connecté. Le rapport affiche les champs suivants : le nom de la personne propriétaire, la date de modification, la taille, le nombre de versions, la source et le type des documents.</td> 
  </tr> 
  <tr> 
   <td>Mes favoris</td> 
   <td>Rapport sur les favoris qui affiche la liste des objets marqués comme favoris par l'utilisateur connecté. Le rapport affiche les champs suivants : le type d’objet et le nom des favoris.</td> 
  </tr> 
  <tr> 
   <td>Mes problèmes</td> 
   <td>Rapport sur les événements qui affiche les événements incomplets affectés à l'utilisateur connecté. Le rapport affiche les champs suivants : le nom de la source, le type de problème, la personne cessionnaire principale, la date d’entrée, le statut et la priorité des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Mes portefeuilles</td> 
   <td>Rapport Portfolio qui affiche les portefeuilles actifs où l'utilisateur connecté est le gestionnaire Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Mes programmes</td> 
   <td>Rapport sur les programmes qui affiche les programmes et leur description, où l'utilisateur connecté est le gestionnaire de programmes.</td> 
  </tr> 
  <tr> 
   <td>Mes événements ouverts dans le projet</td> 
   <td>Rapport sur les événements qui affiche les problèmes incomplets dans les projets dont l'équipe du projet inclut l'utilisateur connecté. Le rapport affiche les champs suivants : le nom de la source, le type de problème, la personne cessionnaire principale, la date d’entrée, le statut et la priorité des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Mes projets</td> 
   <td>Rapport sur les projets qui affiche les projets actuels dont l'équipe de projet inclut l'utilisateur connecté. Le rapport affiche les champs suivants : la description, la date d’achèvement prévue, la date d’achèvement prévisionnelle, le pourcentage terminé, le statut et la priorité des projets.</td> 
  </tr> 
  <tr> 
   <td>Mes problèmes soumis</td> 
   <td>Rapport sur les événements qui affiche les événements soumis par l'utilisateur connecté, qui ont été clos au cours des trois derniers mois ou qui sont actuellement ouverts. Le rapport affiche les champs suivants : le nom de la source, le type de problème, la date d’entrée, le statut et la priorité des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Mes tâches</td> 
   <td>Rapports sur les tâches qui affiche les tâches incomplètes dans les projets actuels affectés à l'utilisateur connecté. Le rapport affiche les champs suivants : la durée prévue, le nom du projet, la personne cessionnaire principale, la date de début prévue, la date d’achèvement prévue, le pourcentage terminé et la priorité des tâches.</td> 
  </tr> 
  <tr> 
   <td>Mes feuilles de temps</td> 
   <td>Rapport sur les feuilles de temps qui affiche toutes les feuilles de temps de l'utilisateur connecté. Le rapport affiche les champs suivants : la période, le nom de la personne propriétaire, le nombre total d’heures, les heures supplémentaires, le nom de l’approbateur ou de l’approbatrice et le statut des feuilles de temps.</td> 
  </tr> 
  <tr> 
   <td>Mes événements non affectés</td> 
   <td>Rapport sur les événements qui affiche les événements ouverts affectés à l'une des fonctions de l'utilisateur connecté et qui ne sont pas affectés à l'utilisateur. Le rapport affiche les champs suivants : le nom de la source, le type de problème, la date d’entrée, le statut et la priorité des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Mes tâches non affectées</td> 
   <td>Rapports sur les tâches qui affiche les tâches incomplètes affectées à l'une des fonctions de l'utilisateur connecté et qui ne sont pas affectées à l'utilisateur. Le rapport affiche les champs suivants : la durée prévue, le nom du projet, la personne cessionnaire principale, la date de début prévue, la date d’achèvement prévue, le pourcentage terminé et la priorité des tâches.</td> 
  </tr> 
  <tr> 
   <td>Mes prochaines tâches</td> 
   <td>Rapports sur les tâches qui affiche les tâches incomplètes censées démarrer au cours des deux prochaines semaines, associées à des projets actuels et affectées à l'utilisateur connecté. Le rapport affiche les champs suivants : le nom du projet, la date d’achèvement prévue, la date d’achèvement prévisionnelle, le pourcentage d’achèvement et le statut des tâches.</td> 
  </tr> 
  <tr> 
   <td>Ouvrir des feuilles de temps (sur invite)</td> 
   <td>Rapport sur les feuilles de temps qui affiche les feuilles de temps ouvertes. Le rapport affiche les champs suivants : la période, la personne propriétaire, le nombre total d’heures, les heures supplémentaires, le nom de la personne chargée de l’approbation et le statut des feuilles de temps. Le rapport est ordonné par : la date de début de la feuille de temps, la date de fin de la feuille de temps, le nom de la personne chargée de l’approbation de la feuille de temps et le nom de l’utilisateur ou de l’utilisatrice.</td> 
  </tr> 
  <tr> 
   <td>Projet dépassant le budget par portefeuille</td> 
   <td>Rapport sur les projets qui affiche le coût prévu et le coût réel des projets. Le rapport est regroupé par nom de portfolio.</td> 
  </tr> 
  <tr> 
   <td>Coût prévu du portefeuille par programme</td> 
   <td>Rapport sur les projets qui affiche le coût prévu et le coût réel des projets. Le rapport est déclenché par nom de portfolio, groupé par nom de programme, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coût prévu du portefeuille par projet</td> 
   <td>Rapport sur les projets qui affiche le coût prévu et le coût réel des projets. Le rapport est ordonné par nom de portfolio, regroupé par nom de projet, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu prévu du portefeuille par programme</td> 
   <td>Rapport sur les projets qui affiche le revenu prévu et le revenu réel des projets. Le rapport est déclenché par nom de portfolio, groupé par nom de programme, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu prévu du portefeuille par projet</td> 
   <td>Rapport sur les projets qui affiche le revenu prévu et le revenu réel des projets. Le rapport est ordonné par nom de portfolio, regroupé par nom de projet, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus / coûts réels par portefeuille</td> 
   <td>Rapport sur les projets qui affiche le coût prévu et le coût réel des projets par Portfolio. Le rapport est regroupé par nom de portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus / coûts réels par programme</td> 
   <td>Rapport sur les projets qui affiche le coût prévu et le coût réel des projets par programme. Le rapport est regroupé par nom de portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus / revenus réels par portefeuille</td> 
   <td>Rapport sur les projets qui affiche le revenu prévu et le revenu réel des projets. Le rapport est regroupé par nom de portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts des dépenses par portefeuille revenus réels par programme</td> 
   <td>Rapport sur les projets qui affiche le revenu prévu et le revenu réel des projets. Le rapport est regroupé par nom de programme et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts du portefeuille, regroupés par programme et par mois</td> 
   <td>Rapport de matrice sur les projets qui affiche le coût prévu, le coût budgété et le coût réel des projets. Le rapport est regroupé par nom de portfolio, nom de programme et mois de la date de début prévue des projets.</td> 
  </tr> 
  <tr> 
   <td>Projets du portefeuille par statut, classés par programme</td> 
   <td>Rapport sur les projets qui affiche le statut des projets. Le rapport est regroupé par nom de programme et par statut du projet, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets du portefeuille regroupés par statut et portefeuille</td> 
   <td>Rapport sur les projets qui affiche le nom du Portfolio et le statut des projets. Le rapport est regroupé en fonction du nom du portfolio et du statut des projets, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu du portefeuille par programme</td> 
   <td>Rapport sur les projets qui affiche le nom du Portfolio, le nom du programme, le revenu prévu et le revenu réel des projets. Le rapport est regroupé par nom de portfolio et par nom de programme, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenus du portefeuille, regroupés par programme et par mois</td> 
   <td>Rapport de matrice sur les projets qui affiche le revenu prévu, le revenu réel, le nom du Portfolio et le nom du programme. Le rapport est regroupé par nom de portfolio, nom de programme et mois de la date de début prévue des projets.</td> 
  </tr> 
  <tr> 
   <td>Coûts et revenus du projet par statut de la tâche</td> 
   <td>Rapport de matrice sur les tâches qui affiche le coût prévu, le coût réel, le revenu prévu, le revenu réel et le nom du projet des tâches. Le rapport est regroupé par nom de projet et par statut des tâches.</td> 
  </tr> 
  <tr> 
   <td>Revenus du projet / revenus par portefeuille</td> 
   <td>Rapport sur les projets qui affiche le nom du Portfolio, le coût réel et le revenu réel des projets. Le rapport est regroupé par nom de portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Frais du projet, par mois et par trimestre</td> 
   <td>Rapport de matrice sur les dépenses qui affiche la date de saisie, le montant prévu, le montant réel et le projet des dépenses. Le rapport est regroupé par nom de projet, trimestre et mois de la date d’entrée des dépenses.</td> 
  </tr> 
  <tr> 
   <td>Coûts horaire du projet, par type d'heures, par mois</td> 
   <td>Rapport de matrice sur les heures qui affiche les champs suivants : heures, date de saisie, coût réel des projets, type d'heures, nom du projet. Le rapport est regroupé par nom de projet, mois de la date d’entrée des heures et type d’heure.</td> 
  </tr> 
  <tr> 
   <td>Coûts des frais et de travail du projet, par mois et par trimestre</td> 
   <td>Rapport de matrice sur les projets qui affiche le coût prévu de la main-d'œuvre, le coût réel de la main-d'œuvre, le coût prévu de dépense et le coût réel de dépense des projets. Le rapport est regroupé par nom de projet et par trimestre et mois de la date de début effective des projets.</td> 
  </tr> 
  <tr> 
   <td>Performances du projet</td> 
   <td>Rapport sur les projets qui affiche les champs suivants des projets actuels : date d'échéance, ICP, IHP, ICH, coût prévu, budget, CRE et Dépenses des projets.</td> 
  </tr> 
  <tr> 
   <td>Demandes de projet</td> 
   <td>Rapport sur les projets qui affiche les projets demandés. Le rapport affiche les champs suivants : la description, la date d’achèvement prévue, la date d’achèvement prévisionnelle, le pourcentage terminé, le statut et la priorité des projets.</td> 
  </tr> 
  <tr> 
   <td>Projets par condition</td> 
   <td>Rapport sur les projets qui affiche le statut des projets. Le rapport est regroupé par statut et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets par condition, par groupe</td> 
   <td>Rapport sur les projets qui affiche le statut de progression et le groupe des projets. Le rapport est regroupé par nom de groupe et par statut de la progression, et il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets par priorité</td> 
   <td>Rapport sur les projets qui affiche la priorité des projets. Le rapport est regroupé par priorité et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets par statut de progression</td> 
   <td>Rapport sur les projets qui affiche le statut de progression des projets. Le rapport est regroupé par statut de la progression et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Tâches par statut de progression</td> 
   <td>Rapport sur les tâches qui affiche le statut de progression de toutes les tâches dans les projets actuels. Le rapport est regroupé par statut de la progression et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Tâches par statut</td> 
   <td>Rapport sur les tâches qui affiche le statut de toutes les tâches. Le rapport est regroupé par statut et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Feuilles de temps à vérifier</td> 
   <td>Rapport sur les feuilles de temps qui affiche les feuilles de temps soumises et rejetées dont l'approbateur est l'utilisateur connecté. Le rapport affiche les champs suivants : Période, Personne propriétaire, Nombre total d’heures, Heures supplémentaires, Nom de l’approbateur ou de l’approbatrice et Statut des feuilles de temps.</td> 
  </tr> 
  <tr> 
   <td>Tâches problématiques</td> 
   <td>Rapports sur les tâches qui affiche les tâches incomplètes avec un statut de progression Tardif ou En retard, une date de remise antérieure à demain et où l'utilisateur connecté fait partie de l'équipe du projet auquel les tâches sont associées. Le rapport affiche les champs suivants : Durée prévue, Nom du projet, Personne cessionnaire principale, Date de début prévue, Date d’achèvement prévue, Pourcentage terminé et Priorité des tâches.</td> 
  </tr> 
  <tr> 
   <td>Connexions utilisateur</td> 
   <td>Rapport sur les utilisateurs qui affiche les champs suivants : ID unique, Nombre de connexions (nombre de fois où l’utilisateur s’est connecté depuis avoir commencé avec Workfront), Date de dernière connexion des utilisateurs. Le rapport est regroupé par niveau d’accès des utilisateurs et utilisatrices.</td> 
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
1. Développez le menu déroulant **Filtre** et sélectionnez **Nouveau filtre**.

1. Cliquez sur **Ajouter une règle de filtre**.
1. Dans le champ **Saisissez le nom du champ**, saisissez **ID global**.

1. Sous l’objet **Rapport**, sélectionnez **ID global**.

1. Dans le menu déroulant du modificateur de filtre, sélectionnez **N’est pas vide**.\
   ![Filtre d’ID global pour les rapports système](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Cliquez sur **Enregistrer le filtre**.\
   La liste des rapports n’affiche que les rapports intégrés.\
   Pour plus d’informations sur les rapports natifs disponibles, consultez la section [Présentation des rapports natifs](#overview-of-built-in-reports) dans cet article.
