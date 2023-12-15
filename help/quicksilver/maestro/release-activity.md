---
title: Activité de mise à jour Adobe Maestro
description: Adobe Manager est actuellement disponible pour sélectionner des clients Workfront. Consultez souvent cet article pour en savoir plus sur les fonctionnalités récemment publiées pour Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 53911aa3-74fd-4747-9008-f86a521ffba6
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '2698'
ht-degree: 0%

---

# Activité de mise à jour Adobe Maestro

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe Workfront.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients. Vous devez être un client Workfront pour utiliser les fonctionnalités de Maestro.
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

<!--
## Week of November 27, 2023

### Maestro permissions for users and groups

Production: November 28, 2023

>[!IMPORTANT]
>
>This functionality is not yet available in Preview.

You can now share a workspace with users and groups. You can set their permissions to different levels, depending on what information they need to view or edit in a Maestro workspace. After you share permissions to a workspace, users have permissions to the record types, records, and fields in that space.

The following are the permissions levels for Maestro workspaces:  

* None: Users cannot access any workspaces in Maestro, even if the Maestro area is shared with them through a layout template. 

* View: Users can view workspaces that are shared with them. They can also view record types, and records from the shared workspace. 

* Contribute: Users can create, edit, or delete records in the workspace that is shared with them.  They cannot create or edit record types or workspaces ones shared with them.  

* Manage: Users can create, edit, and delete record types, records, and fields in workspaces that are shared with them. They cannot create workspaces.  

Only Workfront administrators can create, edit, or delete workspaces and all information associated with them.  

For more information, see [Grant access to Adobe Maestro](../maestro/access/grant-access.md) and [Overview of sharing permissions in Adobe Maestro](../maestro/access/sharing-permissions-overview.md). -->

## Semaine du 18 décembre 2023

### Mettre à jour le champ principal dans une vue de tableau d’un type d’enregistrement

Aperçu et production : 14 décembre 2023

Vous pouvez maintenant choisir le champ à afficher dans la première colonne d&#39;un tableau Maestro. Ce champ est désormais appelé champ principal.

Avant cette amélioration, le champ Nom d’un enregistrement s’affichait toujours dans la première colonne de la vue de tableau et ne pouvait pas être placé à un autre emplacement.

Avec cette amélioration, notez les points suivants :

* Par défaut, la colonne ou le champ Nom est toujours la première colonne d’un tableau.

* Vous pouvez choisir n’importe quel champ des types suivants comme champ principal et remplacer le champ Nom dans la première colonne :

   * Texte à une ligne

   * Nombre

   * Formule

     >[!NOTE]
     >
     >Les champs de type Formule seront publiés ultérieurement.

* Le champ principal d’une vue de tableau est toujours gelé et ne peut pas être déplacé, sauf si vous définissez un autre champ comme champ principal.

* Vous pouvez modifier le champ principal à partir d’un en-tête de colonne non principal.

* Toutes les tables vues d’un type d’enregistrement possèdent le même champ principal que celui sélectionné.

Pour plus d’informations, voir [Gestion du mode Tableau](/help/quicksilver/maestro/views/manage-the-table-view.md).


### Connexion des enregistrements Maestro à Adobe Experience Manager Assets

Version d’aperçu : 14 décembre 2023

Version de production : 15 décembre 2023

>[!IMPORTANT]
>
>L’instance de Workfront de votre entreprise doit être intégrée à Adobe Business Platform ou à Adobe Admin Console pour pouvoir connecter les enregistrements Maestro à Adobe Experience Manager Assets.
>
>Si vous avez des questions sur l’intégration à Adobe Admin Console, reportez-vous à la section [FAQ sur l’expérience unifiée Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).


Vous pouvez maintenant établir une connexion entre les types d’enregistrements Maestro et Adobe Experience Manager Assets.

Une fois la connexion établie, les fonctionnalités suivantes sont disponibles avec cette mise à jour :

* Vous pouvez lier des ressources et des dossiers Experience Manager à un enregistrement Maestro à partir d’un référentiel spécifique dans Experience Manager Assets auquel ils ont accès. Vous pouvez connecter les champs de ressource aux champs Maestro dans ce processus.

* Les utilisateurs de Maestro peuvent afficher le nom des ressources connectées, ainsi que les valeurs des champs connectés dans Maestro.

<!--removed per PM, for now: 
* An Experience Manager Assets record type is automatically created in Maestro after you establish the connection. Connected assets are visible in the Maestro table and timeline views of this new record type.  
-->

* Vous pouvez cliquer sur le nom de la ressource dans la vue de tableau de l’enregistrement Maestro à partir du champ d’enregistrement connecté, puis afficher une fenêtre contextuelle avec la miniature de la ressource et plusieurs champs clés. Dans la fenêtre contextuelle, vous pouvez accéder à la visionneuse de ressources dans Experience Manager et en afficher tous les détails.

Pour plus d’informations, voir [Connexion des types d’enregistrement](/help/quicksilver/maestro/architecture/connect-record-types.md).

## Semaine du 4 décembre 2023

### Copiez et collez des informations d’un champ vers un autre dans la vue Tableau Maestro pour les champs d’enregistrement de type Personnes et liés.

Aperçu et production : 5 décembre 2023

Vous pouvez désormais copier et coller des informations d’un champ vers un autre de même type dans une vue de tableau de type Enregistrement Maestro. Cette fonctionnalité est désormais prise en charge pour les types de champs suivants :

* Personnes
* Champs d’enregistrement liés

Tenez compte des points suivants :

* La copie et le collage de valeurs de champ d’un champ à un autre sont pris en charge pour les champs qui affichent plusieurs valeurs.

* Vous ne pouvez pas copier des informations provenant d’une autre source, autre qu’un champ Maestro du même type que le champ dans lequel vous collez les informations.

* Vous ne pouvez pas copier et coller des valeurs de champ pour les champs qui s’affichent dans la zone Détails d’un enregistrement.

Pour plus d’informations, voir [Modifier des enregistrements](../maestro/records/edit-records.md).

Pour plus d’informations sur les champs liés, voir [Connexion des types d’enregistrement](../maestro/architecture/connect-record-types.md).

## Semaine du 27 novembre 2023

### Copier et coller des informations d’un champ vers un autre dans la vue Tableau Maestro

Aperçu et production : 28 novembre 2023

Vous pouvez désormais copier et coller des informations d’un champ vers un autre de même type dans une vue de tableau de type Enregistrement Maestro.

Tenez compte des points suivants :

* Vous ne pouvez pas copier des informations provenant d’une autre source, autre qu’un champ Maestro du même type que le champ dans lequel vous collez les informations.

* Vous ne pouvez pas copier et coller des valeurs de champ pour les champs qui s’affichent dans la zone Détails d’un enregistrement.

* Vous ne pouvez pas copier et coller des valeurs de champ pour les types de champ suivants :

   * Personnes

   * Champs système

   * Champs liés créés suite à la connexion des enregistrements

Pour plus d’informations, voir [Modifier des enregistrements](../maestro/records/edit-records.md).

## Semaine du 6 novembre 2023

### Regroupement pour la vue de tableau

Aperçu et production : 7 novembre 2023

Vous pouvez désormais regrouper des enregistrements dans la vue de table d’une page de type enregistrement. Vous pouvez regrouper trois champs uniques dans l’interface Maestro <!--checking into this for now: and by four fields when using the API-->.

Pour plus d’informations, voir [Gestion de la vue de tableau](../maestro/views/manage-the-table-view.md).

## Semaine du 30 octobre 2023

### Nouveaux types de champs pour les champs de date et d’utilisateur afin de capturer les personnes qui ont créé ou modifié un enregistrement ou à quelle date.

Aperçu et production : 30 octobre 2023

Nous avons introduit les types de champ suivants pour les enregistrements Maestro :

* Créé par

* Date de création

* Dernière modification par

* Date de dernière modification

Les valeurs de champ des champs créés à partir de ces types de champs sont en lecture seule et capturent le nom de l’utilisateur qui a créé ou modifié pour la dernière fois un enregistrement, ou la date à laquelle l’enregistrement a été créé ou modifié pour la dernière fois.

Pour plus d’informations, voir [Créer des champs](../maestro/fields/create-fields.md).

### Accès aux objets Workfront à partir d’un enregistrement Maestro

Aperçu et production : 31 octobre 2023

Vous pouvez désormais ouvrir les pages d’objet Workfront à partir des zones suivantes de Maestro :

* Vue de la table d’enregistrement d’objet Workfront liée en lecture seule

* Page Détails de l’enregistrement d’objet Workfront en lecture seule

Pour plus d’informations, voir [Connexion d’enregistrements](../maestro/records/connect-records.md).

### Amélioration de la navigation dans la vue Tableau

Aperçu et production : 2 novembre 2023

Nous avons amélioré la navigation dans la vue tabulaire d’une page de type enregistrement.

Voici quelques améliorations :

* Utilisez la touche de tabulation de votre clavier pour parcourir les colonnes et les lignes du tableau.

* Ajoutez un nouvel enregistrement à partir de n’importe quelle position de colonne. Avant cette amélioration, vous ne pouviez ajouter un enregistrement qu’à partir de la première colonne.

* Utilisez la combinaison clavier Maj + Entrée pour ajouter un nouvel enregistrement (ou une nouvelle ligne) dans le tableau.

Pour plus d’informations, voir [Créer des enregistrements](../maestro/records/connect-records.md).

## Semaine du 16 octobre 2023

### Type de champ Nouveau type de personne

Aperçu et production : 16 octobre 2023

Vous pouvez désormais ajouter un champ de type Personnes aux types d’enregistrement Maestro. Vous pouvez utiliser des champs de type Personnes pour associer des utilisateurs existants à un enregistrement. Pour plus d’informations, voir [Créer des champs](../maestro/fields/create-fields.md).

### Format de texte enrichi pour les champs de paragraphe

Aperçu et production : 16 octobre 2023

Nous avons ajouté des contrôles au format Texte enrichi pour les champs de type Paragraphe. Vous pouvez formater vos champs de paragraphe à l’aide de texte enrichi en mode Tableau d’un type d’enregistrement ou dans la page Détails d’un enregistrement. Pour plus d’informations, voir [Modifier des enregistrements](../maestro/records/edit-records.md).


### Enregistrement et regroupement du codage des couleurs pour la vue Chronologie

Aperçu et production : 19 octobre 2023

Vous pouvez maintenant coder par couleur les barres d’enregistrement et les regroupements dans la vue Chronologie.

Vous trouverez ci-dessous des options pour les couleurs que vous pouvez choisir d’afficher pour les barres d’enregistrement et les regroupements en mode Chronologie :

* Les regroupements peuvent correspondre aux couleurs suivantes :

   * Gris (valeur par défaut)

   * La couleur du champ par lequel vous effectuez un groupement

* Les barres peuvent correspondre aux couleurs suivantes :

   * Couleur du type d’enregistrement

   * Couleur d’un champ que vous sélectionnez

   * Couleur du groupement

   * Aucune couleur (valeur par défaut)

Lorsque vous associez des couleurs à un certain champ, vous ne pouvez sélectionner que les champs avec des options codées par couleur.

Pour plus d’informations, voir [Gestion du mode Chronologie](../maestro/views/manage-the-timeline-view.md).

## Semaine du 9 octobre 2023

### Recherche dans la vue Tableau

Aperçu et production : 9 octobre 2023

Vous pouvez désormais rechercher un mot-clé pour trouver rapidement un enregistrement dans le mode Tableau. Vous pouvez utiliser des mots-clés et des caractères spéciaux dans n’importe quel champ visible à l’écran pour trouver un enregistrement. Pour plus d’informations, voir [Gestion de la vue de tableau](../maestro/views/manage-the-table-view.md).

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

   * [Connexion des types d’enregistrement](../maestro/architecture/connect-record-types.md)
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
