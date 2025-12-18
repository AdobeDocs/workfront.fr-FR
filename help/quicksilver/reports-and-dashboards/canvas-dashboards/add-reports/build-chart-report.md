---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Créer un rapport de graphique dans un tableau de bord de zones de travail
description: Vous pouvez ajouter à un tableau de bord de la zone de travail un rapport sous forme de graphique qui affiche vos données sous la forme d’un graphique à barres, à colonnes, en courbes ou en secteurs.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 4262cae8-602f-416d-94b9-409eb9d6241c
source-git-commit: bb65fa45f6fce762920627ad0fb6fd1d832f23a3
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 7%

---

# Créer un rapport de graphique dans un tableau de bord de zones de travail

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elles sont disponibles uniquement dans l’environnement de prévisualisation pour les clientes et les clients.</span>

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Il se peut que certaines parties de la fonction ne soient pas terminées ou ne fonctionnent pas comme prévu à cette étape. Veuillez soumettre tout commentaire concernant votre expérience en suivant les instructions de la section [Fournir un commentaire](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) de l’article de présentation de la version Beta des tableaux de bord de la zone de travail.<br>
>Si vous avez des commentaires concernant un bug ou un problème technique éventuel, envoyez un ticket à l’assistance Workfront. Pour plus d’informations, voir [Contacter le service clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Notez que cette version bêta n’est pas disponible sur les fournisseurs de cloud suivants :
>
>* Apporter votre propre clé pour Amazon Web Services
>* Azure
>* Google Cloud Platform

Vous pouvez créer et ajouter un rapport sous forme de graphique à un tableau de bord Zone de travail pour visualiser vos données sous la forme d’un graphique à barres, à colonnes, en courbes ou en secteurs.

![Rapport de graphique](assets/chart-report-main.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tous </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td> 
<p>Standard</p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurations des niveaux d’accès</p></td> 
   <td><p>Accès en modification aux rapports, aux tableaux de bord et aux calendriers</p>
  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Conditions préalables

Vous devez créer un tableau de bord avant de pouvoir créer un rapport de graphique.

## Créer un rapport de graphique dans un tableau de bord de zones de travail

De nombreuses options de configuration sont disponibles pour créer un rapport de graphique. Dans cette section, nous vous guiderons à travers le processus général de création d’un rapport.

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Cliquez sur **Nouveau tableau de bord** dans le coin supérieur droit.

1. Dans la zone **Créer un tableau de bord**, saisissez les **Nom** et **Description** du tableau de bord.

1. Cliquez sur **Créer**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **Graphique**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. (Facultatif) Suivez les étapes ci-dessous pour configurer la section **Détails** :

   1. Saisissez un rapport **Nom**.

   1. Saisissez un état **Description**.

   1. Si vous le souhaitez, décochez la case **Afficher la série supplémentaire en tant qu’« Autre »**.

      >[!NOTE]
      >
      >Vous pouvez afficher un nombre maximal de 60 séries dans un graphique. Lorsque cette case est cochée, toutes les séries au-dessus de la limite sont consolidées dans un regroupement **Autre** dans le graphique.
1. Choisissez le type de graphique à créer :
   * [Graphique à barres, en colonnes ou en courbes](#bar-column-or-line-chart)
   * [Graphique en secteurs](#pie-chart)

### Graphique à barres, en colonnes ou en courbes

>[!NOTE]
>
>Il peut y avoir d’autres champs en fonction du type de champ que vous sélectionnez. Les options décrites ci-dessous sont standard pour tous les types de champ.


1. Dans le panneau de gauche, cliquez sur l’icône **Créer un graphique** ![Créer un graphique](assets/build-chart-icon.png).

1. Dans la liste déroulante **Type de graphique**, sélectionnez **Barre**, **Colonne** ou **Ligne**.
1. Dans le deuxième menu déroulant, sélectionnez le type de barre, de colonne ou de ligne :
   * **Simple**
   * **Série multiple**
   * **Empilé**

1. Dans la section **Axe inférieur (X)**, sélectionnez le **Champ de mise à jour**, puis recherchez et sélectionnez le champ contenant les données qui seront résumées dans le graphique.
1. Dans la liste déroulante **Type d’agrégation**, sélectionnez la manière dont les données sont cumulées pour produire la sortie du graphique.
1. <span class="preview">(Facultatif) Ajoutez un libellé d’axe dans l’espace fourni.</span>
1. <span class="preview"> (Facultatif) Activez/désactivez le bouton (bascule) **Masquer l’axe**. </span>
1. <span class="preview">(Facultatif) Saisissez une **valeur de ligne de référence** pour définir une cible ou un seuil sur le graphique.</span>
1. Choisissez un **Type de ligne** dans le menu déroulant.
1. Sélectionnez le bouton **Mettre à jour le champ** sous la deuxième section, puis recherchez et sélectionnez le deuxième champ à afficher dans le graphique.


### Graphique en secteurs

>[!NOTE]
>
>Il peut y avoir d’autres champs en fonction du type de champ que vous sélectionnez. Les options décrites ci-dessous sont standard pour tous les types de champ.


1. Dans le panneau de gauche, cliquez sur l’icône **Créer un graphique** ![Créer un graphique](assets/build-chart-icon.png).

1. Dans la liste déroulante **Type de graphique**, sélectionnez **Barre**.
1. Dans la section **Mesure**, sélectionnez le **Champ de mise à jour**, puis recherchez et sélectionnez le champ qui contient les données qui seront résumées dans le graphique.
1. Dans la liste déroulante **Type d’agrégation**, sélectionnez la manière dont les données sont cumulées pour produire la sortie du graphique.
1. Dans la section **Segment**, sélectionnez le champ **Mettre à jour**, puis recherchez et sélectionnez le champ contenant les segments à afficher dans le graphique en secteurs.
1. <span class="preview"> (facultatif) Dans la section **circulaire**, activez l’option **Afficher les libellés de segment** pour afficher les libellés de segment.</span>
1. <span class="preview"> (Facultatif) Activez le bouton (bascule) **Afficher le total** pour afficher le total au milieu du graphique. Lorsque cette option est activée, il existe d’autres options pour afficher un libellé central et choisir le format de la valeur.</span>

>[!NOTE]
>
>Les types d&#39;agrégation se présentent comme suit :
>
>* Compter les types d’agrégation : la valeur centrale affichée est le nombre de tous les segments du graphique.
>* Types d’agrégation des sommes : la valeur centrale affichée est le total agrégé de la valeur numérique ou monétaire.
>* Types d’agrégation Moyenne, Max et Min : la valeur centrale affiche la valeur moyenne, maximale ou minimale en conséquence.

1. <span class="preview">(Facultatif) Dans la section Légende, activez l’option **Afficher la légende** pour afficher la légende du graphique.</span>

1. <span class="preview"> (Facultatif) Choisissez une **Position de la légende** dans le menu déroulant.</span>

## Configurer des paramètres de rapport de graphique supplémentaires

### Filtres

Pour configurer la section **Filtre**, procédez comme suit :

1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer**![&#x200B; Filtrer](assets/filter-icon.png).
1. Sélectionnez **Modifier le filtre**.
1. Cliquez sur **Ajouter une condition** puis spécifiez le champ à utiliser comme filtre et le modificateur qui définit le type de condition auquel le champ doit répondre.
1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OU.

### Paramètres d’exploration

Suivez les étapes ci-dessous pour configurer la section **Paramètres des colonnes d’analyse** :

1. Dans le panneau de gauche, cliquez sur l’icône **Colonnes d’analyse** ![Icône Colonnes d’analyse](assets/drilldown-column.png). Les champs de votre graphique s’affichent automatiquement sous forme de colonnes dans la section de prévisualisation à droite.

1. (Facultatif) Pour mettre à jour l’une des configurations de colonne existantes, sélectionnez la colonne à mettre à jour dans la section **Colonnes actives** puis mettez à jour les informations souhaitées (par exemple, le libellé, le statut lié et les conditions).

1. Cliquez sur **Ajouter une colonne** puis sélectionnez le champ à afficher en tant que colonne dans le tableau. Répétez ce processus pour chaque colonne à ajouter.

### Paramètres du groupe d&#39;analyse

Suivez les étapes ci-dessous pour configurer la section **Paramètres du groupe d’analyse** :

1. Dans le panneau de gauche, cliquez sur l’icône **Paramètres du groupe** ![Paramètres du groupe](assets/drilldown-group-icon.png).

1. Cliquez sur le bouton **Ajouter un regroupement** puis sélectionnez le champ à créer en tant que regroupement.

1. Cliquez sur **Enregistrer** pour créer le rapport et l’ajouter au tableau de bord.

## Création d’un exemple de rapport de graphique

Dans cette section, nous allons passer en revue les étapes pour créer un graphique à colonnes qui affiche les tâches en retard par propriétaire de projet.

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Cliquez sur **Nouveau tableau de bord** dans le coin supérieur droit.

1. Dans la zone **Créer un tableau de bord**, saisissez les **Nom** et **Description** du tableau de bord.

1. Cliquez sur **Créer**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **Graphique**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Saisissez un rapport **Nom** (par exemple *Tâches en retard par le propriétaire du projet*).

   1. Saisissez un état **Description**.

1. Pour configurer la section **Créer un graphique**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Créer un graphique**.

   1. Dans la liste déroulante **Type de graphique**, sélectionnez **Colonne**.

   1. Dans la liste déroulante **Type de colonne**, sélectionnez **Simple**.

   1. Sélectionnez le bouton **Mettre à jour le champ** sous la section **Axe inférieur (X)**, puis recherchez et sélectionnez le champ **Tâche** > **Projet** > **Propriétaire** > **Name**.

      ![Mettre à jour le champ](assets/bottom-x-axis.png)

   1. Cliquez sur le bouton **Sélectionner le champ** sous la section **Axe de gauche (Y)**, puis recherchez et sélectionnez le champ **Tâche** > **Nom**.

   1. Dans le menu déroulant **Type d’agrégation**, sélectionnez **Comptage**.

      ![Champ de type agrégation](assets/left-y-axis.png)

1. Pour configurer la section **Filtre**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer**.

   1. Sélectionnez **Modifier le filtre**.

   1. Cliquez sur **Ajouter une condition**.

   1. Cliquez dans la zone de condition vide, puis sélectionnez **Choisir un champ**.

   1. Sélectionnez le champ **Pourcentage terminé**.

   1. Dans le menu déroulant **Opérateurs**, sélectionnez **Inférieur à**, puis saisissez *100* dans le champ évaluateur.

   1. Cliquez sur **Ajouter une condition**, puis **Choisir un champ**.

   1. Sélectionnez le champ **Date d’achèvement prévue**.

   1. Dans le menu déroulant **Opérateurs**, sélectionnez **Inférieur à**.

   1. Basculez **Définir la date relative** sur **ACTIVÉ**.

   1. Saisissez *$$TODAY* dans le champ évaluateur.

      Pour plus d’informations sur les caractères génériques, consultez la section Variables de filtre de caractères génériques basés sur la date dans l’article [Modifier les filtres de rapport dans un tableau de bord Zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md).

      ![Champ évaluateur](assets/add-condition.png)

1. Suivez les étapes ci-dessous pour configurer la section **Paramètres des colonnes d’analyse** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Colonnes d’analyse** ![Colonnes d’analyse](assets/drilldown-column.png). Les champs de votre graphique s’affichent automatiquement sous forme de colonnes dans la section de prévisualisation à droite.

   1. Cliquez sur **Ajouter une colonne**, puis sélectionnez le champ **Affecté à** > **Nom**.

   1. Cliquez sur **Ajouter une colonne** puis sélectionnez le champ **Date de début prévue**.

   1. Cliquez sur **Ajouter une colonne**, puis sélectionnez le champ **Date d’achèvement prévue**.

   1. Cliquez sur **Ajouter une colonne** puis sélectionnez le champ **Date de la dernière mise à jour**.

   1. (Facultatif) Pour afficher l’heure de mise à jour, sélectionnez l’option **Date de la dernière mise à jour** dans le champ **Colonnes actuelles**, puis sélectionnez une option de valeur d’heure dans le menu déroulant **Format de date**.

1. Suivez les étapes ci-dessous pour configurer la section **Paramètres du groupe d’analyse** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Paramètres du groupe** ![Paramètres du groupe](assets/drilldown-group-icon.png).

   1. Cliquez sur le bouton **Ajouter un regroupement** puis sélectionnez le champ **Projet** > **Nom**.

1. Cliquez sur **Enregistrer** pour créer le rapport et l’ajouter au tableau de bord.

## Remarques concernant la création d’un rapport de graphique

### Utilisation du sélecteur de champ

La liste déroulante **Sections** de la section **Créer un graphique** est conçue pour limiter les choix d&#39;un sélecteur de champ afin de faciliter la recherche d&#39;un objet lors de la création d&#39;un rapport de tableau. Pour commencer, sélectionnez un objet d’entité de base.

* **Toutes les sections** : tous les types d’objet dans Workfront Workflow et Workfront Planning.
* **Objets Workfront** : objets de workflow Workfront natifs.
* **Types d’enregistrements Planning** : types d’enregistrements personnalisés définis dans Workfront Planning.

![Liste déroulante Sections](assets/sections-dropdown.png)

Une fois l’objet d’entité de base sélectionné, la liste déroulante **Sections** est mise à jour avec les options de type de champ applicables parmi lesquelles choisir.

* **Toutes les sections** : champs natifs, champs personnalisés et objets associés.
* **Tous les champs** : champs natifs et personnalisés (sans les relations).
* **Champs personnalisés** : champs définis par le client sur un formulaire personnalisé ou un enregistrement Planning.
* **Champs Workfront** : champs natifs uniquement.
* **Relations** : enregistrements connectés.

![Sélection d&#39;objets à déclarer](assets/reportable-objects-selection.png)

### Référencer des objets enfants

Les relations disponibles pour les colonnes supplémentaires, les options de filtre et les attributs de regroupement sont généralement limitées aux objets situés plus haut dans la hiérarchie d&#39;objets Workfront ou comportent une seule sélection sur l&#39;objet d&#39;entité de base du rapport. Il existe certaines exceptions à cette règle, notamment :

* Projet > Tâches
* Approbation de document > Étapes d&#39;approbation de document
* Étapes d&#39;approbation du document > Participants à l&#39;étape d&#39;approbation du document

Lors de l’utilisation de l’une des relations parent-enfant répertoriées ci-dessus, une ligne s’affiche dans le tableau pour chaque enregistrement enfant connecté à l’objet parent.