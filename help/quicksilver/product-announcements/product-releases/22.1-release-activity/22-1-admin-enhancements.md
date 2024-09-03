---
title: 22.1 Améliorations apportées aux administrateurs et adminstratrices
description: 22.1 Améliorations apportées aux administrateurs et adminstratrices
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1452'
ht-degree: 100%

---

# 22.1 Améliorations apportées aux administrateurs et adminstratrices

Cette page décrit toutes les améliorations apportées aux administrateurs et adminstratrices avec la version 22.1 dans l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

Semaine du 17 janvier 2022.

Pour consulter la liste de tous les changements disponibles avec la version 22.1, voir [Vue d’ensemble de la version 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Téléchargements de documents enregistrés dans la zone Mises à jour

Pour aider vos utilisateurs et utilisatrices à suivre les téléchargements des documents qu’ils stockent dans Workfront, le système enregistre désormais une entrée dans la zone Mises à jour pour un document lorsque quelqu’un le télécharge.

>[!NOTE]
>
>Nous vous recommandons de tester cette fonctionnalité en prévisualisation sur un document nouvellement chargé.

Pour plus d’informations sur la façon dont Workfront consigne les mises à jour automatiques des objets, voir [Mises à jour suivies par le système](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Accorder l’accès aux équipes à l’aide des niveaux d’accès

Une nouvelle section dans la zone des niveaux d’accès vous permet de gérer plus finement l’accès de vos utilisateurs et utilisatrices aux équipes. Vous pouvez désormais déterminer qui peut créer, modifier et consulter les équipes.

Cela ne modifie pas l’accès existant de vos utilisateurs et utilisatrices aux équipes.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Mappage de groupe désormais disponible dans les plans directeurs

Certains plans directeurs incluent désormais des groupes, que vous pouvez personnaliser avant d’installer le plan directeur. Vous pouvez mapper un groupe du plan directeur à un groupe existant dans votre instance Workfront, ou créer un groupe si nécessaire.

Pour plus d’informations, voir [Configurer un plan directeur](../../../administration-and-setup/blueprints/configure-template-package.md).

## Mises à jour de style dans la zone Formulaires personnalisés

La zone des formulaires personnalisés a un nouvel aspect qui la met au diapason de nombreuses autres zones de la nouvelle expérience Workfront.

## De nombreuses améliorations ont été apportées à la création de champs personnalisés calculés.

La création de champs personnalisés calculés est désormais beaucoup plus facile grâce à ces ajouts dans le nouvel éditeur de calculs :

* Vous pouvez pointez sur n’importe quelle expression de votre calcul pour afficher des informations à son sujet, notamment une description, un exemple d’utilisation et un lien vers des informations complémentaires dans un article d’aide.
* Chaque expression que vous ajoutez est codée par une couleur, en fonction de son type. Il est ainsi plus facile de repérer vos expressions et de reconnaître immédiatement leur type.
* Les numéros de ligne permettent d’identifier et de référencer les fonctions dans un long calcul.
* Lorsque vous commencez à saisir une expression ou un nom de champ, une liste des éléments disponibles s’affiche afin que vous puissiez choisir celui que vous souhaitez. De plus, lorsque vous saisissez une parenthèse ouverte, la parenthèse fermante est ajoutée automatiquement.
* Vous pouvez prévisualiser le résultat de votre calcul à l’aide d’un objet existant sans quitter l’éditeur de calculs.

En outre, dans le texte personnalisable « Instructions », vous pouvez pointer sur un champ personnalisé calculé pour afficher ou masquer la formule du champ. Cela s’avère utile si vous pensez que les personnes qui remplissent le formulaire personnalisé n’auront pas besoin de ces informations.

## Afficher des informations du journal d’audit sur les statuts et les entreprises

Désormais, vous pouvez plus facilement résoudre les incidents concernant les statuts et les entreprises en affichant des informations à leur sujet dans la zone des journaux d’audit de la configuration.

Par exemple :

* Vous pouvez savoir qui a renommé, verrouillé ou masqué un statut et quand cela a été effectué.
* Vous pouvez savoir qui a supprimé certaines personnes membres ou certaines fonctions d’une entreprise, et quand cela a été effectué.

Pour plus d’informations sur l’affichage des informations du journal d’audit, voir [Afficher et exporter des journaux d’audit](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Mappage des entreprises avec les plans directeurs et autres améliorations

Les améliorations suivantes apportées aux plans directeurs sont désormais disponibles :

* Certains plans directeurs incluent désormais des entreprises, que vous pouvez personnaliser avant d’installer le plan directeur. Vous pouvez mapper une entreprise du plan directeur à une entreprise existante dans votre instance Workfront, ou créer une entreprise si nécessaire.
* Un nouveau type de plan directeur, Structure organisationnelle, est désormais disponible. Certains plans directeurs incluent des éléments de plusieurs types (par exemple, le modèle de projet et la structure organisationnelle). Vous pouvez filtrer par type de plan directeur sur la page du catalogue.
* Les sections « Installer les préférences » et « Propriété du modèle » sur la page de configuration ont été combinées dans « Préférences du modèle » pour plus de simplicité.

Pour plus d’informations, voir [Configurer un plan directeur](../../../administration-and-setup/blueprints/configure-template-package.md).

## Gérer plus facilement les appartenances à une entreprise

Dans la zone Entreprises, une barre d’outils actualisée facilite l’ajout de personnes Workfront existantes à une entreprise et la suppression de personnes membres d’une entreprise.

Auparavant, ces actions n’étaient disponibles que dans la zone de modification de l’entreprise.

La barre d’outils mise à jour comprend toutes les actions disponibles dans la barre d’outils précédente, comme la modification des informations de profil des utilisateurs et utilisatrices et la désactivation des personnes membres dans le système.

Pour plus d’informations, voir [Gérer les appartenances à une entreprise](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Sélectionner des expressions et des champs dans la nouvelle fenêtre de champ calculé

Nous continuons à faciliter la création d’un champ calculé dans un formulaire personnalisé. Désormais, lorsque vous cliquez sur Agrandir pour ouvrir le nouvel éditeur de calculs, vous pouvez trouver et sélectionner les expressions et les champs dont vous avez besoin.

## Les groupes peuvent configurer leurs propres préférences des feuilles de temps et des heures

>[!NOTE]
>
>Cette fonctionnalité était initialement disponible dans le cadre d’un déploiement par étapes uniquement pour les clientes et clients sur le cluster 4 dans le cadre de la version 21.4. Cette fonctionnalité sera disponible pour tous les clusters restants en production le 8 novembre 2021.

Dans une grande organisation, certains groupes peuvent avoir besoin de configurer les préférences des feuilles de temps et des heures de manière indépendante pour les adapter à leurs workflows uniques, plutôt que d’hériter des préférences configurées par une équipe d’administration au niveau du système. Désormais, l’équipe d’administration de Workfront peut déverrouiller les préférences en matière de feuilles de temps et d’heures pour tous les groupes du système afin qu’ils puissent les configurer.

Cette possibilité a également été ajoutée récemment pour les préférences de projet et pour celles de tâches et de problèmes.

Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront déverrouille une préférence de feuille de temps et d’heure, consultez la section [Déverrouiller les préférences des feuilles de temps et des heures pour les groupes](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) dans l’article [Configuration des préférences de feuilles de temps et des heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Pour plus d’informations sur la façon dont un administrateur ou une administratrice de groupes configure les préférences de tâche et de problème déverrouillés pour un groupe, voir [Configurer des préférences de feuilles de temps et des heures pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Sélectionner plusieurs notifications que vous souhaitez déverrouiller ou reverrouiller pour les groupes

Il est désormais plus rapide et plus facile de verrouiller ou déverrouiller les notifications par e-mail pour les groupes. Désormais, vous pouvez sélectionner plusieurs notifications, vérifier vos sélections pour vous assurer qu’elles sont correctes, puis cliquer sur le nouveau bouton « Déverrouiller » ou « Verrouiller » qui apparaît dans la barre d’outils.

Auparavant, vous deviez verrouiller et déverrouiller les notifications une par une. Actuellement, Workfront comprend 95 notifications, et cela prendrait beaucoup de temps si vous deviez toutes les configurer une par une.

Pour plus d’informations, voir [Déverrouiller ou verrouiller la configuration des notifications d’événements pour tous les groupes](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Pour les administrateurs et administratrices de groupes : il est plus facile de sélectionner un groupe de remplacement lorsque vous supprimez un groupe

Dans la zone de suppression de groupes, deux améliorations facilitent maintenant la sélection du groupe de remplacement pour préserver les utilisateurs et utilisatrices, les éléments de travail et les sous-groupes du groupe supprimé.

* Commencez à saisir le nom du groupe pour le trouver rapidement. Auparavant, il n’y avait qu’une liste déroulante dans laquelle vous ne pouviez pas taper. C’était problématique pour les organisations comportant de nombreux groupes, car il fallait faire défiler la liste pour trouver le groupe que vous vouliez. En outre, la liste déroulante avait une limite d’éléments. Il était donc possible que le groupe souhaité ne s’affiche pas.
* Utilisez la nouvelle icône d’information pour vous assurer que vous sélectionnez le groupe de remplacement que vous souhaitez. Placer le pointeur de la souris sur l’icône affiche une info-bulle répertoriant les informations sur le groupe, telles que la hiérarchie des groupes au-dessus et les noms de ses administrateurs et administratrices.

Pour plus d’informations, voir [Supprimer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Zone plus grande pour la création de champs calculés

Il est désormais plus facile de créer des champs calculés complexes dans un formulaire personnalisé. Cliquez sur le nouveau bouton Agrandir pour ouvrir une grande fenêtre d’édition afin de construire votre calcul. Lorsque vous avez terminé, cliquez sur Réduire pour continuer à travailler sur votre formulaire personnalisé.

## Ajouter des formulaires personnalisés à des groupes

Les formulaires personnalisés sont désormais pris en charge pour l’objet Groupe. Il est ainsi plus facile pour les groupes de votre organisation de capturer et de partager des informations qui répondent à leurs besoins spécifiques et à leurs workflows. Les utilisateurs et utilisatrices peuvent effectuer les opérations suivantes pour un groupe, comme pour d’autres objets Workfront :

* Créer un formulaire personnalisé
* Joindre un formulaire personnalisé
* Enregistrer les données du formulaire personnalisé
* Supprimer un formulaire personnalisé
* Modifier des données personnalisées à partir de listes et, dans la nouvelle expérience Workfront, à partir de la page Groupe

Pour plus d’informations sur les formulaires personnalisés, voir [Formulaires personnalisés](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Créer des applications OAuth2 pour intégrer des applications à Workfront

Vous pouvez désormais intégrer Workfront à d’autres applications pour lesquelles Workfront n’offre pas d’intégration intégrée. En créant une application OAuth2 pour l’application avec laquelle vous souhaitez vous intégrer, vous pouvez permettre à cette application d’accéder à Workfront, tout en sachant que vos données sont protégées par le protocole d’authentification OAuth2, sécurisé et conforme aux normes de l’industrie.

Auparavant, vous ne pouviez vous intégrer à d’autres applications que par le biais d’intégrations intégrées, de Workfront Fusion ou de l’API Workfront.

Pour plus d’informations, voir [Créer des applications OAuth2 pour les intégrations Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Améliorations du texte de l’interface dans la zone Entreprises

Dans la zone Entreprises dans Configuration, de nouveaux messages de confirmation et de légères modifications de la formulation facilitent la gestion des appartenances à une entreprise. Par exemple, le nom de section « Personnes » dans le panneau de gauche est désormais « Personnes membres de l’entreprise ».

Pour plus d’informations sur la gestion de l’appartenance à une entreprise, voir [Gérer l’appartenance à une entreprise](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
