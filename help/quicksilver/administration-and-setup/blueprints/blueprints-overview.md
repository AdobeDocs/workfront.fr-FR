---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Présentation des plans directeurs
description: Les plans directeurs fournissent des éléments de base pour vous aider à créer un système de gestion du travail qui se développe avec vous.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: 006df3f8c391596cd0c769df5d7eb843949b4e01
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Présentation des plans directeurs

Les plans directeurs fournissent des éléments de base pour vous aider à créer un système de gestion du travail qui se développe avec vous. Les administrateurs système peuvent parcourir le catalogue de plans directeurs et installer des modèles de projet, des tableaux de bord et des structures organisationnelles prêts à l’emploi. D’autres utilisateurs peuvent parcourir le catalogue et demander l’installation d’un plan directeur. Pour plus d’informations, voir [Parcourir le catalogue des plans directeurs et demander l’installation des plans directeurs](../../administration-and-setup/blueprints/browse-catalog.md).

Chaque plan directeur est ciblé sur un département et un niveau de maturité spécifique afin de vous aider à mettre en oeuvre plus rapidement les bonnes pratiques éprouvées dans votre système. Les niveaux de maturité présentés ci-dessous sont indiqués dans la carte du catalogue de plans directeurs et dans les détails.

**[!UICONTROL Géré]:** Les modèles de projet gérés aident à l’adoption d’un nouveau processus d’entreprise avant que les activités et les livrables ne soient entièrement acceptés comme une procédure standard. Ils contiennent des tâches permettant de s’assurer que chaque étape du nouveau processus est suivie.

**[!UICONTROL Intégré]:** Les modèles de projet intégrés supposent que les fonctions métier sont prises en charge par le biais d’une procédure de fonctionnement standard. Les contributeurs au processus connaissent les étapes et les tâches qu’ils doivent accomplir pour suivre le processus. Les modèles de projet qui prennent en charge ce processus contiennent moins de tâches pour suivre uniquement les jalons et autres livrables clés nécessaires à la création de rapports.

## Trouver le plan directeur approprié

Vous pouvez parcourir les plans directeurs par cas d’utilisation, niveau de maturité, état d’installation et saisir avec les filtres sur le côté droit du catalogue. Une fois que vous avez trouvé un plan directeur qui vous intéresse, vous pouvez afficher les détails sur la page de détails.

### Types de plan directeur

Le type de plan directeur indique ce qui est inclus dans le plan directeur. Le type est répertorié au bas de la carte de plan directeur dans le catalogue. Notez qu’un plan directeur peut comporter plusieurs types.

Les types de plans directeurs suivants sont disponibles :

* Modèles de projet : comprend des objets standard associés à un modèle de projet (tâches, problèmes, rôles et équipes), ainsi que certaines préférences liées à ces objets. Pour plus d’informations, voir [Configuration d’un plan directeur](../../administration-and-setup/blueprints/configure-template-package.md).
* Structures organisationnelles : comprend les objets associés à la structure d’une organisation (entreprises, groupes, rôles et équipes). Pour plus d’informations, voir [Configuration d’un plan directeur](../../administration-and-setup/blueprints/configure-template-package.md).
* Tableaux de bord : comprend un ou plusieurs tableaux de bord pour un cas d’utilisation spécifique, comme les services de mise en oeuvre.
<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

Pour consulter les plans directeurs actuels, voir [Liste des plans directeurs disponibles](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### Afficher les détails de la 

Chaque plan directeur contient une page de détails. Sur cette page, vous pouvez effectuer les opérations suivantes :

* Afficher un résumé du contenu du workflow
* Lire un bref résumé du plan directeur
* Afficher l’historique d’installation (cliquez sur **[!UICONTROL Voir Détails]** pour afficher la liste complète des objets installés avec le plan directeur)
* Voir les descriptions des rôles, équipes, entreprises et groupes.
* Consultez un exemple visuel du plan directeur spécifique, tel qu’un modèle de projet (vous pouvez prévisualiser l’image complète dans le navigateur ou la télécharger).

![[!UICONTROL Détails du plan directeur] page](assets/blueprint-details-page-2022.png)

## Installer un plan directeur

L’administrateur système peut effectuer l’installation directement dans l’environnement de production ou dans les environnements de test. Pour en savoir plus, voir [Installer un plan directeur](../../administration-and-setup/blueprints/blueprints-install.md) ou [Configuration d’un plan directeur](../../administration-and-setup/blueprints/configure-template-package.md).

Après l’installation, vous pouvez ne pas être certain des meilleures actions à effectuer. Pour plus d’informations, voir [Actions à entreprendre après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## Remarques supplémentaires sur les plans directeurs et les modèles

Les plans directeurs ne remplacent pas la fonctionnalité de modèles de projet dans [!DNL Adobe Workfront]. Les plans directeurs vous permettent de créer de nouveaux modèles plus rapidement afin d’organiser davantage votre travail dans [!DNL Workfront].

Vous ne pouvez pas copier ni modifier un plan directeur. Cependant, une fois que vous avez installé la solution à partir d’un plan directeur, vous pouvez modifier le modèle de projet, les rôles de tâche ou les équipes créés à partir du plan directeur de la même manière que vous mettez normalement à jour ces enregistrements dans la variable [!DNL Workfront] . En outre, lorsque vous installez un plan directeur, le modèle est stocké dans la variable [!UICONTROL Modèles] area of [!DNL Workfront] et le plan directeur d’origine reste dans la variable [!UICONTROL Plans directeurs] zone. Il n’est pas nécessaire d’en faire une copie avant de commencer à la personnaliser à vos besoins.

Les plans directeurs ne suppriment ni ne remplacent les éléments configurés dans votre environnement. Si vous envisagez de remplacer un modèle existant en installant un plan directeur qui crée un nouveau modèle, nous vous recommandons de désactiver la version précédente afin d’éviter toute confusion parmi vos planificateurs qui créent des projets à partir de modèles.
