---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Gestion des clés d’API
description: Afin de minimiser les vulnérabilités de la sécurité des API, les administrateurs Adobe Workfront peuvent gérer les clés d’API utilisées pour permettre aux applications d’accéder à Workfront pour le compte d’un utilisateur.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: f504013e202c57245a2edc3dff2b71d19bcfdbee
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 2%

---

# Gestion des clés d’API

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

Afin de minimiser les vulnérabilités de la sécurité des API, les administrateurs Adobe Workfront peuvent gérer les clés d’API utilisées pour permettre aux applications d’accéder à Workfront pour le compte d’un utilisateur.

Vous pouvez réinitialiser ou supprimer votre clé API d’administrateur actuelle, configurer les clés API pour qu’elles expirent et supprimer les clés API pour tous les utilisateurs.

Voici quelques exemples d’applications qui exploitent l’API Workfront :

* Intégrations de document telles que Dropbox, Google Drive et Workfront DAM
* Applications mobiles Workfront

>[!IMPORTANT]
>
>Lors de la réinitialisation ou de la suppression d’une clé API, toute application qui utilise l’API Workfront et s’authentifie à Workfront via cette clé API doit être reconfigurée afin de récupérer l’accès à Workfront.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Clés d’API Workfront

Chaque utilisateur de Workfront dispose d’une clé API unique. Cette clé est générée par utilisateur au moment où l’utilisateur accède à une intégration qui tire parti de l’API Workfront (telle que l’application mobile Workfront ou une intégration de document).

>[!NOTE]
>
> API Les clés que vous générez dans l’environnement de production sont copiées dans votre environnement Aperçu lors de l’actualisation hebdomadaire. Toutes les clés d’API que vous générez dans l’environnement Aperçu seront remplacées par vos clés d’API de production lors de l’actualisation hebdomadaire.

Les administrateurs Workfront disposent également d’une clé API unique. Lorsqu’une application utilise une clé API d’administrateur pour accéder à Workfront, elle dispose d’un accès administrateur à Workfront.

## Gestion d’une clé d’API d’administrateur

Vous pouvez générer, réinitialiser ou supprimer la clé API de votre compte utilisateur administrateur.

>[!NOTE]
>
>Vous pouvez également générer une clé API via l’API. Pour plus d’informations, voir [API d’abonnement à un événement](../../../wf-api/general/event-subs-api.md) dans [API d’abonnement à un événement](../../../wf-api/general/event-subs-api.md).

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système >** **Informations sur le client**
1. (Conditionnel) Effectuez l’une des actions suivantes :

   Pour générer une clé API : dans la variable **Paramètres de clé API** , cliquez sur **Générer la clé API**.

   Ou\
   Pour réinitialiser une clé API : dans **Paramètres de clé API** , cliquez sur **Réinitialiser**, puis **Réinitialisez.**

   Ou

   Pour supprimer la clé API : dans la variable **Paramètres de clé API** , cliquez sur **Supprimer**, puis **Supprimer**.

## Génération d’une clé API pour les utilisateurs non-administrateurs

Vous pouvez générer et gérer des clés d’API pour les utilisateurs occupant des rôles autres que l’administrateur Workfront.

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre entreprise est activée avec Adobe IMS. Si vous avez besoin d’informations supplémentaires, contactez votre administrateur réseau ou informatique.

1. (Conditionnel) Si votre entreprise utilise la gestion de l’accès par authentification unique (SSO), désactivez temporairement l’option nécessitant l’authentification SSO.

   1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

   1. Développer **Système**, puis cliquez sur **Authentification unique (SSO)**.
   1. Dans le **Type** , sélectionnez le type d’authentification unique utilisé par votre organisation.
   1. Avec le type sélectionné, faites défiler l’écran vers le bas et effacez le **Activer** .
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)
   1. Cliquer sur **Enregistrer**.


1. Dans la barre d’adresse d’un navigateur, saisissez l’appel API suivant :

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**username**&amp;password=**password**&amp;method=PUT

   Remplacer `<domain>` avec votre nom de domaine Workfront, ainsi que votre nom d’utilisateur et votre mot de passe avec les informations d’identification Workfront de l’utilisateur.

1. (Conditionnel) Activez l’option nécessitant une authentification SSO si vous l’avez désactivée à l’étape 1.

   1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

   1. Développer **Système**, puis cliquez sur **Authentification unique (SSO)**.

   1. Sélectionnez votre méthode d’authentification unique dans la **Type** menu déroulant.
   1. Cochez la case nécessitant une authentification SSO.

## Configurer lorsque les clés d’API expirent

Vous pouvez configurer les clés d’API pour qu’elles expirent pour tous les utilisateurs de votre système. À l’expiration de la clé API d’un utilisateur, celui-ci doit se reconnecter à toutes les applications qui utilisent l’API Workfront pour accéder à Workfront. Vous pouvez modifier la fréquence d’expiration des clés API. Vous pouvez également configurer l’expiration des clés API à l’expiration du mot de passe d’un utilisateur.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Informations sur le client**.
1. Dans le **Paramètres de clé API** , dans la zone **Après la création**, **Les clés API expirent dans** , sélectionnez la période d’expiration des clés d’API.

   Lorsque vous modifiez cette option, la nouvelle période commence à partir du moment où vous avez apporté la modification. Par exemple, si vous modifiez cette option à partir de *1 mois* to *6 mois*, les clés API expirent 6 mois à compter du moment où vous effectuez la modification.

   Par défaut, les clés API expirent chaque mois.

1. Pour configurer les clés d’API qui expirent au moment où les mots de passe des utilisateurs expirent, sélectionnez **Supprimer la clé API lorsque le mot de passe d’un utilisateur expire**.

   Par défaut, cette option n’est pas sélectionnée.

   Pour plus d’informations sur la configuration des mots de passe utilisateur à expiration, voir [Configuration des préférences de sécurité système](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Cliquer sur **Enregistrer**.

## Suppression des clés API pour tous les utilisateurs

Si une violation de sécurité spécifique vous préoccupe concernant votre système Workfront, vous pouvez supprimer les clés d’API simultanément pour tous les utilisateurs.

>[!IMPORTANT]
>
>La suppression des clés d’API pour tous les utilisateurs invalide TOUTES les clés d’API pour tous les utilisateurs du système. Cette action provoquera l’échec de toutes vos intégrations dans Workfront jusqu’à ce que vous génériez une nouvelle clé API dans Workfront et que vous mettiez à jour toutes vos intégrations.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Développer **Système**, puis cliquez sur **Informations sur le client**

1. Dans le **Paramètres de clé API** zone, cliquez sur **Suppression de toutes les clés d’API**, puis cliquez sur **Supprimer** **Tous**.

## Limitation des connexions API avec un certificat X.509

>[!IMPORTANT]
>
>La procédure décrite dans cette section s’applique uniquement aux organisations qui n’ont pas encore été intégrées à Adobe Business Platform. La connexion à Workfront par le biais de l’API Workfront n’est pas disponible si votre organisation a été intégrée à Adobe Business Platform.
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Business Platform, voir [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Les applications tierces peuvent communiquer avec Workfront par le biais de l’API. Pour accroître la sécurité de votre site Workfront, vous pouvez configurer Workfront afin de limiter les demandes de connexion à l’API en chargeant un certificat X.509 sur Workfront. Une fois activée, toutes les demandes de connexion via l’API doivent inclure un certificat client en plus du nom d’utilisateur et du mot de passe.

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre entreprise est activée avec Adobe IMS. Si vous avez besoin d’informations supplémentaires, contactez votre administrateur réseau ou informatique.

* [Obtention du certificat X.509](#obtain-the-x-509-certificate)
* [Téléchargement du certificat vers Workfront](#upload-the-certificate-to-workfront)
* [Vérification des restrictions des appels de connexion aux API](#verify-api-login-calls-are-restricted)

### Obtention du certificat X.509 {#obtain-the-x-509-certificate}

Obtenez un certificat X.509 valide auprès d’une autorité de certification approuvée (Verisign, par exemple), puis placez-le dans un emplacement temporaire sur votre poste de travail.

### Téléchargement du certificat vers Workfront {#upload-the-certificate-to-workfront}

Après avoir obtenu le certificat X.509 auprès de votre autorité de certification, vous devez le télécharger vers Workfront.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Développer **Système**, puis cliquez sur **Informations sur le client**.

1. Dans le **Paramètres de clé API** zone, sélectionnez **Activer le certificat X.509**.
1. Sur votre poste de travail, recherchez et sélectionnez le certificat X.509 que vous avez précédemment téléchargé.
1. (Facultatif) Cliquez sur **Afficher les détails** en regard du nom du certificat pour afficher les détails suivants sur le certificat :

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

### Vérification des restrictions des appels de connexion aux API {#verify-api-login-calls-are-restricted}

Avant de configurer votre instance de Workfront pour qu’elle ait besoin d’un certificat X.509, effectuez une requête d’API à l’adresse `/login` point de terminaison à l’aide de paramètres de nom d’utilisateur et de mot de passe valides. Vous recevrez une réponse 200 contenant un ID de session.

Après avoir rendu le certificat X.509 obligatoire via la page d’informations sur le client de votre instance de Workfront, effectuez une autre tentative de connexion. Cette fois, vous recevrez une réponse d’erreur 500 avec le message suivant : &quot;Requête non approuvée. Veuillez contacter votre administrateur système et joindre un certificat.&quot;

Après avoir confirmé que le certificat X.509 est requis, effectuez la même requête de connexion avec un paramètre supplémentaire pour apiCertificate défini sur la valeur de votre certificat. Si cette opération a été effectuée correctement, vous recevrez une réponse 200 contenant un ID de session valide.
