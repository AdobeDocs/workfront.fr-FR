---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Création d’un rapport personnalisé
description: Comprendre comment créer des rapports vous permet d’accéder aux informations dont votre organisation a besoin dans Adobe Workfront. Vous pouvez utiliser n’importe quel rapport intégré disponible dans Workfront ou créer vos propres rapports à partir de zéro.
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '1807'
ht-degree: 1%

---


# Création d’un rapport personnalisé

Vous pouvez donner accès aux informations dont votre organisation a besoin dans Adobe Workfront en créant des rapports. Vous pouvez utiliser n’importe quel rapport intégré disponible dans Workfront ou créer entièrement vos rapports personnalisés.

Pour plus d’informations sur les rapports natifs, voir [Utilisation des rapports intégrés d’Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

Pour plus d’informations sur la création d’un rapport en le copiant, voir [Créer une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Pour plus d’informations sur la création et la gestion des rapports, y compris les classes, les vidéos et les tutoriels, consultez la section En savoir plus sur le site Adobe Experience League.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p><b>NOTE</b></p>
   <p> Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Vous obtiendrez les autorisations de gestion du rapport que vous créez.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Créer un rapport {#create-a-report}

Pour regarder une vidéo de la création d’un rapport, reportez-vous à cette section [Création d’un rapport personnalisé](#Walk-thr) ci-dessous

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **Rapports**.
1. Cliquez sur **Nouveau rapport**, puis sélectionnez le type d’objet que vous souhaitez pour le rapport.

   Le créateur de rapports se charge.

   Pour plus d’informations sur les rapports d’objets disponibles, voir la section [Rapport sur les objets](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) dans l’article [Présentation des objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >Vous pouvez également créer un rapport en faisant une copie d’un rapport existant. Pour plus d’informations, voir [Créer une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

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
      <td> <p>L’ajout de regroupements à votre rapport détermine l’organisation de votre rapport.</p> <p>Pour savoir comment ajouter un groupement, voir <a href="#add-groupings-to-a-report" class="MCXref xref">Ajouter des groupements à un rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Filtres</td> 
      <td> <p>L’ajout de règles de filtrage à votre rapport détermine les informations que vous voyez dans votre rapport.</p> <p>Pour savoir comment ajouter un filtre, voir <a href="#add-filters-to-a-report" class="MCXref xref">Ajout de filtres à un rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Graphique</td> 
      <td> <p>L’ajout d’un graphique à votre rapport détermine la manière dont les informations de votre rapport sont présentées visuellement.</p> <p>Pour savoir comment ajouter un graphique, voir <a href="#add-a-chart-to-a-report" class="MCXref xref">Ajouter un graphique à un rapport</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. À tout moment pendant le processus de création du rapport, cliquez sur **Appliquer** pour enregistrer vos modifications.
1. Lorsque vous avez terminé, cliquez sur **Enregistrer + Fermer**.

### Ajout de colonnes (vue) à un rapport {#add-columns-view-to-a-report}

1. Commencez à créer un rapport comme décrit dans la section [Créer un rapport](#create-a-report) dans cet article.
1. Dans le créateur de rapports, sélectionnez la variable **Colonnes (affichage)** pour identifier les colonnes à afficher dans le rapport.
1. (Facultatif) Cliquez sur **Appliquer une vue existante** pour utiliser une vue existante.

   Pour plus d’informations sur la création d’une vue, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Pour ajouter une nouvelle colonne, cliquez sur **Ajouter une colonne**.

   Ou

   Pour modifier une colonne existante, sélectionnez la colonne à modifier, puis cliquez sur le (x) en regard du nom actuel.

1. Commencez à saisir le champ à ajouter. Si le champ est disponible, il est renseigné pour chaque objet auquel il peut être associé. Cliquez sur le nom du champ à ajouter à la colonne.

   Pour plus d’informations sur les champs que vous voyez dans les colonnes, voir [Glossaire de la terminologie Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![](assets/nwe-add-column-typeahead-350x459.png)

1. (Facultatif) Dans la variable **Paramètres des colonnes** zone, sélectionnez **Trier par colonne** pour trier les valeurs de la colonne, soit par ordre alphabétique croissant, soit par ordre alphabétique décroissant, indiquez si la liste doit utiliser cette colonne comme premier tri.

   Vous pouvez avoir plusieurs niveaux de tri dans une vue de rapport si vous souhaitez trier par valeur dans une colonne en premier, par valeur dans une seconde colonne, par seconde, etc.

   Si plusieurs résultats sont identiques selon les premiers critères de tri, ils les trient dans l’ordre du second critère de tri. Si plusieurs résultats sont identiques selon le premier et le deuxième critère de tri, ils sont triés selon le troisième critère de tri, etc.

   >[!NOTE]
   >
   >Si vous ajoutez un champ qui référence un objet trop éloigné de l’objet sur lequel vous créez un rapport, il se peut que vous ne puissiez pas le trier selon ce champ.\
   >Par exemple, un rapport de problème ne peut pas être trié par champ Propriétaire du projet, car il fait référence à 3 objets supplémentaires : Projet, Propriétaire et Nom. Cependant, vous pouvez toujours ajouter ce champ à un rapport de problème et afficher les informations le concernant.

   <!--outdated: To learn more about cross-object references in reports, see the section "Advanced Reporting Part 1 of 3" in the [Reports and Dashboards Learning Path](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).-->

1. (Facultatif) Si vous utilisez des regroupements et souhaitez résumer (agréger) les informations d’une colonne, cliquez sur le bouton **Résumer cette colonne par** Liste déroulante dans la **Paramètres des colonnes** , puis sélectionnez l’option à utiliser pour agréger les informations dans la colonne.

   Les informations agrégées s’affichent dans la colonne des lignes de groupement.

   ![Résumé agrégé des regroupements](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   Pour plus d’informations sur le résumé des données dans une colonne, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >Les exceptions suivantes s’appliquent aux objets parents (par exemple, les tâches parents) lorsque vous agrègez des valeurs pour les champs suivants en regroupements :
   >
   >* Tous les champs de nombre et de devise, à l’exception des heures réelles (par exemple, le coût du travail planifié/réel, le coût des dépenses planifiées/réelles, le coût planifié/réel, les heures planifiées), ne regroupent que les valeurs des tâches enfants et des tâches autonomes. Ils n’agrégent pas les valeurs des tâches parents ou des parents des parents.
   >* Les heures réelles combinent les valeurs des tâches principales du parent et des tâches autonomes ; elles n’agrégent pas les nombres des parents des tâches parents ou des tâches enfants.
   >* Les champs de données personnalisés pour les valeurs numériques et monétaires regroupent toutes les tâches : parents, enfants, parents de parents et tâches autonomes.

   Pour plus d’informations sur l’utilisation de regroupements dans un rapport, voir [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

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
      <td> <p>Cliquez sur <strong>Ajouter une règle pour cette colonne</strong> pour ajouter une mise en forme conditionnelle à la colonne. Après avoir ajouté une règle, vous pouvez définir des styles de champ et de texte pour l’affichage des champs correspondant à cette règle. Cliquez sur <strong>Ajouter une règle</strong> après avoir défini la règle. Pour plus d’informations sur la mise en forme conditionnelle dans un affichage, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">Utilisation d’une mise en forme conditionnelle dans les vues</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Appliquer** pour appliquer vos modifications jusqu’à présent et poursuivre la modification du rapport avec les options suivantes.

   Cliquez sur **Enregistrer + Fermer** si vous avez terminé de modifier les colonnes du rapport et que vous souhaitez enregistrer le rapport.

### Ajouter des groupements à un rapport {#add-groupings-to-a-report}

1. Commencez à créer un rapport comme décrit dans la section [Créer un rapport](#create-a-report) dans cet article.
1. Dans le créateur de rapports, sélectionnez la variable **Groupements** pour identifier la manière dont vous souhaitez regrouper des éléments dans le rapport.
1. Cliquez sur **Ajouter un groupement** pour ajouter un nouveau groupement.

   Ou

   Choisir **Appliquer un groupement existant** pour sélectionner un groupement existant
   ![](assets/nwe-add-grouping-350x230.png)

1. Commencez à saisir le champ à ajouter en tant que groupe. Si le champ est disponible, il est renseigné pour chaque objet auquel il peut être associé. Cliquez sur le nom du champ à ajouter à ce groupement.
1. (Facultatif) Pour créer un groupement, cliquez sur **Passer en mode Texte**. Pour plus d’informations sur l’utilisation du mode texte, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   Pour plus d’informations sur la création de nouveaux regroupements, voir [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Facultatif) Sélectionnez **Réduire ce groupement par défaut** si vous souhaitez que les résultats de ce regroupement s’affichent réduits plutôt que développés.

   Ce paramètre est désactivé par défaut et les résultats du groupement s’affichent toujours dans une liste étendue.

   >[!TIP]
   >
   >* Lorsque vous ajustez manuellement les groupements lors de l&#39;affichage d&#39;une liste, Workfront mémorise vos préférences manuelles jusqu&#39;à ce que vous vous déconnectiez. Lorsque vous vous reconnectez, la liste s’affiche en fonction de ce paramètre.
   >* Les résultats d’un groupement s’affichent toujours agrandi après leur accès à partir d’un élément de graphique.

1. (Facultatif) Vous pouvez créer un groupement de matrice afin d&#39;afficher vos résultats sous forme de grille.

   Pour plus d’informations sur la création d’un rapport de matrice, voir [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Cliquez sur **Appliquer** pour appliquer vos modifications jusqu’à présent et poursuivre la modification du rapport avec les options suivantes.

   Cliquez sur **Enregistrer + Fermer** si vous avez terminé de modifier les regroupements dans le rapport et que vous souhaitez enregistrer le rapport.

### Ajout de filtres à un rapport {#add-filters-to-a-report}

1. Commencez à créer un rapport comme décrit dans la section [Créer un rapport](#create-a-report) dans cet article.
1. Dans le créateur de rapports, sélectionnez la variable **Filtres** pour identifier la quantité d’informations que le rapport doit inclure.
1. Cliquez sur **Ajouter une règle de filtre** pour ajouter un filtre personnalisé.\
   Ou\
   Choisir **Appliquer un filtre existant** pour utiliser un filtre existant.

   ![](assets/nwe-add-a-filter-350x93.png)

1. Si vous avez cliqué **Ajouter une règle de filtre**, commencez à saisir le champ à ajouter en tant que filtre. Si le champ est disponible, il est renseigné pour chaque objet auquel il peut être associé. Cliquez sur le nom du champ pour l’ajouter à ce filtre.\
   Utilisez des modificateurs de filtre pour créer votre filtre. Pour plus d’informations sur les modificateurs de filtre, voir [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Pour plus d’informations sur la création de filtres, voir [Présentation des filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Facultatif) Pour créer un filtre en mode texte, cliquez sur **Passer en mode Texte**.

   Pour plus d’informations sur l’utilisation du mode texte, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. Cliquez sur **Appliquer** lorsque vous avez terminé de modifier les filtres du rapport afin d’appliquer vos modifications jusqu’à présent, puis de poursuivre la modification du rapport avec les options suivantes.

   Cliquez sur **Enregistrer + Fermer** si le rapport et vous souhaitez l’enregistrer.

### Ajouter un graphique à un rapport {#add-a-chart-to-a-report}

1. Commencez à créer un rapport comme décrit dans la section [Créer un rapport](#create-a-report) dans cet article.
1. Dans le créateur de rapports, sélectionnez la variable **Graphique** puis sélectionnez le type de graphique à ajouter.

   ![](assets/nwe-add-a-chart-350x247.png)

   Pour plus d’informations sur la création d’un graphique dans un rapport, voir [Ajouter un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Cliquez sur **Appliquer** pour appliquer vos modifications jusqu’à présent et poursuivre la modification du rapport avec les options suivantes.

   Cliquez sur **Enregistrer + Fermer** si vous avez terminé de modifier le rapport et que vous souhaitez l’enregistrer.
