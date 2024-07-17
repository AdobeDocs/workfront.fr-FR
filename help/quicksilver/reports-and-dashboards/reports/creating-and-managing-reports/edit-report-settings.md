---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Modifier les paramètres des rapports
description: Vous pouvez modifier les paramètres d’un rapport afin de définir comment il s’affiche pour d’autres utilisateurs ou le type d’informations que les utilisateurs peuvent leur demander avant d’exécuter le rapport.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 22%

---

# Modifier les paramètres des rapports

Vous pouvez modifier les paramètres d’un rapport afin de définir comment il s’affiche pour d’autres utilisateurs ou le type d’informations que les utilisateurs peuvent leur demander avant d’exécuter le rapport.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Étapes pratiques

1. Commencez à créer un rapport en accédant au **menu principal** > **Rapports**, puis sélectionnez l’objet de votre rapport.

   Ou

   Ouvrez un rapport existant, puis cliquez sur **Actions de rapport** > **Modifier**.

1. Cliquez sur **Paramètres de rapport** dans le coin supérieur droit du créateur de rapports.
1. Configurez les paramètres de rapport suivants :

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
      <td role="rowheader">Exécutez ce rapport avec les droits d’accès de</td> 
      <td>Sélectionnez l’utilisateur dont vous souhaitez que ce rapport utilise les droits d’accès lors de l’affichage pour d’autres utilisateurs. Pour plus d’informations sur l’exécution d’un rapport avec les droits d’accès d’un autre utilisateur, reportez-vous à l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Exécution et diffusion d’un rapport avec les droits d’accès d’un autre utilisateur</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Au chargement du rapport, affichez la variable</td> 
      <td>Sélectionnez l'onglet par défaut qui s'affiche pour tous les utilisateurs au chargement du rapport.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lorsque le rapport se charge sur un tableau de bord, affichez ... éléments</td> 
      <td>Spécifiez le nombre d’éléments qui s’affichent pour tous les utilisateurs lorsque le rapport est chargé sur un tableau de bord. La valeur par défaut est de 15 éléments et le nombre maximal d’éléments est de 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Affichage de la grille de ressources dans l’onglet Détails</td> 
      <td> <p>(Rapport utilisateur uniquement) Sélectionnez cette option pour afficher la grille de ressources dans l’onglet Détails du rapport.</p> <p>Remarque : lorsque vous appliquez le mode Grille de ressources à un rapport d’utilisateur, le rapport affiche uniquement les projets qui sont à l’état actuel. Si vous souhaitez afficher les projets dans un autre état, vous pouvez utiliser l’onglet Utilisation de l’utilisateur dans la zone Personnes de la barre de navigation globale, puis appliquer le mode Grille de ressources à cet endroit. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher une vue spéciale sur l’onglet Détails</td> 
      <td>(Rapport de projet uniquement) Spécifiez le type d’affichage que verront les utilisateurs lorsqu’ils accéderont à ces informations dans l’onglet Détails. Par exemple, vous pouvez sélectionner une vue Milestone ou Gantt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher ce rapport dans une vue Gantt par défaut</td> 
      <td>(Rapport de projet et Rapport de tâches uniquement) Sélectionnez cette option pour que la vue Gantt soit activée automatiquement lorsque les utilisateurs consultent l’onglet Détails de ce rapport.<br>Pour plus d’informations sur l’affichage du diagramme de Gantt dans les rapports de projet et de tâche, consultez la section "Affichage des informations sur les tâches dans le diagramme de Gantt de la liste de projets" dans l’article <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Affichage des informations dans le diagramme de Gantt </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser le changement de vue dans ce rapport</td> 
      <td>Sélectionnez cette option pour permettre aux utilisateurs de modifier l’affichage lors de l’exécution du rapport.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser le changement de groupe dans ce rapport</td> 
      <td>Sélectionnez cette option pour permettre aux utilisateurs de modifier le Groupe lors de l’exécution du rapport.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser le changement de filtre dans ce rapport</td> 
      <td>Sélectionnez cette option pour permettre aux utilisateurs de modifier le filtre lors de l’exécution du rapport.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Report Prompts** pour configurer toutes les invites du rapport.\
   Pour plus d’informations sur l’ajout d’invites à un rapport, reportez-vous à l’article [Ajout d’une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Cliquez sur **Terminé,** puis sur **Enregistrer + Fermer**.

## Informations supplémentaires

Voir aussi :

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [Prise en main des rapports](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Utiliser des rapports intégrés Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
