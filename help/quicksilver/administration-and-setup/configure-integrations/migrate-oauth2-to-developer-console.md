---
title: Migration de Workfront OAuth2 vers Adobe Developer Console
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Le service d’application personnalisé OAuth2 hérité de Workfront est en cours de suppression. Découvrez ce qui change, qui est affecté et comment migrer vos intégrations personnalisées vers Adobe Developer Console.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: db7e6a6fa0c5fc5332213c388d9b4db3a5c59f53
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 1%

---

# Migration de Workfront OAuth2 vers Adobe Developer Console

Le service d’application personnalisé OAuth2 hérité de Workfront (les intégrations que vous avez configurées sous **Configuration** > **Système** > **OAuth2**) est en cours de suppression. À l’avenir, toutes les intégrations personnalisées qui s’authentifient sur Workfront devront utiliser le flux d’authentification Adobe Developer Console (developer.adobe.com) à la place.

Cette modification affecte toute intégration personnalisée, tout script ou tout outil tiers qui s’authentifie actuellement à l’aide d’un identifiant client OAuth2 et d’un secret émis par Workfront. Elle n’affecte pas la manière dont vous vous connectez à Workfront, ni les intégrations standard gérées par Adobe, telles que les intégrations Microsoft Teams ou Slack empaquetées, qu’Adobe migre séparément.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès Adobe Workfront</td> 
   <td><p>Administrateur ou administratrice système</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Droits Adobe Developer Console</td> 
   <td><p>Des droits d’administrateur d’organisation IMS complets sont requis pour accéder à Adobe Developer Console for Workfront. Ce rôle est plus large qu’un rôle d’administrateur de produit Workfront, car il gère l’ensemble de l’organisation Adobe et tous les produits qu’elle contient.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Dates clés

| Date | Jalon | Ce que cela signifie pour vous |
|---|---|---|
| 1er novembre 2026 | Création d’application désactivée | Vous ne pouvez plus créer d’applications OAuth2 personnalisées dans Workfront. Les applications existantes continuent de fonctionner. |
| 1Er Février 2027 | Service hérité retiré | Les applications OAuth2 personnalisées existantes ne fonctionnent plus du tout. Toute intégration qui n’a pas migré vers Adobe Developer Console perd l’accès à l’API Workfront à ce stade. |

>[!IMPORTANT]
>
>Nous vous recommandons vivement de planifier et d’effectuer votre migration avant le 1er novembre 2026 afin que vos intégrations continuent de s’exécuter sans interruption et que vous ne migriez pas dans les délais impartis du 1er février 2027.

## Organisations affectées

Votre organisation est concernée par cette modification si elle dispose d’une intégration, d’un script ou d’un outil qui se connecte à Workfront à l’aide d’un identifiant client OAuth2 personnalisé et d’un secret émis via l’écran de configuration OAuth2 hérité de Workfront. Voici quelques exemples courants :

* Intégrations personnalisées que votre équipe d’ingénieurs maintient par rapport à l’API Workfront.
* Connecteurs tiers ou créés par des partenaires configurés avec un identifiant client émis par Workfront. Nous vous recommandons de vérifier auprès de votre fournisseur si vous n&#39;êtes pas sûr de la manière dont son intégration s&#39;authentifie.
* Scripts d’automatisation interne, de création de rapports ou de synchronisation des données qui appellent directement l’API Workfront.

Si vous ne savez pas si votre organisation dispose de l’une de ces fonctionnalités, votre administrateur Workfront peut vérifier la liste des applications OAuth2 sous **Configuration** > **Système** > **OAuth2** pour voir ce qui est actuellement enregistré. Pour plus d’informations, voir [Affichage et gestion des applications OAuth2 personnalisées](/help/quicksilver/administration-and-setup/configure-integrations/manage-custom-oauth2-apps.md).

## Présentation des types d’authentification Adobe Developer Console

Adobe Developer Console prend en charge plusieurs méthodes d’authentification. Vous pouvez sélectionner le type correspondant au fonctionnement de votre intégration :

* **Authentification de serveur à serveur** : pour une application s’exécutant sur votre serveur principal qui appelle les API Adobe au nom de votre organisation, sans qu’aucun utilisateur final ne soit impliqué. Il s’agit de la correspondance la plus proche du modèle OAuth2 Workfront hérité utilisé avec les ID client et les secrets. Il s’agit du type que la plupart des intégrations, scripts et automatisations Workfront personnalisés doivent utiliser.
* **Authentification de l’utilisateur** : dans les cas où un utilisateur Adobe doit se connecter et accorder son consentement avant que votre application puisse afficher ou modifier ses données. Si votre intégration doit agir pour le compte d’un utilisateur Workfront connecté spécifique plutôt que de votre organisation dans son ensemble, utilisez plutôt ce type.

  Si vous choisissez Authentification de l’utilisateur, il existe trois autres options en fonction de l’architecture de votre application :

  * **Application web OAuth** : pour les applications disposant d’une interface utilisateur frontale et d’un serveur principal. Le serveur stocke le secret client en toute sécurité et récupère les jetons.
  * **Application d’une seule page OAuth** : pour les applications web accessibles uniquement par un navigateur, sans serveur principal. L’application web elle-même récupère les jetons.
  * **Application native OAuth** : pour les applications mobiles ou de bureau qui s’exécutent de manière native sur un appareil et n’ont pas de serveur principal. L’application native récupère les jetons.

La plupart des entreprises effectuant la migration d’une intégration, d’un script ou d’une automatisation back-end du service OAuth2 hérité souhaitent une authentification de serveur à serveur.

## Comparaison des fonctionnalités : OAuth2 hérité par rapport à Adobe Developer Console

Le service Workfront OAuth2 hérité (décompte dans **Configuration** > **Système** > **Applications OAuth2**) offre trois types d’applications, avec une limite de 10 applications OAuth2 par instance Workfront. Voici comment ces aspects se comparent à Adobe Developer Console :

| Type de Workfront hérité | Méthode de flux/authentification | Équivalent Developer Console | Ajuster |
|---|---|---|---|
| Application machine à machine (interfaces de ligne de commande, démons, scripts principaux) | JWT avec paire de clés publique/privée | Authentification de serveur à serveur | Même objectif : ne pas impliquer l’utilisateur final, mais le mécanisme change. Le flux hérité utilise une paire de clés publique/privée et JWT, tandis que serveur à serveur utilise un identifiant client et un secret client avec une autorisation d’informations d’identification client OAuth. Il ne s’agit pas d’un échange d’informations d’identification sans rendez-vous. Le code d’authentification de l’intégration doit être modifié, et pas seulement les valeurs d’identification. Pour plus d’informations, voir [Utilisation du flux JWT pour les applications OAuth 2 personnalisées](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md). |
| Application Web (applications côté serveur : Go, Java, .NET, Node, PHP) | Flux de code d’autorisation OAuth 2.0 | Application web OAuth (sous Authentification utilisateur) | Correspondance 1:1 la plus proche. Il présente le même flux et la même forme de base qu’un serveur principal qui stocke le secret client. Pour plus d’informations, voir [Flux de code d’autorisation pour les applications OAuth 2 personnalisées](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md). |
| Application Web Monopage (JS, Angular, React, Vue) | Flux de code d’autorisation avec PKCE, pas de secret client | Application monopage OAuth (sous Authentification utilisateur) | Correspondance 1:1 la plus procheIl s’agit du même flux basé sur PKCE et sans secret. Pour plus d’informations, voir [&#x200B; Utilisation du flux PKCE pour les applications OAuth 2 &#x200B;](/help/quicksilver/wf-api/api/oauth-app-pkce-flow.md). |
| (aucun équivalent hérité) | — | Application native OAuth (sous Authentification utilisateur) | Il s’agit d’une nouvelle fonctionnalité. L’ancien Workfront OAuth2 ne dispose d’aucun type dédié aux applications mobiles ou de bureau natives. |

<!--

>[!NOTE]
>
>A few legacy capabilities don't have a confirmed equivalent yet in Adobe Developer Console, and are being validated with the Developer Console team:
>
>* Per-app controls the legacy UI offers: refresh token rotation toggle, absolute vs. inactivity refresh token expiration, custom logo, privacy policy URL, and developer contact fields.
>* Whether Developer Console enforces a cap on credentials or projects similar to the legacy 10-app-per-instance limit.
>* Whether a JWT/key pair-based option remains available anywhere in Developer Console for Machine to Machine customers, or whether all such integrations must move to the client-secret-based Server-to-Server grant.

-->

## Procédure de migration

### Si vous êtes administrateur système de Workfront

>[!NOTE]
>
>Si vous êtes un administrateur de produit Workfront, mais pas un administrateur d’organisation, vous devez travailler avec l’administrateur de votre organisation pour terminer cette migration, ou demander à en faire une.

1. Connectez-vous à [developer.adobe.com](https://developer.adobe.com) et créez un projet. Les projets sont la manière dont la console organise différentes intégrations ou applications clientes.
1. Dans le projet, ajoutez une API, puis sélectionnez **&#x200B;**. Cette API figure dans la catégorie Experience Cloud . Toutes les API Workfront, notamment Planning, Workflow, ainsi que Review and Approvals, partagent cette API unique.
1. Sélectionnez l’option d’authentification **serveur à serveur**, puis choisissez l’instance appropriée si votre organisation IMS comporte plusieurs instances Workfront.

   Pour plus d’informations sur le choix d’un type d’authentification, voir [Présentation des types d’authentification Adobe Developer Console](#understand-adobe-developer-console-authentication-types) dans cet article.
1. Sur la page Projet , ouvrez les détails de vos nouvelles informations d’identification de serveur à serveur OAuth pour trouver votre identifiant client, votre secret client et les informations nécessaires pour générer des jetons d’accès.
1. Mettez à jour votre intégration, script ou outil pour vous authentifier avec ces nouvelles informations d’identification à la place de l’ancien identifiant client OAuth2 et du secret Workfront.
1. Confirmez l’accès dans Workfront. La création du client API l’ajoute automatiquement en tant qu’utilisateur Workfront « `techacct` ». Par défaut, il est ajouté en tant que contributeur avec un accès limité, mais vous pouvez ajuster son niveau d’accès comme vous le feriez pour tout autre utilisateur.
1. (Facultatif) Pour accorder des droits d’administrateur à l’utilisateur `techacct`, ajoutez l’e-mail du compte technique en tant qu’administrateur du profil de produit approprié dans Admin Console.
1. Testez l’intégration de bout en bout.
1. Supprimez l’ancienne entrée de l’application OAuth2 dans Workfront après avoir confirmé que la nouvelle connexion fonctionne.

Pour obtenir des détails détaillés complets et des captures d’écran, consultez [Obtention de l’accès](https://developer.adobe.com/workfront-apis/guides/gaining_access/) dans la documentation d’Adobe Developer Console.

### Si vous n’êtes pas administrateur système

Vous devez effectuer une boucle dans l’administrateur de l’organisation IMS de votre organisation pour terminer la migration, car la configuration des nouvelles informations d’identification dans Adobe Developer Console nécessite ce niveau d’accès. Si vous gérez ou maintenez une intégration, mais que vous savez qui est l’administrateur de l’organisation IMS de votre organisation, contactez l’un des organismes suivants :

* Votre équipe de compte Workfront
* Votre équipe informatique interne
* Votre contact en ingénierie

## Si vous ne migrez pas

Les intégrations qui utilisent toujours l’ID client/le modèle secret OAuth2 hérité après le 1er février 2027 ne peuvent plus s’authentifier auprès de l’API Workfront et tout workflow, synchronisation ou automatisation dépendant échoue. Aucune extension n’est prévue au-delà de cette date. Effectuez donc la migration de vos intégrations bien avant.

## Questions fréquentes

**Cela affecte-t-il les intégrations empaquetées fournies par Adobe, telles que Slack ou Microsoft Teams ?**

Non. Les applications globales gérées par Adobe sont migrées directement par Adobe et ne nécessitent aucune action de votre part.

**Mon intégration existante cessera-t-elle de fonctionner avant le 1er février 2027 ?**

Non. Les applications OAuth2 personnalisées existantes continuent de fonctionner normalement jusqu’au 1er février 2027. À compter du 1er novembre 2026, seule la possibilité de créer des applications OAuth2 personnalisées est affectée.

**La migration a-t-elle un coût ?**

Non, l’authentification via Adobe Developer Console n’entraîne aucun coût supplémentaire.

**Où puis-je obtenir de l’aide ?**

Contactez votre équipe de compte Workfront ou ouvrez un dossier d’assistance si vous avez des questions sur votre intégration ou votre calendrier spécifique. Pour obtenir une présentation officielle et à jour de la configuration avec des captures d’écran, consultez [Accès](https://developer.adobe.com/workfront-apis/guides/gaining_access/) dans la documentation d’Adobe Developer Console.
