---
title: Améliorations des rapports du troisième trimestre 2026
description: Améliorations des rapports du troisième trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 0c7265c477030137d14e95f42eaf67580589d70b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 1%

---

# Améliorations des rapports du troisième trimestre 2026

Cette page décrit les améliorations apportées aux rapports avec la version du troisième trimestre 2026 dans l’environnement Aperçu. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du troisième trimestre 2026, voir [Présentation de la version du troisième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Contrôle d’accès automatisé pour la planification Workfront dans Snowflake

>[!NOTE]
>
>Aperçu et production pour tous les clients : 16 juillet 2026Hors planning&rbrack;{type=Neutral}

Cette version introduit une gestion des accès automatisée et basée sur les droits pour les données Workfront Planning dans Snowflake dans le cadre de Workfront Data Connect.
Il commence par étendre la génération de vues sécurisées aux tables de planification, établissant ainsi la base requise pour le contrôle d’accès en aval et permettant des subventions basées sur les droits d’accès.Sur cette base, la configuration des comptes de lecteur vérifie désormais les droits TMS au moment de la création et applique ou retient automatiquement les octrois à la base de données Planning, en s’assurant qu’ils sont corrects.
Avant cette amélioration, cette option n’était disponible que pour Workfront.
La mise à jour comprend les fonctionnalités suivantes : 

* Une tâche quotidienne automatisée détecte les modifications de droits pour les clients existants
* Le nouveau traitement accorde, révoque ou conserve l’accès en fonction des droits
* Couverture complète du cycle de vie pour le provisionnement, la création de compte et les modifications de droits en cours.

L’article [Dictionnaire de données de Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md) sera mis à jour après la date de publication.

## Ajouter la prise en charge des données personnalisées pour les nouveaux objets

>[!NOTE]
>
>Aperçu et production pour tous les clients : 7 juillet 2026Hors planning&rbrack;{type=Neutral}

Au cours du deuxième trimestre 2026, nous avons ajouté de nouveaux objets pour prendre en charge les améliorations des opérations d’entreprise dans Workfront.Avec la version actuelle, nous ajoutons également la prise en charge des données personnalisées pour plusieurs nouveaux objets dans le tableau de bord de la zone de travail.

Pour plus d’informations, voir [Présentation du tableau de bord Zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md).

## Valeurs par défaut de l’invite du tableau de bord de la zone de travail et persistance des préférences utilisateur

>[!NOTE]
>
>Aperçu : 25 juin 2026Version rapide de production : 15 juillet 2026Production pour tous : 16 juillet 2026

Pour améliorer l’efficacité pour les utilisateurs qui passent d’un tableau de bord à un enregistrement en préservant leur statut de filtre de travail, les gestionnaires de tableaux de bord peuvent désormais définir des valeurs d’invite par défaut pour les tableaux de bord Zone de travail. Ces valeurs par défaut sont automatiquement appliquées à toutes les visionneuses de tableaux de bord.

Lorsque l’utilisateur met à jour les invites, ses sélections sont enregistrées et restaurées lors de l’actualisation, de la réouverture ou après avoir accédé à un enregistrement et y avoir accédé à nouveau.

Les responsables peuvent réinitialiser à tout moment l’état par défaut du tableau de bord. Les utilisateurs peuvent également revenir rapidement aux valeurs par défaut via le menu à trois points.

Avant cette amélioration, les invites de tableau de bord n&#39;avaient pas de valeur par défaut configurable ou de préférence utilisateur enregistrée pour le statut de l&#39;invite.

Pour plus d’informations, voir [Filtrer un tableau de bord Zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md).

## Ajouter plusieurs plages d’adresses IP Power BI à la fois à la liste autorisée Data Connect

>[!NOTE]
>
>Aperçu : S.O.Version rapide de production : 11 juin 2026Production pour tous : 16 juillet 2026

Les administrateurs Workfront qui connectent Microsoft Power BI à Workfront Data Connect peuvent désormais ajouter en une seule étape à la liste autorisée l’ensemble des plages d’adresses IP d’Azure d’une région. Sur l’onglet Place sur la liste autorisée IP **de** Data Connect **, le bouton** Nouvelle adresse IP **comprend désormais une option** Ajouter des blocs d’adresses IP Power BI **qui ouvre une boîte de dialogue dans laquelle vous pouvez coller les entrées de balise de service Power BI à partir du fichier JSON des plages d’adresses IP et des balises de service Azure publiées Microsoft.**

Cela remplace le workflow précédent qui ajoutait chaque bloc CIDR Power BI un par un, ce qui prenait du temps pour les régions qui publient des dizaines de préfixes d’adresse.

Pour plus d’informations, voir [Établir une connexion à Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).


## Trier la liste Tableaux de bord de la zone de travail

>[!NOTE]
>
>Aperçu : 11 juin 2026Version rapide de production : 15 juillet 2026Production pour tous : 16 juillet 2026
>
>Les tableaux de bord de la zone de travail sont actuellement en version bêta.

Vous pouvez désormais trier la liste Tableaux de bord de la zone de travail en fonction de l’une des colonnes suivantes : **Nom**, **Description**, **Date de création** ou **Date de création**. Cliquez sur un en-tête de colonne pour trier la liste en fonction de cette colonne, puis cliquez de nouveau sur le même en-tête pour inverser le sens du tri. Par défaut, la liste est triée par **Nom** de A à Z. L’ordre de tri est conservé lorsque vous basculez entre les onglets de la liste Tableaux de bord de la zone de travail.

Pour plus d’informations, voir [&#x200B; Utilisation des tableaux de bord de la zone de travail &#x200B;](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Modifications apportées aux heures effectives dans les formules personnalisées

>[!NOTE]
>
>Aperçu : 1er juin 2026Mise à jour rapide de la production : 1er juin 2026Production pour tous : 1 juin 2026

En 2025, un nouveau champ Heures effectives a été ajouté à la base de données Workfront en tant que `actualWorkRequiredDouble` et le champ Heures effectives existant (`actualWorkRequired` dans la base de données) a été renommé Heures effectives héritées. Voir la [note de mise à jour](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md) pour plus d’informations.

En juin 2026, les formules personnalisées existantes utilisant `actualWorkRequired` (heures effectives héritées) ont été migrées pour utiliser `actualWorkRequiredDouble` (heures effectives) à la place. `actualWorkRequired` ne peut plus être utilisé dans les calculs et les formules.

En outre, il est vivement recommandé d’utiliser `actualWorkRequiredDouble` dans tous les rapports.

Lors du remplacement du champ, notez que `actualWorkRequired` stocke les valeurs en minutes, tandis que `actualWorkRequiredDouble` stocke les valeurs en heures avec une précision décimale.

Pour plus d&#39;informations sur les heures réelles, voir [Afficher les heures réelles](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).

## Champs de données de devise personnalisés dans les rapports du tableau de bord de la zone de travail

>[!NOTE]
>
>Aperçu : 28 mai 2026Version rapide de production : 11 juin 2026Production pour tous : 16 juillet 2026

Les rapports Tableau de bord de la zone de travail prennent désormais en charge les champs de données de devise personnalisés sous forme de colonnes, filtres, regroupements et agrégations, y compris lorsque plusieurs taux de change sont configurés dans la configuration du système. Lorsqu’un champ de données de devise personnalisé s’affiche sous la forme d’une colonne ou d’une agrégation, les valeurs sont converties dans la devise sélectionnée dans le bouton (bascule) Taux de change du tableau de bord, sauf si le champ est verrouillé au niveau du rapport.

Les rapports qui échouaient auparavant avec un message de « champ restreint » après l’ajout d’une deuxième devise de taux de change sont désormais rendus. Les champs de devise de planification restent limités lorsque plusieurs taux de change sont définis.

Pour plus d’informations, voir [Utiliser des champs de devise dans les tableaux de bord de la zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md).

## Amélioration de la précision des données dans les rapports du tableau de bord Zone de travail

>[!NOTE]
>
>Aperçu : 14 mai 2026Version rapide de production : 11 juin 2026Production pour tous : 16 juillet 2026
>
>Les tableaux de bord de la zone de travail sont actuellement en version bêta.

Les tableaux de bord de la zone de travail structurent désormais les requêtes de rapport afin d’éviter les lignes en double lorsque les filtres ou les champs recoupent des enregistrements associés. Ainsi, les nombres, les sommes et autres agrégats renvoient des valeurs précises.

Auparavant, une jointure entre des enregistrements associés pouvait répéter les enregistrements parents une fois pour chaque enregistrement associé. Par exemple, dans un rapport de projet filtré en fonction des tâches affectées à un utilisateur spécifique, chaque projet est répété une fois pour chaque tâche correspondante. Un IPC qui additionne le budget du projet pourrait indiquer 6 000 $ au lieu du 1 250 $ correct.

L’interface du tableau de bord de la zone de travail n’a pas été modifiée. Les rapports existants renvoient automatiquement des données précises après cette version.

