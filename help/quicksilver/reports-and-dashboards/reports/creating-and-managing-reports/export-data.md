---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Exporter des données
description: Vous pouvez exporter des données Adobe Workfront à partir de différentes listes, rapports, tableaux de bord et recherches.
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '2203'
ht-degree: 0%

---

# Exporter des données

<!-- Audited: 12/2023 -->

Vous pouvez exporter des données Adobe Workfront à partir de différentes listes, rapports, tableaux de bord et recherches.

Voici quelques raisons d’exporter des données :

* Vous souhaitez fournir une copie papier de vos données à une personne en dehors de Workfront.
* Vous souhaitez envoyer les résultats d’un rapport en pièce jointe à un utilisateur externe.
* Vous souhaitez créer une sauvegarde externe de vos données Workfront.
* Il existe une limite pour afficher seulement 2 000 résultats sur une page de l’application web Workfront. Si votre rapport en produit plus de 2 000, vous pouvez l’exporter dans n’importe quel format disponible et afficher tous les résultats dans le rapport dans une seule liste.

Vous pouvez soit exporter un rapport manuellement à partir de l’interface de Workfront, soit planifier l’envoi d’un rapport qui vous sera envoyé ultérieurement. Pour plus d’informations sur les rapports de planification de diffusion, voir [Présentation de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Les informations contenues dans cet article ne s&#39;appliquent pas aux exports suivants :

* Exporter des informations depuis des rapports graphiques.

  Pour plus d’informations sur l’export d’un rapport graphique, voir [Ajouter un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Exporter des informations à partir du diagramme de Gantt.

  Pour plus d’informations sur l’exportation du diagramme de Gantt, voir [Exportation du diagramme de Gantt vers PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Exporter des informations à partir du planificateur de ressources.

  Pour plus d’informations sur l’exportation des informations à partir du planificateur de ressources, voir &quot;Option d’exportation&quot; dans [Présentation de la navigation de Resource Planner](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>
    <p>Nouveau : clair ou supérieur</p>
    <p>ou</p>
    <p>Actuel : révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage ou accès supérieur aux rapports, tableaux de bord et calendriers pour l’exportation des rapports</p> <p>Affichage ou accès supérieur aux objets que vous affichez dans une liste pour exporter la liste</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher ou des autorisations supérieures à un rapport ou tableau de bord pour exporter le rapport ou le tableau de bord</p> <p>Autorisations d’affichage ou de niveau supérieur des objets que vous affichez dans une liste pour exporter la liste</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Le rapport doit être créé avant de pouvoir exporter ses données.

Pour plus d’informations sur la création de rapports, voir [Création d’un rapport personnalisé](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) ou [Créer une copie d’un rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Formats et limites d’exportation

### Formats d’exportation {#export-formats}

Les informations peuvent être exportées dans les formats suivants :

* PDF (paysage de lettre ou portrait, juridique, grand livre et A4)
* Excel (.xls)
* Excel (.xlsx)
* Délimité par des tabulations

>[!NOTE]
>
>Les tableaux de bord peuvent être imprimés ou exportés uniquement dans un fichier .pdf.

### Limites d’exportation {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

L’affichage des rapports dans Workfront présente plusieurs limites, ainsi que la manière dont ils sont exportés au moyen d’une exportation manuelle, d’un rapport remis ou via l’API.

* **50 000 cellules :** Nombre maximal de cellules autorisées dans un rapport exporté pour des fichiers Excel.
* **50 000 lignes :** Nombre de lignes de données autorisées dans un rapport exporté pour les fichiers .pdf et délimités par des onglets.

   * Pour les fichiers .xls Excel, cette limite est **65 000 lignes**.
   * Pour les fichiers Excel .xlsx, cette limite est **100 000 lignes**.
   * Ces limites excluent les en-têtes de colonne, ainsi que les lignes pour les regroupements dans le rapport. Par exemple, si un rapport comporte 6 groupements et 50 000 lignes de données, le fichier exporté en contiendra 50 000.

  >[!IMPORTANT]
  >
  >L’exportation d’un rapport qui inclut une référence de collection dans une colonne peut entraîner une erreur, même si le rapport se trouve dans les limites d’exportation répertoriées. Si la collection référencée est trop volumineuse, le processus d’exportation expire et entraîne par la suite une erreur.
  >
  >Pour éviter cette erreur, excluez les colonnes qui référencent des collections volumineuses ou réduisez la taille des collections référencées avant l’exportation.
  >

  Si votre rapport contient plus d’éléments que ces limites, vous recevez une erreur indiquant que l’exportation échoue. Réduisez le nombre d’éléments que vous voyez à l’écran pour qu’il soit inférieur ou égal à ces limites afin de pouvoir exporter les résultats.

  Si votre rapport contient plus de 50 000/ 65 000/ 100 000 lignes et que vous souhaitez exporter toutes les données, nous vous suggérons d’utiliser des filtres ou des invites pour obtenir des charges de données moindres et effectuer plusieurs exportations.

  Pour plus d’informations sur l’utilisation des filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Pour plus d’informations sur l’utilisation des invites, voir [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Ces limites s’appliquent à :

   * Exportation manuelle d’un rapport.
   * Rapport planifié.
   * Exportation via une intégration API.
   * Données exportées par le biais d’un démarrage rapide.

     Pour plus d’informations sur l’exportation de données par démarrage rapide, voir [Exporter des données d’Adobe Workfront par le biais de Démarrages de session](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >Vous pouvez exporter 50 000 lignes dans un fichier de démarrage rapide, bien que vous ne puissiez exporter les données qu’vers un fichier au format Excel.

   * Exportation des informations d’utilisation pour un projet.

     Pour plus d’informations sur l’exportation des informations d’utilisation pour un projet, voir [Présentation du rapport Utilisation des ressources](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **Taille de fichier de 10 Mo :** Limite de taille de fichier pour tout rapport exporté planifié pour diffusion. Si un fichier exporté joint à un email dépasse 5 Mo, un lien où le fichier peut être téléchargé est envoyé par courrier électronique au lieu du rapport exporté joint.
* **65 530 liens hypertexte :** Il s’agit d’une limite imposée par Excel aux documents qui contiennent plus de 65 530 liens hypertexte. Ces documents ne peuvent pas être ouverts lorsqu’ils sont exportés manuellement ou envoyés dans un rapport remis. Notez qu’un document Excel ne peut contenir que 200 lignes de données, mais s’il existe plus de 65 530 liens dans le document, celui-ci ne s’ouvre pas. Cette limite existe uniquement pour les fichiers Excel et non pour les autres formats pris en charge. 
* **256 colonnes**: il s’agit d’une limite imposée par Excel pour les documents qui contiennent plus de 256 colonnes. Ces documents ne peuvent pas être exportés manuellement ou envoyés dans un rapport remis. Cette limite existe uniquement pour les fichiers Excel et non pour les autres formats pris en charge.

Si vous tentez d’exporter des données au-delà de cette limite, il se peut que vous ne receviez pas toutes les données attendues dans l’exportation. Au contraire, un rapport modifié est produit dans la limite autorisée.

En outre, les rapports qui durent plus de 60 minutes seront arrêtés.

Si vous rencontrez des problèmes concernant votre limite, contactez le support technique de Workfront.

## Exporter des données

### Exporter des données depuis un rapport ou une liste {#export-data-from-a-report-or-list}

1. Accédez au rapport ou à la liste à exporter.
1. Sélectionnez les éléments à exporter. (La sélection d’éléments individuels exporte uniquement les éléments que vous sélectionnez.)

   Par exemple, dans un projet, sélectionnez les tâches à exporter.

   Ou

   Laissez tous les éléments désélectionnés pour exporter la liste entière.

1. Cliquez sur **Exporter**, puis sélectionnez un format.

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![](assets/nwe-dashboard-export-note-350x271.png)
   -->

   Ou

   Cliquez sur le bouton **Exporter** icon ![Icône Exporter](assets/export-icon-nwe.png), puis sélectionnez un format.

   Les options d’exportation de PDF disponibles dépendent des paramètres régionaux de vos paramètres utilisateur Workfront :

   * Amérique du Nord - lettre (par défaut), juridique, grand livre, A4

     <!--   
     <img src="assets/north-america.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * Tous les emplacements en dehors de l’Amérique du Nord - A3, A4 (par défaut), lettre, juridique, grand livre

     <!--   
     <img src="assets/everywhere-else.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

1. (Conditionnel) Selon le système d’exploitation que vous utilisez, vous avez la possibilité d’ouvrir ou d’enregistrer le fichier. Ouvrez le fichier avec l’application associée ou enregistrez-le sur votre disque dur.
1. Passez à la [Utiliser le document exporté](#use-the-exported-document).

### Exporter des données depuis un tableau de bord {#export-data-from-a-dashboard}

Vous pouvez imprimer les informations à partir d’un tableau de bord ou les exporter au format .pdf .

Pour plus d’informations sur l’export de données depuis un tableau de bord, voir [Exporter un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## Utiliser le document exporté {#use-the-exported-document}

* [Noms de fichiers](#file-names)
* [Titles](#titles)
* [Horodatages](#timestamps)
* [Formatage](#formatting)
* [Liens](#links)
* [Branding](#branding)

### Noms de fichiers {#file-names}

Que vous exportiez une liste d’objets ou un rapport, le fichier exporté aura un nom de fichier et un titre. Vous pouvez trouver le fichier exporté sur votre ordinateur en vous référant au nom du fichier. Le titre du rapport donnera aux utilisateurs une indication de ce que représente le fichier exporté lorsque vous le partagez avec eux.

#### Noms de fichiers pour les listes exportées {#file-names-for-exported-lists}

Lorsque vous exportez une liste d’objets, le type de l’objet est affiché dans le fichier exporté dans le nom du fichier et dans le titre de la liste.

Lorsque vous exportez une liste de tâches ou de problèmes, la variable **Nom du fichier** peut être l’un des suivants :

* Lorsque vous exportez des listes de tâches et de problèmes dans un projet :

   * *The_project_name_Exported_Tasks*(*dans des formats délimités par des tabulations, dans PDF, Excel (.xlsx) ou Excel*
   * *Problèmes_nom_projet_Exported_Issues*(*dans des formats délimités par des tabulations, dans PDF, Excel (.xlsx) ou Excel*

* Lorsque vous exportez des listes de tâches et de problèmes dans une tâche (sous-tâches) :

   * **Le_nom_du_projet_nom_de_la_tâche_exportée_Tâches**(*dans des formats délimités par des tabulations, dans PDF, Excel (.xlsx) ou Excel*
   * **The_project_name_the_task_name_Exported_Issues**(*dans des formats délimités par des tabulations, dans PDF, Excel (.xlsx) ou Excel*

Lorsque vous exportez une liste d’autres objets d’un projet vers un fichier de PDF, le nom de fichier du document exporté indique le type d’objets que vous avez exportés.\
Par exemple, le nom de fichier peut être :

* *Exported_Users*, lors de l’exportation de l’onglet Personnes sur le projet(*dans des formats délimités par des tabulations, dans PDF, Excel (.xlsx) ou Excel*
* *Exported_Risks*, lors de l’export d’une liste de risques sur le projet(*dans des formats délimités par des tabulations, dans PDF, Excel (.xlsx) ou Excel*

#### Noms de fichiers pour les rapports exportés {#file-names-for-exported-reports}

Lorsque vous exportez un rapport, le nom de fichier du rapport exporté est :

*Nom_du_rapport*(*dans des formats délimités par des tabulations, dans PDF, Excel (.xlsx) ou Excel*

### Titles {#titles}

Lorsque vous exportez une liste d’objets, seul le fichier au format PDF est doté d’un titre. Si vous exportez une liste ou un rapport aux formats Excel, Excel (.xlsx) ou Délimité par des onglets, le fichier ne comporte pas de titre.

#### Titre des listes exportées {#titles-for-exported-lists}

Lorsque vous exportez des listes de tâches et de problèmes dans un projet vers un fichier de PDF, le titre du document exporté est l’un des suivants :

* *Nom du projet : tâches exportées*
* *Nom du projet - Problèmes exportés*

Lorsque vous exportez des listes de tâches et de problèmes dans une tâche vers un fichier de PDF, la mosaïque du document exporté est l’une des suivantes :

* *Nom du projet - Nom de la tâche - Tâches exportées*
* *Nom du projet - Nom de la tâche - Problèmes exportés*

Lorsque vous exportez une liste d’autres objets d’un projet vers un fichier de PDF, le titre du document exporté indique le type d’objets que vous avez exportés.\
Par exemple, le titre peut être :

* *Utilisateurs exportés*, lors de l’exportation de l’onglet Personnes sur le projet.
* *Risques exportés*, lors de l’export d’une liste de risques sur le projet.

#### Titres des rapports exportés {#titles-for-exported-reports}

Un titre est attribué au rapport exporté vers un fichier de PDF.

Si le rapport est exporté dans des formats Excel, Excel (.xlsx) ou Délimité par des onglets, le rapport exporté n’aura pas de titre. Le titre du fichier exporté est le nom du rapport tel qu&#39;il apparaît dans l&#39;application web Workfront.

Si le rapport comporte une description, il est inclus dans le fichier exporté.

### Horodatages {#timestamps}

Un horodatage s’affiche sur le document exporté à partir du contexte de l’utilisateur qui a exporté l’élément.

L’horodatage comprend :

* Date
* Heure
* Fuseau horaire lors de l’exportation de l’élément

Selon le type de document que vous exportez, les horodatages s’affichent à différents emplacements :

* **PDF :** Les horodatages s’affichent dans le pied de page de chaque page et dans le nom du fichier.
* **Excel :** Les horodatages s’affichent dans le nom du fichier.

### Formatage {#formatting}

Lorsque vous exportez un projet au format .pdf, toutes les sous-tâches sont affichées en retrait par rapport à leurs tâches parentes. Les listes exportées ne réduisent aucune tâche parent.

Vous recevez toujours l&#39;onglet par défaut d&#39;un rapport lorsqu&#39;un rapport est envoyé ou planifié pour une diffusion, sauf si le rapport a une vue spéciale.

Si votre rapport présente une mise en forme spécifique dans l’application web, elle doit être fournie avec la mise en forme spéciale au moment de la diffusion des onglets Détails et Matrice, pour les fichiers .pdf et Excel uniquement.

>[!NOTE]
>
>Si les données que vous exportez contiennent des colonnes partagées et que vous les exportez au format Excel ou Délimité par des onglets, ces colonnes sont séparées dans le fichier exporté.

Pour plus d’informations sur la personnalisation de la mise en forme dans un rapport, voir [Utilisation d’une mise en forme conditionnelle dans les vues](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Liens {#links}

Les liens peuvent pointer vers n’importe quel objet de Workfront prenant en charge la liaison. Lorsque vous exportez une liste dans Workfront au format .pdf, tous les liens pris en charge existant dans le document d’origine restent actifs dans le document exporté.

>[!TIP]
>
>Si la ligne `valueformat=HTML` apparaît en mode texte pour une colonne de champ personnalisée et les valeurs de lien ne s’affichent pas dans un fichier .pdf exporté. vous devez saisir des lignes de code supplémentaires dans votre colonne en mode texte.
>
>Par exemple, si vous disposez d’un champ personnalisé appelé Open Q1 Projects qui contient des liens, vous devez ajouter le code suivant :
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

Lorsque vous effectuez une exportation vers un format Excel, seuls les liens vers des objets de Workfront sont inclus dans le fichier exporté et ils ne sont pris en charge que dans les emplacements où vous pouvez sélectionner des liens dans les documents Excel exportés, tels que les diffusions de rapports.

## Branding {#branding}

>[!IMPORTANT]
>
>La valorisation de la marque s’applique uniquement aux organisations qui ne sont pas encore intégrées à Adobe Experience Cloud.
>
>Si votre entreprise a été intégrée à Adobe Experience Cloud, la valorisation de marque n’est pas disponible.

Si votre administrateur Workfront a ajouté une valorisation de marque personnalisée à votre instance Workfront pour la barre de navigation globale, les fichiers .pdf exportés incluent également votre logo personnalisé.

Les données exportées dans d’autres formats ne peuvent pas être personnalisées avec votre logo.

Pour plus d’informations sur l’identité graphique de votre instance Workfront et de la barre de navigation globale, voir [Marque votre instance Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
