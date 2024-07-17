---
title: Améliorations apportées à l’administration (version 22.2)
description: Améliorations apportées à l’administration (version 22.2)
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 0%

---

# Améliorations apportées à l’administration (version 22.2)

Cette page décrit toutes les améliorations apportées par l’administrateur à la version 22.2 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semaine du 4 avril 2022. Pour obtenir la liste de toutes les modifications disponibles avec la version 22.2, consultez la [présentation des versions 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Configuration d’un formulaire personnalisé pour une utilisation avec plusieurs types d’objets

Vous pouvez maintenant configurer un formulaire personnalisé nouveau ou existant pour qu’il fonctionne avec plusieurs types d’objets, ce qui rend le formulaire beaucoup plus utile. Les utilisateurs pourront joindre et remplir le formulaire sur les objets de tous les types pour lesquels vous le configurez.

Auparavant, vous pouviez configurer un formulaire personnalisé pour qu’il fonctionne avec un seul type d’objet.

Cette fonctionnalité fonctionne avec tous les formulaires personnalisés créés précédemment dans votre système Workfront. Par exemple, si vous disposez déjà d’un formulaire personnalisé créé pour le type d’objet Tâche , vous pouvez maintenant configurer le formulaire pour qu’il fonctionne avec d’autres types d’objets, tels que Projet et Problème.

Pour plus d’informations, reportez-vous à la section [Démarrage de la création d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start) de l’article [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>* Au moment de la version initiale de l’aperçu de cette fonctionnalité, nous avons temporairement désactivé la possibilité de copier un formulaire personnalisé à plusieurs objets. Cette capacité a été activée le 24 mars. Pour plus d’informations sur la copie d’un formulaire personnalisé, voir [Copier un formulaire personnalisé pour en créer un](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).
>* Dans un champ personnalisé calculé, certains champs que vous référencez peuvent ne pas être compatibles avec les types d’objets configurés pour le formulaire. Notre solution est un caractère générique qui permettra au calcul de produire différentes valeurs, selon l’objet auquel le formulaire est attaché. Nous avons ajouté le joker le 24 mars. Pour plus d’informations sur son utilisation, reportez-vous à la section [Champs personnalisés calculés dans des formulaires personnalisés à plusieurs objets](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat) de l’article [Ajout de données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
>* Pour les sauts de section dans les formulaires personnalisés, nous avons créé un ensemble d’autorisations courantes d’affichage et de modification qui fonctionnent pour tous les types d’objets que vous pouvez configurer pour un formulaire. Dans un scénario, nous avons constaté que l’une de ces autorisations, Modification limitée, pouvait entraîner des erreurs sur un formulaire. Ce problème a été corrigé le 24 mars. Pour plus d’informations sur les sauts de section, voir [Ajout d’un saut de section à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).
>

## Le catalogue des plans directeurs est disponible pour tous les utilisateurs et les administrateurs peuvent autoriser les demandes.

Tous les utilisateurs d’Adobe Workfront peuvent désormais parcourir le catalogue des plans directeurs disponibles. Pour plus d’informations, voir [Parcourir le catalogue des plans directeurs et demander l’installation des plans directeurs](../../../administration-and-setup/blueprints/browse-catalog.md).

En outre, l’administrateur système peut permettre aux utilisateurs de demander l’installation de plans directeurs. L’affectation d’une file d’attente de requêtes pour stocker les requêtes permet aux utilisateurs d’effectuer des requêtes à partir du catalogue de plans directeurs. Pour plus d’informations, voir [Configurer l’accès aux plans directeurs](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## Ajout d’une image à un formulaire personnalisé

Dans un formulaire personnalisé que vous créez ou modifiez, vous pouvez désormais ajouter une image et inclure une info-bulle informative ou instructive que les utilisateurs peuvent lire lorsqu’ils la survolent.

Cela peut s’avérer utile, par exemple, pour afficher l’identité graphique d’un nouveau produit ou pour fournir des informations visuelles dont les utilisateurs ont besoin lorsqu’ils remplissent le formulaire.

Auparavant, les formulaires personnalisés étaient entièrement basés sur du texte.

>[!NOTE]
>
>Dans les nouvelles zones d’expérience Adobe Workfront qui n’ont pas encore été modernisées, comme la zone qui s’affiche lorsque vous modifiez des éléments en masse, les images de formulaire personnalisées ne s’affichent pas. Ils s’afficheront au fur et à mesure que nous continuons à mettre à jour ces zones.

Pour plus d’informations, voir [Ajout ou modification d’un widget de ressource dans un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Nouvelles configurations de niveau d’accès par défaut

Pour mieux répondre aux besoins de la plupart des administrateurs qui créent de nouveaux niveaux d’accès, nous avons modifié la configuration par défaut des options &quot;Ajuster vos paramètres&quot; répertoriées ci-dessous. Elles s’affichent lorsque vous cliquez sur l’icône d’engrenage ![](assets/gear-icon-in-access-levels.png) sur un bouton Modifier.

Toutes ces modifications désactivent une option précédemment activée par défaut. Si cela ne correspond pas aux besoins de votre entreprise, vous pouvez les activer lorsque vous configurez un nouveau niveau d’accès, ou ultérieurement.

>[!IMPORTANT]
>
>Cette modification de configuration par défaut affecte uniquement les niveaux d’accès que vous créez désormais, et non les niveaux que vous avez créés précédemment.

* Dans un nouveau niveau d’accès avec un type de licence Plan :

   * L’option Partager à l’échelle du système est désormais désactivée pour les projets, les tâches, les problèmes, les portefeuilles, les programmes, les rapports, les filtres, les documents et les modèles.
   * L’affichage des rapports intégrés et le partage public des rapports sont également désactivés pour les rapports.
   * Partager des documents La fonction publique est également désactivée pour les documents.

* Dans un nouveau niveau d&#39;accès avec un type de licence Work :

   * Partager à l’échelle du système est désormais désactivé pour les filtres et les documents.
   * Partager des documents La fonction publique est également désactivée pour les documents.

* Dans un nouveau niveau d’accès avec un type de licence Request or Review :

   * Partager à l’échelle du système est désormais désactivé pour les filtres.

## Désactivation d’un groupe

À mesure que vos organisations internes changent, vous devrez peut-être cesser d’utiliser certains groupes dans Workfront et en créer de nouveaux. Pour faciliter cette opération, nous avons ajouté la possibilité de désactiver un groupe sans perdre ses données historiques. Pour les utilisateurs réguliers qui n’ont pas besoin de les voir, les groupes inactifs sont effacés des champs de type anticipé de groupe.

Vous pouvez toujours rechercher et configurer des options, des préférences et des associations d’objets pour les groupes inactifs que vous gérez. Et la désactivation d&#39;un groupe ne change rien aux objets auxquels il est attaché.

Auparavant, il n’était pas possible de désactiver un groupe.

Pour plus d’informations, voir [Désactivation ou réactivation d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Améliorations de l’historique d’installation des plans directeurs

Lorsque vous installez un plan directeur, un message affiche désormais les objets spécifiques (tels que les rôles, les équipes ou les groupes) qui ont été correctement installés avec le plan directeur et les objets qui n’ont pas pu être installés. Vous pouvez également afficher la liste des objets installés sur la page Détails du plan directeur en cliquant sur Afficher les détails en regard d’une installation spécifique dans le tableau de l’historique d’installation.

Pour plus d’informations, voir [Installation d’un plan directeur](../../../administration-and-setup/blueprints/blueprints-install.md).

![](assets/blueprints-installation-history-350x95.png)

## Un avertissement s’affiche maintenant lors de l’installation d’un plan directeur Aperçu uniquement en production.

Certains plans directeurs ne peuvent être installés que dans l’environnement Aperçu à des fins de test.

Si vous accédez au contenu Aperçu uniquement dans votre environnement de production, sandbox 1 ou sandbox 2, le bouton d’installation n’est pas actif et un message d’avertissement peut s’afficher.

Pour plus d’informations, voir [Installation d’un plan directeur](../../../administration-and-setup/blueprints/blueprints-install.md).
