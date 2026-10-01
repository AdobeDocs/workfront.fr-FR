---
title: Améliorations apportées à l’administration pour le quatrième trimestre 2026
description: Améliorations apportées à l’administration pour le quatrième trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: 6fb8df06a03ba2189c16585ffb2844f484f4ca1d
workflow-type: tm+mt
source-wordcount: '1666'
ht-degree: 1%
---
# Améliorations apportées à l’administration pour le quatrième trimestre 2026

Cette page décrit les améliorations apportées par l’administrateur à l’environnement de Prévisualisation avec la version du quatrième trimestre 2026. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du quatrième trimestre 2026, voir [présentation de la version du quatrième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Utiliser l’IA pour générer une localisation personnalisée

>[!NOTE]
>
>Aperçu : 1er octobre 2026
>Version rapide de production : 14 octobre 2026
>Production pour tous : 15 octobre 2026

Pour vous aider à gagner du temps dans la traduction de termes et de libellés de champ personnalisés, nous avons ajouté la possibilité de générer des traductions d’IA pour une localisation personnalisée. Désormais, les administrateurs et administratrices de Workfront peuvent utiliser l’IA pour générer des traductions pour du texte personnalisé non traduit, ou renseigner des traductions supplémentaires pour un terme précédemment localisé, puis consulter et ajuster les résultats avant d’enregistrer.

Pour plus d’informations, voir [Configuration de la localisation personnalisée](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-custom-localization.md).

<!--

## Grant access to MCP Tools

>[!NOTE]
>
>Preview: October 1, 2026
>Production fast release: October 14, 2026
>Production for everyone: October 15, 2026

To make it easier to control secure access to Workfront data, we've added the ability for administrators to configure MCP Tools permissions by access level. Now, you can configure actions a given access level can take through the Workfront MCP.

* No access
* Read
* Create
* Update / Delete

You can edit this access when editing a specific access level, or edit access to MCP tools for multiple access levels at once.

For more information, see [Grant access to MCP Tools](help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-mcp-tools.md).

-->

## Améliorations apportées aux modèles de mise en page

>[!NOTE]
>
>Aperçu : 1er octobre 2026
>Version rapide de production : 14 octobre 2026
>Production pour tous : 15 octobre 2026

Plusieurs améliorations ont été apportées aux modèles de mise en page :

* Les administrateurs système et de groupe peuvent désormais choisir de masquer ou d&#39;afficher les éléments système dans le menu principal, dans le modèle de mise en page. Les éléments système incluent les boutons Configuration et Aide.
* Vous pouvez désormais repositionner les applications personnalisées dans n’importe quel ordre avec les options de menu Workfront par défaut. Cela vous permet de positionner chaque application à l’endroit le plus pertinent. Auparavant, les applications personnalisées étaient toujours les derniers éléments des options du menu principal du modèle de mise en page et ne pouvaient pas être repositionnées.
* Vous pouvez désormais masquer la page Détails d’un objet dans le panneau de navigation de gauche. Au moins un élément doit être affiché dans le panneau de gauche d’un objet. Si tous les autres éléments sont masqués, vous ne pouvez pas masquer le dernier élément restant.

Pour plus d’informations, voir [Personnaliser le menu principal à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) et[Personnaliser le panneau de gauche à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Amélioration de l’expérience de mise à jour des choix de champ dans le concepteur de formulaire personnalisé

>[!NOTE]
>
>Aperçu : 1er octobre 2026
>Version rapide de production : 14 octobre 2026
>Production pour tous : 15 octobre 2026

Lorsque vous utilisez des champs déroulants, des boutons radio et des cases à cocher dans le concepteur de formulaire, vous pouvez désormais ajouter, modifier et supprimer des choix de champ dans une seule boîte de dialogue. Auparavant, vous ajoutiez et modifiiez des choix dans le panneau de droite du concepteur et il n’y avait pas beaucoup d’espace si vous créiez une longue liste de choix.

Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkbox-groups-and-drop-downs).

## Création et gestion des abonnements aux événements dans l’interface de Workfront

Pour faciliter la création et la gestion des abonnements aux événements de votre entreprise, nous avons ajouté la zone Abonnements aux événements à la Configuration. Désormais, vous pouvez :

* Affichez une liste des abonnements aux événements existants :
* Créez des abonnements aux événements, y compris le filtrage par critères que vous spécifiez :
* Supprimez les abonnements aux événements.

<!--ADD LINK WHEN READY-->


## Ajout d’URL de redirection autorisées pour les intégrations MCP

>[!NOTE]
>
>Aperçu : 22 septembre 2026
>Version rapide de production : 14 octobre 2026
>Production pour tous : 15 octobre 2026

Pour rendre les serveurs Workfront MCP plus flexibles et personnalisables pour votre organisation, nous avons ajouté la possibilité d’ajouter des URL de rappel OAuth personnalisées. Les administrateurs et administratrices de Workfront peuvent désormais gérer la liste autorisée de données de leur propre organisation des URL de rappel OAuth approuvées pour les intégrations MCP. Cela vous permet de connecter des plateformes d’agence IA personnalisées dont l’URL de rappel OAuth est unique à votre organisation, au-delà des plateformes que Workfront prend en charge de manière native.

Pour plus d’informations, voir [Ajouter ou supprimer une URL de redirection autorisée](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md#add-or-remove-an-authorized-redirect-url) dans [Configurer les préférences système](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

<!--

## Interface improvements to the Actions list

>[!NOTE]
>
>Preview: August 20, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

The Actions list in the Update Feeds section of the Setup area has an updated look and feel.

The following enhancements are included:

* We removed the Save and Cancel buttons.
* The Track column now appears in the last position.
* We removed the confirmation message that previously displayed when you saved changes in this area.

For information, see [Configure system updates](/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

-->

## Définir un niveau d’accès par défaut pour les utilisateurs configurés dans le Adobe Admin Console

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Vous pouvez désormais définir un niveau d’accès par défaut pour les utilisateurs configurés dans Workfront via Adobe Admin Console. Un administrateur Workfront peut configurer cette valeur par défaut dans les Préférences système.

Auparavant, Workfront attribuait à l’utilisateur un niveau d’accès Contributeur ou Demandeur .

Pour plus d’informations, voir [Configuration des préférences système](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Semaines personnalisées en plus des trimestres personnalisés pour les clients Workfront Planning

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Si votre entreprise a acheté un package Planning, en plus d’un package Workflow, vous pouvez désormais configurer des semaines personnalisées de la même manière que vous configurez des trimestres personnalisés en tant qu’administrateur de Workfront.

Les semaines personnalisées ne sont pas visibles dans Workfront. Ils ne sont visibles que dans la vue chronologique Planification de Workfront.

Pour plus d’informations, voir [Activer les trimestres personnalisés](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Prise en charge des fichiers volumineux pour les intégrations de documents personnalisés

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Les intégrations de documents personnalisés prennent désormais en charge les chargements groupés de fichiers volumineux. Lorsque cette option est activée, les fichiers de plus de 25 Mo sont divisés en plus petits blocs et chargés en parallèle, ce qui rend les chargements de fichiers volumineux plus rapides et plus fiables. Les administrateurs peuvent activer cette option et définir la taille maximale du bloc (jusqu’à 100 Mo) par intégration.

Pour plus d’informations, voir [Configurer des intégrations de documents](/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md).

## Les administrateurs de groupe peuvent gérer les profils professionnels

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Les administrateurs de groupe peuvent désormais créer, modifier et supprimer les profils professionnels des groupes qu’ils administrent, sans avoir besoin d’un accès d’administrateur système. Cela donne aux entreprises plus de flexibilité pour déléguer la gestion des profils métier au niveau du groupe.

Pour plus d’informations, voir [Afficher et gérer les profils métier](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-business-profiles.md).

## Prise en charge des modèles de disposition pour les vues des listes améliorées

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Les vues des listes améliorées sont désormais prises en charge au niveau du système via un modèle de mise en page. Vous pouvez masquer les vues système existantes, affecter une vue spécifique en tant que vue par défaut et ajouter une vue personnalisée à la liste des vues système.

Les exemples de listes améliorées dans le modèle de mise en page sont **Toutes les demandes** et **Affectations avancées**. Une liste améliorée comporte un libellé « Nouvelle expérience » en regard des vues.

Pour plus d&#39;informations, voir [Personnaliser des filtres, des vues et des regroupements à l&#39;aide d&#39;un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Modification en masse de champs de recherche externe

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Les boîtes de dialogue de modification en bloc permettent désormais de modifier les champs de recherche externes. Cela n’était pas possible auparavant.

Dans les cas où un champ de recherche dépend d’un autre champ de recherche, le champ avec la dépendance ne peut pas être modifié en bloc, sauf si le premier champ est le même pour tous les objets en cours de modification.

Par exemple, une liste de pays dépend de la sélection effectuée pour une région. Si la région d&#39;un projet est l&#39;Asie et la région d&#39;un autre projet est l&#39;Europe et que vous modifiez en bloc les deux projets, le champ Pays ne sera pas disponible car les régions ne correspondent pas. Si vous modifiez la région pour qu’elle soit la même pour les deux projets, vous pouvez également sélectionner un pays à utiliser pour les deux projets.

Pour plus d’informations sur les champs de recherche externe, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-external-lookup-fields).

## Logique avancée prise en charge dans l’aperçu du créateur de formulaire personnalisé

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Le mode d’aperçu du créateur de formulaire personnalisé prend désormais en charge les options logiques avancées, notamment la logique d’affichage avancée, la logique de valeur par défaut, la logique de validation, la logique de formatage et la logique d’modifiabilité. Vous pouvez tester les formules logiques dans l’aperçu du formulaire et les ajuster selon vos besoins dans le créateur de logiques. Vous pouvez également sélectionner un objet de test (projet, tâche, problème, etc.) pour prévisualiser le formulaire avec des données contextuelles réelles.

Auparavant, seules les options d’affichage de base et de logique d’omission étaient prises en charge en mode Aperçu.

Notez que ces types de logiques ne sont disponibles que pour les organisations sur les packages Workflow Prime ou Ultimate : affichage avancé, valeur par défaut, mise en forme conditionnelle et modifiabilité.

Pour plus d’informations, consultez les sections [Ajouter des règles de logique aux formulaires et champs personnalisés](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) et [Organiser et prévisualiser un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Suivi des modifications pour révision et approbation unifiées

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

La page Historique des modifications dans Workfront capture désormais l’activité dans les workflows de révision et d’approbation unifiés, offrant ainsi aux administrateurs et administratrices un journal complet de gouvernance pour les événements de cycle de vie des révisions et des documents.

Les actions d’approbation, d’étape et de participant sont désormais suivies. Ces actions peuvent inclure :

* Prendre une décision d’approbation dans la visionneuse Frame.io
* Créer ou supprimer une validation
* Mettre à jour un document, par exemple le renommer, le déplacer ou le supprimer

Chaque entrée comprend les champs suivis standard : date et heure, opération, nom d’utilisateur (ou « généré par le système ») et nom d’objet. Les activités du MCP sont capturées, y compris le LLM (comme Claude) qui a effectué la mise à jour. Les commentaires de la visionneuse Frame.io ne sont pas inclus.

Pour plus d&#39;informations, voir [Afficher et gérer l&#39;historique des modifications](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Définir une application personnalisée comme page de destination dans le modèle de mise en page

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Vous pouvez désormais définir une application personnalisée comme page de destination dans un modèle de mise en page. Les applications personnalisées qui ont déjà été ajoutées au menu principal peuvent être utilisées comme page de destination.

Les applications personnalisées doivent être créées séparément avant d&#39;être disponibles en tant qu&#39;options de menu principal ou de page de destination.

Pour plus d’informations, voir [Personnalisation de la page de destination à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md) et [Création d’applications personnalisées pour Workfront avec Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Configuration des champs suivis dans l’historique des modifications

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Vous pouvez ajouter des champs dont vous souhaitez effectuer le suivi pour un type d’objet particulier dans Workfront. Lorsque les utilisateurs modifient des informations dans ce champ, le système enregistre les informations relatives à la modification sous forme d&#39;entrée dans l&#39;historique des modifications.

Auparavant, l’écran de configuration permettant de définir les champs suivis était en lecture seule.

Pour plus d’informations, voir [Configurer les champs à suivre dans l’historique des modifications](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md).

## Accès administratif à l&#39;historique des modifications ajouté aux niveaux d&#39;accès

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Au niveau d&#39;accès standard, vous pouvez maintenant définir si les utilisateurs disposant de ce niveau doivent avoir accès à la liste Historique des modifications. L’option **Historique des modifications** est disponible dans la section **Autoriser l’accès administratif pour** au niveau de l’accès.

Pour plus d&#39;informations, consultez [Octroi aux utilisateurs d&#39;un accès administratif à certaines zones](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md) et [Affichage et gestion de l&#39;historique des modifications](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).


