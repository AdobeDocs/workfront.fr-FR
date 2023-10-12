---
title: Activité de mise à jour Adobe Maestro
description: Utilisez Maestro pour créer des objets, champs et espaces de travail personnalisés.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '1519'
ht-degree: 0%

---

# Activité de mise à jour Adobe Maestro

>[!IMPORTANT]
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro/maestro-overview.md).

Cet article répertorie les fonctionnalités qui ont été publiées après le lancement du programme bêta fermé de Maestro, le 22 mai 2023.

Les fonctionnalités publiées sont répertoriées dans l’ordre dans lequel elles ont été publiées, avec la version la plus récente en premier. Les clients qui participent au programme bêta fermé Maestro peuvent accéder à toutes les fonctionnalités de leurs environnements Aperçu et Production.

>[!IMPORTANT]
>
>La documentation référencée dans les sections ci-dessous sera disponible une fois les fonctionnalités publiées dans Production.

Cette section répertorie les fonctionnalités et les correctifs qui ont été publiés après le lancement du programme bêta fermé de Maestro, le 22 mai 2023.

Les fonctionnalités sont publiées toutes les semaines et sont répertoriées dans l’ordre dans lequel elles ont été publiées, avec la version la plus récente en premier. Les clients qui participent au programme bêta fermé Maestro peuvent accéder à toutes les fonctionnalités de leurs environnements Aperçu et Production.

## Semaine du 9 octobre 2023

### Recherche dans la vue Tableau

Aperçu et production : 9 octobre 2023

Vous pouvez désormais rechercher un mot-clé pour trouver rapidement un enregistrement dans le mode Tableau. Vous pouvez utiliser des mots-clés et des caractères spéciaux dans n’importe quel champ visible à l’écran pour trouver un enregistrement. Pour plus d’informations, voir [Gestion de la vue de tableau](../maestro/views/manage-the-table-view.md).

<!--
***********WHICH WEEK IS THIS???***********

### New People field type 

Preview and production: ************ADD INFORMATION HERE***********

You can now add a People-type field to Maestro record types. You can use People-type fields to add existing users, job roles, or teams to a record. For information, see [Create fields](../maestro/architecture-and-fields/create-fields.md). 


### Rich Text- format for Paragraph fields

Preview and production: ************ADD INFORMATION HERE***********

We have added Rich Text format controls for Paragraph-type fields. For more information, see [Edit records](../maestro/records/edit-records.md). 

-->

## Semaine du 18 septembre 2023

### Réorganiser les lignes

Aperçu et production : 20 septembre 2023

Vous pouvez désormais réorganiser une ou plusieurs lignes (ou enregistrements) dans la vue Tableau d’une page de type enregistrement. Pour plus d’informations, voir [Gestion de la vue de tableau](../maestro/views/manage-the-table-view.md).

## Semaine du 4 septembre 2023

### Connexion des enregistrements Maestro aux entreprises et aux groupes Workfront

Aperçu et production : 5 septembre 2023

Vous pouvez désormais connecter un enregistrement Maestro à des entreprises et des groupes Workfront. Vous devez d’abord créer une connexion entre un type d’enregistrement Maestro et les types d’objets des sociétés et groupes Workfront. Vous pouvez ensuite connecter un seul enregistrement Maestro du type d’enregistrement sélectionné à des sociétés et groupes Workfront individuels.

Tenez compte des points suivants :

* Vous devez créer une connexion entre les types d’enregistrement Maestro et Workfront Company et les types d’objets Group pour chaque espace de travail.

* Vous ne pouvez pas connecter les types d’enregistrement de taxonomie aux types d’objets Workfront.

* Vous pouvez connecter plusieurs enregistrements Maestro au même groupe ou entreprise Workfront et plusieurs entreprises ou groupes au même enregistrement Maestro.

* Vous ne pouvez pas modifier des entreprises ou des groupes dans Maestro. Toutes les modifications de groupe ou d’entreprise effectuées dans Workfront sont visibles dans Maestro lors de la vérification des enregistrements liés à Maestro.

  Pour plus d’informations, voir les articles suivants :

   * [Connexion des types d’enregistrement](../maestro/architecture-and-fields/connect-record-types.md)
   * [Connexion d’enregistrements](../maestro/records/connect-records.md)

### Prise en charge des URL pour les champs de texte d’une seule ligne

Aperçu et production : 7 septembre 2023

Pour une meilleure visibilité lors de l’utilisation de liens dans la vue Tableau, nous avons ajouté la prise en charge des URL dans les champs de texte d’une seule ligne. En utilisant des URL vers d’autres sites web ou des lecteurs externes lors de la mise à jour d’un champ de texte d’une seule ligne, vous pouvez désormais les identifier comme des liens et cliquer dessus dans le tableau. Avant cette amélioration, les liens s’affichaient sous forme de texte.

## Semaine du 28 août 2023

### Menu de visibilité des champs de la barre d’outils Vue du tableau

Aperçu et production : 31 août 2023

Pour afficher les informations appropriées sur un ensemble donné d&#39;enregistrements, en particulier si vous avez l&#39;intention de partager la vue avec d&#39;autres personnes qui doivent voir certains champs d&#39;un type d&#39;enregistrement, mais pas tous, vous pouvez maintenant sélectionner les champs (ou colonnes) à afficher et ceux à masquer dans la vue Tableau.

Vous pouvez masquer ou afficher des champs individuels de chaque en-tête des colonnes de champs, ou vous pouvez gérer tous les champs du type d’enregistrement à partir d’un paramètre de la barre d’outils de la vue de tableau.

Pour plus d’informations, voir [Gestion de la vue de tableau](../maestro/views/manage-the-table-view.md).

## Semaine du 21 août 2023

### Connexion des enregistrements Maestro aux programmes et portefeuilles

Aperçu et production : 24 août 2023

Vous pouvez désormais connecter un enregistrement Maestro à des programmes et portefeuilles Workfront. Vous devez créer une connexion entre un type d’enregistrement Maestro et un programme ou un portfolio qui crée un champ connecté. Ensuite, vous pouvez connecter tout enregistrement Maestro de tous les autres types d’enregistrements du même espace de travail à des programmes et portefeuilles spécifiques, ce qui crée un programme Workfront en lecture seule ou un type d’enregistrement de Portfolio Workfront dans le même espace de travail. Tenez compte des points suivants :

* Les types d’enregistrement du connecteur Workfront sont uniques pour chaque espace de travail.
* Vous pouvez connecter plusieurs enregistrements Maestro au même programme ou portfolio Workfront, ainsi que plusieurs programmes et portefeuilles au même enregistrement Maestro.
* Vous ne pouvez pas modifier les programmes et les portefeuilles dans Maestro. Toutes les modifications de programme et de portefeuille effectuées dans Workfront sont visibles dans Maestro, lors de la vérification des enregistrements liés.

### Nouvelle fonctionnalité de tri pour la vue de tableau

Aperçu et production : 24 août 2023

Vous pouvez désormais trier les enregistrements dans la vue de tableau d’une page de type enregistrement.
Les fonctionnalités suivantes sont désormais disponibles :

* Tri au niveau du tableau, où vous pouvez trier simultanément plusieurs champs.
* Tri au niveau de la colonne ou du champ, où vous pouvez trier selon un champ individuel à la fois.

### Améliorations de la vue chronologique : nouvelle apparence pour les regroupements et basculement de vue standard/compacte

Aperçu et production : 24 août 2023

Les améliorations suivantes ont été apportées à la vue de la chronologie :

* Vous pouvez maintenant afficher la vue chronologique dans les modes suivants :

   * Standard : affiche les enregistrements dans des lignes distinctes.
   * Compact : affiche les enregistrements dont les dates ne se croisent pas sur la même ligne.

* Nous avons modifié l’aspect des lignes de groupement dans la vue de frise chronologique afin qu’elles s’affichent au-dessus de la frise chronologique des enregistrements qu’elles contiennent. Avant cette amélioration, les lignes de groupement s&#39;affichaient sur toute la longueur de la chronologie.

## Semaine du 14 août 2023

### Réorganiser les colonnes dans la vue de tableau

Vous pouvez désormais réorganiser les colonnes dans la vue Tableau Maestro. Tenez compte des points suivants lors de la réorganisation des colonnes :

* Le champ Nom est toujours le premier champ de la vue table d’une page de type enregistrement.

* Vous ne pouvez pas déplacer le champ Nom vers une autre position.

* Le champ Nom est figé et ne fait pas partie du défilement horizontal.

### Défilement horizontal pour la vue chronologique

Vous pouvez désormais faire défiler horizontalement dans la vue chronologique d’un type d’enregistrement.

## Semaine du 7 août 2023

### Importation de types d’enregistrement à partir d’un fichier Excel

Aperçu et production : 10 août 2023

Vous pouvez désormais importer un fichier Excel pour créer des types d’enregistrement dans un espace de travail. Les feuilles du fichier deviennent les types d’enregistrement et les colonnes du fichier deviennent leurs champs respectifs.

### Expérience améliorée pour la connexion des types d’enregistrement et des projets

Aperçu et production : 10 août 2023

Nous avons amélioré la manière dont vous connectez les types d’enregistrement, y compris la connexion aux projets Workfront. Dans le cadre de cette amélioration, nous avons apporté les modifications suivantes lors de l’ajout d’un champ pour un type d’enregistrement à partir de la vue de tableau :

* Suppression du champ Type de relation de l’onglet &quot;Nouveau champ&quot;.

* Ajoutez un onglet &quot;Nouvelle connexion&quot; dans lequel vous pouvez sélectionner directement l&#39;enregistrement ou le type d&#39;objet auquel vous souhaitez vous connecter, rendant ainsi inutile l&#39;utilisation d&#39;un champ de type Relation .

## Semaine du 10 juillet 2023

### Mettre à jour l’aspect d’un type d’enregistrement

Aperçu et production : 13 juillet 2023

Vous pouvez désormais sélectionner une icône personnalisée pour un type d’enregistrement et une couleur personnalisée pour l’icône de type d’enregistrement.

### Nouveau type de champ de case à cocher

Aperçu et production : 13 juillet 2023

Vous pouvez désormais ajouter un type de champ Case à cocher aux types d’enregistrement Maestro. Vous pouvez utiliser un champ de type Case à cocher pour ajouter une seule option de case à cocher à un enregistrement. Vous pouvez utiliser ce champ pour indiquer un attribut ou un état spécifique pour cet enregistrement. Par exemple, vous pouvez l’utiliser comme indicateur pour le suivi de la fin, de l’approbation ou de tout autre attribut binaire pour chaque enregistrement.

## Semaine du 26 juin 2023

### Activation rapide du menu contextuel dans un tableau

Aperçu et production : 28 juin 2023

Nous avons activé la possibilité d&#39;activer le menu contextuel en cliquant avec le bouton droit de la souris sur une ligne d&#39;enregistrement, lors de l&#39;affichage des enregistrements dans la vue Tableau ou dans un type d&#39;enregistrement. Vous pouvez désormais afficher, supprimer ou copier rapidement un lien vers la page Détails de l’enregistrement lorsque vous accédez au menu contextuel depuis n’importe quel emplacement de la vue de tableau d’un type d’enregistrement. Avant cette amélioration, le menu contextuel était accessible uniquement à partir du menu Plus dans la colonne Nom d’un enregistrement.

## Semaine du 19 juin 2023

### Les noms des champs d’enregistrement sont uniques.

Nous avons introduit une exigence maintenant que les noms de champ d’un type d’enregistrement Maestro doivent avoir des noms uniques. Les champs qui appartiennent à différents types d’enregistrements n’ont pas besoin de noms uniques.

## Semaine du 5 juin 2023

### Connexion d’enregistrements Maestro à des projets Workfront

Aperçu et production : 5 juin 2023

Vous pouvez désormais connecter un enregistrement Maestro à des projets Workfront. Vous devez créer un type d’enregistrement Connector Maestro pour établir la connexion entre les enregistrements Maestro et les projets Workfront. Vous pouvez ensuite connecter n’importe quel enregistrement Maestro de tous les autres types d’enregistrement à l’enregistrement du connecteur à l’aide du champ Relation . Tenez compte des points suivants :

* Vous devez disposer d’un type d’enregistrement de connecteur pour Workfront pour chaque espace de travail.
* Vous pouvez connecter plusieurs enregistrements Maestro au même projet Workfront et plusieurs projets au même enregistrement Maestro.
* Vous ne pouvez pas modifier de projets dans Maestro. Toutes les modifications de projet effectuées dans Workfront sont visibles dans Maestro, lors de la vérification des enregistrements liés.

## Semaine du 29 mai 2023

### Exigences de deux dates pour la création d’une vue de chronologie

Aperçu et production : 31 mai 2023

Pour créer une vue de chronologie, au moins deux champs de date doivent être associés à un type d’enregistrement.
