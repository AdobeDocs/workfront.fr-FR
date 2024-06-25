---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Comprendre la migration de Workfront vers Adobe Admin Console
description: Cet article décrit en termes généraux le processus de déplacement d’une organisation vers Adobe Admin Console, de sorte que vous, en tant qu’administrateur de Workfront, sachiez à quoi vous attendre.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: 633c41eeb570402254125f92f3624cad7befd609
workflow-type: tm+mt
source-wordcount: '1114'
ht-degree: 94%

---

# Comprendre la migration de Workfront vers Adobe Admin Console

Adobe change la manière dont vous gérez les utilisateurs et utilisatrices d’Adobe Workfront, ce qui augmente votre productivité et celle de votre organisation. Dans le cadre de ce changement, Adobe migre votre instance Workfront, ainsi que les utilisateurs et utilisatrices vers Adobe Admin Console. Il s’agit d’une migration nécessaire qui n’aura aucune incidence sur les rapports, les voies d’approbation, le contenu ou les ressources. Elle impacte toutefois la manière dont vous gérez l’accès des personnes et dont vos utilisateurs et utilisatrices se connectent.

Cet article décrit en termes généraux le processus de déplacement d’une organisation vers Adobe Admin Console, de sorte que vous, en tant qu’administrateur de Workfront, sachiez à quoi vous attendre.

Pour découvrir comment utiliser Adobe Admin Console pour gérer vos droits Adobe dans l’ensemble de votre organisation, voir [Gérer les utilisateurs et utilisatrices dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## Qu’est-ce qui change ?

Dans le cadre de la migration, la gestion de vos utilisateurs et utilisatrices passe de l’application Workfront à Adobe Admin Console avec les rôles d’administration suivants :

* Les **administrateurs et administratrices système** sont des super-utilisateurs et super-utilisatrices ayant les privilèges de tous les administrateurs et administratrices. Ils ou elles attribuent tous les rôles administratifs et gèrent les personnes sur l’ensemble de l’organisation et pour tous les produits.

* Les **administrateurs et administratrices de profil de produit (administrateurs et administratrices système Workfront)** gèrent les personnes de l’organisation qui ont accès à Workfront.

* **Les utilisateurs et utilsatrices personnes se connectent avec l’identité Adobe.** Une fois qu’Adobe a migré les personnes vers Adobe Admin Console, elles peuvent se connecter à leurs instances Workfront à l’aide de leur nouvelle identité Adobe : Adobe ID ou Adobe Federated ID (SSO).

* **La façon dont vous gérez toutes les autres fonctionnalités ne change pas** dans l’application Workfront elle-même, notamment la gestion des fonctionnalités, des rôles utilisateur, des espaces de travail, des fonctions et du comportement.

## Chronologie du parcours de migration

Adobe migre d’abord votre instance Workfront vers Adobe Admin Console, puis migre l’ensemble des utilisateurs et utilisatrices ayant des adresses e-mail vérifiées. Si vous êtes administrateur ou administratrice système, ou encore administrateur ou administratrice de profil de produit Workfront (administration du système Workfront), vous recevrez des e-mails vous guidant tout au long du parcours de migration. Voici une chronologie de ce à quoi vous pouvez vous attendre :

### Migration de Workfront vers Adobe Admin Console terminée

Les administrateurs et administratrices système recevront un e-mail une fois la migration de Workfront vers Adobe Admin Console terminée. Actuellement, les administrateurs et administratrices système peuvent avoir besoin d’effectuer certaines étapes requises **avant le début de la migration des utilisateurs et utilisatrices**, afin de minimiser l’impact sur les personnes utilisant Workfront.

* **Si vos utilisateurs et utilisatrices Workfront se connectent actuellement via SSO**, vous devez configurer l’authentification unique sur Adobe Admin Console, afin qu’ils puissent continuer à se connecter via l’authentification unique. Si vos utilisateurs et utilisatrices Workfront n’utilisent pas actuellement l’authentification SSO, mais que vous souhaitez la configurer sur Adobe Admin Console, vous pouvez le faire à ce stade du parcours de migration.
* **Si vous gérez déjà d’autres produits Adobe dans Adobe Admin Console**, Adobe peut demander votre consentement pour migrer automatiquement les utilisateurs et utilisatrices vers votre console existante. Cliquez sur le bouton **Commencer** dans l’e-mail pour accéder à la page de consentement.
* **Si vous avez précédemment supprimé le type de licence Demandeur**, il sera ajouté à votre système. Aucune personne ne sera affectée à ce type de licence, mais il est nécessaire pour la synchronisation entre Workfront et Adobe Admin Console. Aucune action de votre part n’est requise concernant le type de licence Demandeur.

Pour l’instant, la gestion des utilisateurs et utilisatrices n’a pas été modifiée. Les administrateurs et administratrices Workfront continueront à gérer les utilisateurs et utilisatrices dans Workfront et ces derniers continueront à se connecter à l’aide de leur identifiant Workfront ou de leur authentification unique jusqu’à la fin de leur migration.

### Planifier la migration des utilisateurs et utilisatrices

Une fois que l’administration système a rempli les conditions préalables décrites dans la section précédente, Adobe planifie automatiquement la migration de vos utilisateurs et utilisatrices pendant 30 jours après le remplissage de ces conditions préalables et communique avec l’administration du profil de produit Workfront (administration système Workfront) pour gérer la migration des utilisateurs et utilisatrices.

Les administrateurs et administratrices de profil de produit Workfront (administration système Workfront) :

* Reçoivent un e-mail avec la date de début de la migration prévue des utilisateurs et utilisatrices (environ 30 jours après le remplissage de ces conditions préalables).
* Accèdent à la console d’administration Workfront désignée, où ils ont la possibilité de modifier leur date de migration.

  >[!NOTE]
  >
  >En raison de la complexité de la migration, les modifications de date ne sont limitées qu’à 30 jours au maximum au-delà de la date planifiée. Contactez l’assistance si vous avez besoin d’une date ultérieure.

* Reçoivent un e-mail de rappel 1 jour avant la date de début de la migration des utilisateurs et utilisatrices.

### Préparer les utilisateurs et utilisatrices au jour de la migration

En tant qu’administrateur ou administratrice de profil de produit Workfront (administration système Workfront), vous devez vous assurer que l’ensemble des utilisateurs et utilisatrices sont prêts pour le jour de la migration.

* Préparez l’ensemble des utilisateurs et utilisatrices à la migration à venir vers Adobe Identity en leur indiquant les informations suivantes :

   * À mesure que les utilisateurs et utilisatrices migrent, ils reçoivent un e-mail d’Adobe les informant de la modification de la méthode de connexion à Workfront. Les utilisateurs et utilisatrices devront accepter une invitation à se connecter à l’aide d’Adobe Identity pour la première fois, soit en se connectant à l’aide d’un Adobe ID existant, soit en en configurant un nouveau à l’aide du même e-mail.

### À quoi vous attendre le jour de la migration ?

* **La migration des utilisateurs et utilisatrices démarrera à minuit du centre de données Workfront hébergé par la clientèle.**

* **Adobe procède d’abord à la migration automatique des administrateurs et administratrices Workfront.** Lorsque les administrateurs et administratrices Workfront migrent vers Adobe Identity, ils se voient attribuer le rôle d’administrateur ou administratrice de profil de produit Adobe (administration système Workfront). Les rôles existants avant la migration ne seront pas affectés.

  >[!NOTE]
  >
  >L’accès au produit ne sera pas perdu lors de la migration des utilisateurs et utilisatrices. Si une personne est connectée au moment de la migration, cela n’a aucun impact. Cependant, lors de la prochaine connexion, elle devra utiliser Adobe Identity.



* **Lors de la migration, les utilisateurs reçoivent un e-mail d’Adobe les informant de la modification de leur mode de connexion à Workfront.** Les utilisateurs et utilisatrices seront invités à se connecter pour la première fois à l’aide d’Adobe Identity, soit en se connectant à un identifiant Adobe ID existant, soit en en configurant un nouveau à l’aide de la même adresse e-mail.

  Pour plus d’informations sur la connexion à Workfront à l’aide d’un identifiant Adobe ID, voir [Se connecter à Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Fin de la migration des personnes

Adobe avertit par e-mail tous les administrateurs et toutes les administratrices système et de profil de produit (administrateurs et administratrices système de Workfront) une fois que l’ensemble des personnes a été migré. À l’heure actuelle, l’ensemble des utilisateurs et utilisatrices de Workfront de cette instance se connectent à Workfront à l’aide d’Adobe Identity. L’administration système de Workfront et les administrateurs de profil de produit (administration système de Workfront) peuvent gérer l’accès des utilisateurs et utilisatrices dans Adobe Admin Console. Si les clientes et clients n’utilisent pas de forme de synchronisation de répertoires dans Adobe Admin Console, ils peuvent continuer à gérer l’accès à Workfront dans l’application Workfront.

## Obtenir une assistance

Pour toute question ou préoccupation, suivez les étapes décrites dans l’article [Contacter l’assistance clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




