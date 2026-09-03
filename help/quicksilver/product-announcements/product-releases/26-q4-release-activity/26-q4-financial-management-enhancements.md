---
title: Améliorations de la gestion financière pour le quatrième trimestre de 2026
description: Améliorations de la gestion financière pour le quatrième trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 4ca5bba5090d9e3a72c8964bdf6cca1085c314db
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 3%

---

# Améliorations de la gestion financière pour le quatrième trimestre de 2026

Cette page décrit les améliorations apportées à Financial Management avec la version du quatrième trimestre 2026 dans l’environnement de prévisualisation. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du quatrième trimestre 2026, voir [présentation de la version du quatrième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Améliorations des taux de facturation de l’entreprise

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Plusieurs mises à jour ont été apportées à la fonctionnalité des taux de facturation de l’entreprise.

### Pour les clients de tous les packages de Workfront et de workflow

* Nous avons mis à jour les boîtes de dialogue pour ajouter et modifier les taux de facturation des sociétés avec une conception plus moderne et cohérente avec les autres zones de Workfront.
* Le paramètre « Autoriser les taux de facturation au niveau de l’entreprise à remplacer les taux de facturation au niveau du projet » ajoute correctement les remplacements de taux lorsqu’une entreprise est ajoutée à un projet et les calculs de revenus prévus utilisent les taux de facturation au niveau de l’entreprise.
* Les utilisateurs ne disposant pas de l’accès à Modifier les finances générales et Modifier les taux de facturation au niveau du projet ne peuvent plus ajouter une entreprise à ce projet.

### Pour les clients et clientes du package Workflow Ultimate uniquement

Des attributs de taux sont désormais disponibles pour s’appliquer aux taux de facturation au niveau de l’entreprise. Les dates de validité peuvent également être appliquées aux taux d&#39;entreprise.

REMARQUE : les taux au niveau de la société n&#39;ont pas été ajoutés à la hiérarchie des taux.

Pour plus d’informations, voir [Remplacer les taux de facturation des fonctions au niveau de l’entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md) et [Remplacer les taux de facturation au niveau du projet par les taux de facturation au niveau de l’entreprise](/help/quicksilver/manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Les hiérarchies d’attributs restent désormais automatiquement connectées

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026
>Cette fonctionnalité n’est disponible que pour les organisations qui utilisent le package Workflow Ultimate.

Lors de l’utilisation d’attributs de taux en tant que filtres dans différentes zones de Workfront, telles que les affectations avancées, une validation supplémentaire est désormais appliquée au filtrage parent-enfant.

Auparavant, si vous liiez un attribut à un parent, et ce parent à un grand-parent, le système ne reconnaissait pas automatiquement l’attribut d’origine comme appartenant également au grand-parent. Désormais, lorsque vous choisissez l’attribut de niveau le plus bas, chaque niveau au-dessus est automatiquement attribué.

Pour plus d’informations sur les attributs, voir [Définir des attributs de taux](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).
