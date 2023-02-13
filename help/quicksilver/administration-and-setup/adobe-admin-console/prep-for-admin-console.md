---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Préparation à l’intégration de votre organisation à Adobe Admin Console
description: Adobe Workfront étant un produit Adobe, vous pouvez y accéder via Adobe Admin Console. Cela vous permet de gérer Workfront avec d’autres comptes d’Adobe et produits pour vos utilisateurs dans un emplacement central.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Préparation à l’intégration de votre organisation à Adobe Admin Console

Adobe Workfront étant un produit Adobe, vous pouvez y accéder via Adobe Admin Console. Cela vous permet de gérer Workfront avec d’autres comptes d’Adobe et produits pour vos utilisateurs dans un emplacement central.

Tous les clients Workfront finiront par être déplacés vers Adobe Admin Console. Une fois que votre organisation a migré vers Adobe Admin Console, l’authentification Workfront est gérée par Adobe Admin Console. La préparation et la réalisation de cette démarche au plus tôt préparent le terrain pour une gestion efficace du travail et positionnent votre entreprise pour une innovation plus rapide à l’avenir.

Pour un aperçu de Adobe Admin Console, reportez-vous à la section [Présentation du Admin Console](https://helpx.adobe.com/fr/enterprise/using/admin-console.html).

## Liste de contrôle de migration

Pour vous assurer que votre organisation peut migrer vers Adobe Admin Console, vous devez effectuer les actions suivantes :

1. Identifiez le Adobe Admin Console souhaité dans lequel vous souhaitez ajouter Workfront.

   * Si votre entreprise ne dispose pas d’un Adobe Admin Console existant ou si vous ne souhaitez pas utiliser un Adobe Admin Console existant, le support Workfront peut vous aider à en créer un nouveau.

   * Si vous disposez de plusieurs Admin Console d’Adobe et que vous ne savez pas lequel est le plus approprié pour ajouter Adobe Workfront, contactez l’assistance Workfront.

1. Confirmez avec l’assistance Workfront que vous souhaitez utiliser un Adobe Admin Console existant ou en créer un nouveau.

1. Configurez la gestion des identités sur Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Soyez prêt à discuter avec le support Workfront et votre équipe informatique des préférences d’authentification telles que l’authentification unique (SSO) ou non.

   Pour obtenir des instructions, reportez-vous à la section Identity Management du Guide de déploiement pour Adobe Admin Console (https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. (Conditionnel) Si vous utilisez l’authentification unique, connectez le nouveau Adobe Admin Console à votre fournisseur d’authentification unique existant.

   Pour plus d’informations et d’instructions, voir [Configuration de l’identité](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Si votre entreprise n’utilise pas l’authentification unique, tous les utilisateurs migrés vers Adobe Admin Console recevront un e-mail leur indiquant de créer leur compte et leur mot de passe.

1. Assurez-vous que les adresses électroniques des utilisateurs sont prêtes pour la migration :

   1. Suppression des courriers électroniques en double de Workfront

      Pour plus d’informations, voir Mise à jour des adresses électroniques des utilisateurs existants dans votre instance Workfront dans Prévention des doublons d’utilisateurs.

      En cas de doublon d’adresses électroniques dans votre entreprise, l’utilisateur est représenté par l’adresse électronique avec la plus récente `lastLoginDate` sera déplacé vers l’organisation Adobe Admin Console. Tous les autres utilisateurs disposant de cette adresse électronique seront désactivés.

      >[!NOTE]
      >
      >Dans la mesure où un seul utilisateur disposant d’une adresse électronique donnée peut être principal à la fois, si vous devez activer un autre utilisateur ayant la même adresse électronique qu’un utilisateur principal, vous devez d’abord désactiver l’utilisateur principal actuel avant d’activer l’utilisateur désactivé.

   2. (Conditionnel) Si vous utilisez des intégrations d’API personnalisées, vérifiez que ces utilisateurs disposent d’une adresse électronique valide à laquelle ils ont accès.

   3. (Facultatif) Nous vous recommandons de désactiver tous les utilisateurs qui n’ont plus besoin d’accéder à Workfront afin qu’ils ne soient pas ajoutés à Adobe Admin Console.
   >[!IMPORTANT]
   >
   >Ces actions concernant les e-mails des utilisateurs doivent être effectuées avant que votre entreprise ne commence à migrer vers Adobe Admin Console.

1. (Facultatif) Mettez à jour toutes les intégrations personnalisées pour utiliser OAuth2.

   Pour obtenir des instructions sur la configuration des intégrations OAuth2, voir [Création d’applications OAuth2 pour les intégrations Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   La création d’intégrations OAuth2 n’est disponible que dans la nouvelle expérience Workfront.

   >[!NOTE]
   >
   >Cette étape est facultative, mais vivement recommandée, car d’autres formes d’authentification et d’autorisation d’API seront abandonnées à l’avenir.

Une fois votre Adobe Admin Console configuré avec Workfront, vous pouvez l’utiliser pour gérer vos utilisateurs.

Pour plus d’informations, voir [Gestion des utilisateurs dans Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Pour obtenir la liste des autres actions différentes selon que votre organisation a été intégrée à Adobe Admin Console, voir [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
