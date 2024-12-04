---
product-area: documents
navigation-topic: approvals
title: Créer un tableau de bord de révision et d’approbation
description: Vous pouvez consulter les mesures de validation dans les tableaux de bord de la zone de travail.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 48f8605b-c342-493b-96e7-f73248e34b35
source-git-commit: 53db0a80026d003250e3b31063fb9a502d2ddce1
workflow-type: tm+mt
source-wordcount: '2054'
ht-degree: 1%

---

# Créer un tableau de bord de rapport pour révision et approbation

Vous pouvez créer un tableau de bord de rapport dans la zone Tableaux de bord de la zone de travail afin d’afficher des informations détaillées et de haut niveau sur les révisions et validations avec la nouvelle fonctionnalité de validation des documents.

>[!IMPORTANT]
>
>Cette fonctionnalité est disponible uniquement pour les clients qui utilisent le nouveau service d’approbation de document et qui sont inscrits à la version bêta de Tableaux de bord de canevas .


![exemple de tableau de bord](assets/whole-dashboard.png)

## Créer un tableau de bord

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.
1. Cliquez sur **Nouveau tableau de bord**.
1. Nommez votre tableau de bord.
1. (Facultatif) Ajoutez une description.
1. Cliquez sur **Créer**.
   ![ Ajoutez le nom et la description du tableau de bord ](assets/create-a-dashboard.png)

Une fois que vous avez créé un tableau de bord, vous pouvez commencer à ajouter des indicateurs de performance clés, des tableaux et des tableaux. Pour plus d’informations, reportez-vous aux sections suivantes :

* [Ajout d’informations de révision et d’approbation de haut niveau à l’aide des IPC et des tableaux](#add-high-level-review-and-approval-information-with-kpis-and-charts)
* [Ajout d’informations détaillées de révision et d’approbation à l’aide de tableaux](#add-detailed-review-and-approval-information-with-tables)

## Ajout d’informations de révision et d’approbation de haut niveau à l’aide des IPC et des tableaux

Vous pouvez afficher des informations de haut niveau sur les approbations de documents avec des indicateurs de performance clés et des graphiques. Les informations de zoom avant ne sont actuellement pas disponibles en version bêta.

### KPI

>[!IMPORTANT]
>
>Les nouvelles données d&#39;approbation de documents sont actuellement actualisées le soir dans le fuseau horaire de la montagne américaine. Des mises à jour en temps réel sont prévues et seront bientôt disponibles.

![Exemples de KPI](assets/kpi-dashboard.png)

#### Approbations en attente

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **KPI**, cliquez sur **Ajouter**.
1. Saisissez _En attente_ dans la zone de texte **KPI Title**.
1. Saisissez _Validations en attente_ dans la zone de texte **Légende IPC**. Ce texte décrit les indicateurs de performance clés affichés.
1. En haut de la page, cliquez sur **Sélectionner le champ IPC**.
1. Faites défiler l’écran vers le bas et recherchez le **dossier d’approbation de document**.
1. Sélectionnez **Status**, puis **Count** dans le menu déroulant.
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition**.
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **État**.
   1. Laissez l’opérateur **Equal** et saisissez _pending review_ dans la zone de texte.
      ![Exemple de filtre de kpi en attente](assets/pending-kpi-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.


#### Approbations en retard

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **KPI**, cliquez sur **Ajouter**.
1. Saisissez _Overdue_ dans la zone de texte **KPI Title**.
1. Saisissez _Approval Stage Deadline in the Past_ dans la zone de texte **KPI Caption**. Ce texte décrit les indicateurs de performance clés affichés.
1. En haut de la page, cliquez sur **Sélectionner le champ IPC**.
1. Faites défiler l’écran vers le bas et recherchez le **dossier d’approbation de document**.
1. Sélectionnez **Status**, puis **Count** dans le menu déroulant.
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **Date limite**.
   1. Définissez l’opérateur sur **Inférieur à** et activez la date Relative, puis saisissez _$$TODAY_ dans la zone de texte.
      ![exemple de filtre de Kpi en retard](assets/overdue-kpi-filter.png)
1. Cliquez sur **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **État**.
   1. Définissez l’opérateur sur **Not Contains**, puis saisissez _approved_ dans la zone de texte.
      ![exemple de filtre Kpi en retard 2](assets/overdue-kpi-filter-2.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.


#### Approbation terminée

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **KPI**, cliquez sur **Ajouter**.
1. Saisissez _Completed_ dans la zone de texte **KPI Title**.
1. Saisissez _Approval Status Count_ dans la zone de texte **KPI Caption**. Ce texte décrit les indicateurs de performance clés affichés.
1. En haut de la page, cliquez sur **Sélectionner le champ IPC**.
1. Faites défiler l’écran vers le bas et recherchez le **dossier d’approbation de document**.
1. Sélectionnez **Status**, puis **Count** dans le menu déroulant.
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **État**.
   1. Définissez l’opérateur sur **Contains**, puis saisissez _approved_ dans la zone de texte.
      ![exemple de filtre de kpi terminé](assets/completed-kpi-filter.png)
1. Cliquez sur **Ajouter une condition** :
   1. Cliquez sur **And** pour le remplacer par **Or**.
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **État**.
   1. Définissez l’opérateur sur **Equals**, puis saisissez _review_ dans la zone de texte.
      ![exemple de filtre de kpi terminé](assets/completed-kpi-filter-2.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

#### Approbation abandonnée

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **KPI**, cliquez sur **Ajouter**.
1. Saisissez _Abandonné_ dans la zone de texte **KPI Title**.
1. Saisissez _Délai d’approbation de plus de 2 semaines au-delà_ dans la zone de texte **Légende KPI** . Ce texte décrit les indicateurs de performance clés affichés.
1. En haut de la page, cliquez sur **Sélectionner le champ IPC**.
1. Faites défiler l’écran vers le bas et recherchez le dossier **Document Approval Stage**.
1. Sélectionnez **Deadline**, puis **Count** dans le menu déroulant.
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **État**.
   1. Définissez l’opérateur sur **Not Contains**, puis saisissez _approved_ dans la zone de texte.
      ![exemple de filtre de kpi abandonné](assets/abandoned-kpi-filter.png)
1. Cliquez sur **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **Date limite**.
   1. Définissez l’opérateur sur **Inférieur à**, activez la date Relative, puis saisissez _$$TODAY-2w_ dans la zone de texte.
      ![exemple de filtre de kpi abandonné](assets/abandoned-kpi-filter-2.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

### Graphiques

>[!IMPORTANT]
>
>Les nouvelles données d&#39;approbation de documents sont actuellement actualisées le soir dans le fuseau horaire de la montagne américaine. Des mises à jour en temps réel sont prévues et seront bientôt disponibles.

![Exemples de graphiques](assets/chart-dashboard.png)

#### Approbations par graphique à barres de décision

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **Chart**, cliquez sur **Add**.
1. Saisissez _Validations par décision_ dans la zone de texte **Nom**.
1. (Facultatif) Saisissez une description dans la zone de texte **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.
1. Cliquez sur **Ouvrir les détails du graphique**.
1. Dans le menu déroulant **Type de graphique**, laissez le **graphique à barres** sélectionné.
1. Dans le menu déroulant **Type de barre**, laissez **Simple** sélectionné.
1. Cliquez sur **Mettre à jour le champ** pour l’axe **inférieur (X)**, puis sélectionnez le premier dossier **Approbation du document**, puis **État**.
1. Définissez le type Agrégation sur **Count**.
1. Cliquez sur **Mettre à jour le champ** pour l’axe **Gauche (Y)**, puis sélectionnez la première option **Approbation du document** et **État**.
1. Cliquez sur l’onglet Filtre ![icône de l’onglet de filtrage](assets/filter-tab.png).
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **Document Version**.
   1. Définissez l’opérateur sur **Is Not Null**.
      ![exemple de filtre](assets/approvals-by-decision-chart-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.


#### Graphique à barres de révisions

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **Chart**, cliquez sur **Add**.
1. Saisissez _Révisions_ dans la zone de texte **Nom**.
1. Saisissez _Nombre de révisions pour les documents avec des décisions incomplètes prévues avant la fin de ce mois_ dans la zone de texte **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.
1. Cliquez sur **Ouvrir les détails du graphique**.
1. Dans le menu déroulant **Type de graphique**, laissez le **graphique à barres** sélectionné.
1. Dans le menu déroulant **Type de barre**, laissez **Simple** sélectionné.
1. Cliquez sur **Mettre à jour le champ** pour l’axe **inférieur (X)**, puis sélectionnez le premier dossier **Approbation du document**, puis **Version du document** > **Version**.
1. Définissez le type Agrégation sur **Count**.
1. Cliquez sur **Mettre à jour le champ** pour l’axe **Gauche (Y)**, puis sélectionnez la première option **Approbation du document** , puis **Version du document** > **Document** > **Nom**.
1. Cliquez sur l’onglet Filtre ![icône de l’onglet de filtrage](assets/filter-tab.png).
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **Date de décision des participants à l’étape d’approbation**.
   1. Définissez l’opérateur sur **Is Null**.
      ![exemple de filtre de graphique de révisions](assets/revision-chart-filter.png)
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **Date limite d’évaluation d’approbation**.
   1. Définissez l’opérateur sur **Inférieur à ou égal à**, puis activez Définir la date relative activée et saisissez _$$TODAYem_ dans la zone de texte.
      ![exemple de filtre de graphique de révisions](assets/revision-chart-filter-2.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

## Ajout d’informations détaillées de révision et d’approbation à l’aide de tableaux

>[!IMPORTANT]
>
>Les nouvelles données d&#39;approbation de documents sont actuellement actualisées le soir dans le fuseau horaire de la montagne américaine. Des mises à jour en temps réel sont prévues et seront bientôt disponibles.

![exemple de table](assets/table-dashboard.png)

### Liste des validations en attente

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **Table**, cliquez sur **Ajouter**.
1. Saisissez _En attente d’approbation_ dans la zone de texte **Nom**.
1. (Facultatif) Saisissez une description dans la zone de texte **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.
1. Cliquez sur **Ouvrir les paramètres de colonne**.
1. Cliquez sur **Ajouter une colonne**, faites défiler l’écran vers le bas et cliquez sur le premier dossier **Approbations de document**, puis sélectionnez **État**.
1. Ajoutez les colonnes suivantes :

   <table>
    <tr>
    <td><strong>Nom du projet</strong></td>
    <td>Document Version &gt; Document &gt; Projet &gt; Nom</td>
    </tr>
    <tr>
    <td><strong>Nom du document</strong></td>
    <td>Document Version &gt; Document &gt; type _Name_ dans la zone de recherche.</td>
    </tr>
    <tr>
    <td><strong>Version du document</strong></td>
    <td>Document Version &gt; Document &gt; Version</td>
    </tr>
    <tr>
    <td><strong>Échéance</strong></td>
    <td>Document &gt; Etape d’approbation &gt; Date limite</td>
    </tr>
    <tr>
    <td><strong>Demandé par</strong></td>
    <td>Document &gt; Évaluation &gt; Participants à l’étape d’approbation* &gt; Demandeur &gt; type _Name_ dans la zone de recherche.</td>
    </tr>
     <tr>
    <td><strong>Date demandée</strong></td>
    <td>Document &gt; Phase d’approbation &gt; Participants à l’étape d’approbation* &gt; Créé à l’adresse</td>
    </tr>
     <tr>
    <td><strong>Approbateur</strong></td>
    <td>Document &gt; Évaluation &gt; Participants à l’étape d’approbation* &gt; Utilisateur participant &gt; type _Name_ dans la zone de recherche.</td>
    </tr>
    <table>

   *Les participants à l’étape d’approbation sont tronqués à l’étape d’approbation pa.

1. Continuez à [Ajouter le filtre requis sous](#add-the-required-filter).

#### Ajoutez le filtre des validations en attente requis.

1. Cliquez sur l’onglet Filtre ![icône de l’onglet de filtrage](assets/filter-tab.png).
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **État**.
   1. Définissez l’opérateur sur **Equal**, puis saisissez _pending approval_.
      ![Exemple de filtre de table d’approbation en attente](assets/pending-approval-table-filter.png)
1. Ajoutez des filtres facultatifs comme décrit ci-dessous ou cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

**Filtres facultatifs**

Pour afficher des informations plus spécifiques selon votre cas d’utilisation, vous pouvez ajouter des conditions de filtrage supplémentaires. Vous pouvez recréer le tableau et ajouter de nouvelles conditions de filtrage par cas d’utilisation.

+++ Développer pour afficher d’autres options de filtrage

**Mes projets**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **Document version** > **Document** > **Projet** > **Propriétaire** > saisissez _Nom_ dans la zone de recherche.
   1. Définissez l’opérateur sur **Egal**, puis sélectionnez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront dans lesquels vous êtes marqué comme propriétaire du projet.
      ![Exemple de filtre de table d’approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

**Approbations que j’ai envoyées**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **Évaluation** > **Participants à l’évaluation de l’approbation** > **Demandeur** > saisissez _Nom_ dans la zone de recherche.
   1. Définissez l’opérateur sur **Egal**, puis sélectionnez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront dans lesquels vous êtes marqué comme propriétaire du projet.
      ![Exemple de filtre de table d’approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

+++

### Liste des validations en retard

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte Table , cliquez sur **Ajouter**.
1. Saisissez _Overdue Approvals_ dans la zone de texte **Name**.
1. (Facultatif) Saisissez une description dans la zone de texte **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.
1. Cliquez sur **Ouvrir les paramètres de colonne**.
1. Cliquez sur **Ajouter une colonne**, faites défiler l’écran vers le bas et cliquez sur le premier dossier **Approbations de document**, puis sélectionnez **État**.
1. Ajoutez les colonnes suivantes :

   <table>
    <tr>
    <td><strong>Nom du projet</strong></td>
    <td>Document Version &gt; Document &gt; Projet &gt; Nom</td>
    </tr>
    <tr>
    <td><strong>Nom du document</strong></td>
    <td>Document Version &gt; Document &gt; type _Name_ dans la zone de recherche.</td>
    </tr>
    <tr>
    <td><strong>Version du document</strong></td>
    <td>Document Version &gt; Document &gt; Version</td>
    </tr>
    <tr>
    <td><strong>Échéance</strong></td>
    <td>Document &gt; Etape d’approbation &gt; Date limite</td>
    </tr>
    <tr>
    <td><strong>Demandé par</strong></td>
    <td>Document &gt; Évaluation &gt; Participants à l’étape d’approbation* &gt; Demandeur &gt; type _Name_ dans la zone de recherche.</td>
    </tr>
     <tr>
    <td><strong>Date demandée</strong></td>
    <td>Document &gt; Phase d’approbation &gt; Participants à l’étape d’approbation* &gt; Créé à l’adresse</td>
    </tr>
     <tr>
    <td><strong>Approbateur</strong></td>
    <td>Document &gt; Évaluation &gt; Participants à l’étape d’approbation* &gt; Utilisateur participant &gt; type _Name_ dans la zone de recherche.</td>
    </tr>
    <table>

   *Les participants à l’étape d’approbation sont tronqués à l’étape d’approbation pa.

1. Continuez à [Ajouter le filtre requis sous](#add-the-required-filter-1).

#### Ajoutez le filtre des approbations en retard requis.

1. Cliquez sur l’onglet Filtre ![icône de l’onglet de filtrage](assets/filter-tab.png).
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **Évaluation** > **Date limite**.
   1. Définissez l’opérateur sur **Inférieur à**, activez **Définir la date relative**, puis saisissez _$$TODAY_.
      ![exemple de filtre de table d’approbation en retard](assets/overdue-approval.png)
1. Ajoutez des filtres facultatifs comme décrit ci-dessous ou cliquez sur **Terminé** dans le coin supérieur droit de l’écran.


**Filtres facultatifs**

Pour afficher des informations plus spécifiques selon votre cas d’utilisation, vous pouvez ajouter des conditions de filtrage supplémentaires. Vous pouvez recréer le tableau et ajouter de nouvelles conditions de filtrage facultatives par cas d’utilisation.

+++ Développer pour afficher d’autres options de filtrage

**Mes projets**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **Document version** > **Document** > **Projet** > **Propriétaire** > saisissez _Nom_ dans la zone de recherche.
   1. Définissez l’opérateur sur **Egal**, puis sélectionnez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront dans lesquels vous êtes marqué comme propriétaire du projet.
      ![Exemple de filtre de table d’approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

**Approbations que j’ai envoyées**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Sélectionner un champ**, puis sélectionnez **Évaluation** > **Participants à l’évaluation de l’approbation** > **Demandeur** > saisissez _Nom_ dans la zone de recherche.
   1. Définissez l’opérateur sur **Egal**, puis sélectionnez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront dans lesquels vous êtes marqué comme propriétaire du projet.
      ![Exemple de filtre de table d’approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

**Mon équipe**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis sélectionnez **Étape d’approbation** > **Participants de l’étape d’approbation** > **Équipe de participant** > saisissez _Nom_ dans la zone de recherche.
   1. Définissez l’opérateur sur **Egal à**, puis sélectionnez **Mes équipes par défaut (utilisateur connecté)** ou **Mes autres équipes (utilisateur connecté)** pour afficher les projets affectés à votre équipe par défaut ou à d’autres équipes que vous utilisez.
      ![Exemple de filtre de table d’approbation en attente](assets/approvals-ive-submitted-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.
+++
