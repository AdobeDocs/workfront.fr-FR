---
title: 2.1 Améliorations apportées aux administrateurs
description: 2.1 Améliorations apportées aux administrateurs
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# 2.1 Améliorations apportées aux administrateurs

Cette page décrit toutes les améliorations apportées par l’administrateur à la version 22.1 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semaine du 17 janvier 2022.

Pour obtenir la liste de toutes les modifications disponibles avec la version 22.1, voir [Présentation de la version 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Téléchargements de documents connectés dans la zone Mises à jour

Pour aider vos utilisateurs à effectuer le suivi des téléchargements de documents qu’ils stockent dans Workfront, le système consigne désormais une entrée dans la zone Mises à jour d’un document lorsqu’un utilisateur le télécharge.

>[!NOTE]
>
>Nous vous recommandons de tester cette fonctionnalité dans l’aperçu d’un nouveau document téléchargé.

Pour plus d’informations sur la façon dont Workfront consigne les mises à jour automatiques des objets, voir [Mises à jour suivies par le système](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Accorder l’accès aux équipes à l’aide des niveaux d’accès

Une nouvelle section de la zone Niveaux d’accès vous donne des contrôles plus précis pour gérer l’accès de vos utilisateurs aux équipes. Vous pouvez désormais déterminer qui peut créer, modifier et afficher des équipes.

Cela ne modifie pas l’accès existant de vos utilisateurs aux équipes.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Mappage de groupe désormais disponible dans les plans directeurs

Certains plans directeurs incluent désormais des groupes que vous pouvez personnaliser avant d’installer le plan directeur. Vous pouvez mapper un groupe du plan directeur à un groupe existant dans votre instance Workfront ou créer un groupe si nécessaire.

Pour plus d’informations, voir [Configuration d’un plan directeur](../../../administration-and-setup/blueprints/configure-template-package.md).

## Mises à jour de style dans la zone Forms personnalisée

La zone Forms personnalisée a une nouvelle apparence qui la met à jour avec de nombreux autres domaines de la nouvelle expérience Workfront.

Pour plus d’informations sur la création d’un formulaire personnalisé, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## De nombreuses améliorations ont été apportées à la création de champs personnalisés calculés

La création de champs personnalisés calculés est désormais beaucoup plus facile avec ces ajouts dans le nouvel éditeur de calcul :

* Vous pouvez placer le pointeur de la souris sur une expression de votre calcul pour afficher des informations à son sujet, notamment une description, un exemple d’utilisation et un lien vers d’autres informations dans un article d’aide.
* Chaque expression que vous ajoutez est codée par couleur, selon son type. Cela facilite l’identification de vos expressions et la reconnaissance immédiate de leur type.
* Les numéros de ligne permettent d&#39;identifier et de référencer des fonctions dans un calcul long.
* Lorsque vous commencez à saisir une expression ou un nom de champ, une liste des éléments disponibles s’affiche afin que vous puissiez choisir celui qui vous intéresse. Et lorsque vous entrez une parenthèse ouverte, la parenthèse fermante est ajoutée automatiquement.
* Vous pouvez prévisualiser le résultat de votre calcul à l’aide d’un objet existant, sans quitter l’éditeur de calcul.

En outre, dans le texte personnalisable &quot;Instructions&quot;, vous pouvez pointer sur un champ personnalisé calculé pour afficher ou masquer la formule du champ. Cela s’avère utile si vous pensez que les utilisateurs qui remplissent le formulaire personnalisé n’auront pas besoin de ces informations.

Pour plus d’informations sur la création d’un champ personnalisé calculé, voir [Ajout de données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Affichage des informations du journal d’audit sur les états et les entreprises

Vous pouvez désormais résoudre plus facilement les problèmes liés aux états et aux entreprises en affichant des informations les concernant dans la zone Journaux d’audit de la configuration.

Par exemple :

* Vous pouvez déterminer qui a renommé, verrouillé ou masqué un statut, et quand il l’a fait.
* Vous pouvez découvrir qui a supprimé certains membres ou rôles d’emploi d’une entreprise, et quand ils l’ont fait.

Pour plus d’informations sur l’affichage des informations du journal d’audit, voir [Affichage et exportation des journaux d’audit](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Mappage des entreprises avec les plans directeurs et autres améliorations

Les améliorations suivantes apportées aux plans directeurs sont désormais disponibles :

* Certains plans directeurs incluent désormais des entreprises, que vous pouvez personnaliser avant d’installer le plan directeur. Vous pouvez mapper une société du plan directeur à une société existante dans votre instance Workfront ou créer une société si nécessaire.
* Un nouveau type de plan directeur, Structure organisationnelle, est désormais disponible. Certains plans directeurs incluent des éléments de plusieurs types (par exemple, le modèle de projet et la structure organisationnelle). Vous pouvez filtrer par type de plan directeur sur la page du catalogue.
* Les sections &quot;Installer les préférences&quot; et &quot;Propriété du modèle&quot; sur la page de configuration ont été combinées dans &quot;Préférences du modèle&quot; pour plus de simplicité.

Pour plus d’informations, voir [Configuration d’un plan directeur](../../../administration-and-setup/blueprints/configure-template-package.md).

## Gérer plus facilement les appartenances à une entreprise

Dans la zone Sociétés, une barre d’outils mise à jour permet d’ajouter facilement des utilisateurs Workfront existants à une entreprise et de supprimer des membres de cette dernière.

Auparavant, ces actions n’étaient disponibles que dans la zone Modifier la société .

La barre d’outils mise à jour contient également toutes les actions disponibles dans la barre d’outils précédente, telles que la modification des informations de profil utilisateur des membres et leur désactivation dans le système.

Pour plus d’informations, voir [Gestion des appartenances à une entreprise](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Sélectionner des expressions et des champs dans la nouvelle fenêtre de champ calculé

Nous continuons à faciliter la création d’un champ calculé dans un formulaire personnalisé. Désormais, lorsque vous cliquez sur Maximiser pour ouvrir le nouvel éditeur de calcul, vous pouvez rechercher et sélectionner les expressions et les champs dont vous avez besoin.

Pour plus d’informations, voir [Ajout de données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Les groupes peuvent configurer leurs propres préférences de feuille de temps et d’heure.

>[!NOTE]
>
>Cette fonctionnalité était initialement disponible dans le cadre d’un déploiement par étapes uniquement pour les clients sur la grappe 4 dans le cadre de la version 21.4. Cette fonctionnalité sera disponible pour toutes les grappes restantes en production le 8 novembre 2021.

Dans une grande entreprise, certains groupes peuvent avoir besoin de configurer les préférences de la feuille de temps et de l’heure indépendamment pour s’adapter à leurs workflows uniques, plutôt que d’hériter des préférences configurées par un administrateur au niveau du système. Désormais, les administrateurs de Workfront peuvent déverrouiller les préférences de feuille de temps et d’heure pour tous les groupes du système afin de pouvoir les configurer eux-mêmes.

Cette fonctionnalité a également été ajoutée récemment pour les préférences de projet et de tâche et de problème.

Pour plus d’informations sur la façon dont un administrateur Workfront déverrouille une feuille de temps et des préférences d’heure, consultez la section . [Déverrouiller les préférences de feuille de temps et d’heure pour les groupes ;](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) dans l’article [Configuration des préférences de feuille de temps et d’heure](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Pour plus d’informations sur la façon dont un administrateur de groupe configure une tâche déverrouillée et les préférences de problème pour un groupe, voir [Configuration des préférences de feuille de temps et d’heure pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Sélectionner plusieurs notifications que vous souhaitez déverrouiller ou reverrouiller pour les groupes

Déverrouiller ou reverrouiller les notifications électroniques pour les groupes est désormais plus rapide et plus facile. Vous pouvez maintenant sélectionner plusieurs notifications, vérifier vos sélections pour vous assurer qu’elles sont correctes, puis cliquer sur le nouveau bouton Déverrouiller ou Verrouiller qui s’affiche dans la barre d’outils.

Auparavant, vous deviez déverrouiller et reverrouiller les notifications une par une. Workfront comporte actuellement 95 notifications, donc cela a pris un certain temps si vous deviez le faire pour toutes ou plusieurs d’entre elles.

Pour plus d’informations, voir [Déverrouiller ou verrouiller la configuration des notifications d’événement pour tous les groupes](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Pour les administrateurs de groupe : il est plus facile de sélectionner un groupe de remplacement lorsque vous supprimez un groupe.

Lorsque vous supprimez un groupe, deux améliorations de la zone Supprimer le groupe permettent de sélectionner plus facilement le groupe de remplacement dont vous souhaitez conserver les utilisateurs, les tâches et les sous-groupes du groupe supprimé :

* Vous pouvez saisir le nom du groupe pour le trouver rapidement. Auparavant, vous ne pouviez entrer que la liste déroulante. C’était problématique pour les organisations comportant de nombreux groupes, car il fallait faire défiler la liste pour trouver le groupe que vous vouliez. En outre, la liste déroulante contenait une limite d’éléments. Il était donc possible que le groupe souhaité ne s’affiche pas.
* Vous pouvez utiliser la nouvelle icône d’informations pour vous assurer que vous sélectionnez le groupe de remplacement souhaité. Placez le pointeur de la souris sur l’icône pour afficher une info-bulle contenant des informations sur le groupe, telles que la hiérarchie des groupes au-dessus et les noms de ses administrateurs.

Pour plus d’informations, voir [Suppression d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Zone plus grande pour la création de champs calculés

Il est désormais plus facile de créer des champs calculés complexes dans un formulaire personnalisé. Cliquez sur le nouveau bouton Maximiser pour ouvrir une grande fenêtre d’édition afin de créer votre calcul. Lorsque vous avez terminé, cliquez sur Réduire pour continuer à travailler sur votre formulaire personnalisé.

Pour plus d’informations, voir [Ajout de données calculées à un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Ajout de formulaires personnalisés à des groupes

Les formulaires personnalisés sont désormais pris en charge pour l’objet Group. Cela permet aux groupes de votre entreprise de capturer et de partager plus facilement des informations qui répondent à leurs besoins spécifiques et à leurs workflows. Les utilisateurs peuvent effectuer les opérations suivantes pour un groupe, comme pour d’autres objets Workfront :

* Création d’un formulaire personnalisé
* Joindre un formulaire personnalisé
* Enregistrer les données de formulaire personnalisées
* Suppression d’un formulaire personnalisé
* Modifier des données personnalisées à partir de listes et, dans la nouvelle expérience Workfront, à partir de la page Groupe

Pour plus d’informations sur les formulaires personnalisés, voir [Formulaires personnalisés](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Création d’applications OAuth2 pour intégrer des applications à Workfront

Vous pouvez désormais intégrer Workfront à d’autres applications pour lesquelles Workfront ne propose pas d’intégration intégrée. En créant une application OAuth2 pour l’application que vous souhaitez intégrer, vous pouvez autoriser cette application à accéder à Workfront, tout en sachant que vos données sont protégées par le protocole d’authentification OAuth2 sécurisé et standard.

Auparavant, vous pouviez uniquement intégrer à d’autres applications par le biais d’intégrations intégrées, de Workfront Fusion ou de l’API Workfront.

Pour plus d’informations, voir [Création d’applications OAuth2 pour les intégrations Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Améliorations du texte de l’interface dans la zone Entreprises

Dans la zone Entreprises de la configuration, de nouveaux messages de confirmation et de légères modifications de la formulation facilitent la gestion des adhésions aux entreprises. Par exemple, le nom de section &quot;Personnes&quot; dans le panneau de gauche est désormais &quot;Membres de la société&quot;.

Pour plus d’informations sur la gestion des adhésions aux entreprises, voir [Gestion des appartenances à une entreprise](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
