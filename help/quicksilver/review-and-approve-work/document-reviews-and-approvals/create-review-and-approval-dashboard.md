---
product-area: documents
navigation-topic: approvals
title: Créer un tableau de bord de révision et d’approbation
description: Vous pouvez consulter les mesures d’approbation dans les Tableaux de bord de la zone de travail.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 48f8605b-c342-493b-96e7-f73248e34b35
source-git-commit: 9c86cf877e0d1bbb0c4700dfc362062028496e3c
workflow-type: tm+mt
source-wordcount: '1991'
ht-degree: 1%

---

# Créer un tableau de bord de rapports à réviser et à approuver

Vous pouvez créer un tableau de bord de rapports dans la zone Tableaux de bord de la zone de travail pour afficher des informations détaillées et de haut niveau sur les révisions et les approbations à l’aide de la nouvelle fonctionnalité d’approbation des documents.

>[!IMPORTANT]
>
>Cette fonctionnalité est disponible uniquement pour les clients qui utilisent le nouveau service d’approbation des documents et qui sont inscrits à la version Beta des tableaux de bord de la zone de travail.


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

Vous pouvez afficher des informations générales sur les approbations de documents avec des indicateurs clés de performance et des graphiques. Les informations détaillées ne sont actuellement pas disponibles dans la version bêta.

### KPI

![Exemples d’indicateurs de performance clés](assets/kpi-dashboard.png)

#### Approbations en attente

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **KPI**, cliquez sur **Ajouter**.
1. Saisissez _En attente_ dans la zone de texte **Titre de l’indicateur de performance clé**.
1. Tapez _Approbations en attente_ dans la zone de texte **Légende des indicateurs de performance clés**. Ce texte décrit l’affichage de l’indicateur de performance clé.
1. En haut de la page, cliquez sur **Sélectionner le champ de KPI**.
1. Faites défiler vers le bas et recherchez le **dossier Approbation du document**.
1. Choisissez **Statut**, puis sélectionnez **Nombre** dans le menu déroulant.
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition**.
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Statut**.
   1. Laissez l’opérateur sur **Égal** et saisissez _en attente de révision_ dans la zone de texte.
      ![exemple de filtre kpi en attente](assets/pending-kpi-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.


#### Approbations en retard

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **KPI**, cliquez sur **Ajouter**.
1. Saisissez _Overdue_ dans la zone de texte **Titre de l’indicateur de performance clé**.
1. Tapez _Échéance de l’étape d’approbation dans le passé_ dans la zone de texte **Légende des indicateurs de performance clés**. Ce texte décrit l’affichage de l’indicateur de performance clé.
1. En haut de la page, cliquez sur **Sélectionner le champ de KPI**.
1. Faites défiler vers le bas et recherchez le **dossier Approbation du document**.
1. Choisissez **Statut**, puis sélectionnez **Nombre** dans le menu déroulant.
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Échéance**.
   1. Remplacez l’opérateur par **Inférieur à**, puis activez Date relative sur, puis saisissez _$$TODAY_ dans la zone de texte.
      ![exemple de filtre kpi en retard](assets/overdue-kpi-filter.png)
1. Cliquez sur **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Statut**.
   1. Modifiez l’opérateur sur **Ne contient pas**, puis saisissez _approuvé_ dans la zone de texte.
      ![exemple 2 de filtre kpi en retard](assets/overdue-kpi-filter-2.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.


#### Validations terminées

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **KPI**, cliquez sur **Ajouter**.
1. Saisissez _Terminé_ dans la zone de texte **Titre de l’indicateur de performance clé**.
1. Saisissez _Nombre de statuts d’approbation_ dans la zone de texte **Légende des indicateurs de performance clés**. Ce texte décrit l’affichage de l’indicateur de performance clé.
1. En haut de la page, cliquez sur **Sélectionner le champ de KPI**.
1. Faites défiler vers le bas et recherchez le **dossier Approbation du document**.
1. Choisissez **Statut**, puis sélectionnez **Nombre** dans le menu déroulant.
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Statut**.
   1. Remplacez l’opérateur par **Contient** et saisissez _Approved_ dans la zone de texte.
      ![exemple de filtre kpi terminé](assets/completed-kpi-filter.png)
1. Cliquez sur **Ajouter une condition** :
   1. Cliquez sur **Et** pour le remplacer par **Ou**.
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Statut**.
   1. Remplacez l’opérateur par **Est égal à**, puis saisissez _Révisé_ dans la zone de texte.
      ![exemple de filtre kpi terminé](assets/completed-kpi-filter-2.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

#### Approbations abandonnées

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **KPI**, cliquez sur **Ajouter**.
1. Saisissez _Abandonné_ dans la zone de texte **Titre de l’indicateur de performance clé**.
1. Saisissez _Date limite de validation supérieure à 2 semaines_ dans la zone de texte **Légende des indicateurs de performance clés**. Ce texte décrit l’affichage de l’indicateur de performance clé.
1. En haut de la page, cliquez sur **Sélectionner le champ de KPI**.
1. Faites défiler vers le bas et recherchez le dossier **Étape d’approbation du document**.
1. Choisissez **Échéance**, puis sélectionnez **Comptage** dans le menu déroulant.
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Statut**.
   1. Modifiez l’opérateur sur **Ne contient pas** et saisissez _approuvé_ dans la zone de texte.
      ![exemple de filtre kpi abandonné](assets/abandoned-kpi-filter.png)
1. Cliquez sur **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Échéance**.
   1. Remplacez l’opérateur par **Inférieur à**, puis activez Date relative sur, puis saisissez _$$TODAY-2w_ dans la zone de texte.
      ![exemple de filtre kpi abandonné](assets/abandoned-kpi-filter-2.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

### Graphiques

![Exemples de graphiques](assets/chart-dashboard.png)

#### Graphique à barres Approbations par décision

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **Graphique**, cliquez sur **Ajouter**.
1. Saisissez _Validations par décision_ dans la zone de texte **Nom**.
1. (Facultatif) Saisissez une description dans la zone de texte **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.
1. Cliquez sur **Ouvrir les détails du graphique**.
1. Dans le menu déroulant **Type de graphique**, laissez l’option **Graphique à barres** sélectionnée.
1. Dans le menu déroulant **Type de barre**, laissez l’option **Simple** sélectionnée.
1. Cliquez sur **Mettre à jour le champ** pour l’**Axe inférieur (X)** et choisissez le premier dossier **Approbation du document** puis **Statut**.
1. Définissez le Type d’agrégation sur **Nombre**.
1. Cliquez sur **Mettre à jour le champ** pour l’axe **Gauche (Y)** et choisissez la première option **Approbation du document** puis **Statut**.
1. Cliquez sur l’onglet Filtre ![icône de l’onglet Filtre](assets/filter-tab.png).
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Version du document**.
   1. Remplacez l’opérateur par **N’est pas nul**.
      ![exemple de filtre](assets/approvals-by-decision-chart-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.


#### Graphique à barres Révisions

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **Graphique**, cliquez sur **Ajouter**.
1. Saisissez _Revisions_ dans la zone de texte **Nom**.
1. Tapez _Nombre de révisions des documents dont les décisions sont incomplètes et prévues avant la fin du mois_ dans la zone de texte **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.
1. Cliquez sur **Ouvrir les détails du graphique**.
1. Dans le menu déroulant **Type de graphique**, laissez l’option **Graphique à barres** sélectionnée.
1. Dans le menu déroulant **Type de barre**, laissez l’option **Simple** sélectionnée.
1. Cliquez sur **Mettre à jour le champ** pour l’**Axe inférieur (X)** et choisissez le premier dossier **Approbation du document** puis **Version du document** > **Version**.
1. Définissez le Type d’agrégation sur **Nombre**.
1. Cliquez sur **Mettre à jour le champ** pour l’axe **Gauche (Y)** et choisissez la première option **Approbation du document** puis **Version du document** > **Document** > **Name**.
1. Cliquez sur l’onglet Filtre ![icône de l’onglet Filtre](assets/filter-tab.png).
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Date de décision des participants à l’étape d’approbation**.
   1. Remplacez l’opérateur par **Est nul**.
      ![exemple de filtre de graphique de révisions](assets/revision-chart-filter.png)
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Date limite de l’étape d’approbation**.
   1. Remplacez l’opérateur par **Inférieur ou égal à**, puis activez l’option Définir la date relative sur et saisissez _$$TODAYem_ dans la zone de texte.
      ![exemple de filtre de graphique de révisions](assets/revision-chart-filter-2.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

## Ajouter des informations de révision et d’approbation détaillées avec les tableaux

![exemple de tableau](assets/table-dashboard.png)

### Liste des validations en attente

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte **Tableau**, cliquez sur **Ajouter**.
1. Saisissez _Approbations en attente_ dans la zone de texte **Nom**.
1. (Facultatif) Saisissez une description dans la zone de texte **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.
1. Cliquez sur **Ouvrir les paramètres de colonne**.
1. Cliquez sur **Ajouter une colonne**, faites défiler l’écran vers le bas et cliquez sur le premier dossier **Approbations de documents**, puis choisissez **Statut**.
1. Ajoutez les colonnes suivantes :

   <table>
    <tr>
    <td><strong>Nom du projet</strong></td>
    <td>Version du document &gt; Document &gt; Projet &gt; Nom</td>
    </tr>
    <tr>
    <td><strong>Nom du document</strong></td>
    <td>Version du document &gt; Document &gt; saisissez _Name_ dans la zone de recherche.</td>
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
    <td>Document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Demandeur &gt; saisissez _Name_ dans la zone de recherche.</td>
    </tr>
     <tr>
    <td><strong>Date demandée</strong></td>
    <td>Document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Créé à</td>
    </tr>
     <tr>
    <td><strong>Approbateur</strong></td>
    <td>Document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Utilisateur participant &gt; saisissez _Name_ dans la zone de recherche.</td>
    </tr>
    <table>

   *Les participants à l’étape d’approbation sont tronqués à la page de l’étape d’approbation.

1. Passez à [ Ajouter le filtre requis ci-dessous ](#add-the-required-filter).

#### Ajouter le filtre des validations en attente obligatoire

1. Cliquez sur l’onglet Filtre ![icône de l’onglet Filtre](assets/filter-tab.png).
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Statut**.
   1. Remplacez l’opérateur par **Égal**, puis saisissez _en attente d’approbation_.
      ![exemple de filtre de table d&#39;approbation en attente](assets/pending-approval-table-filter.png)
1. Ajoutez des filtres facultatifs comme décrit ci-dessous ou cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

**Filtres facultatifs**

Pour afficher des informations plus spécifiques en fonction de votre cas d’utilisation, vous pouvez ajouter des conditions de filtre supplémentaires. Vous pouvez recréer le tableau et ajouter de nouvelles conditions de filtrage par cas d’utilisation.

+++ Développer pour afficher des options de filtre supplémentaires

**Mes projets**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Version du document** > **Document** > **Projet** > **Propriétaire** > saisissez _Name_ dans la zone de recherche.
   1. Remplacez l’opérateur par **Égal**, puis choisissez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront dans lesquels vous êtes marqué comme propriétaire du projet.
      ![exemple de filtre de table d&#39;approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

**Approbations que j&#39;ai envoyées**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Étape d’approbation** > **Participants à l’étape d’approbation** > **Demandeur** > saisissez _Nom_ dans la zone de recherche.
   1. Remplacez l’opérateur par **Égal**, puis choisissez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront dans lesquels vous êtes marqué comme propriétaire du projet.
      ![exemple de filtre de table d&#39;approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

+++

### Liste des approbations échues

1. [Créez un tableau de bord](#create-a-dashboard) comme décrit dans la section ci-dessus.
1. Dans la carte Tableau , cliquez sur **Ajouter**.
1. Saisissez _Approbations en retard_ dans la zone de texte **Nom**.
1. (Facultatif) Saisissez une description dans la zone de texte **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.
1. Cliquez sur **Ouvrir les paramètres de colonne**.
1. Cliquez sur **Ajouter une colonne**, faites défiler l’écran vers le bas et cliquez sur le premier dossier **Approbations de documents**, puis choisissez **Statut**.
1. Ajoutez les colonnes suivantes :

   <table>
    <tr>
    <td><strong>Nom du projet</strong></td>
    <td>Version du document &gt; Document &gt; Projet &gt; Nom</td>
    </tr>
    <tr>
    <td><strong>Nom du document</strong></td>
    <td>Version du document &gt; Document &gt; saisissez _Name_ dans la zone de recherche.</td>
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
    <td>Document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Demandeur &gt; saisissez _Name_ dans la zone de recherche.</td>
    </tr>
     <tr>
    <td><strong>Date demandée</strong></td>
    <td>Document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Créé à</td>
    </tr>
     <tr>
    <td><strong>Approbateur</strong></td>
    <td>Document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Utilisateur participant &gt; saisissez _Name_ dans la zone de recherche.</td>
    </tr>
    <table>

   *Les participants à l’étape d’approbation sont tronqués à la page de l’étape d’approbation.

1. Passez à [ Ajouter le filtre requis ci-dessous ](#add-the-required-filter-1).

#### Ajouter le filtre des approbations en retard obligatoire

1. Cliquez sur l’onglet Filtre ![icône de l’onglet Filtre](assets/filter-tab.png).
1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Étape d&#39;approbation** > **Échéance**.
   1. Remplacez l’opérateur par **Inférieur à**, activez le bouton (bascule) **Définir la date relative** puis saisissez _$$TODAY_.
      ![exemple de filtre de table des approbations échues](assets/overdue-approval.png)
1. Ajoutez des filtres facultatifs comme décrit ci-dessous ou cliquez sur **Terminé** dans le coin supérieur droit de l’écran.


**Filtres facultatifs**

Pour afficher des informations plus spécifiques en fonction de votre cas d’utilisation, vous pouvez ajouter des conditions de filtre supplémentaires. Vous pouvez recréer le tableau et ajouter de nouvelles conditions de filtre facultatives par cas d’utilisation.

+++ Développer pour afficher des options de filtre supplémentaires

**Mes projets**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Version du document** > **Document** > **Projet** > **Propriétaire** > saisissez _Name_ dans la zone de recherche.
   1. Remplacez l’opérateur par **Égal**, puis choisissez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront dans lesquels vous êtes marqué comme propriétaire du projet.
      ![exemple de filtre de table d&#39;approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

**Approbations que j&#39;ai envoyées**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Étape d’approbation** > **Participants à l’étape d’approbation** > **Demandeur** > saisissez _Nom_ dans la zone de recherche.
   1. Remplacez l’opérateur par **Égal**, puis choisissez **Moi (utilisateur connecté)** pour afficher les projets dans Workfront dans lesquels vous êtes marqué comme propriétaire du projet.
      ![exemple de filtre de table d&#39;approbation en attente](assets/pending-approvals-my-project-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.

**Mon équipe**

1. Cliquez sur **Modifier le filtre** > **Ajouter une condition** :
   1. Cliquez dans le filtre de condition vide, cliquez sur **Choisir un champ**, puis choisissez **Étape d’approbation** > **Participants à l’étape d’approbation** > **Équipe de participants** > saisissez _Nom_ dans la zone de recherche.
   1. Remplacez l’opérateur par **Égal**, puis choisissez **Mes équipes par défaut (Utilisateur connecté)** ou **Mes autres équipes (Utilisateur connecté)** pour afficher les projets affectés à votre équipe par défaut ou aux autres équipes auxquelles vous appartenez.
      ![exemple de filtre de table d&#39;approbation en attente](assets/approvals-ive-submitted-filter.png)
1. Cliquez sur **Terminé** dans le coin supérieur droit de l’écran.
+++
