---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Exécuter un rapport
description: Vous pouvez exécuter tous les rapports que vous pouvez afficher.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 83%

---


# Exécuter un rapport

Vous pouvez exécuter tous les rapports que vous pouvez afficher.

<!-- Audited: 11/2024 -->

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
      <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès à l’affichage de rapports, tableaux de bord, calendriers</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage pour un rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exécuter un rapport

1. Cliquez sur l’icône de **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône de **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Rapports]**.

1. Sélectionnez l’une des options suivantes :

   * **Mes rapports :** rapports que vous avez créés.
   * **Partagé(s) avec moi :** rapports que d’autres utilisateurs et utilisatrices ont partagés avec vous.
   * **Tous les rapports :** tous les rapports du système auxquels vous avez accès.

1. Cliquez sur le nom du rapport à exécuter.\
   Ou\
   Si le rapport a été créé à l’aide d’invites, sélectionnez les informations appropriées dans les menus déroulants, puis cliquez sur **Exécuter le rapport**.\
   Pour plus d’informations sur les invites, consultez la section [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   L’horodatage du rapport s’affiche dans le coin supérieur droit, comprenant la date, l’heure et le fuseau horaire de l’exécution du rapport à partir du contexte de l’utilisateur ou de l’utilisatrice à l’origine de l’exécution du rapport.

1. (Facultatif) Cliquez sur l’icône **** ![Icône Recharger](assets/unshimmed-report-refresh-icon.png) pour actualiser les résultats dans un rapport si le rapport s’affiche dans votre navigateur depuis un certain temps.

1. (Le cas échéant) Si le rapport utilise des filtres ou des invites, cliquez sur **Afficher les filtres et les invites** pour afficher la liste des filtres et des invites utilisés sur le rapport que vous consultez. Si le rapport ne comporte que des filtres ou des invites, le choix **Afficher les filtres** ou **Afficher les invites** apparaît à la place.

   ![Affichage des filtres et des invites](assets/unshimmed-show-filters-and-prompts.png)

   Les informations s’affichent sous le nom du rapport sur le côté gauche de la page. Pour les invites, il s’agit d’informations sur les sélections d’invites effectuées au moment de l’exécution du rapport, comme décrit à l’étape 3.

1. Si vous utilisez des invites personnalisées, elles ne s’affichent pas. Seules les invites du système s’affichent. Les filtres personnalisés s’affichent toujours.

## Afficher un rapport mis en cache

Votre rapport peut être mis en cache s’il est resté affiché dans votre navigateur pendant un certain temps. Vous pouvez forcer un rapport mis en cache à charger de nouveau en effectuant l’une des actions suivantes :

* Modifiez les paramètres du rapport et enregistrez-le.
* Modifiez l’affichage, le groupe ou le filtre.
* Cliquez sur l&#39;**icône de rechargement** ![icône de rechargement](assets/unshimmed-report-refresh-icon.png)
Cette option est disponible dans le coin supérieur droit de la page, dans la zone de message, pour indiquer l’heure d’enregistrement du rapport ou dans le coin supérieur droit du tableau de bord sur lequel le rapport est placé. Pour plus d’informations sur la façon de charger à nouveau des tableaux de bord, consultez la section « Afficher les tableaux de bord » de l’article [Commencer avec les tableaux de bord](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* Naviguez vers les onglets Résumé, Matrice ou Graphique pour accéder à n’importe quelle page du rapport au-delà de la première.
