---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Exporter les données
description: Vous pouvez exporter des données Adobe Workfront à partir de listes, de rapports, de tableaux de bord et de recherches.
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '2252'
ht-degree: 81%

---

# Exporter des données

<!-- Audited: 5/2025 -->

Vous pouvez exporter des données Adobe Workfront à partir de listes, de rapports, de tableaux de bord et de recherches.

Voici quelques raisons d’exporter des données :

* Vous souhaitez fournir une copie physique de vos données à une personne en dehors de Workfront.
* Vous souhaitez envoyer les résultats d’un rapport en tant que pièce jointe à un utilisateur ou à une utilisatrice externe.
* Vous souhaitez créer une sauvegarde externe de vos données Workfront.
* Il existe une limite d’affichage de 2 000 résultats au maximum par page dans l’application web Workfront. Si votre rapport en produit plus de 2 000, vous pouvez l’exporter dans un des formats disponibles et afficher tous les résultats du rapport dans une seule liste.

Vous pouvez soit exporter un rapport manuellement à partir de l’interface de Workfront, soit planifier la remise d’un rapport qui vous sera envoyé ultérieurement. Pour plus d’informations sur la planification de remises de rapports, voir [Vue d’ensemble des remises de rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Les informations contenues dans cet article ne s’appliquent pas aux exports suivants :

* Export d’informations depuis des rapports de graphiques.

  Pour plus d’informations sur l’export d’un rapport de graphique, voir [Ajouter un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Export d’informations à partir d’un graphique de Gantt.

  Pour plus d’informations sur l’export du graphique de Gantt, voir [Exporter le graphique de Gantt au format PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Export d’informations à partir du planificateur de ressources.

  Pour plus d’informations sur l’export d’informations à partir du planificateur de ressources, voir « Options d’export » dans [Vue d’ensemble de la navigation du planificateur de ressources](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

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
      <p>Léger</p>
      <p>Vérifier</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès Afficher ou supérieur aux rapports, tableaux de bord et calendriers pour exporter des rapports</p> <p>Accès Afficher ou supérieur aux objets que vous affichez dans une liste pour exporter la liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Afficher ou supérieures pour un rapport ou un tableau de bord, pour exporter le rapport ou le tableau de bord.</p> <p>Autorisation Afficher ou supérieure pour les objets que vous affichez dans une liste, pour exporter la liste.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Le rapport doit être créé avant de pouvoir exporter les données qu’il contient.

Pour plus d’informations sur la création de rapports, voir [Créer un rapport personnalisé](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) ou [Créer une copie d’un rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Formats et limites d’export

### Formats d’export {#export-formats}

Les informations peuvent être exportées dans les formats suivants :

* PDF (paysage ou portrait)
* Excel
* Excel (.xlsx)
* Délimité par des tabulations

>[!NOTE]
>
>Les tableaux de bord peuvent être imprimés ou exportés uniquement dans un fichier PDF.

### Limites d’export {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

L’affichage des rapports dans Workfront présente plusieurs limites, ainsi que leur export lorsqu’il est effectué manuellement ou via une remise de rapport, ou via l’API.

* **50 000 cellules :** nombre maximal de cellules autorisées dans un rapport exporté pour des fichiers Excel.
* **50 000 lignes :** nombre de lignes de données autorisées dans une exportation de rapport pour les fichiers PDF et délimités par des tabulations.

   * Pour les fichiers Excel, cette limite est de 65 000 lignes **&#x200B;**.
   * Pour les fichiers Excel(.xlsx), cette limite est de 100 000 lignes **&#x200B;**.
   * Ces limites excluent les en-têtes de colonne, ainsi que les lignes des regroupements dans le rapport. Par exemple, si un rapport comporte 6 regroupements et 50 000 lignes de données, le fichier exporté contiendra 50 000 lignes.

  >[!IMPORTANT]
  >
  >L’export d’un rapport qui inclut une référence de collection dans une colonne peut entraîner une erreur, même si le rapport respecte les limites d’export spécifiées. Si la collection référencée est trop volumineuse, le processus d’export expire et entraîne par conséquent une erreur.
  >
  >Pour éviter cette erreur, excluez les colonnes qui référencent des collections volumineuses ou réduisez la taille des collections référencées avant l’export.

  Si le nombre d’éléments de votre rapport dépasse ces limites, vous recevez une erreur indiquant que l’export a échoué. Réduisez le nombre d’éléments que vous voyez à l’écran pour qu’il soit inférieur ou égal à ces limites afin de pouvoir exporter les résultats.

  Si votre rapport contient plus de 50 000/65 000/100 000 lignes et que vous souhaitez exporter toutes les données, nous vous conseillons d’utiliser des filtres ou des invites pour obtenir des charges de données plus petites, et d’effectuer plusieurs exports.

  Pour plus d’informations sur l’utilisation de filtres, voir [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Pour plus d’informations sur l’utilisation d’invites, voir [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Ces limites s’appliquent aux éléments suivants :

   * Export manuel d’un rapport.
   * Rapport planifié.
   * Export via une intégration API.
   * Données exportées via un Kickstart.

     Pour plus d’informations sur l’export de données via Kickstart, voir [Exporter des données à partir d’Adobe Workfront via Kickstart](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >Vous pouvez exporter 50 000 lignes dans un fichier Kickstart, mais vous ne pouvez exporter les données que dans un fichier au format Excel.

   * Export d’informations d’utilisation pour un projet.

     Pour plus d’informations sur l’export des informations d’utilisation pour un projet, voir [Vue d’ensemble du rapport d’utilisation des ressources](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **Taille de fichier de 10 Mo :** limite de taille de fichier pour tout rapport exporté dont la remise est planifiée. Si un fichier exporté joint à un e-mail dépasse 5 Mo, un lien pour le téléchargement du fichier est envoyé par e-mail à la place du rapport exporté joint.
* **65 530 liens hypertexte :** il s’agit d’une limite imposée par Excel aux documents qui contiennent plus de 65 530 liens hypertexte. Ces documents ne peuvent pas être ouverts lorsqu’ils sont exportés manuellement ou envoyés dans un rapport diffusé. Notez qu’un document Excel peut ne contenir que 200 lignes de données, mais s’il existe plus de 65 530 liens dans le document, celui-ci ne s’ouvre pas. Cette limite existe uniquement pour les fichiers Excel, et non pour les autres formats pris en charge.
* **256 colonnes** : limite imposée par Excel pour les documents qui contiennent plus de 256 colonnes. Ces documents ne peuvent pas être exportés manuellement ni envoyés dans un rapport diffusé. Cette limite existe uniquement pour les fichiers Excel, et non pour les autres formats pris en charge.

  >[!IMPORTANT]
  >
  >L’exportation d’un rapport qui comprend une colonne Rapports peut entraîner une erreur, même si le rapport se situe par ailleurs dans les limites d’exportation répertoriées.
  >
  >Si vous utilisez la fonctionnalité d’exportation pour partager un rapport contenant une colonne Rapports avec d’autres personnes, pensez à partager le rapport en le rendant public à la place. Pour plus d’informations sur la publication d’un rapport, voir [Partager un rapport dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
  >
  >Si vous utilisez la fonction d’exportation pour évaluer les données en externe, nous vous recommandons d’utiliser Workfront Data Connect à la place. Pour plus d&#39;informations, consultez [Présentation de Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

Si vous tentez d’exporter des données au-delà de cette limite, il se peut que vous ne receviez pas toutes les données attendues dans l’export. Au contraire, un rapport modifié est produit dans les limites autorisées.

En outre, les rapports qui mettent plus de 60 minutes à s’exécuter seront arrêtés.

Si vous avez des questions ou rencontrez des problèmes concernant votre limite, contactez l’assistance technique de Workfront.

## Exporter des données

### Exporter des données à partir d’un rapport ou d’une liste {#export-data-from-a-report-or-list}

1. Accédez au rapport ou à la liste que vous souhaitez exporter.
1. Sélectionnez les éléments que vous souhaitez exporter. La sélection d’éléments individuels exporte uniquement les éléments que vous sélectionnez.

   Par exemple, dans un projet, sélectionnez les tâches que vous souhaitez exporter.

   Ou

   Ne sélectionnez aucun élément pour exporter l’ensemble de la liste.

1. Cliquez sur **Exporter**, puis sélectionnez un format.

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![Export dashboard note](assets/nwe-dashboard-export-note-350x271.png)
   -->

   Ou

   Cliquez sur l’icône **Exporter** ![Icône Exporter](assets/export-icon-nwe.png), puis sélectionnez un format.

   Les options disponibles pour l’exportation de PDF dépendent des paramètres régionaux des e-mails définis dans les paramètres utilisateur de Workfront :

   * Amérique du Nord - Lettre - Paysage, Lettre - Portrait, Autres tailles

   * Tous les emplacements hors Amérique du Nord - A4 - Paysage, A4 - Portrait, Autres tailles

1. (Le cas échéant) Selon le système d’exploitation que vous utilisez, vous avez éventuellement la possibilité d’ouvrir ou d’enregistrer le fichier. Ouvrez le fichier avec l’application associée ou enregistrez-le sur votre disque dur.
1. Pour comprendre comment les informations s’affichent dans le fichier exporté, poursuivez la lecture de la section [Utiliser le document exporté](#use-the-exported-document) de cet article.

### Exporter des données à partir d’un tableau de bord {#export-data-from-a-dashboard}

Vous pouvez imprimer les informations à partir d’un tableau de bord ou les exporter sous forme de fichier PDF.

Pour plus d’informations sur l’export de données à partir d’un tableau de bord, voir [Exporter un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## Utiliser le document exporté {#use-the-exported-document}

Les sections suivantes décrivent l’affichage des informations dans un fichier exporté :

* [Noms des fichiers](#file-names)
* [Titres](#titles)
* [Horodatages](#timestamps)
* [Formatage](#formatting)
* [Liens](#links)
* [Branding](#branding)

### Noms des fichiers {#file-names}

Lors de l’export d’une liste d’objets ou d’un rapport, le fichier exporté aura un nom de fichier et un titre. Pour trouver le fichier exporté sur votre ordinateur, recherchez-le par son nom de fichier. Le titre du rapport exporté fournira aux utilisateurs et utilisatrices un contexte lorsque vous le partagez avec eux.

#### Noms de fichiers pour les listes exportées {#file-names-for-exported-lists}

Lorsque vous exportez une liste d’objets, le type de l’objet est affiché dans le nom du fichier exporté et dans le titre de la liste.

Lorsque vous exportez une liste de tâches ou de problèmes, le **Nom du fichier** peut ressembler à ce qui suit :

* Lorsque vous exportez des listes de tâches et de problèmes dans un projet :

   * *Nom_du_projet_Tâches_exportées* (*dans des formats PDF, Excel, Excel (.xlsx) ou délimité par des tabulations)*
   * *Nom_du_projet_Problèmes_exportés* (*dans des formats PDF, Excel, Excel (.xlsx) ou délimité par des tabulations)*

* Lorsque vous exportez des listes de tâches et de problèmes dans une tâche (sous-tâches) :

   * **Nom_du_projet_nom_de_la_tâche_Tâches_exportées** (*dans des formats PDF, Excel, Excel (.xlsx) ou délimité par des tabulations)*
   * **Nom_du_projet_nom_de_la_tâche_Problèmes_exportés** (*dans des formats PDF, Excel, Excel (.xlsx) ou délimité par des tabulations)*

Lorsque vous exportez une liste d’autres objets d’un projet vers un fichier PDF, le nom du fichier du document exporté indique le type d’objets que vous avez exportés.\
Le nom du fichier peut ressembler à ceci :

* *Personnes_exportées*, lors de l’export de l’onglet Personnes sur le projet (*dans des formats PDF, Excel, Excel (.xlsx) ou délimité par des tabulations)*
* *Risques_exportés*, lors de l’export d’une liste de risques sur le projet (*dans des formats PDF, Excel, Excel (.xlsx) ou délimité par des tabulations)*

#### Noms de fichiers pour les rapports exportés {#file-names-for-exported-reports}

Lorsque vous exportez un rapport, le nom du fichier du rapport exporté ressemble à ceci :

*Nom_du_rapport* (*dans des formats PDF, Excel, Excel (.xlsx) ou délimité par des tabulations)*

### Titres {#titles}

Lorsque vous exportez une liste d’objets, seul le fichier au format PDF contient un titre. Si vous exportez une liste ou un rapport aux formats Excel, Excel (.xlsx) ou délimité par des tabulations, le fichier ne comporte pas de titre.

#### Titres des listes exportées {#titles-for-exported-lists}

Lorsque vous exportez des listes de tâches et de problèmes d’un projet vers un fichier PDF, le titre du document exporté ressemble à ceci :

* *Nom du projet - Tâches exportées*
* *Nom du projet - Problèmes exportés*

Lorsque vous exportez des listes de tâches et de problèmes d’une tâche vers un fichier PDF, le titre du document exporté ressemble à ceci :

* *Nom du projet - Nom de la tâche - Tâches exportées*
* *Nom du projet - Nom de la tâche - Problèmes exportés*

Lorsque vous exportez une liste d’autres objets d’un projet vers un fichier PDF, le titre du document exporté indique le type d’objets que vous avez exportés.\
Le titre peut ressembler à ceci :

* *Personnes exportées*, lors de l’export de l’onglet Personnes sur le projet.
* *Risques exportés*, lors de l’export d’une liste de risques sur le projet.

#### Titres des rapports exportés {#titles-for-exported-reports}

Un titre est attribué au rapport exporté vers un fichier PDF.

Si le rapport est exporté aux formats Excel, Excel (.xlsx) ou délimité par des tabulations, le rapport exporté ne comportera pas de titre. Le titre du fichier exporté est le nom du rapport tel qu’il s’affiche dans l’application web Workfront.

Si le rapport comporte une description, elle est incluse dans le fichier exporté.

### Horodatages {#timestamps}

Un horodatage s’affiche sur le document exporté d’après le contexte de l’utilisateur ou de l’utilisatrice qui a exporté l’élément.

L’horodatage comprend :

* Date
* Heure
* Fuseau horaire lors de l’export de l’élément

Selon le type de document que vous exportez, les horodatages s’affichent à différents emplacements :

* **PDF :** les horodatages s’affichent dans le pied de page de chaque page et dans le nom du fichier.
* **Excel :** les horodatages s’affichent dans le nom du fichier.

### Formatage {#formatting}

Lorsque vous exportez un projet vers PDF, toutes les sous-tâches sont mises en retrait par rapport à leurs tâches parents. Les listes exportées ne réduisent aucune tâche parent.

Vous recevez toujours l’onglet par défaut d’un rapport lorsqu’un rapport est envoyé ou planifié pour une remise, sauf si le rapport possède une vue spécifique.

Si votre rapport possède une mise en forme spéciale dans l’application web, il doit être diffusé avec une mise en forme spéciale lorsque les onglets Détails et Matrice sont diffusés, pour les fichiers PDF et Excel uniquement.

>[!NOTE]
>
>Si les données que vous exportez contiennent des colonnes partagées et que vous les exportez au format Excel ou dans un format délimité par des tabulations, ces colonnes sont séparées dans le fichier exporté.

Pour plus d’informations sur la personnalisation de la mise en forme dans un rapport, voir [Utiliser une mise en forme conditionnelle dans les vues](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Liens {#links}

Les liens peuvent pointer vers n’importe quel objet de Workfront prenant en charge les liens. Lorsque vous exportez une liste dans Workfront vers PDF, tous les liens pris en charge qui existent dans le document d’origine restent actifs dans le document exporté.

>[!TIP]
>
>Si la ligne `valueformat=HTML` apparaît en mode texte pour une colonne de champ personnalisé et que les valeurs de lien ne s’affichent pas dans un fichier PDF exporté, vous devez saisir des lignes de code supplémentaires dans votre colonne en mode texte.
>
>Par exemple, si vous disposez d’un champ personnalisé appelé « Open Q1 Projects » (Projets ouverts du premier trimestre) qui contient des liens, vous devez ajouter le code suivant :
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

Lorsque vous effectuez un export vers un format Excel, seuls les liens pointant vers des objets Workfront sont inclus dans le fichier exporté et ils ne sont pris en charge que dans les emplacements où vous pouvez sélectionner des liens dans les documents Excel exportés, tels que les remises de rapports.

## Branding {#branding}

>[!IMPORTANT]
>
>Le branding s’applique uniquement aux organisations qui ne sont pas encore intégrées à Adobe Experience Cloud.
>
>Si votre organisation est intégrée à Adobe Experience Cloud, le branding n’est pas disponible.

Si votre administrateur Workfront a ajouté une valorisation de marque personnalisée à votre instance Workfront pour la barre de navigation globale, les fichiers PDF exportés incluent également votre logo personnalisé.

Les données exportées dans d’autres formats ne peuvent pas être personnalisées avec votre logo.

Pour plus d’informations sur le branding de votre instance Workfront et de la barre de navigation globale, voir [Branding de votre instance Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
