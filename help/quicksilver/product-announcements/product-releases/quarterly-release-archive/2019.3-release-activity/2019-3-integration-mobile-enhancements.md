---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3 Intégration et améliorations apportées aux appareils mobiles
description: Cette page décrit toutes les modifications apportées à l’intégration et aux améliorations apportées aux appareils mobiles avec la version 2019.3. Cela a été rendu disponible dans l’environnement de production dans la semaine du 19 août 2019.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 100%

---

# 2019.3 Intégration et améliorations apportées aux appareils mobiles

Cette page décrit toutes les modifications apportées à l’intégration et aux améliorations apportées aux appareils mobiles avec la version 2019.3. Cela a été rendu disponible dans l’environnement de production dans la semaine du 19 août 2019.

Pour obtenir la liste de toutes les modifications apportées à la version 2019.3, voir [Vue d’ensemble de l’activité de la version 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Prise en charge des éléments partagés dans l’intégration de MS OneDrive

Vous pouvez désormais lier vos fichiers et dossiers OneDrive partagés à des objets Workfront. À l’inverse, vous pouvez charger des fichiers dans Workfront vers des dossiers partagés dans OneDrive.

Pour plus d’informations, voir les sections [Lier un document externe à Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents), [Lier un ou plusieurs dossiers externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder) et [Mettre à jour et lier un document de Workfront à un fournisseur cloud externe](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) dans l’article [Lier des documents à partir d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Pour plus d’informations, voir la section [Lier un document externe à Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) dans l’article [Lier des documents à partir d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Spécification de domaine requise pour toutes les connexions Workfront

Pour toutes les connexions Workfront, la personne doit désormais spécifier le domaine si ce dernier n’est pas déjà spécifié dans l’URL Workfront. Ces informations sont requises pour rendre votre instance Workfront plus sécurisée. En outre, si votre implémentation de Workfront comporte plusieurs instances, cette amélioration vous permet d’ajouter la même personne à chaque instance de Workfront dans votre implémentation.

Cette modification peut avoir une incidence sur les connexions utilisateur et les intégrations d’API :

* **Connexions utilisateur**

  Si le domaine de votre entreprise n’est pas inclus dans l’URL de Workfront, un nouveau champ Domaine s’affiche désormais dans l’écran de connexion, en plus des champs Nom d’utilisateur ou d’utilisatrice et Mot de passe.

  Pour la plus grande partie de la clientèle, aucune modification n’est requise, car les informations de domaine sont déjà incluses dans l’URL Workfront. Par exemple, « *domain*.my.workfront.com ».

* **Intégrations d’API**

  Si un code d’API est envoyé à une adresse qui n’inclut pas votre nom de domaine, il ne fonctionnera plus.

Pour plus d’informations, voir [Se connecter à Adobe Workfront](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md).

## Convertir des tâches et des problèmes en projets à l’aide de l’application mobile sur iOS

Vous pouvez désormais convertir des tâches et des problèmes individuels en projets dans l’application mobile Workfront sur iOS.

## Connectez-vous à l’application mobile avec l’empreinte digitale ou la reconnaissance faciale.

En fonction de votre appareil, vous pouvez choisir de vous connecter à l’application mobile Workfront à l’aide de la technologie d’empreinte digitale ou de reconnaissance faciale. Lorsque vous vous connectez à l’application mobile, vous devrez vous connecter à l’aide de la méthode d’authentification prise en charge par votre téléphone.

Pour plus d’informations sur la gestion de cette fonctionnalité, voir [Adobe Workfront pour iOS](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) ou [Adobe Workfront pour Android](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md).

## Nouveau paramètre pour déconnecter automatiquement les personnes sur mobile

Afin de rendre l’application mobile Workfront plus sécurisée pour vous et votre entreprise, les personnes seront automatiquement déconnectées après 15 jours d’inactivité. L’équipe d’administration de Workfront peut personnaliser cette limite de temps dans l’application web sous Configuration > Système > Préférences.

Pour plus d’informations, voir [Configurer les préférences de sécurité système](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## L’application mobile nécessite un domaine lors de la connexion.

Pour améliorer la sécurité, l’application mobile Workfront exige désormais que vous fournissiez votre domaine si vous ne vous connectez pas avec des informations SSO.

>[!NOTE]
>
>Disponibilité sur iOS : 12 juin 2019
>
>Disponibilité de la production : 17 juin 2019

## Supprimer des objets à l’aide de l’application mobile sur iOS

>[!NOTE]
>
>Cette fonctionnalité a été mise à disposition dans les boutiques d’applications d’iOS au cours de la semaine du 19 août 2019.

Vous pouvez désormais supprimer des objets tels que des tâches, des problèmes et des feuilles de temps dans l’application mobile iOS. Vous devez disposer des autorisations appropriées sur l’objet pour le supprimer.

## Filtrer par projets immobilisés dans l’application mobile

>[!NOTE]
>
>Cette fonctionnalité sera disponible dans les boutiques d’applications pour iOS et Android au cours de la semaine du 19 août 2019.

Nous avons ajouté l’option de filtrage Projets immobilisés sous l’onglet Projets de l’application mobile.

## Réinitialiser votre mot de passe à l’aide de l’application mobile

Vous pouvez utiliser l’application mobile Workfront pour réinitialiser votre mot de passe si vous l’avez oublié. Appuyez sur Mot de passe oublié ? et suivez les invites à l’écran. Vous ne pouvez pas réinitialiser votre mot de passe SSO sur l’application mobile.

## Nouvel aspect pour mobile

Nous avons ajouté les améliorations suivantes au niveau de l’aspect afin d’améliorer votre expérience dans l’application mobile Workfront.

* Déplacement des éléments suivants de la barre supérieure de la page Détails vers des zones plus importantes de l’écran :

   * L’icône Plus se trouve maintenant dans le coin inférieur gauche de l’écran.
   * La coche permettant de commencer à travailler sur un élément est désormais un bouton Travailler sur ce projet dans la partie supérieure de l’écran.

* Vous pouvez désormais afficher les formulaires personnalisés joints en appuyant sur Afficher plus au bas de la page Détails.
* Modification de l’aspect des pages que vous utilisez pour envoyer des tâches, des problèmes et des requêtes.

