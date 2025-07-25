---
product-area: documents
navigation-topic: approvals
title: Créer un tableau de bord de révision et d’approbation
description: Vous pouvez consulter les mesures d’approbation dans les Tableaux de bord de la zone de travail.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 48f8605b-c342-493b-96e7-f73248e34b35
source-git-commit: 0b4884d6c9a88c096b15af65a2aff0a54ca66811
workflow-type: tm+mt
source-wordcount: '2520'
ht-degree: 1%

---

# Créer un tableau de bord de rapports à réviser et à approuver

Vous pouvez créer un tableau de bord de rapports dans la zone Tableaux de bord de la zone de travail afin d’afficher des informations détaillées et de haut niveau sur les révisions et les approbations avec la fonctionnalité d’approbations unifiées.

>[!IMPORTANT]
>
>Cette fonctionnalité est disponible uniquement pour les clients qui utilisent le service Validations unifiées et qui sont inscrits à la version Beta des tableaux de bord de la zone de travail. Pour plus d’informations, voir [Informations bêta sur les tableaux de bord de la zone de travail](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).


![exemple de tableau de bord](assets/whole-dashboard.png)

## Créer un tableau de bord

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.
1. Cliquez sur **Nouveau tableau de bord**.
1. Nommez votre tableau de bord .
1. (Facultatif) Ajoutez une description.
1. Cliquez sur **Créer**.
   ![ajouter un nom et une description au tableau de bord](assets/create-a-dashboard.png)

Une fois que vous avez créé un tableau de bord, vous pouvez commencer à ajouter des indicateurs clés de performance, des graphiques et des tableaux. Pour plus d’informations, consultez les sections suivantes :

* [Ajouter des informations de révision et d’approbation de haut niveau avec des indicateurs clés de performance et des graphiques](#add-high-level-review-and-approval-information-with-kpis-and-charts)
* [Ajouter des informations de révision et d’approbation détaillées avec les tableaux](#add-detailed-review-and-approval-information-with-tables)

## Ajouter des informations de révision et d’approbation de haut niveau avec des indicateurs clés de performance et des graphiques

Vous pouvez afficher des informations générales sur les approbations de documents avec des indicateurs clés de performance et des graphiques.

Pour plus d’informations, voir [Création d’un rapport sur les indicateurs de performance clés](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md) et [Création d’un rapport graphique](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

### KPI

![Exemples d’indicateurs de performance clés](assets/kpi-dashboard.png)

#### Approbations en attente

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans l’angle supérieur droit de la page des détails du tableau de bord, cliquez sur **Ajouter un rapport**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **KPI**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Saisissez *En attente* dans le champ **Nom**.
   1. Saisissez *Approbations en attente* dans le champ **Description**. S’affiche sous la valeur de l’indicateur de performance clé sous forme de légende.

1. Suivez les étapes ci-dessous pour configurer la section **Créer un KPI** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Créer un KPI** ![Créer un KPI](assets/build-kpi-icon.png).

   1. Cliquez sur **Sélectionner un champ**.

   1. Recherchez et sélectionnez le dossier **Approbation du document**.

   1. Sélectionnez **Statut**.

   1. Dans le menu déroulant **Type d’agrégation**, sélectionnez **Comptage**.

1. Pour configurer la section **Filtre**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![Icône Filtrer](assets/filter-icon.png).

   1. Sélectionnez **Modifier le filtre**.

   1. Cliquez sur **Ajouter une condition**.

   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Statut**.
   1. Laissez l’opérateur sur **Égal**, puis saisissez _en attente de révision_ dans la zone de texte.

      ![exemple de filtre kpi en attente](assets/pending-kpi-filter.png)
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.


#### Approbations en retard

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans l’angle supérieur droit de la page des détails du tableau de bord, cliquez sur **Ajouter un rapport**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **KPI**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Saisissez _Overdue_ dans le champ **Name**.
   1. Tapez _Échéance de l’étape d’approbation dans le passé_ dans le champ **Description**. Cette description s’affiche sous forme de légende sous la valeur de l’indicateur de performance clé.

1. Suivez les étapes ci-dessous pour configurer la section **Créer un KPI** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Créer un KPI** ![Créer un KPI](assets/build-kpi-icon.png).

   1. Cliquez sur **Sélectionner un champ**.

   1. Recherchez et sélectionnez le dossier **Approbation du document**.

   1. Sélectionnez **Statut**.

   1. Dans le menu déroulant **Type d’agrégation**, sélectionnez **Comptage**.

1. Pour configurer la section **Filtre**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![Icône Filtrer](assets/filter-icon.png).

   1. Sélectionnez **Modifier le filtre**.

   1. Cliquez sur **Ajouter une condition**.

   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.

   1. Sélectionnez **Étape d’approbation** > **Échéance**.
   1. Remplacez l’opérateur par **Inférieur à**.
   1. Basculez **Définir la date relative** sur **ON**, puis saisissez _$$TODAY_ dans la zone de texte.

      ![exemple de filtre kpi en retard](assets/overdue-kpi-filter.png)
   1. Cliquez sur **Ajouter une condition**.
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Statut**.
   1. Modifiez l’opérateur sur **Ne contient pas**, puis saisissez _approuvé_ dans la zone de texte.

      ![exemple 2 de filtre kpi en retard](assets/overdue-kpi-filter-2.png)
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.


#### Validations terminées


1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans l’angle supérieur droit de la page des détails du tableau de bord, cliquez sur **Ajouter un rapport**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **KPI**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Saisissez _Completed_ dans le champ **Name**.
   1. Saisissez _Nombre de statuts d’approbation_ dans le champ **Description**. Cette description s’affiche sous forme de légende sous la valeur de l’indicateur de performance clé.

1. Suivez les étapes ci-dessous pour configurer la section **Créer un KPI** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Créer un KPI** ![Créer un KPI](assets/build-kpi-icon.png).

   1. Cliquez sur **Sélectionner un champ**.

   1. Recherchez et sélectionnez le dossier **Approbation du document**.

   1. Sélectionnez **Statut**.

   1. Dans le menu déroulant **Type d’agrégation**, sélectionnez **Comptage**.

1. Pour configurer la section **Filtre**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![Icône Filtrer](assets/filter-icon.png).

   1. Sélectionnez **Modifier le filtre**.

   1. Cliquez sur **Ajouter une condition**.

   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.

   1. Sélectionnez **Statut**.

   1. Remplacez l’opérateur par **Contient** et saisissez _Approved_ dans la zone de texte.

      ![exemple de filtre kpi terminé](assets/completed-kpi-filter.png)
   1. Cliquez sur **Ajouter une condition**.
   1. Cliquez sur **Et** pour le remplacer par **Ou**.
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Statut**.
   1. Remplacez l’opérateur par **Égal**, puis saisissez _révisé_ dans la zone de texte.

      ![exemple de filtre kpi terminé](assets/completed-kpi-filter-2.png)
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.

#### Approbations abandonnées

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans l’angle supérieur droit de la page des détails du tableau de bord, cliquez sur **Ajouter un rapport**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **KPI**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Saisissez _Abandonné_ dans le champ **Nom**.
   1. Saisissez _échéance de validation supérieure à 2 semaines_ dans le champ **Description**. Cette description s’affiche sous forme de légende sous la valeur de l’indicateur de performance clé.

1. Suivez les étapes ci-dessous pour configurer la section **Créer un KPI** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Créer un KPI** ![Créer un KPI](assets/build-kpi-icon.png).

   1. Cliquez sur **Sélectionner un champ**.

   1. Recherchez et sélectionnez le dossier **Étape d’approbation du document**.

   1. Sélectionnez **Échéance**.

   1. Dans le menu déroulant **Type d’agrégation**, sélectionnez **Comptage**.

1. Pour configurer la section **Filtre**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![Icône Filtrer](assets/filter-icon.png).

   1. Sélectionnez **Modifier le filtre**.

   1. Cliquez sur **Ajouter une condition**.

   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.

   1. Sélectionnez **Statut**.

   1. Modifiez l’opérateur sur **Ne contient pas** et saisissez _approuvé_ dans la zone de texte.

      ![exemple de filtre kpi abandonné](assets/abandoned-kpi-filter.png)
   1. Cliquez sur **Ajouter une condition**.
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Échéance**.
   1. Remplacez l’opérateur par **Inférieur à**, puis activez le bouton (bascule) **Définir la date relative** sur **ACTIVÉ**.
   1. Saisissez _$$TODAY-2w_ dans la zone de texte.

      ![exemple de filtre kpi abandonné](assets/abandoned-kpi-filter-2.png)
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.

### Graphiques

![Exemples de graphiques](assets/chart-dashboard.png)

#### Graphique à barres Approbations par décision

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans l’angle supérieur droit de la page des détails du tableau de bord, cliquez sur **Ajouter un rapport**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **Graphique**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Saisissez _Validations par décision_ dans le champ **Nom**.
   1. (Facultatif) Saisissez une description dans le champ **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.
1. Pour configurer la section **Créer un graphique**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Créer un graphique** ![Créer un graphique](assets/build-chart-icon.png).

   1. Dans le menu déroulant **Type de graphique**, laissez **Barre** sélectionné.
   1. Dans le menu déroulant **Type de barre**, laissez l’option **Simple** sélectionnée.
   1. Cliquez sur **Mettre à jour le champ** pour l&#39;axe **Bas (X)**, puis sélectionnez **Approbation du document** > **Statut**.
   1. Définissez le **Type d’agrégation** sur **Nombre**.
   1. Cliquez sur **Mettre à jour le champ** pour l’axe **Gauche (Y)**, puis sélectionnez **Statut**.
1. Pour configurer la section **Filtre**, procédez comme suit :
   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![icône de l’onglet Filtrer](assets/filter-tab.png).
   1. Cliquez sur **Modifier le filtre**, puis **Ajouter une condition**.
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Version du document** > **Version**.
   1. Remplacez l’opérateur par **N’est pas nul**.

      ![exemple de filtre](assets/approvals-by-decision-chart-filter.png)
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.


#### Graphique à barres Révisions

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans l’angle supérieur droit de la page des détails du tableau de bord, cliquez sur **Ajouter un rapport**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **Graphique**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Saisissez _Révisions_ dans le champ **Nom**.
   1. Tapez _Nombre de révisions des documents dont les décisions sont incomplètes et prévues avant la fin du mois_ dans le champ **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.

1. Pour configurer la section **Créer un graphique**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Créer un graphique** ![Créer un graphique](assets/build-chart-icon.png).

   1. Dans le menu déroulant **Type de graphique**, laissez **Barre** sélectionné.
   1. Dans le menu déroulant **Type de barre**, laissez l’option **Simple** sélectionnée.
   1. Cliquez sur **Mettre à jour le champ** pour l’**Axe inférieur (X)**, puis sélectionnez **Approbation du document** > **Version du document** > **Version**.
   1. Définissez le **Type d’agrégation** sur **Nombre**.
   1. Cliquez sur **Mettre à jour le champ** pour l’axe **Gauche (Y)**, puis sélectionnez **Approbation du document** > **Version du document** > **Document** > **Name**.

1. Pour configurer la section **Filtre**, procédez comme suit :
   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![icône de l’onglet Filtrer](assets/filter-tab.png).
   1. Cliquez sur **Modifier le filtre**, puis **Ajouter une condition**.
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.

   1. Sélectionnez **Étape d’approbation** > **Participants à l’étape d’approbation** > **Date de décision**.

   1. Remplacez l’opérateur par **Est nul**.

      ![exemple de filtre de graphique de révisions](assets/revision-chart-filter.png)
   1. Cliquez sur **Ajouter une condition**.
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Étape d’approbation** > **Échéance**.
   1. Remplacez l’opérateur par **Inférieur ou égal à**, puis activez l’option **Définir la date relative** sur **ACTIVÉ**.
   1. Saisissez _$$TODAYem_ dans la zone de texte.

      ![Exemple de filtre de graphique de révisions](assets/revision-chart-filter-2.png)
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.

## Ajouter des informations de révision et d’approbation détaillées avec les tableaux

Pour plus d&#39;informations sur la création d&#39;un rapport tabulaire, voir [Créer un rapport tabulaire](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

![exemple de tableau](assets/table-dashboard.png)

### Liste des validations en attente

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans l’angle supérieur droit de la page des détails du tableau de bord, cliquez sur **Ajouter un rapport**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **Tableau**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Saisissez _Approbations en attente_ dans le champ **Nom**.
   1. Saisissez une description dans le champ **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.

1. Pour configurer la section **Créer une table**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Colonnes du tableau** ![Icône Colonnes du tableau](assets/drilldown-column.png).
   1. Cliquez sur **Ajouter une colonne**.
   1. Faites défiler vers le bas et sélectionnez **Approbations de documents** > **Statut**.
   1. Ajoutez les colonnes suivantes :

   <table>
    <tr>
    <td><strong>Nom du projet</strong></td>
    <td>Version du document &gt; Document &gt; Projet &gt; Nom</td>
    </tr>
    <tr>
    <td><strong>Nom du document</strong></td>
    <td>Version du document &gt; Document &gt; saisissez <em>Nom</em> dans la zone de recherche.</td>
    </tr>
    <tr>
    <td><strong>Version du document</strong></td>
    <td>Version Du Document &gt; Document &gt; Version</td>
    </tr>
    <tr>
    <td><strong>Échéance</strong></td>
    <td>Approbation du document &gt; Étape d’approbation &gt; Échéance</td>
    </tr>
    <tr>
    <td><strong>Demandé par</strong></td>
    <td>Approbation du document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Demandeur &gt; saisissez <em>Nom</em> dans la zone de recherche.</td>
    </tr>
    <tr>
    <td><strong>Date demandée</strong></td>
    <td>Approbation du document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Créé le</td>
    </tr>
    <tr>
    <td><strong>Approbateur</strong></td>
    <td>Approbation du document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Utilisateur participant &gt; saisissez <em>Nom</em> dans la zone de recherche.</td>
    </tr>
    </table>


   *Les participants à l&#39;étape d&#39;approbation sont tronqués à _Pa étape d&#39;approbation_.


1. Pour configurer la section **Filtre**, procédez comme suit :
   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![icône de l’onglet Filtrer](assets/filter-tab.png).
   1. Cliquez sur **Modifier le filtre**, puis **Ajouter une condition**.
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Statut**.
   1. Remplacez l’opérateur par **Égal**, puis saisissez _en attente d’approbation_ dans la zone de texte.

      ![exemple de filtre de table d&#39;approbation en attente](assets/pending-approval-table-filter.png)
   1. (Facultatif) Ajoutez des filtres supplémentaires comme décrit dans la section **Filtres facultatifs** ci-dessous.
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.


**Filtres facultatifs**

Pour afficher des informations plus spécifiques en fonction de votre cas d’utilisation, vous pouvez ajouter des conditions de filtre supplémentaires. Vous pouvez recréer le tableau et ajouter de nouvelles conditions de filtrage par cas d’utilisation.

+++ Développer pour afficher des options de filtre supplémentaires

**Mes projets**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Version du document** > **Document** > **Projet** > **Propriétaire** > saisissez _Nom_ dans la zone de recherche.
   1. Remplacez l’opérateur par **Égal**, puis choisissez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront où vous êtes marqué comme propriétaire du projet.

      ![exemple de filtre de table d&#39;approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.

**Approbations que j&#39;ai envoyées**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Étape d’approbation** > **Participants à l’étape d’approbation** > **Demandeur** > saisissez _Nom_ dans la zone de recherche.
   1. Remplacez l’opérateur par **Égal**, puis choisissez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront où vous êtes marqué comme propriétaire du projet.

      ![exemple de filtre de table d&#39;approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.

+++

### Liste des approbations échues

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.

1. Dans l’angle supérieur droit de la page des détails du tableau de bord, cliquez sur **Ajouter un rapport**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **Tableau**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Saisissez _Approbations en retard_ dans le champ **Nom**.
   1. (Facultatif) Saisissez une description dans le champ **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.

1. Pour configurer la section **Créer une table**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Colonnes du tableau** ![Icône Colonnes du tableau](assets/drilldown-column.png).
   1. Cliquez sur **Ajouter une colonne**.
   1. Faites défiler vers le bas et sélectionnez **Approbations de documents** > **Statut**.
   1. Ajoutez les colonnes suivantes :

      <table>
        <tr>
        <td><strong>Nom du projet</strong></td>
        <td>Version du document &gt; Document &gt; Projet &gt; Nom</td>
        </tr>
        <tr>
        <td><strong>Nom du document</strong></td>
        <td>Version du document &gt; Document &gt; saisissez <em>Nom</em> dans la zone de recherche.</td>
        </tr>
        <tr>
        <td><strong>Version du document</strong></td>
        <td>Version Du Document &gt; Document &gt; Version</td>
        </tr>
        <tr>
        <td><strong>Échéance</strong></td>
        <td>Document &gt; Étape d’approbation &gt; Échéance</td>
        </tr>
        <tr>
        <td><strong>Demandé par</strong></td>
        <td>Document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Demandeur &gt; saisissez <em>Nom</em> dans la zone de recherche.</td>
        </tr>
        <tr>
        <td><strong>Date demandée</strong></td>
        <td>Document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Créé à</td>
        </tr>
        <tr>
        <td><strong>Approbateur</strong></td>
        <td>Document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Utilisateur participant &gt; saisissez <em>Nom</em> dans la zone de recherche.</td>
        </tr>
        </table>

      *Les participants à l&#39;étape d&#39;approbation sont tronqués à _Pa étape d&#39;approbation_.

1. Pour configurer la section **Filtre**, procédez comme suit :
   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![icône de l’onglet Filtrer](assets/filter-tab.png).
   1. Cliquez sur **Modifier le filtre**, puis **Ajouter une condition**.
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Étape d’approbation** > **Échéance**.
   1. Remplacez l’opérateur par **Inférieur à**, puis activez le bouton (bascule) **Définir la date relative** sur **ACTIVÉ**.
   1. Saisissez _$$TODAY_ dans le champ de texte.

      ![exemple de filtre de table des approbations échues](assets/overdue-approval.png)
   1. (Facultatif) Ajoutez des filtres supplémentaires comme décrit dans la section **Filtres facultatifs** ci-dessous.
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.



**Filtres facultatifs**

Pour afficher des informations plus spécifiques en fonction de votre cas d’utilisation, vous pouvez ajouter des conditions de filtre supplémentaires. Vous pouvez recréer le tableau et ajouter de nouvelles conditions de filtre facultatives par cas d’utilisation.

+++ Développer pour afficher des options de filtre supplémentaires

**Mes projets**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Version du document** > **Document** > **Projet** > **Propriétaire** > saisissez _Nom_ dans la zone de recherche.
   1. Remplacez l’opérateur par **Égal**, puis choisissez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront dans lesquels vous êtes marqué comme propriétaire du projet.

      ![exemple de filtre de table d&#39;approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.

**Approbations que j&#39;ai envoyées**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Étape d’approbation** > **Participants à l’étape d’approbation** > **Demandeur** > saisissez _Nom_ dans la zone de recherche.
   1. Remplacez l’opérateur par **Égal**, puis choisissez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront dans lesquels vous êtes marqué comme propriétaire du projet.

      ![exemple de filtre de table d&#39;approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.

**Mon équipe**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Étape d’approbation** > **Participants à l’étape d’approbation** > **Équipe de participants** > saisissez _Nom_ dans la zone de recherche.
   1. Remplacez l’opérateur par **Égal**, puis choisissez **Mes équipes par défaut (Utilisateur connecté)** ou **Mes autres équipes (Utilisateur connecté)** pour afficher les projets affectés à votre équipe par défaut ou aux autres équipes auxquelles vous appartenez.

      ![exemple de filtre de table d&#39;approbation en attente](assets/approvals-ive-submitted-filter.png)
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.
+++
