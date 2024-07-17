---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Créer un rapport personnalisé
description: Vous pouvez donner accès aux informations dont votre organisation a besoin dans Adobe Workfront en créant des rapports. Vous pouvez utiliser n’importe quel rapport intégré disponible dans Workfront ou créer entièrement vos rapports personnalisés.
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '1828'
ht-degree: 7%

---


# Créer un rapport personnalisé

<!--Audited: 12/2023-->

Vous pouvez donner accès aux informations dont votre organisation a besoin dans Adobe Workfront en créant des rapports. Vous pouvez utiliser n’importe quel rapport intégré disponible dans Workfront ou créer entièrement vos rapports personnalisés.

Pour plus d’informations sur les rapports natifs, voir [Utilisation des rapports natifs Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

Pour plus d’informations sur la création d’un rapport en le copiant, voir [Création d’une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Pour plus d’informations sur la création et la gestion des rapports, y compris les classes, les vidéos et les tutoriels, consultez la section En savoir plus sur le site Adobe Experience League.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td> <p>Nouvelle : standard </p>
   ou
   <p>Actuelle : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p><b>NOTE</b></p>
   <p> Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Vous obtenez les autorisations Gérer pour les rapports que vous créez.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Créer un rapport {#create-a-report}

{{step1-to-reports}}

1. Cliquez sur **Nouveau rapport**, puis sélectionnez le type d’objet souhaité pour le rapport.

   Le créateur de rapports se charge.

   Pour plus d’informations sur les rapports d’objets disponibles, reportez-vous à la section [Rapport sur les objets](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) de l’article [Comprendre les objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >Vous pouvez également créer un rapport en faisant une copie d’un rapport existant. Pour plus d’informations, voir [Création d’une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Dans le créateur de rapports, ajoutez les éléments suivants à votre rapport :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Fonctionnalité</th> 
      <th>Description</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Colonnes (Affichage)</td> 
      <td> <p>L’ajout de colonnes à votre rapport détermine les informations que contient votre rapport.</p> <p>Pour savoir comment ajouter une colonne, voir <a href="#add-columns-view-to-a-report" class="MCXref xref">Ajout de colonnes (vue) à un rapport</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>Regroupements</td> 
      <td> <p>L’ajout de regroupements à votre rapport détermine l’organisation de votre rapport.</p> <p>Pour savoir comment ajouter un groupement, voir <a href="#add-groupings-to-a-report" class="MCXref xref">Ajout de groupements à un rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Filtres</td> 
      <td> <p>L’ajout de règles de filtrage à votre rapport détermine les informations que vous voyez dans votre rapport.</p> <p>Pour savoir comment ajouter un filtre, voir <a href="#add-filters-to-a-report" class="MCXref xref">Ajout de filtres à un rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Graphique</td> 
      <td> <p>L’ajout d’un graphique à votre rapport détermine la manière dont les informations de votre rapport sont présentées visuellement.</p> <p>Pour savoir comment ajouter un graphique, reportez-vous à la section <a href="#add-a-chart-to-a-report" class="MCXref xref">Ajout d’un graphique à un rapport</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. À tout moment pendant le processus de création du rapport, cliquez sur **Appliquer** pour enregistrer vos modifications.
1. Une fois que vous avez terminé, cliquez sur **Enregistrer + Fermer**.

### Ajout de colonnes (vue) à un rapport {#add-columns-view-to-a-report}

1. Commencez à créer un rapport comme décrit dans la section [Créer un rapport](#create-a-report) de cet article.
1. Dans le créateur de rapports, sélectionnez l’onglet **Colonnes (vues)** pour identifier les colonnes à afficher dans le rapport.
1. (Facultatif) Cliquez sur **Appliquer une vue existante** et cliquez sur le nom d’une vue dans le menu déroulant pour utiliser une vue existante.

   Pour plus d’informations sur la création d’une vue, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (Facultatif) Pour supprimer une colonne existante, cliquez sur la colonne à supprimer, puis cliquez sur le **x** en regard du nom actuel dans l’en-tête de la colonne.

1. Pour ajouter une nouvelle colonne, cliquez sur **Ajouter une colonne**.

   Ou

   Pour modifier une colonne existante, cliquez sur la colonne, cliquez sur l’icône **Supprimer** ![](assets/x-icon-circled.png) située à gauche du champ actif dans la zone **Afficher dans ce champ de colonne** située dans le coin supérieur gauche du créateur de rapports, puis commencez à saisir un nouveau champ, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   Pour plus d’informations sur les champs affichés dans les colonnes, voir [Glossaire de la terminologie Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![](assets/nwe-add-column-typeahead-350x459.png)

1. (Facultatif) Dans la zone **Paramètres de colonne**, sélectionnez **Trier par cette colonne** pour trier les valeurs de la colonne par ordre alphabétique croissant, puis indiquez si la liste doit utiliser cette colonne comme premier tri.

   Vous pouvez avoir plusieurs niveaux de tri dans une vue de rapport si vous souhaitez trier par valeur dans une colonne en premier, par valeur dans une seconde colonne, par seconde, etc.

   Si plusieurs résultats sont identiques selon les premiers critères de tri, ils les trient dans l’ordre du second critère de tri. Si plusieurs résultats sont identiques selon le premier et le deuxième critère de tri, ils sont triés selon le troisième critère de tri, etc.

   >[!NOTE]
   >
   >Si vous ajoutez un champ qui référence un objet trop éloigné de l’objet sur lequel vous créez un rapport, il se peut que vous ne puissiez pas le trier selon ce champ.\
   >Par exemple, un rapport de problème ne peut pas être trié par champ Propriétaire du projet, car il fait référence à 3 objets supplémentaires : Projet, Propriétaire et Nom. Cependant, vous pouvez toujours ajouter ce champ à un rapport de problème et afficher les informations le concernant.

   <!--outdated: To learn more about cross-object references in reports, see the section "Advanced Reporting Part 1 of 3" in the [Reports and Dashboards Learning Path](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).-->

1. (Facultatif) Si vous utilisez des groupements et souhaitez résumer (agréger) les informations d&#39;une colonne, cliquez sur la liste déroulante **Résumer cette colonne par** de la zone **Paramètres de colonne**, puis sélectionnez l&#39;option à utiliser pour agréger les informations de la colonne.

   Les informations agrégées s’affichent dans la colonne des lignes de groupement.

   ![Résumé agrégé sur les regroupements](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   Pour plus d’informations sur le résumé des données dans une colonne, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >Les exceptions suivantes s’appliquent aux objets parents (par exemple, les tâches parents) lorsque vous agrègez des valeurs pour les champs suivants en regroupements :
   >
   >* Tous les champs Nombre et Devise, à l’exception des Heures réelles (par exemple, Coût du travail planifié ou réel, Coût des dépenses planifié ou réel, Coût planifié ou réel, Heures planifiées), ne regroupent que les valeurs des tâches enfants et des tâches autonomes. Ils n’agrégent pas les valeurs des tâches parents ou des parents des parents.
   >* Les heures réelles combinent les valeurs des tâches principales du parent et des tâches autonomes ; elles n’agrégent pas les nombres des parents des tâches parents ou des tâches enfants.
   >* Les champs de données personnalisés pour les valeurs numériques et monétaires regroupent toutes les tâches : parents, enfants, parents de parents et tâches autonomes.

   Pour plus d’informations sur l’utilisation des groupements dans un rapport, consultez la [présentation des groupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Facultatif) Cliquez sur **Options avancées** pour spécifier les informations suivantes pour la colonne :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Personnaliser le libellé de colonne</td> 
      <td> <p>Spécifiez un libellé personnalisé pour la colonne. Ce libellé remplace le libellé par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format du champ</td> 
      <td> <p>Sélectionnez le format d'affichage des valeurs des champs de la colonne.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher cette colonne lorsque le graphique est visible sur un tableau de bord.</td> 
      <td> <p>Sélectionnez cette option pour afficher cette colonne sur un tableau de bord, lorsque le rapport est affiché côte à côte avec un autre rapport. Lorsque cette option n'est pas sélectionnée, cette colonne ne s'affiche pas lors de l'affichage du rapport dans un tableau de bord où les rapports sont affichés côte à côte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Règles de la colonne</td> 
      <td> <p>Cliquez sur <strong>Ajouter une règle pour cette colonne</strong> pour ajouter une mise en forme conditionnelle à la colonne. Après avoir ajouté une règle, vous pouvez définir des styles de champ et de texte pour l’affichage des champs correspondant à cette règle. Cliquez sur <strong>Ajouter une règle</strong> une fois la définition de la règle terminée. Pour plus d’informations sur la mise en forme conditionnelle dans une vue, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">Utilisation de la mise en forme conditionnelle dans les vues</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Appliquer** pour appliquer vos modifications jusqu’à présent et continuez à modifier le rapport avec les options suivantes.

   Cliquez sur **Enregistrer + Fermer** si vous avez terminé de modifier les colonnes du rapport et souhaitez enregistrer le rapport.

### Ajouter des groupements à un rapport {#add-groupings-to-a-report}

1. Commencez à créer un rapport comme décrit dans la section [Créer un rapport](#create-a-report) de cet article.
1. Dans le créateur de rapports, sélectionnez l’onglet **Groupements** pour identifier la manière dont vous souhaitez regrouper des éléments dans le rapport.
1. Cliquez sur **Ajouter un groupement** pour ajouter un nouveau groupement.

   Ou

   Sélectionnez **Appliquer un groupement existant** pour sélectionner un groupement existant lorsqu&#39;il s&#39;affiche dans la liste.

   ![](assets/nwe-add-grouping-350x230.png)

1. Commencez à saisir le champ à ajouter en tant que groupe. Si le champ est disponible, il est renseigné pour chaque objet auquel il peut être associé. Cliquez sur le nom du champ à ajouter à ce groupement.
1. (Facultatif) Vous pouvez choisir de créer un regroupement en mode texte en cliquant sur **Passer en mode texte**. Pour plus d’informations sur l’utilisation du mode texte, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   Pour plus d’informations sur la création de nouveaux regroupements, voir [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Facultatif) Sélectionnez **Réduire ce regroupement par défaut** si vous souhaitez que les résultats de ce regroupement s’affichent réduits plutôt que développés.

   Ce paramètre est désactivé par défaut et les résultats du groupement s’affichent toujours dans une liste étendue.

   >[!TIP]
   >
   >* Lorsque vous ajustez manuellement les groupements lors de l&#39;affichage d&#39;une liste, Workfront mémorise vos préférences manuelles jusqu&#39;à ce que vous vous déconnectiez. Lorsque vous vous reconnectez, la liste s’affiche en fonction de ce paramètre.
   >* Les résultats d’un groupement s’affichent toujours agrandi après leur accès à partir d’un élément de graphique.

1. (Facultatif) Cliquez sur **Basculer vers le groupement matriciel** pour créer un groupement de matrice et afficher vos résultats dans un format de grille.

   Pour plus d’informations sur la création d’un rapport de matrice, voir [Création d’un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Cliquez sur **Appliquer** pour appliquer vos modifications jusqu’à présent et continuez à modifier le rapport avec les options suivantes.

   Cliquez sur **Enregistrer + Fermer** si vous avez terminé de modifier les regroupements dans le rapport et souhaitez enregistrer le rapport.

### Ajout de filtres à un rapport {#add-filters-to-a-report}

1. Commencez à créer un rapport comme décrit dans la section [Créer un rapport](#create-a-report) de cet article.
1. Dans le créateur de rapports, sélectionnez l’onglet **Filtres** pour identifier la quantité d’informations que le rapport doit inclure.
1. Cliquez sur **Ajouter une règle de filtre** pour ajouter un filtre personnalisé.\
   Ou\
   Sélectionnez **Appliquer un filtre existant** pour utiliser un filtre existant.

   ![](assets/nwe-add-a-filter-350x93.png)

1. Si vous avez cliqué sur **Ajouter une règle de filtre**, commencez à saisir le champ à ajouter en tant que filtre. Si le champ est disponible, il est renseigné pour chaque objet auquel il peut être associé. Cliquez sur le nom du champ pour l’ajouter à ce filtre.\
   Utilisez des modificateurs de filtre pour créer votre filtre. Pour plus d’informations sur les modificateurs de filtre, voir [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Pour plus d’informations sur la création de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facultatif) Vous pouvez choisir de créer un filtre en mode texte en cliquant sur **Passer en mode texte**.

   Pour plus d’informations sur l’utilisation du mode texte, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. Cliquez sur **Appliquer** lorsque vous avez terminé de modifier les filtres du rapport pour appliquer vos modifications jusqu’à présent et continuez à modifier le rapport avec les options suivantes.

   Cliquez sur **Enregistrer + Fermer** si le rapport et vous souhaitez l’enregistrer.

### Ajouter un graphique à un rapport {#add-a-chart-to-a-report}

1. Commencez à créer un rapport comme décrit dans la section [Créer un rapport](#create-a-report) de cet article.
1. Dans le créateur de rapports, sélectionnez l’onglet **Graphique**, puis sélectionnez le type de graphique à ajouter.

   ![](assets/nwe-add-a-chart-350x247.png)

   Pour plus d’informations sur la création d’un graphique dans un rapport, voir [Ajout d’un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Cliquez sur **Appliquer** pour appliquer vos modifications jusqu’à présent et continuez à modifier le rapport avec les options suivantes.

   Cliquez sur **Enregistrer + Fermer** si vous avez terminé de modifier le rapport et souhaitez l’enregistrer.
