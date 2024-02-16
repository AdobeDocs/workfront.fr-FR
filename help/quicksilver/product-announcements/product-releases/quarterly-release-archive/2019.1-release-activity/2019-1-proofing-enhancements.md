---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 Améliorations de la vérification
description: Cette page décrit toutes les améliorations de vérification incluses dans la version 2019.1. Cette fonctionnalité est désormais disponible dans l’environnement de production.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# 2019.1 Améliorations de la vérification

Cette page décrit toutes les améliorations de vérification incluses dans la version 2019.1. Cette fonctionnalité est désormais disponible dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2019.1, voir [Présentation de l’activité de la version 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Pour les administrateurs

* [Configuration du rôle de vérification par défaut pour les non-destinataires ayant ouvert un bon à tirer](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## Pour tous les utilisateurs

* [Contenu interactif de BAT dans la visionneuse de BAT Web](#proof-interactive-content-in-the-web-proofing-viewer)
* [L’ordre de tri par défaut des commentaires dans la visionneuse de vérification est désormais le plus ancien au plus récent](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [Amélioration de la révision des commentaires dans la visionneuse de vérification associée à une plage de vidéos](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [Lien vers les détails du document à partir d’une notification de BAT ou de la visionneuse de vérification](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [Modification des notifications électroniques dans la visionneuse de vérification](#change-your-email-notifications-in-the-proofing-viewer)
* [Modification de la couleur d’arrière-plan dans la visionneuse de vérification de l’ordinateur de bureau](#change-the-background-color-in-the-desktop-proofing-viewer)
* [Effacement des données du navigateur mises en cache à partir d’un bon à tirer dans la visionneuse de vérification de l’appli de bureau](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## Configuration du rôle de vérification par défaut pour les non-destinataires ayant ouvert un bon à tirer {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Les administrateurs Workfront peuvent désormais configurer le rôle de vérification par défaut pour les utilisateurs qui ne sont pas désignés comme destinataires dans le workflow du BAT, mais qui ont accès au BAT via son objet Workfront (projet, tâche ou problème, par exemple).

Auparavant, lorsque les utilisateurs et les invités avaient accès à un BAT sans être ajoutés à son workflow, leur rôle de vérification par défaut était Réviseur.

Cette fonctionnalité s’applique uniquement aux BAT créés dans Workfront, et non dans Workfront BAT.

## Contenu interactif de BAT dans la visionneuse de BAT Web {#proof-interactive-content-in-the-web-proofing-viewer}

Si les stratégies de sécurité de votre entreprise n’autorisent pas l’utilisation de l’application de visionneuse de vérification de l’appli de bureau autonome, votre administrateur Workfront peut désormais activer le contenu interactif dans la visionneuse de vérification de l’application Web. Le contenu doit être regroupé dans un fichier ZIP avant de créer le BAT.

Pour plus d’informations, voir dans l’article .

VIDÉO

## L’ordre de tri par défaut des commentaires dans la visionneuse de vérification est désormais le plus ancien au plus récent  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

Dans la visionneuse de vérification, l’ordre de tri par défaut des commentaires sur un BAT est désormais le plus ancien au plus récent, comme dans une conversation verbale.

Auparavant, l’ordre de tri par défaut était Le plus récent au plus ancien.

Vous pouvez sélectionner une autre option de tri qui est mémorisée pour tous les autres bons à tirer que vous ouvrez.

Pour plus d’informations, reportez-vous à la section de l’article .

## Amélioration de la révision des commentaires dans la visionneuse de vérification associée à une plage de vidéos {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

Lorsque vous passez en revue un commentaire associé à une plage de séquences vidéo dans la visionneuse de vérification, vous pouvez maintenant cliquer sur Lecture pour afficher la gamme complète de séquences. La lecture s’interrompt lorsqu’elle atteint la fin de la plage. Le commentaire reste ouvert afin que vous ne perdiez pas de vue où vous êtes.

Auparavant, lorsque vous ouvriez un commentaire pour une plage de séquences vidéo, vous deviez rechercher manuellement le début de la plage en observant les numéros d’images affichés sur le commentaire avant de cliquer sur Lecture. Dans le cas contraire, la visionneuse de vérification a commencé la lecture à l’endroit où vous cliquiez pour la dernière fois dans la chronologie de la vidéo et elle ne s’est pas arrêtée à la fin de la plage. En outre, le commentaire s’est effondré lorsque vous avez cliqué sur Lire. Il n’était donc plus clair quel commentaire vous passiez en revue.

Pour plus d’informations sur la révision des BAT vidéo, voir .

VIDÉO

## Lien vers les détails du document à partir d’une notification de BAT ou de la visionneuse de vérification {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

Lorsque vous recevez un courrier électronique vous invitant à réviser un BAT ou que vous passez en revue un BAT dans la visionneuse de BAT, vous pouvez désormais accéder rapidement à la page Détails du document du BAT. Sur cette page, vous pouvez voir l’objet Workfront (tel qu’une tâche, un projet ou un problème) associé au BAT. Cela fournit un contexte pour vous aider à comprendre le travail que vous devez faire sur le BAT.

Cette fonctionnalité peut fonctionner uniquement pour les nouveaux utilisateurs que vous ajoutez à votre système. Ce problème est temporaire.

Pour plus d’informations, voir l’article .

VIDÉO

## Modification des notifications électroniques dans la visionneuse de vérification {#change-your-email-notifications-in-the-proofing-viewer}

Désormais, tous les réviseurs de vérification peuvent spécifier les notifications de BAT qu’ils souhaitent recevoir pour un BAT. Ceci est particulièrement important lors de la collaboration avec des parties prenantes externes.

Auparavant, seul le propriétaire du BAT ou le responsable du trafic pouvait configurer les alertes par email d’un BAT pour les réviseurs qu’il avait ajoutés au BAT. Les collaborateurs externes n’ont pas été en mesure de contrôler quelles alertes par e-mail ils ont reçues au sujet du BAT, car ils n’avaient pas l’accès requis à Workfront ni le niveau d’autorisation approprié.

Ces paramètres sont distincts des paramètres d’alerte par e-mail que vous pouvez configurer dans Workfront.

Pour plus d’informations, voir [Gestion des notifications pour les commentaires et les décisions de BAT](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

VIDÉO

## Modification de la couleur d’arrière-plan dans la visionneuse de vérification de l’ordinateur de bureau {#change-the-background-color-in-the-desktop-proofing-viewer}

Vous pouvez désormais modifier la couleur d’arrière-plan de la visionneuse de vérification de l’ordinateur de bureau, de la couleur par défaut proche du noir à la couleur blanche. Cela facilite l’affichage de contenu de vérification avec un arrière-plan transparent.

Pour plus d’informations, voir [Configuration des paramètres de la visionneuse de vérification](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDÉO

## Effacement des données du navigateur mises en cache à partir d’un bon à tirer dans la visionneuse de vérification de l’appli de bureau {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

Lorsque les paramètres de cookie et de cache de votre navigateur sont définis pour bloquer le contenu tel que les fenêtres contextuelles, ce comportement de blocage peut également se produire dans la visionneuse de vérification de l’appli de bureau, ce qui empêche les réviseurs de voir et de commenter le contenu contextuel de votre BAT.

Vous pouvez désormais effacer les données du cache du navigateur qui peuvent être enregistrées avec un BAT afin que tout le contenu apparaisse dans la visionneuse de vérification de l’appli de bureau et que les réviseurs puissent y voir et y ajouter des commentaires.

Pour plus d’informations, voir [Configuration des paramètres de la visionneuse de vérification](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDÉO
