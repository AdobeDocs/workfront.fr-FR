---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Améliorations de la relecture (version 2020.2)
description: Cette page décrit toutes les améliorations de la vérification des performances apportées à la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 2%

---

# Améliorations de la relecture (version 2020.2)

Cette page décrit toutes les améliorations de la vérification des performances apportées à la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.2, consultez la [présentation de la version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Le domaine de vérification passe de proofhq.com à workfront.com.

>[!NOTE]
>
>Cette fonctionnalité a été initialement communiquée dans le cadre de la version 2020.1, mais a été supprimée de la version avant de la publier en production.

Si votre pare-feu ou votre serveur de messagerie est configuré pour autoriser l’accès uniquement à des fournisseurs spécifiques, vous devez ajouter l’URL supplémentaire suivante à votre liste autorisée pour vous assurer que les utilisateurs de votre entreprise peuvent afficher les bons à tirer dans Workfront dans la visionneuse de vérification de l’orthographe du navigateur et la visionneuse de vérification de l’ordinateur de bureau :

&#42;.workfront.com

L’URL &#42;proofhq.com est également requise.

Pour plus d’informations sur la mise à jour de votre liste autorisée, voir [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Cette mise à jour s’applique uniquement à la correction d’épreuves dans Workfront ; elle ne s’applique pas lors de l’utilisation de l’application autonome Workfront Proof.

## Les commentaires de vérification des invités apparaissent dans la zone Mises à jour .

Pour simplifier la collaboration sur les bons à tirer, les commentaires des invités apparaissent dans la zone Mises à jour .

Auparavant, les commentaires de BAT des invités n&#39;étaient disponibles que dans le BAT.
