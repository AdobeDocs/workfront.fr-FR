---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Gestion des clés d’API
description: Afin de minimiser les vulnérabilités de sécurité de l’API, les administrateurs et administratrices d’Adobe Workfront peuvent gérer les clés API utilisées pour permettre aux applications d’accéder à Workfront pour le compte d’un utilisateur ou d’une utilisatrice.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '1322'
ht-degree: 98%

---

# Gérer les clés API

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

Afin de minimiser les vulnérabilités de sécurité de l’API, les administrateurs et administratrices d’Adobe Workfront peuvent gérer les clés API utilisées pour permettre aux applications d’accéder à Workfront pour le compte d’un utilisateur ou d’une utilisatrice.

Vous pouvez réinitialiser ou supprimer votre clé API d’administrateur ou d’administratrice actuelle, configurer l’expiration des clés API et supprimer les clés API pour tous les utilisateurs et utilisatrices.

Voici quelques exemples d’applications qui utilisent l’API Workfront :

* Intégrations de documents telles que Dropbox, Google Drive et Workfront DAM
* Applications mobiles Workfront

>[!IMPORTANT]
>
>Lors de la réinitialisation ou de la suppression d’une clé API, toute application qui utilise l’API Workfront et s’authentifie auprès de Workfront via cette clé API doit être reconfigurée pour pouvoir accéder à nouveau à Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Clés API Workfront

Chaque utilisateur et utilisatrice de Workfront dispose d’une clé API unique. Cette clé est générée par utilisateur ou utilisatrice au moment où la personne accède à une intégration qui utilise l’API Workfront (telle que l’application mobile Workfront ou une intégration de document).

>[!NOTE]
>
> Les clés API que vous générez dans l’environnement de production sont copiées dans votre environnement de prévisualisation lors de l’actualisation hebdomadaire. Les clés API que vous générez dans l’environnement de prévisualisation seront remplacées par vos clés API de production lors de l’actualisation hebdomadaire.

Les administrateurs et administratrices Workfront disposent également d’une clé API unique. Lorsqu’une application utilise une clé API d’administrateur ou d’administratrice pour accéder à Workfront, elle dispose d’un accès administrateur ou administratrice à Workfront.

## Gérer une clé API d’administrateur ou d’administratrice

Vous pouvez générer, réinitialiser ou supprimer la clé API de votre compte d’utilisateur ou d’utilisatrice d’administration.

>[!NOTE]
>
>Vous pouvez également générer une clé API via l’API. Pour plus d’informations, voir la section [API d’abonnement aux événements](../../../wf-api/general/event-subs-api.md) dans [API d’abonnement aux événements](../../../wf-api/general/event-subs-api.md).

{{step-1-to-setup}}

1. Cliquez sur **Système >** **Infos client**.
1. (Le cas échéant) Effectuez l’une des actions suivantes :

   Pour générer une clé API : dans la section **Paramètres de la clé API**, cliquez sur **Générer la clé API**.

   Ou\
   Pour réinitialiser une clé API : dans la section **Paramètres de la clé API**, cliquez sur **Réinitialiser**, puis sur **Réinitialiser.**

   Ou

   Pour supprimer la clé API : dans la section **Paramètres de la clé API**, cliquez sur **Supprimer**, puis sur **Supprimer**.

## Générer une clé API pour les utilisateurs et utilisatrices non administrateurs et non administratrices

Vous pouvez générer et gérer des clés API pour les utilisateurs et utilisatrices ayant des rôles autres que l’administrateur ou l’administratrice Workfront.

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre entreprise est activée avec Adobe IMS. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

1. (Le cas échéant) Si votre entreprise utilise la gestion des accès par authentification unique (SSO), désactivez temporairement l’option exigeant l’authentification SSO.

   {{step-1-to-setup}}

   1. Développez **Système**, puis cliquez sur **Authentification unique (SSO)**.
   1. Dans le champ **Type**, sélectionnez le type de SSO utilisé par votre entreprise.
   1. Avec le type sélectionné, faites défiler l’écran vers le bas et décochez la case **Activer**.
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)
   1. Cliquer sur **Enregistrer**.


1. Dans la barre d’adresse d’un navigateur, saisissez l’appel API suivant :

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**username**&amp;password=**password**&amp;method=PUT

   Remplacez `<domain>` avec votre nom de domaine Workfront, et votre nom d’utilisateur ou d’utilisatrice et votre mot de passe par les informations d’identification Workfront de l’utilisateur ou l’utilisatrice.

1. (Le cas échéant) Activez l’option exigeant l’authentification SSO si vous l’avez désactivée à l’étape 1.

   {{step-1-to-setup}}

   1. Développez **Système**, puis cliquez sur **Authentification unique (SSO)**.

   1. Sélectionnez votre méthode d’authentification unique dans le menu déroulant **Type**.
   1. Cochez la case exigeant une authentification SSO.

## Configurer l’expiration des clés API

Vous pouvez configurer l’expiration des clés API pour tous les utilisateurs et toutes les utilisatrices de votre système. À l’expiration de la clé API d’un utilisateur ou d’une utilisatrice, celui-ci ou celle-ci doit se reconnecter à toutes les applications qui utilisent l’API Workfront pour accéder à Workfront. Vous pouvez modifier la fréquence d’expiration des clés API. Vous pouvez également configurer l’expiration des clés API à l’expiration du mot de passe d’un utilisateur ou d’une utilisatrice.

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Infos client**.
1. Dans la zone **Paramètres de la clé API**, dans la liste déroulante **Après leur création**, **les clés API expirent dans**, sélectionnez le délai d’expiration souhaité des clés API.

   Lorsque vous modifiez cette option, le nouveau délai commence à partir du moment où vous avez apporté la modification. Par exemple, si vous modifiez cette option de *1 mois* à *6 mois*, les clés API expirent 6 mois à partir du moment où vous apportez la modification.

   Par défaut, les clés API expirent chaque mois.

1. Pour configurer l’expiration des clés API sur l’expiration des mots de passe des utilisateurs et utilisatrices, sélectionnez **Supprimer la clé API lorsque le mot de passe d’un utilisateur ou d’utilisatrice expire**.

   Par défaut, cette option n’est pas sélectionnée.

   Pour plus d’informations sur la configuration de l’expiration des mots de passe des utilisateurs et utilisatrices, voir [Configurer les préférences de sécurité système](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Cliquer sur **Enregistrer**.

## Supprimer les clés API pour tous l’ensemble des utilisateurs et utilisatrices

Si une violation de sécurité spécifique vous préoccupe concernant votre système Workfront, vous pouvez supprimer les clés API simultanément pour l’ensemble des utilisateurs et utilisatrices.

>[!IMPORTANT]
>
>La suppression des clés API pour l’ensemble des utilisateurs et utilisatrices invalide TOUTES les clés API pour l’ensemble des utilisateurs et utilisatrices du système. Cette action provoquera l’échec de toutes vos intégrations dans Workfront jusqu’à ce que vous génériez une nouvelle clé API dans Workfront et que vous mettiez à jour toutes vos intégrations.

{{step-1-to-setup}}

1. Développez **Système**, puis cliquez sur **Infos client**.

1. Dans la zone **Paramètres de clé API**, cliquez sur **Supprimer toutes les clés API**, puis sur **Tout** **supprimer**.

## Limiter les connexions à l’API avec un certificat X.509

>[!IMPORTANT]
>
>La procédure décrite dans cette section s’applique uniquement aux organisations qui n’ont pas encore été intégrées à Adobe Business Platform. La connexion à Workfront par le biais de l’API Workfront n’est pas disponible si votre organisation a été intégrée à Adobe Business Platform.
>
>Pour obtenir une liste de procédures qui varient selon que votre organisation a été intégrée ou non à Adobe Business Platform, voir [Différences d’administration en fonction de la plateforme (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Les applications tierces peuvent communiquer avec Workfront par le biais de l’API. Pour renforcer la sécurité de votre site Workfront, vous pouvez configurer Workfront afin de limiter les demandes de connexion à l’API en chargeant un certificat X.509 sur Workfront. Une fois activé, toutes les demandes de connexion via l’API doivent inclure un certificat client ou en plus du nom d’utilisateur ou d’utilisatrice et du mot de passe.

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre entreprise est activée avec Adobe IMS. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

* [Obtenir le certificat X.509](#obtain-the-x-509-certificate)
* [Charger le certificat dans Workfront](#upload-the-certificate-to-workfront)
* [Vérifier que les appels de connexion à l’API sont limités](#verify-api-login-calls-are-restricted)

### Obtenir le certificat X.509 {#obtain-the-x-509-certificate}

Obtenez un certificat X.509 valide auprès d’une autorité de certification approuvée (Verisign, par exemple), puis placez-le dans un emplacement temporaire sur votre poste de travail.

### Charger le certificat dans Workfront {#upload-the-certificate-to-workfront}

Après avoir obtenu le certificat X.509 auprès de votre autorité de certification, vous devez le charger dans Workfront.

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis sur **Configuration** ![](assets/gear-icon-settings.png).

1. Développez **Système**, puis cliquez sur **Infos client**.

1. Dans la zone **Paramètres de clé API**, sélectionnez **Activer le certificat X.509**.
1. Sur votre poste de travail, recherchez et sélectionnez le certificat X.509 que vous avez précédemment chargé.
1. (Facultatif) Cliquez sur **Afficher les détails** en regard du nom du certificat pour afficher les détails suivants sur le certificat :

   * Nom courant du sujet
   * Organisation du sujet
   * Unité organisationnelle du sujet
   * Nom courant de l&#39;émetteur
   * Organisation de l&#39;émetteur
   * Unité organisationnelle de l&#39;émetteur
   * Numéro de série
   * Date de l&#39;événement
   * Date d&#39;expiration

1. Cliquer sur **Enregistrer**.

### Vérifier que les appels de connexion à l’API sont limités {#verify-api-login-calls-are-restricted}

Avant de configurer votre instance de Workfront pour qu’elle exige un certificat X.509, effectuez une demande d’API auprès du point d’entrée `/login` à l’aide de paramètres de nom d’utilisateur ou d’utilisatrice et de mot de passe valides. Vous recevrez une réponse 200 contenant un ID de session.

Après avoir rendu le certificat X.509 obligatoire via la page d’informations sur le client de votre instance de Workfront, effectuez une autre tentative de connexion. Cette fois, vous recevrez une réponse d’erreur 500 avec le message suivant : « Demande non fiable. Contactez votre administrateur système et joignez un certificat. »

Après avoir confirmé que le certificat X.509 est requis, effectuez la même demande de connexion avec un paramètre supplémentaire pour apiCertificate défini sur la valeur de votre certificat. Si cette opération a été effectuée correctement, vous recevrez une réponse 200 contenant un ID de session valide.
