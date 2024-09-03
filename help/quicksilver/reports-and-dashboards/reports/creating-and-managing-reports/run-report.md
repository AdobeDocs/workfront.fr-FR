---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Exécuter un rapport
description: Vous pouvez exécuter tous les rapports que vous pouvez afficher.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 100%

---


# Exécuter un rapport

Vous pouvez exécuter tous les rapports que vous pouvez afficher.

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès à l’affichage de rapports, tableaux de bord, calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage pour un rapport</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Exécuter un rapport

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Rapports**.

1. Sélectionnez l’une des options suivantes :

   * **Mes rapports :** rapports que vous avez créés.
   * **Partagé(s) avec moi :** rapports que d’autres utilisateurs et utilisatrices ont partagés avec vous.
   * **Tous les rapports :** tous les rapports du système auxquels vous avez accès.

1. Cliquez sur le nom du rapport à exécuter.\
   Ou\
   Si le rapport a été créé à l’aide d’invites, sélectionnez les informations appropriées dans les menus déroulants, puis cliquez sur **Exécuter le rapport**.\
   Pour plus d’informations sur les invites, consultez la section [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   L’horodatage du rapport s’affiche dans le coin supérieur droit, comprenant la date, l’heure et le fuseau horaire de l’exécution du rapport à partir du contexte de l’utilisateur ou de l’utilisatrice à l’origine de l’exécution du rapport.

1. (Facultatif) Cliquez sur l’**icône Charger à nouveau** ![](assets/qs-report-refresh-icon.png) pour actualiser les résultats d’un rapport si le rapport est resté affiché dans votre navigateur pendant un certain temps.

1. (Le cas échéant) Si le rapport utilise des filtres ou des invites, cliquez sur **Afficher les filtres et les invites** pour afficher la liste des filtres et des invites utilisés sur le rapport que vous consultez. Si le rapport ne comporte que des filtres ou des invites, le choix **Afficher les filtres** ou **Afficher les invites** apparaît à la place.

   ![Affichage des filtres et des invites](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   Les informations s’affichent sous le nom du rapport sur le côté gauche de la page. Pour les invites, il s’agit d’informations sur les sélections d’invites effectuées au moment de l’exécution du rapport, comme décrit à l’étape 4.

1. Si vous utilisez des invites personnalisées, elles ne s’affichent pas. Seules les invites du système s’affichent. Les filtres personnalisés s’affichent toujours.

## Afficher un rapport mis en cache

Votre rapport peut être mis en cache s’il est resté affiché dans votre navigateur pendant un certain temps. Vous pouvez forcer un rapport mis en cache à charger de nouveau en effectuant l’une des actions suivantes :

* Modifiez les paramètres du rapport et enregistrez-le.
* Modifiez l’affichage, le groupe ou le filtre.
* Cliquer sur l’**icône Charger à nouveau**
Pour indiquer l’heure d’enregistrement du rapport, cette option est disponible soit dans le coin supérieur droit de la page, dans la zone de message, soit dans le coin supérieur droit du tableau de bord où le rapport est affiché. Pour plus d’informations sur la façon de charger à nouveau des tableaux de bord, consultez la section « Afficher les tableaux de bord » de l’article [Commencer avec les tableaux de bord](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Naviguez vers les onglets Résumé, Matrice ou Graphique pour accéder à n’importe quelle page du rapport au-delà de la première.
