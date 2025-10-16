---
content-type: release-notes
title: Activité de la version du premier trimestre 2026 pour Adobe Workfront Planning
description: Il s’agit de l’activité de publication du produit Planification d’Adobe Workfront pour le premier trimestre 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: fdfb1ecb61fd85fa927fc7c3443c2a7f23409873
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 2%

---

# Activité de la version du premier trimestre 2026 pour Adobe Workfront Planning

Cet article décrit les nouvelles fonctionnalités de Workfront Planning de la version du premier trimestre 2026.

<!--keep the sentence below for all future quarterly release pages-->

Pour obtenir la liste de toutes les fonctionnalités publiées pour Adobe Workfront Planning, voir [Activité de version d’Adobe Workfront Planning : index des articles](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


## Types d’enregistrements globaux et possibilité de les ajouter en tant que types d’enregistrements existants à d’autres espaces de travail

>[!NOTE]
>
>Aperçu : 16 octobre 2025
>&#x200B;>Version rapide de production : 13 novembre 2025
>&#x200B;>Production pour tous : 15 janvier 2026

Lors de l’implémentation de Workfront Planning pour une organisation multi-équipes avec des workflows communs, vous devrez peut-être définir une structure et des métadonnées cohérentes pour les types d’enregistrements clés (tels que les campagnes ou les éléments livrables) qui peuvent être ajoutés aux espaces de travail de chaque équipe pour capturer et gérer leur travail.

En outre, vous aurez peut-être besoin du travail de chaque équipe pour atteindre un niveau central.

Dans un tel workflow, vous pouvez vous assurer que les équipes capturent leur travail de manière cohérente tout en déverrouillant la visibilité entre les équipes, sans avoir à ajouter tous les membres de l’organisation à chaque espace de travail. Pour ce faire, vous pouvez utiliser des types d’enregistrements globaux.

Vous pouvez désormais désigner un type d’enregistrement comme global et l’utiliser sur plusieurs espaces de travail. Les utilisateurs peuvent utiliser la même structure de champs et les mêmes connexions que celles déjà configurées dans un espace de travail central.

Pour plus d’informations, consultez les articles suivants :

* [Présentation du type d’enregistrement de l’espace de travail](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [Configurer les fonctionnalités inter-espaces de travail du type d’enregistrement](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [Ajouter des types d’enregistrements existants depuis un autre espace de travail](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## Nouvelle limite pour les champs de connexion d’un type d’enregistrement

>[!NOTE]
>
>Aperçu : 16 octobre 2025
>&#x200B;>Version rapide de production : 13 novembre 2025
>&#x200B;>Production pour tous : 15 janvier 2026

Nous avons introduit une limite de 30 champs de connexion pour chaque type d’enregistrement.

REMARQUE : si votre organisation compte actuellement plus de 30 champs de connexion pour un type d’enregistrement, vous pouvez conserver les champs supplémentaires qui dépassent la limite de 30. Cependant, vous ne pouvez pas ajouter d’autres champs de connexion aux types d’enregistrements qui dépassent la limite. À l’avenir, la nouvelle limite de 30 champs de connexion sera appliquée.

Pour plus d’informations, voir [Présentation des types d’enregistrements connectés](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Définir des valeurs conviviales pour les choix de champs de type sélectionné

>[!NOTE]
>
>Aperçu : 16 octobre 2025
>&#x200B;>Version rapide de production : 13 novembre 2025
>&#x200B;>Production pour tous : 15 janvier 2026

Lors de l’ajout de choix de champs à un champ à sélection unique ou multiple, Workfront attribue désormais des valeurs conviviales uniques à chaque choix. Avant cette amélioration, Workfront générait un identifiant alphanumérique difficile à comprendre et à utiliser dans les appels d’API et d’autres intégrations.

Tenez compte des points suivants grâce à cette amélioration :

* Les nouvelles valeurs seront ajoutées aux nouveaux choix de champ. Les choix de champs existants conserveront leurs identifiants alphanumériques.

* Les valeurs de choix sont uniques pour un champ, mais peuvent être répétées entre différents champs.

* Renommer un choix ne met pas à jour sa valeur d’origine.

* Les valeurs de choix s’affichent en minuscules et sont séparées par des traits de soulignement dans le cas de choix comportant plusieurs mots. Si vous utilisez un libellé déjà utilisé comme autre nom de choix pour le même champ, Workfront ajoute un numéro séquentiel à la valeur.

Pour plus d’informations, consultez [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).