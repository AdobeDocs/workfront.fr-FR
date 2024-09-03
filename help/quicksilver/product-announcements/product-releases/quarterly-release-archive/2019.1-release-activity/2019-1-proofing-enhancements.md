---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Améliorations apportées à la relecture dans la version 2019.1
description: Cette page décrit toutes les améliorations apportées à la relecture incluses dans la version 2019.1. Cette fonctionnalité est désormais disponible dans l’environnement de production.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 100%

---

# Améliorations apportées à la relecture dans la version 2019.1

Cette page décrit toutes les améliorations apportées à la relecture incluses dans la version 2019.1. Cette fonctionnalité est désormais disponible dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2019.1, consultez la section [Vue d’ensemble de l’activité de la version 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Pour les administrateurs et administratrices

* [Configurer le rôle de relecture par défaut pour les personnes non-destinataires ayant ouvert une épreuve](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## Pour tous les utilisateurs et utilisatrices

* [Contenu interactif de l’épreuve dans la visionneuse de relecture web](#proof-interactive-content-in-the-web-proofing-viewer)
* [L’ordre de tri par défaut des commentaires dans la visionneuse de relecture est désormais du plus ancien au plus récent.](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [Amélioration de la révision des commentaires dans la visionneuse de relecture associée à une plage de vidéos](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [Lien vers les détails du document à partir d’une notification d’épreuve ou de la visionneuse de relecture](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [Modifier vos notifications par e-mail dans la visionneuse de relecture](#change-your-email-notifications-in-the-proofing-viewer)
* [Modifier la couleur d’arrière-plan dans la visionneuse de relecture de bureau](#change-the-background-color-in-the-desktop-proofing-viewer)
* [Effacer les données du navigateur mises en cache à partir d’une épreuve dans la visionneuse de relecture de bureau](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## Configurer le rôle de relecture par défaut pour les personnes non-destinataires ayant ouvert une épreuve {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Les administrateurs et les administratrices Workfront peuvent désormais configurer le rôle de relecture par défaut pour les personnes qui ne sont pas désignées comme destinataires dans le workflow de l’épreuve, mais qui ont accès à l’épreuve via son objet Workfront (projet, tâche ou problème, par exemple).

Auparavant, lorsque les utilisateurs et utilisatrices et les personnes invitées avaient accès à une épreuve sans être ajoutés à son workflow, leur rôle de relecture par défaut était personne réviseuse.

Cette fonctionnalité s’applique uniquement aux épreuves créés dans Workfront, et non dans Workfront Proof.

## Contenu interactif de l’épreuve dans la visionneuse de relecture web {#proof-interactive-content-in-the-web-proofing-viewer}

Si les politiques de sécurité de votre entreprise n’autorisent pas l’utilisation de l’application de la visionneuse de relecture de bureau autonome, votre administrateur ou administratrice Workfront peut désormais activer le contenu interactif dans la visionneuse de relecture web. Le contenu doit être regroupé dans un fichier ZIP avant de créer l’épreuve.

Pour plus d’informations, voir l’article .

VIDÉO

## L’ordre de tri par défaut des commentaires dans la visionneuse de relecture est désormais du plus ancien au plus récent.  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

Dans la visionneuse de relecture, l’ordre de tri par défaut des commentaires sur une épreuve est désormais du plus ancien au plus récent, comme dans une conversation verbale.

Auparavant, l’ordre de tri par défaut était du plus récent au plus ancien.

Vous pouvez sélectionner une autre option de tri qui sera mémorisée pour toutes les autres épreuves que vous ouvrirez.

Pour plus d’informations, reportez-vous à la section de l’article .

## Amélioration de la révision des commentaires dans la visionneuse de relecture associée à une plage de vidéos {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

Lorsque vous révisez un commentaire associé à une plage d’enregistrements vidéo dans la visionneuse de relecture, vous pouvez désormais cliquer sur Lecture pour afficher l’ensemble des enregistrements. La lecture s’interrompt lorsqu’elle atteint la fin de la plage. Le commentaire reste ouvert afin que vous ne perdiez pas de vue où vous êtes.

Auparavant, lorsque vous ouvriez un commentaire pour une plage d’enregistrements vidéo, vous deviez rechercher manuellement le début de la plage en observant les numéros d’images affichés sur le commentaire avant de cliquer sur Lecture. Sinon, la visionneuse de relecture commençait la lecture à l’endroit où vous cliquiez pour la dernière fois dans la chronologie de la vidéo et elle ne s’arrêtait pas à la fin de la plage. En outre, le commentaire se réduisait lorsque vous cliquiez sur Lecture, si bien que vous ne saviez plus clairement quel commentaire vous étiez en train de réviser.

Pour plus d’informations sur la révision des épreuves vidéo, voir .

VIDÉO

## Lien vers les détails du document à partir d’une notification d‘épreuve ou de la visionneuse de relecture {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

Lorsque vous recevez un e-mail vous invitant à réviser une épreuve ou que vous révisez une épreuve dans la visionneuse de relecture, vous pouvez maintenant accéder rapidement à la page Détails du document de l’épreuve. Sur cette page, vous pouvez voir l’objet Workfront (tel qu’une tâche, un projet ou un problème) associé à l‘épreuve. Cela fournit un contexte pour vous aider à comprendre le travail que vous devez faire sur l‘épreuve.

Il se peut que cette fonctionnalité ne fonctionne que pour les nouvelles personnes que vous ajoutez à votre système. Ce problème est temporaire.

Pour plus d’informations, consultez l’article .

VIDÉO

## Modifier vos notifications par e-mail dans la visionneuse de relecture {#change-your-email-notifications-in-the-proofing-viewer}

Désormais, toutes les personnes chargées de la relecture peuvent spécifier les notifications qu’elles souhaitent recevoir pour une épreuve. Ceci est particulièrement important lors de la collaboration avec des parties prenantes externes.

Auparavant, la configuration des notifications d’épreuves par e-mail pour les personnes en charge de leur révision ne pouvait être effectuée que par la personne propriétaire de l’épreuve ou responsable du trafic. Les personnes collaboratrices externes ne pouvaient pas gérer les notifications par e-mail relatives à l’épreuve car elles n’avaient ni l’accès nécessaire à Workfront, ni les autorisations requises.

Ces paramètres sont distincts des paramètres de notification par e-mail que vous pouvez configurer dans Workfront.

Pour plus d’informations, voir la section [Gérer les notifications pour les commentaires et les décisions sur des épreuves](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

VIDÉO

## Modifier la couleur d’arrière-plan dans la visionneuse de relecture de bureau {#change-the-background-color-in-the-desktop-proofing-viewer}

Vous pouvez désormais modifier la couleur d’arrière-plan de la visionneuse de relecture de bureau, de la couleur par défaut proche du noir à la couleur blanche. Il est ainsi plus facile de réviser le contenu d’une épreuve qui a un arrière-plan transparent.

Pour plus d’informations, consultez la section [Configurer les paramètres de la visionneuse de relecture](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDÉO

## Effacer les données du navigateur mises en cache à partir d’une épreuve dans la visionneuse de relecture de bureau {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

La configuration de votre navigateur pour bloquer des éléments comme les fenêtres pop-up peut interférer avec la visionneuse de relecture de bureau, empêchant les personnes chargées de la révision de voir et de commenter le contenu des fenêtres pop-up dans votre épreuve.

Vous pouvez maintenant effacer les données de cache stockées par votre navigateur pour une épreuve, assurant ainsi que l’intégralité du contenu soit accessible et commentable dans la visionneuse de relecture de bureau pour les personnes chargées de la révision.

Pour plus d’informations, consultez la section [Configurer les paramètres de la visionneuse de relecture](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDÉO
