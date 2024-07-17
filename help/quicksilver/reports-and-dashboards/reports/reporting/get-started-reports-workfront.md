---
content-type: overview;reference
product-area: reporting
navigation-topic: reporting-navigation-topic
title: Prise en main des rapports
description: Les rapports fournissent une visibilité sur ce qui se passe avec les utilisateurs et le travail. Les rapports vous permettent d’afficher des informations sur les objets dans Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 478512af-a47c-4488-878a-581e238e0064
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '3294'
ht-degree: 1%

---

# Prise en main des rapports

<!-- Audited: 12/2023 -->

Les rapports fournissent une visibilité sur ce qui se passe avec les utilisateurs et le travail. Les rapports vous permettent d’afficher des informations sur les objets dans Adobe Workfront.

Pour plus d’informations sur la compréhension des objets et sur la manière dont ils peuvent être signalés dans l’application Workfront, voir [Présentation des objets Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Éléments de rapport

Les rapports sont une combinaison des trois éléments suivants dans Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Afficher</td> 
   <td> <li>Définit les colonnes de votre rapport et les informations que vous pouvez inclure dans chaque colonne.</li> <li>Pour plus d’informations sur les vues, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Présentation des vues dans Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Regroupement </td> 
   <td> <li>Classe les informations en fonction d’un élément d’information commun et répertorie les résultats du rapport sous des en-têtes.</li> <li>Pour plus d’informations sur les regroupements, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Présentation des regroupements dans Adobe Workfront</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtre</td> 
   <td> <li>Contrôle la quantité d’informations affichées dans un rapport.</li> <li>Pour plus d’informations sur les filtres, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Présentation des filtres</a>.</li> <li>Pour plus d’informations sur les modificateurs de filtre, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificateurs de filtre et de condition</a>.</li> <li>Vous pouvez filtrer à l’aide de caractères génériques, afin de rendre vos filtres plus généraux et de leur offrir une plus grande flexibilité d’utilisation.</li> <li>Pour plus d’informations sur l’utilisation de caractères génériques dans les filtres, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variables de filtre génériques</a>.</li> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Lorsque vous sélectionnez un nouveau filtre, une nouvelle vue ou un nouveau regroupement dans une liste, cette sélection est conservée même si vous vous déconnectez de Workfront ou que vous fermez votre navigateur.

Pour plus d’informations sur les éléments de rapport, voir [Eléments de rapport : filtres, vues et regroupements](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

Pour améliorer vos rapports, vous pouvez ajouter les éléments suivants :

* Un graphique : une représentation visuelle des résultats dans votre rapport.\
  Pour plus d’informations sur les rapports de graphique, voir [Ajout d’un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Un groupement de type matrice : résume les informations du rapport sous la forme d&#39;un tableau agrégé.\
  Pour plus d’informations sur les rapports de matrice, voir [Création d’un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Une invite : un filtre ouvert que vous pouvez personnaliser et appliquer différemment à chaque exécution du rapport.\
  Pour plus d&#39;informations sur les invites, voir [Ajout d&#39;une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

Lors de la création d’un rapport, vous pouvez modifier individuellement l’un de ces éléments dans le créateur de rapports.

Une autre manière d’améliorer la pertinence des informations incluses dans vos rapports consiste à appliquer une mise en forme conditionnelle à vos vues.\
Pour plus d’informations sur l’utilisation de la mise en forme conditionnelle, voir [Utilisation de la mise en forme conditionnelle dans les vues](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## Rapports système

Workfront fournit plusieurs rapports système qui sont chargés par défaut dans votre système.\
Après avoir saisi des informations dans votre système, vous pouvez utiliser ces rapports pour afficher les informations visuellement.

Pour plus d’informations sur l’accès aux rapports système et les rapports système disponibles, voir [Utilisation des rapports intégrés Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## Création de rapports

Outre les rapports système fournis par Workfront, vous pouvez créer vos propres rapports personnalisés pour répondre aux besoins de votre entreprise.

Pour créer un rapport, vous pouvez effectuer l’une des opérations suivantes :

* Créez un rapport à partir de zéro.
* Copiez un rapport existant.\
  Vous devez disposer d’au moins l’autorisation Afficher pour copier un rapport créé par une autre personne. Pour plus d’informations sur la copie d’un rapport, voir [Création d’une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Pour plus d’informations sur la création de rapports, reportez-vous à la section [Présentation des rapports du calendrier](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

### Prérequis pour la création de rapports {#prerequisites-for-creating-reports}

* Pour créer vos propres rapports, vous devez disposer d’une licence Plan (licences actuelles) ou d’une licence Standard (nouvelles licences).\
  Pour plus d’informations sur les types de licences Workfront, consultez [Présentation des licences](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) pour les licences actuelles et [Présentation des nouvelles licences](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md) pour les nouvelles licences.

* Votre administrateur Workfront doit vous donner accès à l’option Modifier les rapports dans votre niveau d’accès.\
  Pour plus d’informations sur l’octroi de l’accès à Modifier les rapports, voir [Octroi de l’accès aux rapports, tableaux de bord et calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* L’administrateur Workfront doit vous donner accès aux options Modifier les filtres, les vues et les groupes de votre niveau d’accès.

  Pour plus d’informations sur l’octroi de l’accès aux filtres, vues et regroupements d’édition, voir [Octroi de l’accès aux filtres, vues et regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Vous devez définir un objet sur lequel vous souhaitez générer des rapports. Les rapports sont spécifiques à un objet dans Workfront. Vous devez commencer par sélectionner un type d’objet avant de pouvoir commencer à créer le rapport. Vous pouvez uniquement créer des rapports sur les objets disponibles dans l’interface de Workfront.

### Propriété du rapport {#report-ownership}

Lorsque vous créez un rapport dans Workfront, vous devenez le propriétaire par défaut du rapport, qui s’affiche dans votre section Mes rapports . Vous ne pouvez pas modifier le propriétaire d’un rapport.

Lorsque vous copiez un rapport, vous devenez automatiquement propriétaire du rapport copié.
Pour plus d&#39;informations sur la copie de rapports, voir [Création d&#39;une copie d&#39;un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Vous pouvez voir qui possède un rapport en consultant le champ **Entré par**.

![Entré par champ](assets/nwe-entered-by-350x218.png)

### Création de rapports dans l’interface du créateur {#create-reports-in-the-builder-interface}

Nous vous recommandons d’utiliser d’abord l’interface de création de rapports pour créer un nouveau rapport. L’interface propose un ensemble simplifié d’outils qui vous guident tout au long de l’assemblage d’éléments pour créer le rapport de votre choix. Vous pouvez sélectionner des objets et des champs dans des listes et les ajouter à tous vos éléments de création de rapports.\
Pour plus d’informations sur la création de rapports dans l’interface de création de rapports, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour obtenir la liste des objets sur lesquels vous pouvez créer des rapports, reportez-vous à la section [Rapport sur les objets](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#report-on-objects) de l’article [Présentation des objets Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Pour plus d’informations sur les champs que vous pouvez afficher dans les rapports, voir le [Glossaire de la terminologie Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### Création de rapports en mode Texte {#create-reports-in-text-mode}

Parfois, il se peut que vous ne trouviez pas certains champs dans l’interface du créateur, mais ils peuvent être disponibles dans l’API.\
Pour plus d’informations sur les champs disponibles dans l’API, consultez l’article [API Explorer](../../../wf-api/general/api-explorer.md).

Pour plus d’informations sur l’utilisation de l’API Explorer, consultez l’article [Utilisation de l’API Explorer](../../../wf-api/general/using-api-explorer.md).

>[!NOTE]
>
>Vous ne pouvez pas générer de rapports dans l’interface de Workfront sur les objets qui ne sont pas disponibles dans le créateur de rapports. Cependant, vous pouvez créer des rapports sur les champs associés aux objets dans le créateur de rapports si ces champs sont disponibles via l’API. Pour ce faire, vous devez utiliser l’interface Mode texte .

Le mode Texte permet de créer des vues, filtres, regroupements et invites plus complexes en vous permettant d’utiliser des champs qui ne sont pas disponibles dans l’interface de mode standard.

#### Terminologie du mode texte {#text-mode-terminology}

Vous devez utiliser une syntaxe spécifique pour utiliser l’interface Mode texte de Workfront.

Pour plus d’informations sur la syntaxe Workfront pour le mode texte, voir [Présentation de la syntaxe du mode texte](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

#### Colonnes calculées, mise en forme conditionnelle et autres utilisations du mode Texte {#calculated-columns-conditional-formatting-and-other-uses-of-text-mode}

En dehors des rapports sur les champs qui ne sont pas disponibles dans l’interface du créateur, vous pouvez utiliser le mode Texte pour afficher des calculs ou des comparaisons entre certains champs.

Pour obtenir la liste des utilisations les plus courantes du mode Texte dans un rapport, reportez-vous à la section [Présentation des utilisations courantes du mode Texte](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Pour plus d’informations sur l’inclusion des données personnalisées calculées dans les rapports, voir [Données personnalisées calculées dans les rapports](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Pour plus d’informations sur la comparaison de champs dans la mise en forme conditionnelle, voir [Comparaison de champs dans la mise en forme conditionnelle](../../../reports-and-dashboards/reports/text-mode/compare-fields-conditional-formatting.md).

Vous pouvez également vous référer aux champs de collection à l’aide du mode Texte dans les rapports.\
Pour plus d’informations sur l’utilisation du mode Texte pour afficher les informations sur la collection dans un rapport, voir [Référencer des collections dans un rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

#### Exemples de mode texte {#text-mode-samples}

Nous disposons d’une bibliothèque d’exemples des vues, filtres et regroupements les plus utilisés que vous pouvez créer en mode texte.

Pour parcourir cette bibliothèque et utiliser certains des exemples que nous proposons, consultez l’article [Affichage personnalisé, filtrage et regroupement d’exemples : index de l’article](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Onglets d’un rapport

Un rapport peut contenir plusieurs onglets lors de son exécution dans l’interface.

Pour plus d’informations sur l’exécution d’un rapport, reportez-vous à l’article [Exécution d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

Sur chaque onglet, les informations que vous incluez dans le rapport s’affichent dans des formats légèrement différents. Choisissez le format qui répond le mieux aux besoins de votre entreprise.

Vous pouvez faire de n’importe quel onglet l’onglet par défaut du rapport. L’onglet par défaut est le premier onglet qui s’affiche lorsque vous cliquez sur le nom d’un rapport pour l’ouvrir, et c’est celui qui s’affiche lorsque vous placez le rapport sur un tableau de bord.

### Onglet Détails {#details-tab}

L&#39;onglet Détails d&#39;un rapport affiche dans un formulaire de liste l&#39;objet des rapports et les attributs que vous choisissez pour cet objet. Chaque rapport comporte un onglet Détails .

>[!IMPORTANT]
>
>Les informations de l’onglet Détails peuvent s’afficher différemment de l’onglet Graphique en fonction de votre fuseau horaire.\
>Par exemple, un utilisateur situé en Californie a effectué une tâche à 21 h 30 (heure du Pacifique) le 12 février. Lorsqu’un utilisateur de New York affiche un rapport qui inclut la fin de la tâche, la date d’achèvement réelle s’affiche le 13 février dans l’onglet Détails et les détails du graphique, car elle a été complétée à 00h30 (heure de l’Est) le 13 février. Cependant, dans le graphique, il est inclus dans le regroupement du 12 février jusqu’à ce que vous développiez l’élément de graphique.

### Onglet Résumé {#summary-tab}

Les rapports qui incluent un groupement comportent un onglet Résumé .

Les mêmes informations affichées au format liste dans l&#39;onglet Détails sont résumées et agrégées en fonction des regroupements dans le rapport de l&#39;onglet Résumé .

Pour plus d’informations sur les regroupements, voir [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

### Onglet Matrice {#matrix-tab}

Les rapports qui incluent un groupement matriciel ont un onglet Matrice.

Les mêmes informations affichées au format Liste dans l&#39;onglet Détails sont affichées dans un tableau, regroupées par groupe dans le rapport sous l&#39;onglet Matrice.

Lorsque vous ajoutez un groupement Matrice à un rapport, l&#39;onglet Résumé est remplacé par l&#39;onglet Matrice.

Pour plus d’informations sur la création d’un groupement matrice, reportez-vous à l’article [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

### Onglet Graphique {#chart-tab}

Les rapports qui incluent un graphique sont dotés d’un onglet Graphique .

Pensez à inclure un graphique dans vos rapports pour les tableaux de bord ayant un impact sur vos cadres. Les graphiques constituent un moyen concis d’afficher les informations d’un rapport. Vous pouvez développer un élément de graphique en cliquant dessus pour afficher les éléments inclus dans cet élément.

>[!IMPORTANT]
>
>Lorsque vous cliquez sur un élément de graphique, les informations développées peuvent s’afficher différemment du graphique en fonction de votre fuseau horaire.\
>Par exemple, un utilisateur situé en Californie a effectué une tâche à 21 h 30 (heure du Pacifique) le 12 février. Lorsqu’un utilisateur de New York affiche un rapport qui inclut la fin de la tâche, la date d’achèvement réelle s’affiche le 13 février dans l’onglet Détails et les détails du graphique, car elle a été complétée à 00h30 (heure de l’Est) le 13 février. Cependant, dans le graphique, il est inclus dans le regroupement du 12 février jusqu’à ce que vous développiez l’élément de graphique.

Pour plus d’informations sur la création d’un rapport avec un graphique, reportez-vous à l’article [Ajout d’un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

### Onglet Invite {#prompts-tab}

Les rapports qui incluent une invite sont dotés d’un onglet Invite .

Une invite vous permet d’ajouter un filtre à un rapport chaque fois que vous exécutez le rapport. Lorsque vous ajoutez une invite au rapport, l&#39;onglet Invite devient automatiquement l&#39;onglet par défaut du rapport. Il ne peut pas être remplacé par un autre onglet.

Pour plus d’informations sur la création d’une invite pour un rapport, reportez-vous à l’article [Ajout d’une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Partage de rapports

Après avoir créé un rapport, vous pouvez le partager avec d’autres utilisateurs.

### Attribution d’autorisations de partage à un rapport {#give-sharing-permissions-to-a-report}

Vous pouvez accorder des autorisations de partage à un autre utilisateur pour Afficher ou Gérer un rapport que vous créez. Vous pouvez accorder à un autre utilisateur un niveau d’autorisation inférieur ou égal au vôtre. Vous pouvez également rendre un rapport public à l’aide d’autorisations de partage. Pour plus d’informations sur le partage d’un rapport, voir [Partage d’un rapport dans Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Planification de la remise d’un rapport {#schedule-a-report-delivery}

Vous pouvez planifier la remise d’un rapport. Les utilisateurs avec lesquels vous partagez le rapport reçoivent un courrier électronique contenant une pièce jointe des résultats du rapport. La pièce jointe peut être aux formats suivants :

* HTML
* PDF
* Excel
* .TSV

Pour plus d’informations sur la planification de la remise d’un rapport, reportez-vous à la section [Présentation de la remise d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

### Exporter les résultats d’un rapport {#export-the-results-of-a-report}

Vous pouvez exporter les résultats d’un rapport aux formats de fichier suivants :

* PDF
* Excel (formats .xls et .xlsx)
* Délimité par des tabulations

Pour plus d&#39;informations sur l&#39;export des résultats d&#39;un rapport, voir [Export de données](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Une fois le rapport exporté dans l’un de ces formats, vous pouvez le partager avec d’autres utilisateurs en l’envoyant par courrier électronique en pièce jointe ou en l’imprimant.

### Ajouter un rapport à un tableau de bord {#add-a-report-to-a-dashboard}

Vous pouvez ajouter un rapport à un tableau de bord et le partager avec d’autres utilisateurs. Pour plus d’informations sur l’ajout de rapports à un tableau de bord, voir [Ajout d’un rapport à un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

## Création de calendriers

Si vous souhaitez afficher vos données sous forme de calendrier, vous pouvez créer des calendriers plutôt que des rapports.

Pour plus d’informations sur la création et l’utilisation des calendriers, consultez la [présentation des rapports sur les calendriers](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Utilisation des rapports

Après avoir créé des rapports et les avoir partagés avec d’autres utilisateurs, vous pouvez suivre la fréquence à laquelle ils utilisent ces rapports.
Pour plus d’informations sur l’utilisation des rapports, notamment la fréquence de leur affichage, l’utilisateur et les tableaux de bord qu’ils affichent, reportez-vous à l’article [Aperçu de l’utilisation des rapports](../../../reports-and-dashboards/reports/report-usage/report-usage-overview.md).

## Termes courants faisant référence aux rapports

Les termes suivants sont utilisés en référence aux rapports Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Terme ou expression</strong> </th> 
   <th><strong>Définition</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Options avancées</td> 
   <td> <p>Fait référence au lien de l’onglet Colonnes (vues) du Créateur de rapports qui permet d’effectuer les opérations suivantes :</p> 
    <ul> 
     <li>Définissez la mise en forme conditionnelle de style de colonne du texte et des images en fonction des critères que vous sélectionnez.</li> 
     <li>Relancez votre colonne.</li> 
     <li>Mettez en forme les valeurs de votre colonne.</li> 
    </ul> <p>Par exemple, vous pouvez afficher toutes les tâches parentes en gras ou la Date d’achèvement prévue en rouge si la tâche est en retard.</p> </td> 
  </tr> 
  <tr> 
   <td>Attribut</td> 
   <td> Champ d’un objet tel que défini dans la base de données. Il est utilisé dans une expression Mode Texte. <br>Par exemple, le champ Statut s’affiche sous la forme <em>status</em> lorsqu’il est utilisé dans une expression Mode texte. </td> 
  </tr> 
  <tr> 
   <td>Bean ou JavaBean</td> 
   <td>Un Bean représente un élément de programmation réutilisable. Le terme Bean identifie les relations entre différents objets dans l’application Workfront. Il est important de connaître ces relations lorsque vous essayez d’afficher des attributs supplémentaires sur un objet qui ne sont pas disponibles dans les outils de création de rapports de base.</td> 
  </tr> 
  <tr> 
   <td>Interface ou Report Builder du créateur</td> 
   <td>L’interface du créateur est une série de menus déroulants contenant les champs affichés dans les onglets Colonnes (vues), Filtre et Regroupement. Il fournit un mappage intuitif des relations Bean pour aider à identifier les colonnes dans une vue, les critères d’un filtre et les attributs communs d’un groupement.</td> 
  </tr> 
  <tr> 
   <td>Camel Case</td> 
   <td> <p>La casse Camel fait référence à une manière spécifique d’écrire des éléments de programmation pour associer des attributs à plusieurs mots. Lors de l’orthographe d’un attribut en majuscules, la première lettre du premier mot est en minuscules, il n’y a pas d’espace entre les mots et la première lettre d’un mot consécutif est en majuscule.</p> <p>Par exemple, le groupe d’accueil est écrit <em>homeGroup</em>, le pool de ressources est <em>resourcePool</em> et la date de début réelle est <em>realStartDate</em>.</p> </td> 
  </tr> 
  <tr> 
   <td>Graphique</td> 
   <td> <p>Un onglet du créateur de rapports, un onglet de rapport, après l’enregistrement du rapport, ainsi qu’un élément facultatif d’un rapport qui vous permet d’ajouter un graphique à n’importe quel rapport. Vous devez définir un Regroupement dans le rapport avant de pouvoir créer un graphique.</p> <p>Voici les types de graphiques qui peuvent être ajoutés à n’importe quel rapport :<br></p> 
    <ul> 
     <li>Colonnes</li> 
     <li>Barres</li> 
     <li>Secteurs</li> 
     <li>Lignes</li> 
     <li>Jauge</li> 
     <li>Bulles</li> 
    </ul> <p>Pour plus d’informations sur l’ajout de graphiques aux rapports, consultez l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Ajout d’un graphique à un rapport</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Détails</td> 
   <td>Il s’agit de l’un des onglets d’un rapport, une fois le rapport enregistré. Il affiche les résultats de votre rapport, affichés dans la vue et le regroupement de votre choix.</td> 
  </tr> 
  <tr> 
   <td>Expression...</td> 
   <td>Une expression est une formule écrite en mode Texte pour transmettre des informations à rechercher ou à afficher lors de l’utilisation de l’interface Mode Texte . Il s’agit généralement d’une ligne dans une instruction Text Mode plus grande.</td> 
  </tr> 
  <tr> 
   <td>Champs</td> 
   <td> <p>Fait référence aux attributs de vos objets. Par exemple, "État" est un champ pour les projets, les tâches ou les problèmes. "Gestionnaire de Portfolios" est un champ destiné à l’objet de Portfolio.</p> <p>Vous pouvez également avoir des champs personnalisés que vous créez vous-même et ajoutez à des formulaires personnalisés.<br>Pour plus d’informations sur la création de formulaires personnalisés, reportez-vous à l’article <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Création ou modification d’un formulaire personnalisé</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Nom de champ </td> 
   <td>La valeur d’un attribut qui s’affiche dans une vue, ou qui est utilisée dans la condition d’un filtre, ou comme élément commun d’un regroupement. Les options proposées pour le champ Nom dépendent de la sélection du Source de champ.</td> 
  </tr> 
  <tr> 
   <td>Source de champ </td> 
   <td>La valeur d’un objet affiché dans une vue, ou utilisé dans la condition d’un filtre, ou comme élément commun d’un regroupement. Les options du Source du champ dépendent du type d’objet de l’élément d’interface utilisateur en cours de création. Le Source de champ vous permet de référencer des attributs à partir d’objets autres que le type d’objet de l’élément d’interface utilisateur.</td> 
  </tr> 
  <tr> 
   <td>Filtre</td> 
   <td>Élément de rapport principal qui détermine les résultats qui s’affichent dans le rapport.</td> 
  </tr> 
  <tr> 
   <td>Formulaire </td> 
   <td>Utilisé de manière interchangeable avec "Formulaire personnalisé". Les champs et sections sont ajoutés aux formulaires, qui sont ensuite joints à un objet afin d’étendre le nombre de champs que vous pouvez associer à un objet.</td> 
  </tr> 
  <tr> 
   <td>Regroupement  </td> 
   <td>Élément de rapport principal qui identifie l’organisation d’une liste de résultats. Le groupement crée des barres horizontales dans tout le rapport afin de regrouper les résultats selon des attributs communs définis lors de sa création. Les groupes sont utilisés dans les rapports matriciels pour agréger les données, ainsi que dans les graphiques, afin de déterminer les axes des graphiques.</td> 
  </tr> 
  <tr> 
   <td>Objet ou type d’objet</td> 
   <td> Un objet est un élément d’application Workfront (par exemple, Projet, Tâche, Groupe, Société, Filtre). Le type d’objet est utilisé lors de la création d’un rapport, d’une vue, d’un filtre ou d’un regroupement afin d’identifier l’objet qui est le centre d’intérêt du rapport. Les rapports ne peuvent comporter qu’un seul type d’objet, qui est l’objet principal du rapport.<br>Les objets parents peuvent être référencés dans le même rapport.<br> Pour plus d’informations sur la hiérarchie des objets, reportez-vous à la section "Présentation de l’interdépendance et de la hiérarchie des objets" de l’article <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Présentation des objets Adobe Workfront</a>.</td> 
  </tr> 
  <tr> 
   <td>Invite</td> 
   <td> <p>Élément de rapport facultatif qui peut être ajouté à un rapport lorsque vous devez utiliser un filtre différent chaque fois que vous exécutez le rapport.</p> <p>Pour plus d'informations sur les invites, voir <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Ajout d'une invite à un rapport</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Qualificateur ou modificateurs de condition</td> 
   <td> <p>Ce champ s’affiche dans les zones suivantes d’un rapport :</p> 
    <ul> 
     <li>Sous l’onglet Filtre</li> 
     <li>L’écran Options avancées de la colonne dans l’onglet Colonnes (affichage) . En définissant un qualificateur, vous pouvez comparer le nom du champ à un autre champ ou valeur.</li> 
     <li> Dans une invite personnalisée<br><p>Pour plus d'informations sur les invites, voir <a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">Ajout d'une invite à un rapport</a>.</p>.</li> 
    </ul> <p>Par exemple, lors de la création d’un filtre pour les tâches avec une date d’achèvement planifiée d’aujourd’hui, vous sélectionnez <strong>Égal à</strong> dans votre champ Qualificateur et la date d’aujourd’hui dans le champ Date :</p> <p><em>Tâche&gt; Date d’achèvement planifiée&gt;Égal&gt;(date d’aujourd’hui)</em> </p> <p>Dans ce scénario, le qualificateur est <strong>Equal</strong>.<br>Pour plus d’informations sur les qualificateurs, consultez l’article <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificateurs de condition et de filtre</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Rapport </td> 
   <td>Combinaison d’une vue, d’un filtre et (parfois) d’un regroupement. Le but d’un rapport est d’afficher les données de manière cohérente dans l’interface, de distribuer les informations et d’éliminer la nécessité d’exécuter régulièrement la même recherche ou requête.</td> 
  </tr> 
  <tr> 
   <td>Statement</td> 
   <td>Se compose de plusieurs expressions qui sont assemblées pour définir les informations affichées dans un rapport lors de l’utilisation du mode Texte. Une instruction peut être créée pour une vue, un filtre, un regroupement ou pour une invite personnalisée dans un rapport.</td> 
  </tr> 
  <tr> 
   <td>Résumé</td> 
   <td>Il s’agit de l’un des onglets d’un rapport, une fois le rapport enregistré. Cet onglet n'est créé que lorsque vous définissez un groupement pour le rapport. Il résume les informations en fonction du groupement défini lors de la création du rapport et donne un aperçu rapide des objets agrégés du rapport. Il n’affiche pas tous les objets du rapport, mais uniquement ceux qui sont agrégés.</td> 
  </tr> 
  <tr> 
   <td>Interface du mode Texte</td> 
   <td>Permet de créer ou de modifier le code des vues, filtres, regroupements et invites personnalisés créés à l’origine via l’interface du créateur. Il est conseillé de créer initialement les éléments du rapport par le biais de l’interface du créateur, puis de les convertir en mode texte après leur enregistrement afin de simplifier le codage des vues avancées, des filtres, des regroupements ou des invites.</td> 
  </tr> 
  <tr> 
   <td>Interface utilisateur</td> 
   <td>Fait référence aux composants ou aux blocs de création de ce qui s’affiche à l’écran d’un utilisateur à un moment donné.</td> 
  </tr> 
  <tr> 
   <td>Affichage (ou colonnes)</td> 
   <td>Un des principaux éléments d'un rapport. Il identifie les en-têtes de colonne qui seront affichés dans la liste d’un rapport.</td> 
  </tr> 
 </tbody> 
</table>
