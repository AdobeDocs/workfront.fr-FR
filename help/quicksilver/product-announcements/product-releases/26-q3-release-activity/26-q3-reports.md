---
title: Améliorations des rapports du troisième trimestre 2026
description: Améliorations des rapports du troisième trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 9a86968cf8fff2c7c930aa6c8408ab8566905cb8
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 6%

---

# Améliorations des rapports du troisième trimestre 2026

Cette page décrit les améliorations apportées aux rapports avec la version du troisième trimestre 2026 dans l’environnement Aperçu. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du troisième trimestre 2026, voir [Présentation de la version du troisième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Amélioration de la précision des données dans les rapports du tableau de bord Zone de travail

>[!NOTE]
>
>Aperçu : 14 mai 2026>Version rapide de production : 11 juin 2026>Production pour tous : 16 juillet 2026
>
>Les tableaux de bord de la zone de travail sont actuellement en version bêta.

Les tableaux de bord de la zone de travail structurent désormais les requêtes de rapport afin d’éviter les lignes en double lorsque les filtres ou les champs recoupent des enregistrements associés. Ainsi, les nombres, les sommes et autres agrégats renvoient des valeurs précises.

Auparavant, une jointure entre des enregistrements associés pouvait répéter les enregistrements parents une fois pour chaque enregistrement associé. Par exemple, dans un rapport de projet filtré en fonction des tâches affectées à un utilisateur spécifique, chaque projet est répété une fois pour chaque tâche correspondante. Un IPC qui additionne le budget du projet pourrait indiquer 6 000 $ au lieu du 1 250 $ correct.

L’interface du tableau de bord de la zone de travail n’a pas été modifiée. Les rapports existants renvoient automatiquement des données précises après cette version.
