---
title: 2.2 Améliorations apportées aux administrateurs et administratrices
description: 2.2 Améliorations apportées aux administrateurs et administratrices
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 97%

---

# 2.2 Améliorations apportées aux administrateurs et administratrices

Cette page décrit toutes les améliorations pour les administrateurs et administratrices apportées à l’environnement de prévisualisation dans la version 22.2. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semaine du 4 avril 2022. Pour obtenir la liste de toutes les modifications disponibles avec la version 22.2, voir [Présentation de la version 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Configurer un formulaire personnalisé pour l’utiliser avec plusieurs types d’objets

Vous pouvez désormais configurer un formulaire personnalisé nouveau ou existant pour qu’il fonctionne avec plusieurs types d’objets, ce qui rend le formulaire beaucoup plus utile. Les utilisateurs et utilisatrices pourront joindre et remplir le formulaire sur tous les types d’objets pour lesquels vous l’avez configuré.

Auparavant, vous pouviez configurer un formulaire personnalisé pour qu’il ne fonctionne qu’avec un seul type d’objet.

Cette fonctionnalité fonctionne avec tous les formulaires personnalisés créés précédemment dans votre système Workfront. Par exemple, si vous disposez déjà d’un formulaire personnalisé créé pour le type d’objet Tâche, vous pouvez maintenant configurer le formulaire pour qu’il fonctionne également avec d’autres types d’objets, tels que Projet et Problème.

>[!NOTE]
>
>* Au moment de la version de prévisualisation initiale de cette fonctionnalité, nous avons temporairement désactivé la possibilité de copier un formulaire personnalisé à plusieurs objets. Cette capacité a été activée le 24 mars.
>* Dans un champ personnalisé calculé, certains champs que vous référencez peuvent ne pas être compatibles avec les types d’objets configurés pour le formulaire. Notre solution est un joker qui permettra au calcul de produire différentes valeurs, selon l’objet auquel le formulaire est attaché. Nous avons ajouté le joker le 24 mars.
>* Pour les sauts de section dans les formulaires personnalisés, nous avons créé un jeu d’autorisations d’affichage et de modification communes qui fonctionnent pour tous les types d’objets que vous pouvez configurer pour un formulaire. Dans un scénario, nous avons constaté que l’une de ces autorisations, Modification limitée, pouvait provoquer des erreurs dans un formulaire. Ce problème a été corrigé le 24 mars.
>

## Le catalogue de plans directeurs est accessible à tous les utilisateurs et utilisatrices, et les administrateurs et administratrices peuvent autoriser les demandes

Tous les utilisateurs et utilisatrices d’Adobe Workfront peuvent désormais consulter le catalogue des plans directeurs disponibles. Pour plus d’informations, voir [Parcourir le catalogue de plans directeurs et demander l’installation de plans directeurs](../../../administration-and-setup/blueprints/browse-catalog.md).

En outre, l’administrateur ou l’administratrice du système peut permettre aux utilisateurs et utilisatrices de demander l’installation de plans directeurs. L’attribution d’une file d’attente de demandes pour stocker les demandes permet aux utilisateurs et utilisatrices d’effectuer des demandes à partir du catalogue de plans directeurs. Pour plus d’informations, voir [Configurer l’accès aux plans directeurs](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## Ajouter une image à un formulaire personnalisé

Dans un formulaire personnalisé que vous créez ou modifiez, vous pouvez désormais ajouter une image et inclure une infobulle informative ou instructive que les utilisateurs et utilisatrices peuvent lire lorsqu’ils placent la souris sur l’image.

Cette fonction peut être utile, par exemple, pour présenter le branding d’un nouveau produit ou pour fournir des informations visuelles dont les personnes ont besoin lorsqu’elles remplissent le formulaire.

Auparavant, les formulaires personnalisés étaient entièrement basés sur du texte.

>[!NOTE]
>
>Dans les zones de la nouvelle expérience Adobe Workfront qui n’ont pas encore été modernisées, telles que la boîte qui s’affiche lorsque vous modifiez des éléments en masse, les images des formulaires personnalisés ne s’affichent pas. Elles s’afficheront au fur et à mesure de la mise à jour de ces zones.


## Nouvelles configurations du niveau d’accès par défaut

Pour mieux répondre aux besoins de la plupart des administrateurs et administratrices qui créent des niveaux d’accès, nous avons modifié la configuration par défaut des options « Ajuster vos paramètres » énumérées ci-dessous. Elles s’affichent lorsque vous cliquez sur l’icône d’engrenage ![](assets/gear-icon-in-access-levels.png) sur un bouton Modifier.

Toutes ces modifications désactivent une option qui était auparavant activée par défaut. Si cela ne correspond pas aux besoins de votre organisation, vous pouvez les activer lors de la configuration d’un nouveau niveau d’accès, ou à tout moment par la suite.

>[!IMPORTANT]
>
>Cette modification de la configuration par défaut n’affecte que les niveaux d’accès que vous créez par la suite, et non ceux que vous avez créés précédemment.

* Dans un nouveau niveau d’accès avec une licence de type Plan :

   * L’option Partager sur le système est désormais désactivée pour les projets, les tâches, les problèmes, les portfolios, les programmes, les rapports, les filtres, les documents et les modèles.
   * Les options Afficher les rapports intégrés et Partager les rapports publiquement sont également désactivées pour les rapports.
   * L’option Partager les documents publiquement est également désactivée pour les documents.

* Dans un nouveau niveau d’accès avec une licence de type Travail :

   * L’option Partager sur le système est désormais désactivée pour les filtres et les documents.
   * L’option Partager les documents publiquement est également désactivée pour les documents.

* Dans un nouveau niveau d’accès avec un type de licence Demande ou Révision :

   * Le partage à l’échelle du système est désormais désactivé pour les filtres.

## Désactiver un groupe

Au fur et à mesure que vos organisations internes changent, vous devrez peut-être cesser d’utiliser certains groupes dans Workfront et en créer de nouveaux. Pour cela, nous avons ajouté la possibilité de désactiver un groupe sans perdre ses données historiques. Pour les utilisatrices et utilisateurs réguliers qui n’ont pas besoin de les voir, les groupes inactifs sont supprimés des champs de type de groupe.

Vous pouvez toujours trouver et configurer des options, des préférences et des associations d’objets pour les groupes inactifs que vous gérez. La désactivation d’un groupe ne modifie en rien les objets auxquels il est rattaché.

Auparavant, il n’était pas possible de désactiver un groupe.

Pour plus d’informations, voir [Désactiver ou réactiver un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Améliorations apportées à l’historique d’installation des plans directeurs

Lorsque vous installez un plan directeur, un message affiche désormais les objets spécifiques (tels que les rôles, les équipes ou les groupes) qui ont été installés avec succès avec le plan directeur et tous les objets dont l’installation a échoué. Vous pouvez également consulter la liste des objets installés sur la page Détails du plan directeur en cliquant sur Afficher les détails à côté d’une installation spécifique dans le tableau de l’historique des installations.

Pour plus d’informations, voir [Installer un plan directeur](../../../administration-and-setup/blueprints/blueprints-install.md).

![](assets/blueprints-installation-history-350x95.png)

## Un avertissement s’affiche désormais lors de l’installation en production d’un plan directeur de type Prévisualisation.

Certains plans directeurs ne peuvent être installés que dans l’environnement de prévisualisation à des fins de test.

Si vous accédez à du contenu de prévisualisation uniquement dans votre environnement de production, sandbox 1, ou sandbox 2, le bouton d’installation n’est pas actif et un message d’avertissement peut s’afficher.

Pour plus d’informations, voir [Installer un plan directeur](../../../administration-and-setup/blueprints/blueprints-install.md).
