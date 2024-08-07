---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Autres améliorations (version 2020.1)
description: Cette page décrit toutes les améliorations apportées aux zones générales de Workfront avec la version 2020.1. Ces améliorations sont actuellement disponibles dans l’environnement Aperçu et seront disponibles dans l’environnement Production à la fin du mois de mars ou au début du mois d’avril 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 1%

---

# Autres améliorations (version 2020.1)

Cette page décrit toutes les améliorations apportées aux zones générales de Workfront avec la version 2020.1. Ces améliorations sont actuellement disponibles dans l’environnement Aperçu et seront disponibles dans l’environnement Production à la fin du mois de mars ou au début du mois d’avril 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.1, consultez la [présentation de la version 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Modification requise pour ajouter des bons à tirer à la liste autorisée

>[!NOTE]
>
>Cette fonctionnalité a été supprimée de la version 2020.1. Il sera disponible ultérieurement.

Le domaine de vérification passe de from proofhq.com à workfront.com.

Si votre pare-feu ou votre serveur de messagerie est configuré pour autoriser l’accès uniquement à des fournisseurs spécifiques, vous devez ajouter l’URL supplémentaire suivante à votre liste autorisée pour vous assurer que les utilisateurs de votre entreprise peuvent afficher les bons à tirer dans Workfront dans la visionneuse de vérification de l’orthographe du navigateur et la visionneuse de vérification de l’ordinateur de bureau :

&#42;.workfront.com

L’URL &#42;proofhq.com est également requise.

Pour plus d’informations sur la mise à jour de votre liste autorisée, voir [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Cette mise à jour s’applique uniquement à la correction d’épreuves dans Workfront ; elle ne s’applique pas lors de l’utilisation de l’application autonome Workfront Proof.

## Comportement des cookies Workfront mis à jour pour maintenir la compatibilité avec Chrome

Pour maintenir la compatibilité avec une mise à jour de Google Chrome (Chrome v80) à venir, nous avons mis à jour la plateforme Workfront afin de nous assurer que les cookies sont correctement envoyés avec les requêtes.

Cette mise à jour de Chrome modifie la valeur par défaut de l’attribut de cookie SameSite. Si vous souhaitez tester le comportement de votre instance Workfront après la mise à jour de Google Chrome, ajustez les indicateurs dans Chrome et activez les options suivantes :

* Cookies samesite par défaut
* &quot;Les cookies sans samesite doivent être sécurisés&quot;

## Synchronisation des commentaires Workfront avec Jira

L’intégration Workfront for Jira synchronise désormais vos commentaires Workfront dans le flux de commentaires natif de Jira.

Auparavant, vous pouviez synchroniser les commentaires de Jira vers Workfront, mais pas de Workfront vers Jira.

Pour plus d’informations, voir [Configuration d’Adobe Workfront pour Jira](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Flash Portfolio Optimizer a été supprimé.

Nous avons supprimé la possibilité de basculer entre le nouvel Portfolio Optimizer et l’ancien Optimizer (basé sur le Flash) de l’environnement Workfront Classic pour tous les clients. La fonctionnalité héritée de Portfolio Optimizer est obsolète et les nouveaux outils offrent la même fonctionnalité aujourd’hui.

Pour plus d’informations sur l’optimiseur de portefeuille, voir https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

Pour plus d’informations sur l’obsolescence des outils basés sur des Flashs dans Workfront, voir [Remplacement des outils basés sur des Flashs dans Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
