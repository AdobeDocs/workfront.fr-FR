---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Créer un rapport de tableau croisé dynamique dans un tableau de bord Zone de travail
description: Vous pouvez ajouter un rapport de tableau croisé dynamique à un tableau de bord Zone de travail pour afficher les totaux agrégés de vos données sous la forme d'un tableau.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 58c5f4a08b2083d7350c19b6c1d8383fa0dbb124
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 9%

---

# Créer un rapport de tableau croisé dynamique dans un tableau de bord Zone de travail

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Il se peut que certaines parties de la fonction ne soient pas terminées ou ne fonctionnent pas comme prévu à cette étape. Veuillez soumettre tout commentaire concernant votre expérience en suivant les instructions de la section [Fournir un commentaire](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) de l’article de présentation de la version Beta des tableaux de bord de la zone de travail.<br>
>Si vous avez des commentaires concernant un bug ou un problème technique éventuel, envoyez un ticket à l’assistance Workfront. Pour plus d’informations, consultez la section [Contacter l’assistance clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Notez que cette version bêta n’est pas disponible sur les fournisseurs de cloud suivants :
>
>* Apporter votre propre clé pour Amazon Web Services
>* Azure
>* Google Cloud Platform

Vous pouvez ajouter un rapport de tableau croisé dynamique à un tableau de bord Zone de travail pour afficher les totaux agrégés de vos données, tels que les sommes, les nombres et les moyennes, sous la forme d&#39;un tableau. Les tableaux croisés dynamiques sont utiles lors de la comparaison de plusieurs valeurs agrégées ou de décomptes par rapport à plusieurs dimensions.

![ Exemple de rapport de tableau croisé dynamique ](assets/pivot-table-example.png)

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

Vous devez créer un tableau de bord avant de pouvoir créer un rapport de tableau croisé dynamique. Pour plus d’informations, voir [Créer un tableau de bord Zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Créer un rapport de tableau croisé dynamique dans un tableau de bord Zone de travail

De nombreuses options de configuration sont disponibles pour créer un rapport de tableau croisé dynamique. Dans cette section, nous vous guiderons à travers le processus général de création d’un rapport.

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord de la zone de travail**, puis cliquez sur le nom du tableau de bord auquel vous souhaitez ajouter le rapport.

1. Cliquez sur **Ajouter un rapport** dans le coin supérieur droit de la page.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **Tableau croisé dynamique**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. (Facultatif) Suivez les étapes ci-dessous pour configurer la section **Détails** :

   1. Sélectionnez l’**Entité racine** pour le rapport.

      >[!NOTE]
      >
      > L&#39;entité racine définit l&#39;objet d&#39;où proviennent vos champs. Une fois sélectionné, chaque sélecteur de champ que vous utiliserez plus loin dans ce rapport commence par cet objet. Vous pouvez donc accéder directement au champ de votre choix.


   1. Saisissez un rapport **Nom**.

   1. Saisissez un état **Description**.

   1. (Facultatif) Dans le champ **Exécuter ce rapport avec les droits d&#39;accès de**, commencez à saisir le nom de l&#39;utilisateur dont vous souhaitez que le rapport utilise les autorisations, puis sélectionnez l&#39;utilisateur lorsqu&#39;il apparaît dans la liste. Lorsque vous configurez un rapport pour qu’il s’exécute en tant qu’autre utilisateur, toutes les visionneuses du tableau de bord voient les mêmes données, quel que soit leur propre niveau d’accès. Si vous ne sélectionnez pas d’utilisateur, chaque visionneuse voit les données en fonction de ses propres autorisations.

      >[!IMPORTANT]
      >
      >Si l’utilisateur sélectionné est désactivé ou perd l’accès aux espaces de travail ou aux types d’enregistrements appropriés, le rapport peut afficher des données incomplètes ou dont le rendu échoue.

1. Pour configurer la section **Mesures**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Afficher les mesures** ![Créer un KPI](assets/build-kpi-icon.png).

   1. Cliquez sur **Ajouter une mesure** puis sélectionnez le champ de votre choix. Le champ s’affiche sous forme de colonne dans la section de prévisualisation à droite.

      >[!NOTE]
      >
      > Une mesure (également appelée mesure) est un champ numérique que vous souhaitez additionner ou totaliser. Par exemple, vous pouvez additionner tous les coûts ou compter le nombre de tâches.


   1. Saisissez un **libellé de colonne**.

   1. Dans la liste déroulante **Type d’agrégation**, sélectionnez la manière dont les données sont cumulées pour ce champ. Les options de ce champ varient en fonction du type de champ que vous avez sélectionné.

   1. Répétez les deux étapes ci-dessus pour chaque mesure que vous souhaitez ajouter.

1. Pour configurer la section **Segments**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Segments** ![Icône de groupe d’analyse](assets/drilldown-group-icon.png).

   1. Cliquez sur **Ajouter un segment** puis sélectionnez le segment de votre choix. Le champ s’affiche sous forme de colonne dans la section de prévisualisation à droite.

      >[!NOTE]
      >
      >Un segment est la catégorie que vous utilisez pour regrouper vos données, comme le regroupement des tâches par statut ou par propriétaire. C’est ainsi que vos mesures sont triées et totalisées.


   1. Répétez les deux étapes ci-dessus pour ajouter jusqu’à 2 segments.

1. Pour configurer la section **Filtre**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![Icône Filtrer](assets/filter-icon.png).

   1. Sélectionnez **Modifier le filtre**.

   1. Cliquez sur **Ajouter une condition** puis spécifiez le champ à utiliser comme filtre et le modificateur qui définit le type de condition auquel le champ doit répondre.

   1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OU.

1. Suivez les étapes ci-dessous pour configurer la section **Paramètres des colonnes d’analyse** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Colonnes d’analyse** ![Icône Colonnes d’analyse](assets/drilldown-column.png).

   1. Cliquez sur **Ajouter une colonne** puis sélectionnez le champ à afficher en tant que colonne dans le tableau d&#39;analyse. Répétez ce processus pour chaque colonne à ajouter.

1. Cliquez sur **Enregistrer** pour créer le rapport et l’ajouter au tableau de bord.

## Exemple de rapport de tableau croisé dynamique

Dans cette section, nous allons passer en revue les étapes de création d&#39;un rapport de tableau croisé dynamique qui résume les données d&#39;achèvement d&#39;une tâche.

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord de la zone de travail**, puis cliquez sur le nom du tableau de bord auquel vous souhaitez ajouter le rapport.

1. Cliquez sur **Ajouter un rapport** dans le coin supérieur droit de la page.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **Tableau croisé dynamique**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Choisissez **Tâche** comme **Entité racine**.
   1. Tapez *heures prévues par rapport aux heures réelles par portefeuille et projet* dans le champ **Nom**.
   1. Saisissez une description dans le champ **Description**.

1. Pour configurer la section **Mesures**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Afficher les mesures** ![Créer un KPI](assets/build-kpi-icon.png).
   1. Cliquez sur **Ajouter une mesure**, puis sélectionnez **Nom**. Saisissez *Nombre de tâches* dans le champ **Libellé de colonne**. Dans le menu déroulant **Type d’agrégation**, sélectionnez **Comptage**.
   1. Cliquez sur **Ajouter une mesure** puis sélectionnez **Heures réelles**. Saisissez *Heures réelles* dans le champ **Libellé de colonne**. Dans le menu déroulant **Type d’agrégation**, sélectionnez **Somme**.
   1. Cliquez sur **Ajouter une mesure** puis sélectionnez **Heures prévues**. Saisissez *Nombre total d’heures prévues* dans le champ **Libellé de colonne**. Dans le menu déroulant **Type d’agrégation**, sélectionnez **Somme**.

1. Pour configurer la section **Segments**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Segments** ![Icône de groupe d’analyse](assets/drilldown-group-icon.png).
   1. Cliquez sur **Ajouter un segment**, puis sélectionnez **Projet** > **Portfolio** > **Nom**.
   1. Cliquez sur **Ajouter un segment**, puis sélectionnez **Projet** > **Nom**.

1. Pour configurer la section **Filtre**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![Icône Filtrer](assets/filter-icon.png).
   1. Sélectionnez **Modifier le filtre**, puis **Ajouter une condition**.
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Statut**.
   1. Remplacez l’opérateur par **Égal**, puis choisissez *en cours*.

1. Suivez les étapes ci-dessous pour configurer la section **Paramètres des colonnes d’analyse** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Colonnes d’analyse** ![Icône Colonnes d’analyse](assets/drilldown-column.png).
   1. Cliquez sur **Ajouter une colonne**, puis sélectionnez **Nom**.
   1. Cliquez sur **Ajouter une colonne**, puis sélectionnez **Affecté à** > **Nom**.
   1. Cliquez sur **Ajouter une colonne**, puis sélectionnez **Date d’achèvement prévue**.

1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.

## Remarques concernant la création d&#39;un rapport de tableau croisé dynamique

### Rapports avec des données financières

Les utilisateurs disposant d’un accès en affichage ou en modification aux données financières dans leur niveau d’accès verront toujours les données financières dans les visualisations du tableau de bord de la zone de travail, même si l’autorisation Afficher les données financières est supprimée au niveau de la tâche ou du projet.

* Les personnes ne disposant pas de droits d’accès aux données financières ne verront pas les données financières dans les rapports.
* Les personnes qui ne voient pas les données financières sont limitées aux documents qu’elles sont déjà autorisées à consulter (projets, tâches, problèmes, etc.). Elles ne verront pas les valeurs financières des documents auxquels elles ne peuvent pas accéder.
* Les personnes à l’origine des rapports doivent faire preuve de prudence lors de l’inclusion de données financières dans les tableaux de bord et bien vérifier avec qui elles partagent les tableaux de bord afin d’éviter tout accès involontaire.

Il s’agit d’une limite connue et nous prévoyons d’y remédier à l’avenir.

### Utilisation du sélecteur de champ

La liste déroulante **Sections** de la section **Créer un tableau croisé dynamique** est conçue pour limiter les choix d&#39;un sélecteur de champ afin de faciliter la recherche d&#39;un objet lors de la création d&#39;un rapport de tableau croisé dynamique. Pour commencer, sélectionnez un objet d’entité de base.

* **Toutes les sections** : tous les types d’objet dans Workfront et Workfront Planning.
* **Objets Workfront** : objets Workfront natifs.
* **Types d’enregistrements Planning** : types d’enregistrements personnalisés définis dans Workfront Planning.

![Liste déroulante Sections](assets/sections-dropdown.png)

Une fois l’objet d’entité de base sélectionné, la liste déroulante **Sections** est mise à jour avec les options de type de champ applicables parmi lesquelles choisir.

* **Toutes les sections** : champs natifs, champs personnalisés et objets associés.
* **Tous les champs** : champs natifs et personnalisés (sans les relations).
* **Champs personnalisés** : champs définis par le client sur un formulaire personnalisé ou un enregistrement Planning.
* **Champs Workfront** : champs natifs uniquement.
* **Relations** : enregistrements connectés.

![Sélection d&#39;objets à déclarer](assets/reportable-objects-selection.png)

### Référencer des objets associés

Nous limitons l’accès au choix des objets enfants en tant que segments d’un tableau croisé dynamique. Les options de segment peuvent être des attributs de l&#39;enregistrement lui-même ou d&#39;autres enregistrements associés qui ne représentent pas une relation 1:many ou plusieurs:many.

Nous limitons également l’accès au référencement de tout attribut parent ou enfant en tant que mesure afin de réduire le risque de double comptage ou de double synthèse des valeurs, ce qui entraîne une fausse représentation des données réelles.

