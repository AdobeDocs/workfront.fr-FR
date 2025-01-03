---
title: Améliorations de la gestion de projets (version 20.4)
description: Améliorations de la gestion de projets (version 20.4)
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: 12bab42ab13935fa284aa334120afcfb602bf412
workflow-type: tm+mt
source-wordcount: '1365'
ht-degree: 100%

---

# Améliorations de la gestion de projets (version 20.4)

Cette page décrit toutes les améliorations apportées à la gestion des projets dans l’environnement de prévisualisation avec la version 20.4. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 9 novembre 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 20.4, voir [Vue d’ensemble de la version 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Nouveauté pour les administrateurs et administratrices : contrôle du partage d’un champ personnalisé

Pour vous offrir un meilleur contrôle sur les personnes qui peuvent modifier, supprimer et utiliser les champs personnalisés que vous créez, nous avons ajouté la possibilité de les configurer exactement selon la manière dont vous souhaitez les partager.

Jusqu’à présent, lorsque vous créiez un champ personnalisé, il était modifiable par tout le monde dans le système. Il s’agit toujours de l’état par défaut d’un champ personnalisé, mais vous pouvez désormais limiter le partage d’un champ personnalisé à certains utilisateurs et utilisatrices, rôles, équipes, groupes et entreprises. Vous pouvez également déterminer si vos personnes destinataires peuvent gérer ou uniquement afficher le champ personnalisé.

De plus, pour que cette expérience vous soit familière, nous avons conçu l’interface utilisateur afin que cette fonctionnalité soit similaire aux autres partages de zones d’objets dans Workfront.

## Nouveauté pour les administrateurs et les administratrices : partage normalisé de formulaires personnalisés

Nous avons normalisé le partage des formulaires personnalisés afin que vous puissiez utiliser le processus de partage d’objets Workfront que vous connaissez déjà. De plus, la nouvelle expérience de partage vous permet de mieux contrôler qui peut modifier, supprimer et utiliser les formulaires personnalisés que vous créez. Vous pouvez limiter le partage d’un formulaire personnalisé à certains utilisateurs et utilisatrices, rôles, équipes, groupes et entreprises. Vous pouvez également déterminer si ces personnes destinataires peuvent afficher ou gérer le formulaire personnalisé.

Pour plus d’informations, voir [Partager un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Exporter des formulaires personnalisés et des informations de vue d’ensemble à partir de la section Détails d’un projet, d’une tâche ou d’un problème

Vous pouvez désormais exporter les informations d’un formulaire personnalisé vers un fichier PDF. Vous pouvez exporter des formulaires personnalisés à partir de projets, de tâches ou de problèmes lorsque vous accédez au formulaire dans la section Détails des objets.

En plus de l’export de formulaires personnalisés de projets, de tâches et de problèmes, vous pouvez désormais inclure la zone Vue d’ensemble à votre PDF exporté.

Pour plus d’informations sur l’export de formulaires personnalisés à partir d’un objet, voir [Exporter des formulaires personnalisés et les détails d’un objet](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Ajouter rapidement une itération

>[!NOTE]
>
>Cette fonctionnalité a été temporairement supprimée de l’environnement de production. Cette page sera mise à jour lorsque la fonctionnalité sera disponible.

Pour simplifier l’expérience de création d’une itération, nous avons ajouté un nouveau bouton qui vous permet d’ajouter une itération à partir de l’onglet itérations. D’ici, vous pouvez créer une itération, puis ajouter des tâches et des problèmes ultérieurement.

Vous pouvez toujours créer une itération sur la balise de liste d’attente de travail comme auparavant.

Pour plus d’informations, voir [Créer une itération](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Nouvelle section Mesures disponible dans les projets

Pour gagner du temps et améliorer la compréhension de l’état général d’un projet, une section Mesures est désormais disponible dans un projet et inclut des informations sur les éléments suivants :

* Le travail terminé, incomplet, en retard et à venir
* Les quantités de tâches et de problèmes regroupées par statut ou par priorité
* Le travail affecté à chaque utilisateur ou utilisatrice

Vous pouvez effectuer des sélections dans les graphiques pour voir les différents aspects des tâches et des problèmes d’un projet, puis cliquer sur certains éléments pour afficher les informations d’une tâche.

<!--This feature is now included in the [Planner Fundamentals, Part 3 learning path](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) on Workfront One. -->

## Nouveauté pour les administrateurs et les administratrices : affecter un chef ou une cheffe d’entreprise à un groupe

Pour vous aider à mieux organiser et définir vos groupes, nous avons ajouté la possibilité d’affecter un utilisateur ou une utilisatrice à un groupe (ou à un sous-groupe) en tant que chef ou cheffe d’entreprise. Un chef ou une cheffe d’entreprise est un utilisateur ou une utilisatrice Workfront qui prend des décisions commerciales pour un groupe.

Le nouveau champ Chef ou cheffe d’entreprise peut être utilisé dans les filtres de rapports, les vues et les regroupements. Par exemple, vous pouvez filtrer selon un certain chef ou une certaine cheffe d’entreprise afin de n’afficher que les groupes pour lesquels cette personne est affectée à ce rôle.

Pour plus d’informations, voir [Vue d‘ensemble du rôle de chef ou cheffe d’entreprise](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## Nouveauté pour les administrateurs et les administratrices : association de portfolios, de programmes et d’entreprises à des groupes

Lorsque des administrateurs et des administratrices Workfront créent ou modifient un portfolio, un programme ou une entreprise, ils peuvent l’affecter à un groupe. Avec des groupes affectés à ces objets, il est facile d’identifier les responsabilités de votre groupe envers ces derniers.

Par exemple, vous pouvez répertorier tous les portfolios de votre entreprise dans un rapport et consulter la colonne Groupe pour voir sur lesquels votre groupe travaille.

Pour plus d’informations, voir la section « Association d’un groupe à un objet » dans l’article [Vue d’ensemble des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## Nouveauté pour les administrateurs et administratrices : les administrateurs et administratrices d’un groupe affecté à une entreprise peuvent gérer l’entreprise.

Nous avons facilité la gestion par un administrateur ou une administratrice de groupe d’une entreprise associée à son groupe dans Workfront. L’accès à la gestion de l’entreprise devient automatiquement disponible lorsque l’association est créée. Ceci est particulièrement important lorsque l’administrateur ou l’administratrice de groupe ne dispose pas d’un accès administratif aux entreprises.

Pour plus d’informations, voir [Créer et modifier des entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

Pour plus d’informations sur l’accès administratif aux entreprises, voir [Accorder aux utilisateurs et aux utilisatrices un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## Remplacer le bouton Travailler sur ce projet avec un bouton Démarrer

Pour faciliter la capture de la date et de l’heure de début réelles du travail sur un élément de travail, les utilisateurs et les utilisatrices peuvent remplacer le bouton Travailler sur ce projet par un bouton Démarrer qui met automatiquement à jour le statut et la Date de début effective de l’élément de travail.

Mise à jour du 24 septembre : après avoir cliqué sur Démarrer la tâche ou Démarrer le problème, vous avez désormais la possibilité de revenir sur votre choix et d’indiquer que vous n’êtes pas en mesure de commencer à travailler sur une tâche en cliquant sur Annuler. Le statut de l’élément de travail repasse en Nouveau et la Date d’engagement et la Date de début effective sont supprimées. L’option Annuler s’affiche pendant un court laps de temps et disparaît lorsque que vous quittez la page ou que vous l’actualisez.

Pour plus d’informations sur la configuration de cette option, voir [Remplacer le bouton Travailler sur ce projet par un bouton Démarrer](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

<!--This feature is now included in the [Worker Fundamentals learning path](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) and the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## Autoriser plusieurs brouillons pour une rubrique de file d’attente

Pour vous donner plus de liberté lorsque vous utilisez des demandes, il n’y a désormais plus de limite de nombre de brouillons que vous pouvez enregistrer pour une rubrique de file d’attente donnée. Lors de la création d’une nouvelle demande, vous pouvez sélectionner un brouillon existant dans une liste de brouillons pour la même rubrique de file d’attente, le remplacer et l’envoyer en tant que nouvelle demande. Vous pouvez également créer une nouvelle demande à partir de zéro.

Avant cette amélioration, Workfront n’enregistrait qu’un seul brouillon pour chaque rubrique de file d’attente de votre file d’attente des demandes.

Pour plus d’informations sur l’envoi de demandes, voir [Créer et soumettre des demandes Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Affecter un groupe à une équipe

Pour faciliter la gestion et des équipes associées à un groupe ainsi que la création de rapports sur celles-ci, vous pouvez désormais affecter n’importe quel groupe à une équipe sur laquelle vous disposez d’un accès de modification.

Lorsque vous affectez une équipe à un groupe, ses administrateurs et administratrices de groupes peuvent gérer l’équipe sans en être membre. Sur la page Détails de l’équipe, ceux-ci peuvent voir les équipes affectées aux groupes qu’ils gèrent. Ils peuvent également exécuter un rapport pour répertorier toutes les équipes associées à un certain groupe.

Pour plus d’informations, voir [Créer une équipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## Les nouveaux champs vous permettent de créer des rapports sur les données d’un groupe de niveau supérieur et de l’ensemble de ses sous-groupes.

Pour vous aider à identifier les données associées à un groupe de niveau supérieur et à ses sous-groupes, nous avons ajouté un nouveau champ Identifiant de parent supérieur que vous pouvez utiliser dans Filtres, Vues et Regroupements lorsque vous créez des rapports sur des objets de type Groupe.

Ce champ est particulièrement utile pour les administrateurs et les administratrices de groupes qui gèrent des groupes comportant plusieurs sous-groupes.

Imaginez, par exemple, que vous gérez un groupe appelé Marketing qui comporte les sous-groupes Marketing de terrain et Marketing numérique. Vous pouvez répertorier les projets qui appartiennent aux trois groupes en créant un filtre de zone Projets qui inclut la règle de filtrage suivante :
<pre>Groupe : Nom du parent principal &gt; Égal &gt; Marketing</pre>Nous avons également ajouté un nouveau champ Nom du parent principal que vous pouvez utiliser pour identifier les données associées aux groupes de niveau supérieur dans Vues (pas dans Filtres ni Regroupements).

Pour plus d’informations sur l’utilisation des champs dans les listes et les rapports, voir [Glossaire de la terminologie Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Nouvelle option pour annuler votre action lors de l’abandon d’un brouillon de requête

Lorsque vous abandonnez un brouillon enregistré, vous pouvez maintenant cliquer sur Annuler dans le message de confirmation qui vous informe que votre brouillon sera supprimé. De cette façon, vous ne perdez pas le brouillon au cas où vous décidez de ne plus l’abandonner.

Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Workfront. Pour plus d’informations, voir [Créer et envoyer des demandes Workfront](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html).

