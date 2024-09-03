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

Adobe modifie la gestion des utilisateurs et utilisatrices d’Adobe Workfront, ce qui se traduit par une productivité accrue pour vous et votre entreprise. Dans le cadre de ce changement, Adobe migre votre instance Workfront et ses utilisateurs et utilisatrices vers Adobe Admin Console. Il s’agit d’une migration nécessaire, qui n’affectera pas les rapports, les voies d’approbation, le contenu ou les ressources. Elle aura un impact sur la façon dont vous gérez l’accès des personnes et sur la façon dont elles se connectent.

Cet article décrit en termes généraux le processus de déplacement d’une organisation vers Adobe Admin Console, de sorte que vous, en tant qu’administrateur de Workfront, sachiez à quoi vous attendre.

Pour savoir comment utiliser Adobe Admin console pour gérer vos droits Adobe dans l’ensemble de votre entreprise, voir [Gérer les personnes dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## Qu’est-ce qui change?

Dans le cadre de la migration, la gesion des utilisateurs et utilisatrices passe de l’application Workfront à Adobe Admin Console avec les rôles administratifs suivants :

* Les **administrateurs et administratrices système** sont des super utilisateurs et utilisatrices qui ont les mêmes privilèges que tous les administrateurs et administratrices. Ils attribuent tous les rôles administratifs et gèrent les personnes de l’ensemble de l’organisation pour tous les produits.

* **Les administrateurs et administratrices du profil du produit (administrateurs et administratrices du système Workfront)** gèrent les personnes de l’organisation qui ont accès à Workfront.

* **Les personnes se connecteront avec Adobe Identity.** Après la migration des utilisateurs et utilisatrices existants vers Adobe Admin Console, les personnes se connecteront à leurs instances Workfront à l’aide de leur nouvelle identité Adobe Identity, qu’il s’agisse d’un Adobe ID ou d’un Adobe Federated ID (SSO).

* **Il n’y a aucun changement dans la façon dont vous gérez toutes les autres fonctionnalités** dans l’application Workfront elle-même, y compris la gestion des fonctions, des rôles d’utilisateur ou d’utilisatrice, des espaces de travail, des fonctionnalités et du comportement.

## Chronologie du parcours de migration

Adobe commencera par migrer votre instance Workfront vers Adobe Admin Console, puis migrera toutes les personnes existantes dont l’adresse e-mail a été vérifiée. Si vous êtes administrateur ou administratrice système ou de profil de produit Workfront (administrateur ou administratrice système Workfront), vous recevrez des e-mails vous guidant tout au long du processus de migration. Voici une chronologie de ce à quoi vous pouvez vous attendre :

### Migration de Workfront vers Adobe Admin Console terminée

Les administrateurs et administratrices système recevront un e-mail lorsque la migration de Workfront vers Adobe Admin Console sera terminée. À ce stade, les administrateurs et administrtrices système peuvent devoir effectuer certaines étapes obligatoires **avant que la migration des personnes ne commence**, afin de minimiser l’impact sur les utilisateurs et utilisatrices de Workfront.

* **Si vos utilisateurs et utilisatrices Workfront se connectent actuellement avec l’authentification unique**, vous devez configurer l’authentification unique sur Adobe Admin Console pour qu’ils puissent continuer à se connecter ainsi. Si vos utilisateurs et utilisatrices Workfront n’utilisent pas encore l’authentification unique, mais que vous souhaitez la configurer dans Adobe Admin Console, vous pouvez le faire à ce stade de la migration.
* **Si vous gérez déjà d’autres produits Adobe dans votre Adobe Admin Console**, Adobe peut vous demander votre consentement pour migrer automatiquement les personnes vers votre console existante. Cliquez sur le bouton **Commencer** dans l’e-mail pour accéder à la page de consentement.
* **Si vous avez précédemment supprimé le type de licence Demandeur**, il sera ajouté à votre système. Aucune personne ne sera affectée à ce type de licence, mais il est nécessaire pour la synchronisation entre Workfront et Adobe Admin Console. Aucune action de votre part n’est requise concernant le type de licence Demandeur.

Pour l’instant, la gestion des utilisateurs et utilisatrices n’a pas été modifiée. Les administrateurs et administratrices Workfront continueront à gérer les personnes dans Workfront, et les personnes continueront à se connecter avec leur ID Workfront ou l’authentification unique jusqu’à ce que la migration des personnes soit terminée.

### Planifier la migration des personnes

Une fois que l’administrateur ou l’administratrice système a effectué les étapes obligatoires préalables décrites dans la section précédente, Adobe planifie automatiquement la migration des personnes 30 jours après l’achèvement de ces conditions préalables et communique avec les administrateurs et administratrices de profil de produit Workfront (administrateurs et administratrices système Workfront) pour gérer la migration des personnes.

Les administrateurs et administratrices du profil de produit Workfront (administrateurs et administratrices système Workfront) effectuent les opérations suivantes :

* Ils reçoivent un e-mail indiquant la date de début de la migration des personnes (environ 30 jours après l’achèvement des étapes obligatoires préalables).
* Ils accèdent à la console d’administration Workfront désignée, où ils ont la possibilité de modifier leur date de migration.

  >[!NOTE]
  >
  >En raison de la complexité de la migration, les changements de date sont limités à un maximum de 30 jours après la date prévue. Contactez l’assistance si vous souhaitez une date ultérieure.

* Ils reçoivent un e-mail de rappel un jour avant la date de début de la migration des personnes.

### Ils préparent les personnes au jour de la migration.

En tant qu’administrateur ou administratrice de profil de produit Workfront (administration système Workfront), vous devez vous assurer que l’ensemble des utilisateurs et utilisatrices sont prêts pour le jour de la migration.

* Préparez l’ensemble des utilisateurs et utilisatrices à la migration à venir vers Adobe Identity en leur indiquant les informations suivantes :

   * À mesure que les utilisateurs et utilisatrices migrent, ils reçoivent un e-mail d’Adobe les informant de la modification de la méthode de connexion à Workfront. Les personnes seront invitées à accepter une invitation à se connecter pour la première fois à l’aide d’Adobe Identity, soit en se connectant avec un Adobe ID existant, soit en en créant un nouveau en utilisant la même adresse e-mail.

### À quoi s’attendre le jour de la migration

* **La migration des personnes commencera à minuit dans le centre de données Workfront d’hébergement de la clientèle.**

* **Adobe migrera automatiquement les administrateurs et administratrices Workfront en premier.** Lorsque les administrateurs et administratrices Workfront migrent vers Adobe Identity, ils se voient attribuer le rôle d’administrateurs et administratrices de profil de produit Adobe (administrateurs et administratrices système Workfront). Les rôles existants qu’une personne pouvait avoir avant la migration ne seront pas affectés.

  >[!NOTE]
  >
  >Il n’y aura pas de perte d’accès au produit pendant la migration des personnes. Si une personne est connectée pendant la période de migration, il n’y aura pas d’impact. Cependant, lors de sa prochaine connexion, il lui sera demandé d’utiliser son Adobe Identity.



* **Au fur et à mesure de la migration, les personnes recevront un e-mail d’Adobe les informant de la modification de leur mode de connexion à Workfront.** Les personnes seront invitées à accepter une invitation à se connecter pour la première fois à l’aide d’Adobe Identity, soit en se connectant avec un Adobe ID existant, soit en créant un Adobe ID en utilisant la même adresse e-mail.

  Pour plus d’informations sur la façon de se connecter à Workfront avec un Adobe ID, voir [Se connecter à Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Migration des personnes terminée

Adobe informera tous les administrateurs et administratrices système et de profil de produit (administrateurs et administratrices système Workfront) par e-mail une fois que tous les administrateurs, administratrices et personnes auront migré. À ce moment-là, tous les utilisateurs et utilisatrices de Workfront pour cette instance se connecteront à Workfront à l’aide d’Adobe Identity. Les administrateurs et administratrices système Workfront et ceux du profil de produit (administrateurs et administratrices système Workfront) peuvent gérer l’accès des personnes dans Adobe Admin Console. Si les clientes et clients n’utilisent pas une forme de synchronisation d’annuaire dans la console d’administration, ils peuvent continuer à gérer l’accès à Workfront dans l’application Workfront.

## Obtenir de l’aide

Pour toute question ou préoccupation, veuillez suivre les étapes décrites dans l’article [Contacter l’assistance clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




