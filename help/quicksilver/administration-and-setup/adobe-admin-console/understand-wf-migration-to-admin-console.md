---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Présentation de la migration de Workfront vers Adobe Admin Console
description: Présentation de la migration des utilisateurs et des produits Workfront vers Adobe Admin Console
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: 99b94c246f14110e37b23c95a178efd5b9042a9d
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# Présentation de la migration de Workfront vers Adobe Admin Console

Adobe change la manière dont vous gérez les utilisateurs d’Adobe Workfront, ce qui vous apporte une productivité accrue, ainsi qu’à votre entreprise. Dans le cadre de cette modification, Adobe migre votre instance Workfront et les utilisateurs vers Adobe Admin Console. Il s’agit d’une migration nécessaire qui n’aura aucune incidence sur les chemins de création de rapports, d’approbation, de contenu ou de ressources. Cela aura une incidence sur la manière dont vous gérez l’accès des utilisateurs et dont vos utilisateurs se connectent.

Pour savoir comment utiliser Adobe Admin Console pour gérer vos droits d’Adobe dans l’ensemble de votre organisation, voir [Gestion des utilisateurs dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## Qu’est-ce qui change ?

Dans le cadre de la migration, la gestion des utilisateurs passe de l’application Workfront à Adobe Admin Console avec les rôles d’administration suivants :

* **Administrateurs système** sont des super-utilisateurs dotés de privilèges de tous les administrateurs. Ils attribuent tous les rôles administratifs et gèrent les utilisateurs pour l’ensemble de l’organisation pour tous les produits.

* **Administrateurs de profil de produit (administrateurs système Workfront)** gérer les utilisateurs de l’entreprise qui ont accès à Workfront.

* **Les utilisateurs se connecteront avec l’identité de l’Adobe.** Une fois qu’Adobe migre les utilisateurs existants vers Adobe Admin Console, les utilisateurs se connectent à leurs instances Workfront à l’aide de leur nouvelle identité d’Adobe : Adobe ID ou Adobe Federated ID (SSO).

* **La façon dont vous gérez toutes les autres fonctionnalités n’a pas changé** dans l’application Workfront elle-même, notamment la gestion des fonctionnalités, des rôles utilisateur, des espaces de travail, des fonctionnalités et du comportement.

## Chronologie du Parcours de migration

Adobe migre d’abord votre instance Workfront vers Adobe Admin Console, puis migre tous les utilisateurs existants avec des adresses électroniques vérifiées. Si vous êtes administrateur système ou administrateur de profil de produit Workfront (administrateur système Workfront), vous recevrez des e-mails vous guidant tout au long du parcours de migration. Voici une chronologie de ce à quoi vous pouvez vous attendre :

### Migration de Workfront vers Adobe Admin Console terminée

Les administrateurs système recevront un e-mail une fois la migration de Workfront vers Adobe Admin Console terminée. Actuellement, les administrateurs système peuvent avoir besoin d’effectuer certaines étapes requises. **avant le début de la migration des utilisateurs**, afin de minimiser l’impact sur les utilisateurs de Workfront.

* **Si vos utilisateurs Workfront se connectent actuellement avec SSO**, vous devez configurer l’authentification unique sur Adobe Admin Console afin que vos utilisateurs puissent continuer à se connecter avec l’authentification unique. Si vos utilisateurs Workfront n’utilisent pas actuellement la fonction SSO, mais que vous souhaitez la configurer sur Adobe Admin Console, vous pouvez le faire à ce stade du parcours de migration.
* **Si vous gérez déjà d’autres produits Adobe dans votre Adobe Admin Console**, Adobe peut demander votre consentement pour migrer automatiquement les utilisateurs vers votre console existante. Cliquez sur le bouton **Prise en main** dans le courrier électronique pour accéder à la page de consentement.

Pour l’instant, la gestion des utilisateurs n’a pas été modifiée. Les administrateurs de Workfront continueront à gérer les utilisateurs dans Workfront et les utilisateurs continueront à se connecter à l’aide de leur identifiant Workfront ou de leur authentification unique jusqu’à la fin de la migration des utilisateurs.

### Planification de la migration des utilisateurs

Une fois que l’administrateur système a rempli les conditions préalables décrites dans la section précédente, Adobe planifie automatiquement la migration de vos utilisateurs pendant 30 jours après l’achèvement de ces conditions préalables et communique avec les administrateurs du profil de produit Workfront (administrateurs système Workfront) pour gérer la migration des utilisateurs.

Les administrateurs de profil de produit Workfront (administrateurs système Workfront) :

* Recevez un courrier électronique avec la date de début de la migration des utilisateurs prévue (environ 30 jours après l’achèvement de ces conditions préalables).
* Accédez à la console d’administration Workfront désignée, où ils ont la possibilité de modifier leur date de migration.

  >[!NOTE]
  >
  >En raison de la complexité de la migration, les modifications de date ne sont limitées qu’à 30 jours au maximum au-delà de la date planifiée. Contactez l’assistance si vous avez besoin d’une date ultérieure.

* Recevez un email de rappel 1 jour avant la date de début de la migration des utilisateurs

### Préparation des utilisateurs pour le jour de migration

En tant qu’administrateur de profil de produit Workfront (administrateur système Workfront), est chargé de s’assurer que tous les utilisateurs sont prêts pour le jour de migration.

* Préparez tous les utilisateurs à la migration à venir vers Adobe Identity en leur signalant les informations suivantes :

   * À mesure que les utilisateurs migrent, ils reçoivent un courrier électronique de l’Adobe les informant de la modification de leur manière de se connecter à Workfront. Les utilisateurs seront invités à accepter une invitation à se connecter à l’aide d’Adobe Identity pour la première fois, soit en se connectant à l’aide d’une Adobe ID existante, soit en en configurant une nouvelle à l’aide de la même adresse électronique.

### À quoi vous attendre le jour de la migration

* **La migration des utilisateurs démarrera à minuit du centre de données Workfront hébergé par le client.**

* **Adobe procède d’abord à la migration automatique des administrateurs Workfront.** Lorsque les administrateurs Workfront sont migrés vers Adobe Identity, ils se voient attribuer le rôle d’ administrateur de profil de produit Adobe (administrateur système Workfront) . Les rôles existants qu’un utilisateur peut posséder avant la migration ne seront pas affectés.

  >[!NOTE]
  >
  >L’accès au produit ne sera pas perdu lors de la migration des utilisateurs. Si un utilisateur est connecté au moment de la migration de son utilisateur, cela n’a aucun impact. Cependant, lors de leur prochaine connexion, ils devront utiliser leur identité d’Adobe.



* **Lorsque les utilisateurs sont migrés, ils reçoivent un courrier électronique de l’Adobe les informant de la modification de leur manière de se connecter à Workfront.** Les utilisateurs seront invités à accepter une invitation à se connecter à l’aide d’Adobe Identity pour la première fois, soit en se connectant à un Adobe ID existant, soit en configurant une nouvelle Adobe ID à l’aide de la même adresse électronique.

  Pour plus d’informations sur la connexion à Workfront avec Adobe ID, voir [Connexion à Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Migration des utilisateurs terminée

Adobe avertit par e-mail tous les administrateurs système et administrateurs de profil de produit (administrateurs système Workfront) une fois tous les administrateurs et utilisateurs migrés. À l’heure actuelle, tous les utilisateurs Workfront de cette instance se connectent à Workfront à l’aide d’Adobe Identity. Les administrateurs système Workfront et les administrateurs de profil de produit (administrateurs système Workfront) peuvent gérer l’accès des utilisateurs dans Adobe Admin Console. Si les clients n’utilisent pas de forme de synchronisation d’annuaires dans la console d’administration, ils peuvent continuer à gérer l’accès à Workfront dans l’application Workfront.

## Obtenir une assistance

Pour toute question ou question, veuillez suivre les étapes décrites dans cet article. [Contacter le service clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




