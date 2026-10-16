---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Convertir des objets hérités en espace de stockage Adobe
description: Découvrez les trois cas où vous pouvez convertir un objet de stockage Workfront hérité en espace de stockage Adobe et déterminez ce qui bouge et ce qui reste lors de chaque conversion.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 1%

---
# Convertir des objets hérités en espace de stockage Adobe

Dans la plupart des scénarios, vous ne pouvez déplacer, copier et convertir des objets Workfront qu’entre des modèles de stockage similaires. Par exemple, vous pouvez déplacer une tâche d’un projet d’espace de stockage dans le cloud Adobe vers un autre projet d’espace de stockage dans le cloud Adobe. Dans trois cas spécifiques, vous pouvez convertir un objet de stockage Workfront hérité en espace de stockage Adobe :

* Convertir une tâche de stockage Workfront héritée en projet de stockage dans le cloud Adobe
* Conversion d’un ancien portfolio de stockage Workfront en portfolio de stockage dans le cloud Adobe
* Création d’un projet de stockage dans le cloud Adobe à partir d’un modèle de stockage Workfront hérité

Pour découvrir les nouveautés de la migration et l’évolution de l’espace de stockage dans le cloud Adobe, voir [Déplacer vers Workfront sur l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

<!-- 
need to validate with PM
>[!NOTE]
>
>In all three conversion scenarios, documents and document folders don't move from legacy Workfront storage to Adobe cloud storage. Documents that exist on the legacy object before the conversion remain on legacy storage.
-->

## Convertir une tâche héritée en projet d’espace de stockage Adobe

Pour convertir une tâche de stockage Workfront héritée en projet de stockage dans le cloud Adobe, utilisez le flux de conversion en projet existant sur la tâche. Pendant la conversion :

* Les sous-tâches et les événements sont déplacés vers le nouveau projet.
* Les documents joints à la tâche et leurs workflows d’approbation restent dans le projet d’origine.
* Les approbations de travail et les liens d&#39;objet de résolution sont supprimés.
* La tâche originale est supprimée.

## Conversion d’un portfolio hérité en portfolio de stockage dans le cloud Adobe

Un administrateur Workfront peut convertir un ancien portfolio de stockage Workfront en portfolio de stockage dans le cloud Adobe à partir de la zone Configuration . Après la conversion :

* Vous ne pouvez plus déplacer les projets de stockage Workfront hérités vers le portefeuille.
* Tous les nouveaux projets créés dans le portefeuille utilisent l’espace de stockage dans le cloud d’Adobe.
* Frame.io est la visionneuse de documents dans les projets de stockage dans le cloud Adobe du portfolio.
* Les projets enfants qui utilisent le stockage Workfront hérité restent sur le stockage hérité.
* Les programmes enfants restent sur l’ancien stockage.

>[!NOTE]
>
>Un programme hérité enfant est automatiquement converti en espace de stockage Adobe uniquement lorsqu’un utilisateur y ajoute manuellement un projet d’espace de stockage Adobe.

Pour plus d’informations, voir [Conversion de portefeuilles hérités en espace de stockage Adobe](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md).

## Création d’un projet de stockage dans le cloud Adobe à partir d’un modèle hérité

Lorsque vous créez un projet à partir d’un modèle de stockage Workfront hérité, la case à cocher **Créer ce projet dans l’espace de stockage Adobe** de la boîte de dialogue de création de projet détermine le type de stockage du nouveau projet. Le comportement des cases à cocher dépend de l’emplacement où vous créez le projet :

* **En dehors d&#39;un portfolio** : la case à cocher est disponible et désactivée par défaut. Sélectionnez-le pour créer le projet dans l’espace de stockage cloud d’Adobe.
* **Dans un portfolio de stockage dans le cloud Adobe** : la case est cochée et verrouillée. Le nouveau projet doit correspondre au type de stockage du portefeuille.
* **Dans un portfolio de stockage Workfront hérité** : la case à cocher n’est pas disponible. Le nouveau projet utilise l’ancien stockage Workfront.

Pour plus d’informations, voir [Créer des projets](/help/quicksilver/manage-work/projects/create-projects/create-project.md).
