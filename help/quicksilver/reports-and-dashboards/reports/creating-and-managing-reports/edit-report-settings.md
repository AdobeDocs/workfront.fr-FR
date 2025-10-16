---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Modifier les paramètres des rapports
description: Vous pouvez modifier les paramètres d’un rapport afin de définir comment il s’affiche pour d’autres personnes ou le type d’informations que les personnes peuvent demander avant d’exécuter le rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 98%

---

# Modifier les paramètres des rapports

<!-- Audited: 11/2024 -->

Vous pouvez modifier les paramètres d’un rapport afin de définir comment il s’affiche pour d’autres personnes ou le type d’informations que les personnes peuvent demander avant d’exécuter le rapport.

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
      <p>Standard</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Accès en modification aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
 <td> <p>Gérer les autorisations d’un rapport</p></td>  
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Étapes pratiques

1. Commencez à créer un rapport en accédant à **Menu principal** > **Rapports**, puis en sélectionnant l’objet de votre rapport.

   Ou

   Ouvrez un rapport existant, puis cliquez sur **Actions de rapport** > **Modifier**.

1. Cliquez sur **Paramètres des rapports** dans le coin supérieur droit du créateur de rapport.
1. Configurez les paramètres de rapport suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Titre du rapport</td> 
      <td>Indiquez un titre pour le rapport.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Spécifiez une instruction décrivant l’objectif et l’utilisation du rapport.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exécuter ce rapport avec les droits d’accès suivants :</td> 
      <td>Sélectionnez la personne dont vous souhaitez que ce rapport utilise les droits d’accès lors de l’affichage pour d’autres personnes. Pour plus d’informations sur l’exécution d’un rapport avec les droits d’accès d’une autre personne, consultez l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Exécuter et diffuser un rapport avec les droits d’accès d’une autre personne</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lors du chargement du rapport, afficher le :</td> 
      <td>Sélectionnez l’onglet par défaut qui s’affiche pour toutes les personnes lors du chargement du rapport.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lorsque ce rapport se charge sur un tableau de bord, afficher ... éléments.</td> 
      <td>Spécifiez le nombre d’éléments qui s’affichent pour toutes les personnes lorsque le rapport charge sur un tableau de bord. La valeur par défaut est de 15 éléments et le nombre maximal d’éléments est de 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher la vue Grille des ressources dans l’onglet Détails</td> 
      <td> <p>(Rapport d’utilisateur ou d’utilisatrice uniquement) Sélectionnez cette option pour afficher la grille de ressources dans l’onglet Détails du rapport.</p> <p>Note : lorsque vous appliquez la vue Grille de ressources à un rapport d’utilisateur ou d’utilisatrice, le rapport affiche uniquement les projets qui ont le statut Actuel. Si vous souhaitez afficher les projets ayant un autre statut, vous pouvez utiliser l’onglet Allocation des utilisateurs et utilisatrices dans la zone Personnes de la barre de navigation globale, puis appliquer la vue Grille de ressources à cet endroit. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher une vue spéciale dans l’onglet Détails</td> 
      <td>(Rapport de projet uniquement) Spécifiez le type de vue que verront les personnes lorsqu’elles accéderont à ces informations dans l’onglet Détails. Par exemple, vous pouvez sélectionner une vue Jalon ou Gantt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher ce rapport dans une vue Gantt par défaut</td> 
      <td>(Rapport de projet et rapport de tâches uniquement) Sélectionnez cette option pour que la vue Gantt soit activée automatiquement lorsque les personnes consultent l’onglet Détails de ce rapport.<br>Pour plus d’informations sur l’affichage du graphique de Gantt dans les rapports de projet et de tâche, consultez la section « Afficher des informations sur les tâches dans le graphique de Gantt de la liste de projets » dans l’article <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Afficher des informations dans le graphique de Gantt </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser le changement de vue dans ce rapport</td> 
      <td>Sélectionnez cette option pour permettre aux personnes de modifier la vue lors de l’exécution du rapport.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser le changement de groupe dans ce rapport</td> 
      <td>Sélectionnez cette option pour permettre aux personnes de modifier le groupe lors de l’exécution du rapport.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser le changement de filtre dans ce rapport</td> 
      <td>Sélectionnez cette option pour permettre aux personnes de modifier le filtre lors de l’exécution du rapport.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Invite de rapports** pour configurer les invites du rapport.\
   Pour plus d’informations sur l’ajout d’invites à un rapport, consultez l’article [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Cliquez sur **Terminé** puis sur **Enregistrer + Fermer**.

## Informations supplémentaires

Voir aussi :

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [Commencer avec les rapports](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Utiliser les rapports intégrés d’Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
