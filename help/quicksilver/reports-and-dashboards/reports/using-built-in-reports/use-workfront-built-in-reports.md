---
product-area: reporting
navigation-topic: using-built-in-reports
title: Utiliser les rapports intégrés d’Adobe Workfront
description: Adobe Workfront contient une liste complète de rapports natifs prêts à l’emploi. Les administrateurs de Workfront peuvent masquer les rapports intégrés afin que les utilisateurs n’y aient pas accès.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: 49bd393af77a67aa1e3a443c4189569178e99ada
workflow-type: tm+mt
source-wordcount: '2951'
ht-degree: 11%

---

# Utiliser les rapports intégrés d’Adobe Workfront

<!--Audited: 07/2024-->

Adobe Workfront contient une liste complète de rapports intégrés que vous pouvez utiliser.

Les administrateurs de Workfront peuvent masquer les rapports intégrés afin que les utilisateurs n’y aient pas accès.

Pour plus d’informations sur la façon de masquer les rapports natifs, voir [Masquage des rapports natifs](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouvelle : contributeur ou contributrice ou supérieure</p>  
   <p>Actuelle : demande ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Affichage ou accès supérieur à Reports, Dashboard, Calendriers</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport pour ajouter ou modifier un filtre sur un rapport</p> <p>Gérer les autorisations d'un filtre pour l'éditer dans une liste</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Présentation des rapports natifs {#overview-of-built-in-reports}

Vous pouvez personnaliser un rapport intégré et l’enregistrer en tant que nouveau rapport. Pour plus d’informations sur la personnalisation des rapports intégrés, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Les rapports suivants sont fournis avec le package Workfront. Les rapports sont disponibles pour tous les utilisateurs qui disposent au moins des droits d’affichage pour les rapports natifs à leur niveau d’accès.

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
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets. Le rapport est regroupé par nom de programme, sous la forme d’un nom de Portfolio, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coût réel du portefeuille par projet</td> 
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets. Le rapport est regroupé par nom de projet, en fonction du nom du Portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu réel du portefeuille par programme</td> 
   <td>Rapport Projet qui affiche les Recettes prévues et les Recettes réelles des projets. Le rapport est regroupé par nom de programme, sous la forme d’un nom de Portfolio, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu réel du portefeuille par projet</td> 
   <td>Rapport Projet qui affiche les Recettes prévues et les Recettes réelles des projets. Le rapport est regroupé par nom de projet, en fonction du nom du Portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenus réels par entreprise</td> 
   <td>Rapport Projet qui affiche les recettes réelles et la société des projets. Le rapport est regroupé par nom d’entreprise et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenus réels par groupe</td> 
   <td>Rapport Projet qui affiche les recettes réelles et le groupe des projets. Le rapport est regroupé par nom de groupe et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Toutes les feuilles de temps ouvertes</td> 
   <td>Rapport de feuille de temps qui affiche les feuilles de temps ouvertes. Le rapport affiche les champs suivants : plage de dates, nom du propriétaire, nombre total d’heures, période de dépassement, nom du approbateur et état des feuilles de temps.</td> 
  </tr> 
  <tr> 
   <td>Approbation des feuilles de temps (sur invite)</td> 
   <td>Rapport de feuille de temps qui affiche les feuilles de temps envoyées ou rejetées avec les approbateurs. Le rapport affiche les champs suivants : plage de dates, propriétaire, heures totales, heures de dépassement, nom de l’approbateur et état des feuilles de temps. Le rapport est invité par : Date de début de la feuille de temps, Date de fin de la feuille de temps, Nom de l’approbateur de la feuille de temps et Nom d’utilisateur.</td> 
  </tr> 
  <tr> 
   <td>Projets à risque</td> 
   <td>Rapport Projet qui affiche les projets en cours et planifiés présentant une situation de risque ou de problème. Le rapport affiche les champs suivants : Description, Date de fin planifiée, Date de fin prévue, Pourcentage de fin terminée, État et Priorité des projets. Le rapport est regroupé par nom de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Facturation des revenus par entreprise</td> 
   <td>Rapport Projet qui affiche la société et les recettes de facturation des projets. Le rapport est regroupé par nom d’entreprise et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Facturation des revenus par groupe</td> 
   <td>Rapport Projet qui affiche les recettes de facturation et le groupe des projets. Le rapport est regroupé par nom de groupe et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Facturation des revenus par mois</td> 
   <td>Rapport d’enregistrement de facturation qui affiche le nom du projet, les recettes de facturation du projet et la date de facturation des enregistrements de facturation. Le rapport est regroupé par mois de la Date de facturation des enregistrements de facturation et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Événements conclus par semaine</td> 
   <td>Rapport Problème qui affiche la date d’achèvement réelle des problèmes. Le rapport est regroupé par semaine de la date d’achèvement réelle des problèmes et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Événements conclus par semaine et par utilisateur</td> 
   <td>Rapport Problème qui affiche la date d’achèvement réelle et les affectations des problèmes. Le rapport est regroupé par personne désignée principale et par semaine de la date d’achèvement réelle des problèmes. Il comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets actuels</td> 
   <td>Rapport Projet qui affiche tous les projets en cours. Le rapport affiche les champs suivants : Description, Date de fin planifiée, Date de fin prévue, Pourcentage de fin terminée, État et Priorité des projets.</td> 
  </tr> 
  <tr> 
   <td>Coûts horaires par utilisateur par mois</td> 
   <td>Rapport d’heure matrice qui affiche le nombre d’heures journalisées et leur coût réel. Le rapport est regroupé par nom de propriétaire et par mois de la Date d’entrée des heures.</td> 
  </tr> 
  <tr> 
   <td>Heures par utilisateur</td> 
   <td>Rapport Heure qui affiche le nombre d’heures journalisées. Le rapport est regroupé par nom de propriétaire et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Heures, par utilisateur, par semaine</td> 
   <td>Rapport Heure de matrice qui affiche le nombre d’heures enregistrées au cours des quatre dernières semaines et la date d’entrée des heures. Le rapport est généré par la Date d’entrée des heures et est regroupé par Nom du propriétaire et par le mois de la Date d’entrée des heures.</td> 
  </tr> 
  <tr> 
   <td>Événements par statut</td> 
   <td>Rapport Problème qui affiche le statut des problèmes. Le rapport est regroupé par Etat des problèmes et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Événements par statut et projet</td> 
   <td>Rapport de problèmes matrice qui affiche le statut des problèmes dans les projets en cours et le nom du projet. Le rapport est regroupé par nom de projet et état des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Main-d'œuvre / Coûts des dépenses par portefeuille</td> 
   <td>Rapport Projet qui affiche le coût de la main-d’oeuvre planifié, le coût de la main-d’oeuvre réel, le coût des dépenses planifiées et le coût des dépenses réelles des projets. Le rapport est regroupé par nom de Portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Main-d'œuvre / Coûts des dépenses par programme</td> 
   <td>Rapport Projet qui affiche le coût de la main-d’oeuvre planifié, le coût de la main-d’oeuvre réel, le coût des dépenses planifiées et le coût des dépenses réelles des projets. Le rapport est regroupé par nom de Portfolio et nom de programme et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus/coûts réels mensuels du portefeuille par projet</td> 
   <td>Rapport de projet (données financières) matrice qui affiche la date d’allocation, le coût total prévu, le coût réel total et l’écart total des coûts des projets. Le rapport est regroupé par nom de projet, par trimestre et par mois de la date d’attribution.</td> 
  </tr> 
  <tr> 
   <td>Revenus prévus/revenus réels mensuels du portefeuille par projet</td> 
   <td>Rapport Tableau de projets (données financières) qui affiche la date d’attribution, le total des recettes prévues, le total des recettes réelles et l’écart total des recettes des projets. Le rapport est regroupé par nom de projet, par trimestre et par mois de la date d’attribution.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus/coûts réels mensuels du projet</td> 
   <td>Rapport de projet (données financières) matrice qui affiche la date d’allocation, le coût total prévu, le coût réel total et l’écart total des coûts des projets. Le rapport est regroupé par nom de projet, par trimestre et par mois de la date d’attribution. Le nom du projet vous y invite.</td> 
  </tr> 
  <tr> 
   <td>Revenus prévus/revenus réels mensuels du projet</td> 
   <td>Rapport Tableau de projets (données financières) qui affiche la date d’attribution, le total des recettes prévues, le total des recettes réelles et l’écart total des recettes des projets. Le rapport est regroupé par nom de projet, par trimestre et par mois de la date d’attribution. Le nom du projet vous y invite.</td> 
  </tr> 
  <tr> 
   <td>Mes documents</td> 
   <td>Rapport Document qui affiche les documents téléchargés par l’utilisateur connecté. Le rapport affiche les champs suivants : Nom du propriétaire, Date de modification, Taille, Nombre de versions, Source et Type des documents.</td> 
  </tr> 
  <tr> 
   <td>Mes favoris</td> 
   <td>Rapport Favoris qui affiche la liste des objets marqués comme favoris par l’utilisateur connecté. Le rapport affiche les champs suivants : Type d’objet et Nom des favoris.</td> 
  </tr> 
  <tr> 
   <td>Mes problèmes</td> 
   <td>Rapport Problème qui affiche les problèmes incomplets affectés à l’utilisateur connecté. Le rapport affiche les champs suivants : Nom Source, Type de problème, personne désignée principale, Date d’entrée, État et Priorité des problèmes.</td> 
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
   <td>Rapport Problème qui affiche des problèmes incomplets dans les projets dont l’équipe de projet inclut l’utilisateur connecté. Le rapport affiche les champs suivants : Nom Source, Type de problème, personne désignée principale, Date d’entrée, État et Priorité des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Mes projets</td> 
   <td>Rapport Projet qui affiche les projets en cours dont l’équipe de projet inclut l’utilisateur connecté. Le rapport affiche les champs suivants : Description, Date de fin planifiée, Date de fin prévue, Pourcentage de fin terminée, État et Priorité des projets.</td> 
  </tr> 
  <tr> 
   <td>Mes problèmes soumis</td> 
   <td>Rapport de problèmes qui affiche les problèmes envoyés par l’utilisateur connecté, qui ont été fermés au cours des trois derniers mois ou qui sont actuellement ouverts. Le rapport affiche les champs suivants : Nom Source, Type de problème, Date d’entrée, État et Priorité des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Mes tâches</td> 
   <td>Rapport Tâche qui affiche des tâches incomplètes dans les projets actuels affectés à l’utilisateur connecté. Le rapport affiche les champs suivants : Durée planifiée, Nom du projet, personne désignée principale, Début planifié, Fin planifiée, Pourcentage terminé et Priorité des tâches.</td> 
  </tr> 
  <tr> 
   <td>Mes feuilles de temps</td> 
   <td>Rapport de feuille de temps qui affiche toutes les feuilles de temps de l’utilisateur connecté. Le rapport affiche les champs suivants : plage de dates, nom du propriétaire, nombre total d’heures, période de dépassement, nom du approbateur et état des feuilles de temps.</td> 
  </tr> 
  <tr> 
   <td>Mes événements non affectés</td> 
   <td>Un rapport Problème qui affiche les problèmes en cours affectés à l’un des rôles de tâche de l’utilisateur connecté et qui ne sont pas affectés à l’utilisateur. Le rapport affiche les champs suivants : Nom Source, Type de problème, Date d’entrée, État et Priorité des problèmes.</td> 
  </tr> 
  <tr> 
   <td>Mes tâches non affectées</td> 
   <td>Rapport Tâche qui affiche les tâches incomplètes affectées à l’un des rôles de tâche de l’utilisateur connecté et qui ne sont pas affectées à l’utilisateur. Le rapport affiche les champs suivants : Durée planifiée, Nom du projet, personne désignée principale, Date de début planifiée, Date d’achèvement planifiée, Pourcentage d’achèvement terminé et Priorité des tâches.</td> 
  </tr> 
  <tr> 
   <td>Mes prochaines tâches</td> 
   <td>Rapport Tâche qui affiche les tâches incomplètes qui doivent commencer dans les deux semaines à venir, qui se trouvent sur les projets en cours et qui sont affectées à l’utilisateur connecté. Le rapport affiche les champs suivants : Nom du projet, Date de fin planifiée, Date de fin prévue, Pourcentage d’achèvement prévu et État des tâches.</td> 
  </tr> 
  <tr> 
   <td>Ouvrir des feuilles de temps (sur invite)</td> 
   <td>Rapport de feuille de temps qui affiche les feuilles de temps ouvertes. Le rapport affiche les champs suivants : plage de dates, propriétaire, heures totales, heures supplémentaires, nom de l’approbateur, état des feuilles de temps. Le rapport est invité par : Date de début de la feuille de temps, Date de fin de la feuille de temps, Nom de l’approbateur de la feuille de temps et Nom d’utilisateur.</td> 
  </tr> 
  <tr> 
   <td>Projet dépassant le budget par portefeuille</td> 
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets. Le rapport est regroupé par nom de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Coût prévu du portefeuille par programme</td> 
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets. Le rapport est généré par le nom du Portfolio, regroupé par nom de programme, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coût prévu du portefeuille par projet</td> 
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets. Le rapport est généré par le nom du Portfolio, regroupé par nom du projet et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu prévu du portefeuille par programme</td> 
   <td>Rapport Projet qui affiche les recettes prévues et les recettes réelles des projets. Le rapport est généré par le nom du Portfolio, regroupé par nom de programme, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu prévu du portefeuille par projet</td> 
   <td>Rapport Projet qui affiche les recettes prévues et les recettes réelles des projets. Le rapport est généré par le nom du Portfolio, regroupé par nom du projet et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus / coûts réels par portefeuille</td> 
   <td>Rapport Projet qui affiche par Portfolio le coût planifié et le coût réel des projets. Le rapport est regroupé par nom de Portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus / coûts réels par programme</td> 
   <td>Rapport Projet qui affiche le coût planifié et le coût réel des projets par programme. Le rapport est regroupé par nom de Portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts prévus / revenus réels par portefeuille</td> 
   <td>Rapport Projet qui affiche les Recettes prévues et les Recettes réelles des projets. Le rapport est regroupé par nom de Portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts des dépenses par portefeuille revenus réels par programme</td> 
   <td>Rapport Projet qui affiche les Recettes prévues et les Recettes réelles des projets. Le rapport est regroupé par nom de programme et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Coûts du portefeuille, regroupés par programme et par mois</td> 
   <td>Rapport Tableau de projets qui affiche le coût planifié, le coût budgété et le coût réel des projets. Le rapport est regroupé par nom de Portfolio, nom du programme et mois de la date de début prévue des projets.</td> 
  </tr> 
  <tr> 
   <td>Projets du portefeuille par statut, classés par programme</td> 
   <td>Rapport Projet qui affiche le statut des projets. Le rapport est regroupé par nom de programme et état du projet et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets du portefeuille regroupés par statut et portefeuille</td> 
   <td>Rapport Projet qui affiche le nom du Portfolio et le statut des projets. Le rapport est regroupé par nom de Portfolio et état des projets, avec un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenu du portefeuille par programme</td> 
   <td>Rapport Projet qui affiche le nom du Portfolio, le nom du programme, les recettes prévues et les recettes réelles des projets. Le rapport est regroupé par nom de Portfolio et nom de programme, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Revenus du portefeuille, regroupés par programme et par mois</td> 
   <td>Rapport de projet matrice qui affiche les Recettes prévues, les Recettes réelles, le Nom du Portfolio et le Nom du programme. Le rapport est regroupé par nom de Portfolio, nom du programme et mois de la date de début prévue des projets.</td> 
  </tr> 
  <tr> 
   <td>Coûts et revenus du projet par statut de la tâche</td> 
   <td>Rapport de tâches de matrice qui affiche le coût planifié, le coût réel, les recettes planifiées, les recettes réelles et le nom du projet des tâches. Le rapport est regroupé par nom de projet et état des tâches.</td> 
  </tr> 
  <tr> 
   <td>Revenus du projet / revenus par portefeuille</td> 
   <td>Rapport Projet qui affiche le nom du Portfolio, le coût réel et les recettes réelles des projets. Le rapport est regroupé par nom de Portfolio et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Frais du projet, par mois et par trimestre</td> 
   <td>Rapport de dépenses matrice qui affiche la date d’entrée, le montant planifié, le montant réel et le projet des dépenses. Le rapport est regroupé par nom de projet, trimestre et mois de la Date d'entrée des dépenses.</td> 
  </tr> 
  <tr> 
   <td>Coûts horaire du projet, par type d'heures, par mois</td> 
   <td>Rapport Heure matriciel qui affiche les champs suivants : Heures, Date d’entrée, Coût réel des projets, Type d’heure, Nom du projet. Le rapport est regroupé par nom de projet, mois de la date d’entrée des heures et type d’heure.</td> 
  </tr> 
  <tr> 
   <td>Coûts des frais et de travail du projet, par mois et par trimestre</td> 
   <td>Rapport Tableau de projets qui affiche le coût du travail planifié, le coût réel du travail, le coût planifié des dépenses et le coût réel des dépenses des projets. Le rapport est regroupé par nom de projet et par trimestre et par mois de la Date de début réelle des projets.</td> 
  </tr> 
  <tr> 
   <td>Performances du projet</td> 
   <td>Un rapport Projet qui affiche les champs suivants des projets en cours : Date d’échéance, IPC, IPC, experts, coûts planifiés, budget, EAC et dépenses des projets.</td> 
  </tr> 
  <tr> 
   <td>Demandes de projet</td> 
   <td>Rapport Projet qui affiche les projets demandés. Le rapport affiche les champs suivants : Description, Date de fin planifiée, Date de fin prévue, Pourcentage de fin terminée, État et Priorité des projets.</td> 
  </tr> 
  <tr> 
   <td>Projets par condition</td> 
   <td>Rapport Projet qui affiche la condition des projets. Le rapport est regroupé par condition et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets par condition, par groupe</td> 
   <td>Rapport Projet qui affiche l’état d’avancement et le groupe des projets. Le rapport est regroupé par nom de groupe et état d’avancement, et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets par priorité</td> 
   <td>Rapport Projet qui affiche la priorité des projets. Le rapport est regroupé par priorité et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Projets par statut de progression</td> 
   <td>Rapport Projet qui affiche l’état d’avancement des projets. Le rapport est regroupé par Etat d'avancement et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Tâches par statut de progression</td> 
   <td>Rapport Tâche qui affiche l’état d’avancement de toutes les tâches dans les projets en cours. Le rapport est regroupé par Etat d'avancement et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Tâches par statut</td> 
   <td>Un rapport Tâche qui affiche le Statut de toutes les tâches. Le rapport est regroupé par statut et comprend un graphique.</td> 
  </tr> 
  <tr> 
   <td>Feuilles de temps à vérifier</td> 
   <td>Rapport de feuille de temps qui affiche les feuilles de temps Envoyé et Refusé dont l’approbateur est l’utilisateur connecté. Le rapport affiche les champs suivants : plage de dates, propriétaire, heures totales, heures supplémentaires, nom de l’approbateur et état des feuilles de temps.</td> 
  </tr> 
  <tr> 
   <td>Tâches problématiques</td> 
   <td>Rapport Tâche qui affiche des tâches incomplètes avec un état de progression en retard ou en arrière, une date de remise antérieure à demain et où l’utilisateur connecté fait partie de l’équipe de projet du projet sur laquelle se trouvent les tâches. Le rapport affiche les champs suivants : Durée planifiée, Nom du projet, personne désignée principale, Début planifié, Fin planifiée, Pourcentage terminé et Priorité des tâches.</td> 
  </tr> 
  <tr> 
   <td>Connexions utilisateur</td> 
   <td>Rapport Utilisateur qui affiche les champs suivants : identifiant unique, nombre de connexions (nombre de fois où l’utilisateur s’est connecté depuis qu’il a commencé avec Workfront), date de dernière connexion des utilisateurs. Le rapport est regroupé par niveau d'accès des utilisateurs.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Accès aux rapports natifs

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

{{step1-click-main-menu}}

1. Cliquez sur **Rapports**.
1. Cliquez sur **Tous les rapports**.
1. Développez le menu déroulant **Filtre**, puis sélectionnez **Nouveau filtre**.

1. Cliquez sur **Ajouter une règle de filtre**.
1. Dans le champ **Commencer à saisir le nom du champ**, commencez à saisir **ID global**.

1. Sous l’objet **Report** , sélectionnez **Global ID**.

1. Dans le menu déroulant du modificateur de filtre, sélectionnez **N’est pas vierge**.\
   ![](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Cliquez sur **Enregistrer le filtre**.\
   La liste des rapports affiche uniquement les rapports intégrés.\
   Pour plus d’informations sur les rapports natifs disponibles, reportez-vous à la section [Présentation des rapports natifs](#overview-of-built-in-reports) de cet article.
