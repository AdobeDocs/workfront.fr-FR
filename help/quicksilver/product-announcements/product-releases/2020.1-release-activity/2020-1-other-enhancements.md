---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Autres améliorations de la version 2020.1
description: Cette page décrit toutes les améliorations apportées aux zones générales de Workfront avec la version 2020.1. Ces améliorations sont actuellement disponibles dans l’environnement de prévisualisation et seront disponibles dans l’environnement de production à la fin du mois de mars ou au début du mois d’avril 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
TQID: https://experienceleague.adobe.com/I5djuVv0ixHspF6afQaa5-jTkl0uXl26VlKf8BXqhO4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: b8ea32d4-f1fe-4c71-8871-afe5a702a009
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 433
ht-degree: 100%

---

# Autres améliorations de la version 2020.1

Cette page décrit toutes les améliorations apportées aux zones générales de Workfront avec la version 2020.1. Ces améliorations sont actuellement disponibles dans l’environnement de prévisualisation et seront disponibles dans l’environnement de production à la fin du mois de mars ou au début du mois d’avril 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.1, voir [Vue d’ensemble de la version 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Modification requise pour ajouter des épreuves à la liste autorisée

>[!NOTE]
>
>Cette fonctionnalité a été supprimée de la version 2020.1. Elle sera disponible ultérieurement.

Le domaine de relecture passe de from proofhq.com à workfront.com.

Si votre pare-feu ou votre serveur de messagerie est configuré pour n’autoriser l’accès qu’à des fournisseurs spécifiques, vous devez ajouter l’URL supplémentaire suivante à votre liste autorisée pour vous assurer que les utilisateurs et les utilisatrices de votre organisation peuvent visualiser les épreuves dans Workfront, aussi bien dans la visionneuse de relecture web que dans la visionneuse de relecture de bureau :

&#42;.workfront.com

L’URL &#42;proofhq.com est également requise.

Pour plus d’informations sur la mise à jour de votre liste autorisée, voir [Configurer la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Cette mise à jour s’applique uniquement à la relecture dans Workfront ; elle ne s’applique pas lors de l’utilisation de l’application autonome Workfront Proof.

## Mise à jour du comportement des cookies de Workfront pour maintenir la compatibilité avec Chrome

Pour maintenir la compatibilité avec une mise à jour prochaine de Google Chrome (Chrome v80), nous avons mis à jour la plateforme Workfront afin de nous assurer que les cookies sont correctement envoyés avec les demandes.

Cette mise à jour de Chrome modifie la valeur par défaut de l’attribut de cookie SameSite. Si vous souhaitez tester le comportement de votre instance Workfront après la mise à jour de Google Chrome, ajustez les indicateurs dans Chrome et activez les options suivantes :

* « Cookies SameSite par défaut »
* « Les cookies sans SameSite doivent être sécurisés »

## Synchronisation des commentaires Workfront avec Jira

L’intégration Workfront pour Jira synchronise désormais vos commentaires Workfront dans le flux de commentaires natif de Jira.

Auparavant, vous pouviez synchroniser les commentaires de Jira à Workfront, mais pas de Workfront à Jira.

Pour plus d’informations, consultez la section [Configurer Adobe Workfront pour Jira](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## L’optimisateur de portfolio Flash a été supprimé.

Nous avons supprimé la possibilité de basculer entre le nouveau et l’ancien optimisateur de portfolio (basé sur Flash) dans l’environnement Workfront Classic pour l’ensemble de la clientèle. L’optimisateur de portfolio hérité est obsolète et les nouveaux outils offrent la même fonctionnalité aujourd’hui.

Pour plus d’informations sur l’optimisateur de portfolio, consultez https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079.

Pour plus d’informations sur la suppression des outils Flash dans Workfront, consultez la section [Remplacer les outils Flash dans Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
