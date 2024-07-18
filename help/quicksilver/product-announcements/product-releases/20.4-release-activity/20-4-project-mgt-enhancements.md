---
title: Améliorations de la gestion de projets (version 20.4)
description: Améliorations de la gestion de projets (version 20.4)
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1474'
ht-degree: 1%

---

# Améliorations de la gestion de projets (version 20.4)

Cette page décrit toutes les améliorations apportées à la gestion de projet avec la version 20.4 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production durant la semaine du 9 novembre 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 20.4, consultez la [présentation de la version 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Nouveau pour les administrateurs : contrôle du partage d’un champ personnalisé

Pour vous donner un meilleur contrôle sur les personnes qui peuvent modifier, supprimer et utiliser des champs personnalisés que vous créez, nous avons ajouté la possibilité de configurer exactement la manière dont vous souhaitez les partager.

Jusqu’à présent, lorsque vous avez créé un champ personnalisé, il était modifiable par tous les membres du système. Il s’agit toujours de l’état par défaut d’un champ personnalisé, mais vous pouvez désormais limiter le partage d’un champ personnalisé à certains utilisateurs, rôles, équipes, groupes et entreprises. Et vous pouvez déterminer si vos destinataires peuvent gérer ou afficher uniquement le champ personnalisé.

En outre, pour que cette expérience vous soit familière, nous avons conçu l’interface utilisateur afin que cette fonctionnalité soit similaire aux autres zones d’objet partageant sur Workfront.

## Nouveau pour les administrateurs : partage de formulaires personnalisés normalisé

Nous avons normalisé le partage pour les Forms personnalisées afin que vous puissiez utiliser le même processus de partage d’objet Workfront que vous connaissez déjà. De plus, la nouvelle expérience de partage vous permet de mieux contrôler qui peut modifier, supprimer et utiliser le Forms personnalisé que vous créez. Vous pouvez limiter le partage d’un formulaire personnalisé à certains utilisateurs, rôles, équipes, groupes et entreprises. Et vous pouvez déterminer si ces destinataires peuvent afficher ou gérer le formulaire personnalisé.

Pour plus d’informations, voir [Partage d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Exportation de formulaires personnalisés et informations d’aperçu à partir de la section Détails d’un projet, d’une tâche ou d’un problème

Vous pouvez désormais exporter les informations de formulaire personnalisées vers un fichier .pdf. Vous pouvez exporter des formulaires personnalisés à partir de projets, de tâches ou de problèmes lorsque vous accédez au formulaire dans la section Détails des objets.

Outre l’exportation de formulaires personnalisés de projets, de tâches et de problèmes, vous pouvez désormais inclure la zone Aperçu à votre PDF exporté.

Pour plus d’informations sur l’exportation de formulaires personnalisés à partir d’un objet, voir [Exportation de formulaires personnalisés et de détails d’objet](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Ajouter rapidement une itération

>[!NOTE]
>
>Cette fonctionnalité a été temporairement supprimée de l’environnement de production. Cette page sera mise à jour lorsque la fonctionnalité sera disponible.

Pour simplifier la création d&#39;une itération, nous avons ajouté un nouveau bouton qui permet d&#39;ajouter une itération depuis l&#39;onglet itérations . Ici, vous pouvez créer une itération, puis ajouter des tâches et des problèmes ultérieurement.

Vous pouvez toujours créer une itération sur la balise de journal comme auparavant.

Pour plus d’informations, voir [Création d’une itération](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Nouvelle section Mesures disponible dans les projets

Pour gagner du temps et améliorer la compréhension de l’intégrité globale d’un projet, une section Mesures est désormais disponible dans un projet qui comprend des informations sur les éléments suivants :

* Travail terminé, incomplet, en retard et à venir
* Sommes des tâches et des problèmes regroupées par statut ou priorité
* Travail assigné à chaque utilisateur

Vous pouvez effectuer des sélections dans les graphiques pour voir les différents aspects des tâches et problèmes d’un projet, puis cliquer sur certains éléments pour afficher les informations sur la tâche.

Cette fonctionnalité est désormais incluse dans les [Principes de planification, Partie 3 du parcours d’apprentissage](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) sur Workfront One.

## Nouveau destiné aux administrateurs : Affectation d’un chef d’entreprise à un groupe

Pour vous aider à mieux organiser et définir vos groupes, nous avons ajouté la possibilité d’affecter un utilisateur en tant que chef d’entreprise à un groupe (ou sous-groupe). Un chef d’entreprise est un utilisateur de Workfront qui prend des décisions commerciales pour un groupe.

Le nouveau champ Business Leader peut être utilisé dans les filtres de rapports, les vues et les regroupements. Par exemple, vous pouvez filtrer selon un certain chef d’entreprise afin de n’afficher que les groupes pour lesquels cette personne est affectée à ce rôle.

Pour plus d’informations, voir [Présentation du chef de l’entreprise](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

Cette fonctionnalité est désormais incluse dans les [fondamentaux de l’administrateur, parcours d’apprentissage Partie 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) sur Workfront One.

## Nouveautés pour les administrateurs : Association de portefeuilles, de programmes et d’entreprises à des groupes

Lorsque les administrateurs Workfront créent ou modifient un portfolio, un programme ou une entreprise, ils peuvent l’affecter à un groupe. Avec des groupes affectés à ces objets, il est facile d’identifier les responsabilités de votre groupe pour eux.

Par exemple, vous pouvez répertorier tous les portefeuilles de votre entreprise dans un rapport et consulter la colonne Groupe pour voir sur lesquels votre groupe travaille.

Pour plus d’informations, voir la section &quot;A propos de l’association d’un groupe à un objet&quot; dans l’article [Présentation des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Cette fonctionnalité est désormais incluse dans les [fondamentaux de l’administrateur, parcours d’apprentissage Partie 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) sur Workfront One.

## Nouveau destiné aux administrateurs : les administrateurs d’un groupe affecté à une entreprise peuvent gérer l’entreprise.

Nous avons facilité la gestion par un administrateur de groupe d’une entreprise associée à son groupe dans Workfront. L’accès à la gestion de l’entreprise est automatiquement disponible lorsque l’association est créée. Ceci est particulièrement important lorsque l’administrateur de groupe n’a pas d’accès administratif aux entreprises.

Pour plus d’informations, voir [Création et modification d’entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

Pour plus d&#39;informations sur l&#39;accès administratif aux entreprises, voir [Octroi aux utilisateurs d&#39;un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Cette fonctionnalité est désormais incluse dans les [fondamentaux de l’administrateur, parcours d’apprentissage Partie 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) sur Workfront One.

## Remplacer le bouton Travailler sur ce projet par un bouton Démarrer

Pour vous aider à capturer la date et l’heure du début réel du travail sur un élément de travail, les utilisateurs peuvent remplacer le bouton Travailler dessus par un bouton Début qui met automatiquement à jour l’état et la Date de début réelle de l’élément de travail.

Mise à jour le 24 septembre : après avoir cliqué sur Démarrer la tâche ou Démarrer le problème, vous avez désormais la possibilité de rétablir votre choix et d’indiquer que vous ne serez peut-être pas prêt à commencer à travailler sur une tâche en cliquant sur Annuler. L’élément de travail revient à l’état Nouveau et la Date de validation et la Date de début réelle sont supprimées. L’option Annuler s’affiche pendant une très courte période et est effacée une fois que vous avez quitté la page ou que vous l’avez actualisée.

Pour plus d&#39;informations sur la configuration de cette option, voir le bouton [Remplacer le travail dessus par un bouton Démarrer](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Cette fonctionnalité est désormais incluse dans le [chemin d’apprentissage des fondamentaux du traitement](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) et dans les [fondamentaux de l’administrateur, chemin d’apprentissage de la partie 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) sur Workfront One.

## Autorisation de plusieurs brouillons pour une rubrique de file d’attente

Pour vous donner plus de liberté lors de l’utilisation de requêtes, il n’existe plus de limite pour le nombre de brouillons que vous pouvez enregistrer pour une rubrique de file d’attente. Lors de la création d’une nouvelle requête, vous pouvez sélectionner un brouillon existant dans une liste de brouillons pour la même rubrique de file d’attente, le remplacer et l’envoyer en tant que nouvelle requête. Vous pouvez également créer une nouvelle requête à partir de zéro.

Avant cette amélioration, Workfront n’enregistrait qu’un seul brouillon pour chaque rubrique de file d’attente de votre file d’attente de requêtes.

Pour plus d’informations sur l’envoi de requêtes, voir &quot; [Création et envoi de requêtes Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)&quot;.

## Affectation d’un groupe à une équipe

Pour faciliter la gestion et la création de rapports sur les équipes associées à un groupe, vous pouvez désormais affecter n’importe quel groupe à une équipe que vous avez accès à la modification.

Lorsque vous affectez une équipe à un groupe, ses administrateurs de groupe peuvent gérer l’équipe sans en être membre. Sur la page Détails de l’équipe , ils peuvent voir les équipes affectées aux groupes qu’ils gèrent. Et ils peuvent exécuter un rapport pour répertorier toutes les équipes associées à un certain groupe.

Pour plus d’informations, voir [Création d’une équipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Cette fonctionnalité est désormais incluse dans les [fondamentaux de l’administrateur, parcours d’apprentissage Partie 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) sur Workfront One.

## Les nouveaux champs vous permettent de créer des rapports sur les données d’un groupe de niveau supérieur et de tous ses sous-groupes.

Pour vous aider à identifier les données associées à un groupe de niveau supérieur et à ses sous-groupes, nous avons ajouté un nouveau champ Identifiant parent supérieur que vous pouvez utiliser dans Filtres, Vues et Groupes lorsque vous créez des rapports sur les objets Groupe.

Ce champ doit être particulièrement utile pour les administrateurs de groupe qui gèrent les groupes qui contiennent plusieurs sous-groupes.

Imaginez, par exemple, que vous gériez un groupe appelé Marketing qui comporte les sous-groupes Marketing par champs et Marketing numérique. Vous pouvez répertorier les projets appartenant aux trois groupes en créant un filtre de zone Projets qui comporte la règle de filtrage suivante :
<pre>Groupe : Nom du parent supérieur &gt; Égal &gt; Marketing</pre>Nous avons également ajouté un nouveau champ Nom du parent supérieur que vous pouvez utiliser pour identifier les données associées aux groupes de niveau supérieur dans les vues (et non dans les filtres ou les groupes).

Pour plus d’informations sur l’utilisation des champs dans les listes et les rapports, voir [Glossaire de la terminologie Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Nouvelle option pour annuler votre action lors de l’abandon d’un brouillon de requête

Lorsque vous ignorez un brouillon enregistré, vous pouvez maintenant cliquer sur Annuler dans le message de confirmation qui vous informe que votre brouillon sera supprimé. De cette façon, vous ne perdez pas le brouillon au cas où vous changeriez d&#39;avis sur le rejet.

Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Workfront. Pour plus d’informations, voir [Création et envoi de requêtes Workfront](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html).

