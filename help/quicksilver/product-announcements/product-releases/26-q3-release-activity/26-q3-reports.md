---
title: Améliorations des rapports du troisième trimestre 2026
description: Améliorations des rapports du troisième trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a177e2887c2b8b281b19cda45ce59c6f8149cefb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 4%

---

# Améliorations des rapports du troisième trimestre 2026

Cette page décrit les améliorations apportées aux rapports avec la version du troisième trimestre 2026 dans l’environnement Aperçu. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du troisième trimestre 2026, voir [Présentation de la version du troisième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Champs de données de devise personnalisés dans les rapports du tableau de bord de la zone de travail

>[!NOTE]
>
>Aperçu : 28 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026

Les rapports Tableau de bord de la zone de travail prennent désormais en charge les champs de données de devise personnalisés sous forme de colonnes, filtres, regroupements et agrégations, y compris lorsque plusieurs taux de change sont configurés dans la configuration du système. Lorsqu’un champ de données de devise personnalisé s’affiche sous la forme d’une colonne ou d’une agrégation, les valeurs sont converties dans la devise sélectionnée dans le bouton (bascule) Taux de change du tableau de bord, sauf si le champ est verrouillé au niveau du rapport.

Les rapports qui échouaient auparavant avec un message de « champ restreint » après l’ajout d’une deuxième devise de taux de change sont désormais rendus. Les champs de devise de planification restent limités lorsque plusieurs taux de change sont définis.

Pour plus d’informations, voir [Utiliser des champs de devise dans les tableaux de bord de la zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md).

## Amélioration de la précision des données dans les rapports du tableau de bord Zone de travail

>[!NOTE]
>
>Aperçu : 14 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026
>
>Les tableaux de bord de la zone de travail sont actuellement en version bêta.

Les tableaux de bord de la zone de travail structurent désormais les requêtes de rapport afin d’éviter les lignes en double lorsque les filtres ou les champs recoupent des enregistrements associés. Ainsi, les nombres, les sommes et autres agrégats renvoient des valeurs précises.

Auparavant, une jointure entre des enregistrements associés pouvait répéter les enregistrements parents une fois pour chaque enregistrement associé. Par exemple, dans un rapport de projet filtré en fonction des tâches affectées à un utilisateur spécifique, chaque projet est répété une fois pour chaque tâche correspondante. Un IPC qui additionne le budget du projet pourrait indiquer 6 000 $ au lieu du 1 250 $ correct.

L’interface du tableau de bord de la zone de travail n’a pas été modifiée. Les rapports existants renvoient automatiquement des données précises après cette version.
