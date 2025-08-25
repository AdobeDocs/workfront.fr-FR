---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Préparation à l’intégration de votre entreprise à Adobe Admin Console
description: Adobe Workfront étant un produit Adobe, vous pouvez y accéder via l’Adobe Admin Console. Cela vous permet de gérer Workfront ainsi que d’autres comptes et produits Adobe pour vos utilisateurs et utilisatrices depuis un seul endroit.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 96%

---

# Préparer l’intégration de votre entreprise à l’Adobe Admin Console

<!-- Audited: 12/2023 -->

Adobe Workfront étant un produit Adobe, vous pouvez y accéder via l’Adobe Admin Console. Cela vous permet de gérer Workfront ainsi que d’autres comptes et produits Adobe pour vos utilisateurs et utilisatrices depuis un seul endroit.

Tous les clientes et clients Workfront seront à terme transférés vers l’Adobe Admin Console. Une fois que votre entreprise est passée à l’Adobe Admin Console, l’authentification Workfront est gérée par la console. Préparer et effectuer ce changement plus tôt permet d’établir les bases d’une gestion efficace du travail et d’assurer à votre entreprise une innovation plus rapide à l’avenir.

Pour une vue d’ensemble dl’Adobe Admin Console, voir [Vue d’ensemble d’Admin Console](https://helpx.adobe.com/fr/enterprise/using/admin-console.html).

## Liste de contrôle de migration

Pour que votre organisation puisse migrer vers l’Adobe Admin Console, vous devez effectuer les opérations suivantes.

1. Identifiez l’Adobe Admin Console dans laquelle vous souhaitez ajouter Workfront.

   * Si votre entreprise ne dispose pas d’une Adobe Admin Console existante, ou que vous ne souhaitez pas en utiliser une, le support Workfront peut vous aider à en créer une.

   * Si vous disposez de plusieurs Adobe Admin Consoles et que vous ne savez pas laquelle est la plus appropriée pour ajouter Workfront, contactez le support Workfront.

1. Confirmez auprès du support Workfront que vous souhaitez utiliser une Adobe Admin Console existante ou en créer une.

1. Configurez l’Identity Management sur l’Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Préparez-vous à discuter avec le support Workfront et votre équipe informatique des préférences d’authentification, telles que l’authentification unique (SSO) ou non SSO.

   Pour obtenir des instructions, voir la section Identity Management du [Guide de déploiement pour Adobe Admin Console](https://helpx.adobe.com/fr/enterprise/using/deployment-planning.html).

1. (Le cas échéant) Si vous utilisez l’authentification unique, connectez la nouvelle Adobe Admin Console à votre fournisseur d’authentification unique existant.

   Pour plus d’informations et d’instructions, voir [Définir l’identité](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Si votre entreprise n’utilise pas l’authentification unique, tous les utilisateurs et utilisatrices ayant migré vers l’Adobe Admin Console recevront un e-mail leur demandant de créer un compte et un mot de passe.

1. Veillez à ce que les adresses e-mail des utilisateurs et utilisatrices soient prêtes pour la migration :

   1. Supprimez les e-mails en double de Workfront.

      Pour obtenir des instructions, voir [Mettre à jour les adresses e-mail des utilisateurs et utilisatrices existants dans votre instance Workfront](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) dans [Empêcher les doublons d’utilisateurs et d’utilisatrices](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).

      Si votre entreprise compte des adresses e-mail en double, la personne associée à l’adresse avec la `lastLoginDate` la plus récente sera déplacé vers l’entreprise de l’Adobe Admin Console. Tous les autres utilisateurs et utilisatrices ayant cette adresse e-mail seront désactivés.

      >[!NOTE]
      >
      >Étant donné qu’une seule personne disposant d’une certaine adresse e-mail peut être active à un moment donné, si vous devez activer une autre personne possédant la même adresse qu’une personne actuellement active, vous devez d’abord désactiver cette dernière avant d’activer la personne désactivée.

   1. (Le cas échéant) Si vous utilisez des intégrations API personnalisées, confirmez que ces utilisateurs et utilisatrices ont une adresse e-mail valide à laquelle ils ont accès.

   1. (Facultatif) Nous vous recommandons de désactiver les utilisateurs et utilisatrices qui n’ont plus besoin d’accéder à Workfront, afin qu’ils ne soient pas ajoutés à l’Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Ces actions relatives aux e-mails des utilisateurs et utilisatrices doivent être terminées avant que votre entreprise ne commence à migrer vers l’Adobe Admin Console.

1. (Facultatif) Mettez à jour toutes les intégrations personnalisées pour utiliser OAuth2.

   Pour obtenir des instructions sur la configuration des intégrations OAuth2, voir [Créer des applications OAuth2 pour les intégrations Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   >[!NOTE]
   >
   >Cette étape est facultative, mais fortement recommandée, car les autres formes d’authentification et d’autorisation API seront supprimées à l’avenir.

Une fois que votre Adobe Admin Console est configurée avec Workfront, vous pouvez l’utiliser pour créer vos administrateurs et administratrices de système Workfront.

Pour plus d’informations, voir [Gestion des utilisateurs dans Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Pour obtenir une liste des autres actions qui diffèrent selon que votre entreprise a été intégrée ou non à l’Adobe Admin Console, voir [Différences d’administration en fonction de la plateforme (Adobe Workfront Fusion/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
