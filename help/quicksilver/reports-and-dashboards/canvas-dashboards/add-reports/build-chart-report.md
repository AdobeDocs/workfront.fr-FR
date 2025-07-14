---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Créer un rapport de graphique
description: Vous pouvez ajouter à un tableau de bord de la zone de travail un rapport sous forme de graphique qui affiche vos données sous la forme d’un graphique à barres, à colonnes, en courbes ou en secteurs.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 4262cae8-602f-416d-94b9-409eb9d6241c
source-git-commit: ba9256255905e139c281099555a6d129fc570984
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 6%

---

# Créer un rapport de graphique

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Pour plus d’informations, voir [Informations bêta sur les tableaux de bord de la zone de travail](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Vous pouvez créer et ajouter un rapport sous forme de graphique à un tableau de bord Zone de travail pour visualiser vos données sous la forme d’un graphique à barres, à colonnes, en courbes ou en secteurs.

![Rapport de graphique](assets/chart-report-main.png)

+++ Développez pour afficher les exigences d’accès.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront</p></td> 
   <td> 
<p>Tous </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td> 
<p>Actuelle : formule </p> 
<p>Nouveau : Standard</p> 
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
      >Un graphique peut afficher un nombre maximal de séries. Lorsque cette case est cochée, toutes les séries au-dessus de la limite sont consolidées dans un regroupement **Autre** dans le graphique.

1. Pour configurer la section **Créer un graphique**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Créer un graphique** ![Créer un graphique](assets/build-chart-icon.png).

   1. Dans la liste déroulante **Type de graphique**, sélectionnez le type de graphique à créer :

      * **Barre**
      * **Colonne**
      * **Ligne**
      * **Secteurs**

   1. Dans la liste déroulante **Type de colonne**, sélectionnez le type de colonne :
      * **Simple**
      * **Série multiple**
      * **Empilé**

   1. Sélectionnez le bouton **Mettre à jour le champ** dans la première section, puis recherchez et sélectionnez le champ contenant les données qui seront résumées dans le graphique.
   1. Dans la liste déroulante **Type d’agrégation**, sélectionnez la manière dont les données sont cumulées pour produire la sortie du graphique.

   1. Sélectionnez le bouton **Mettre à jour le champ** sous la deuxième section, puis recherchez et sélectionnez le deuxième champ à afficher dans le graphique.

1. Pour configurer la section **Filtre**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer**![ Filtrer](assets/filter-icon.png).
   1. Sélectionnez **Modifier le filtre**.
   1. Cliquez sur **Ajouter une condition** puis spécifiez le champ à utiliser comme filtre et le modificateur qui définit le type de condition auquel le champ doit répondre.
   1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OU.

1. Suivez les étapes ci-dessous pour configurer la section **Paramètres des colonnes d’analyse** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Colonnes d’analyse** ![Icône Colonnes d’analyse](assets/drilldown-column.png). Les champs de votre graphique s’affichent automatiquement sous forme de colonnes dans la section de prévisualisation à droite.

   1. (Facultatif) Pour mettre à jour l’une des configurations de colonne existantes, sélectionnez la colonne à mettre à jour dans la section **Colonnes actives** puis mettez à jour les informations souhaitées (par exemple, le libellé, le statut lié et les conditions).

   1. Cliquez sur **Ajouter une colonne** puis sélectionnez le champ à afficher en tant que colonne dans le tableau. Répétez ce processus pour chaque colonne à ajouter.

1. Suivez les étapes ci-dessous pour configurer la section **Paramètres du groupe d’analyse** :

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