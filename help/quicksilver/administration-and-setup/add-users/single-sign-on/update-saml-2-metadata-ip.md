---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Mise à jour des métadonnées SAML 2.0 dans votre fournisseur d’identité
description: Vous pouvez mettre à jour les métadonnées SAML 2.0 dans votre fournisseur d’identité.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 4%

---

# Mise à jour des métadonnées SAML 2.0 dans votre fournisseur d’identité

{{important-admin-console-onboard}}

Les sections suivantes décrivent comment mettre à jour vos métadonnées SAML (Security Assertion Markup Language) 2.0 lors de l’utilisation des services de fédération Active Directory (ADFS) comme fournisseur d’identité.

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
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Utilisation d’ADFS comme fournisseur d’identité

Vous pouvez mettre à jour vos métadonnées ADFS avant qu’Adobe Workfront ne mette à jour le certificat SAML 2.0 ou après. Si vous choisissez de mettre à jour les métadonnées ADFS avant que Workfront ne mette à jour le certificat SAML 2.0, des étapes supplémentaires sont requises.

* [Mise à jour de vos métadonnées ADFS](#update-your-adfs-metadata)
* [Forcer la mise à jour de vos métadonnées ADFS](#force-your-adfs-metadata-to-update)

### Mise à jour de vos métadonnées ADFS {#update-your-adfs-metadata}

Pour définir vos métadonnées ADFS à mettre à jour automatiquement, suivez les étapes de cette section.

Par défaut, ADFS est configuré pour vérifier automatiquement les mises à jour de toutes les métadonnées de confiance de son partenaire de confiance ; toutefois, la valeur par défaut est définie sur interroger uniquement toutes les 24 heures. Vous pouvez modifier cette valeur à l’aide des commandes powershell.

1. Connectez-vous au serveur ADFS et ouvrez la console de gestion ADFS.
1. Dans le panneau de gauche, développez **ADFS 2.0,** puis développer **Relations de confiance.**

1. Cliquez sur le bouton **Confiance des parties** dossier.
1. Sélectionnez la confiance de la partie de confiance que vous avez précédemment configurée pour être utilisée avec Workfront, puis, dans le panneau de droite, cliquez sur **Mise à jour à partir des métadonnées de fédération**.
1. (Conditionnel) Si cette option est grisée (ce qui signifie que la confiance de la partie de confiance a été précédemment configurée à l’aide d’un fichier de métadonnées), procédez comme suit.

   1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

   1. Cliquez sur **Système** > **Authentification unique (SSO)**.

   1. Cliquez sur **Modifier les paramètres.**
   1. Cliquez sur **Modifier la configuration**, puis sélectionnez **SAML 2.0** dans le **Type** liste déroulante.

   1. Copiez le **URL de métadonnées**, qui doit être similaire à ce qui suit :

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Sur le serveur ADFS, cliquez avec le bouton droit de la souris sur l’approbation de la partie de confiance que vous avez précédemment configurée, puis cliquez sur **Propriétés.**
   1. Cliquez sur le bouton **Surveillance** , puis collez l’URL copiée à partir de Workfront dans la **URL des métadonnées de fédération de l’utilisateur de confiance** champ .

   1. Cochez les options pour **Surveiller le partenaire de confiance** et **Mettre automatiquement à jour le partenaire de confiance**.

   1. Cliquez sur **OK.**
   1. Sélectionnez la confiance de la partie de confiance que vous avez précédemment configurée pour être utilisée avec Workfront, puis, dans le panneau de droite, cliquez sur **Mise à jour à partir des métadonnées de fédération.**

1. Cliquez sur **OK** pour ignorer le message concernant une partie du contenu des métadonnées de fédération non prises en charge par ADFS 2.0.
1. Ouvrir **Modules Windows Powershell.**
1. Une fois tous les modules chargés, exécutez la commande suivante dans powershell :

   `Get-ADFSProperties`

1. Recherchez la valeur en regard de **Intervalle de surveillance.**

   Il s’agira d’un nombre représentant le nombre de minutes entre les sondages. La valeur par défaut doit être 1 440 (1 440 minutes = 24 heures).

1. Définissez une nouvelle valeur en exécutant la commande suivante dans powershell :

   `Set-ADFSProperties -MonitoringInterval 1`

   L’intervalle de surveillance passe ainsi de toutes les 24 heures à toutes les minutes. Vous pouvez définir la valeur 1 sur une autre valeur plus grande si vous souhaitez qu’elle interroge moins fréquemment.

1. Pour vérifier que cela fonctionne correctement, utilisez la variable **Visionneuse d’événements** pour rechercher les informations suivantes dans les journaux ADFS2.0 :

   **Identifiants d’événement 156 et 157**

### Forcer la mise à jour de vos métadonnées ADFS {#force-your-adfs-metadata-to-update}

Pour mettre à jour vos métadonnées ADFS, procédez comme décrit dans la section suivante.

Pour forcer l’échange de métadonnées entre Workfront et votre fournisseur SAML 2.0 lors de l’utilisation des services de fédération Active Directory (ADFS) :

>[!NOTE]
>
>Certaines de ces modifications devront peut-être être effectuées par votre service informatique.

1. Connectez-vous au serveur ADFS et ouvrez le **Console de gestion ADFS**.
1. Dans le panneau de gauche, développez **ADFS 2.0**, puis développez **Relations de confiance**.

1. Cliquez sur le bouton **Confiance des parties** dossier.
1. Sélectionnez la confiance de la partie de confiance que vous avez précédemment configurée pour être utilisée avec Workfront, puis, dans le panneau de droite, cliquez sur **Mise à jour à partir des métadonnées de fédération**.

   Si cette option est grisée et ne peut pas être sélectionnée, procédez comme suit :

   (L’option est grisée uniquement lorsque la confiance de la partie de confiance a été précédemment configurée à l’aide d’un fichier de métadonnées.)

   1. Dans Workfront, dans la zone Configuration, copiez la variable **URL de métadonnées** dans l’écran de configuration de l’authentification unique de Workfront.

      Pour accéder aux informations du **URL de métadonnées**:

      1. Cliquez sur **Configuration** près du coin supérieur droit d’Adobe Workfront dans la barre de navigation globale.
      1. Cliquez sur > **Système** > **Authentification unique (SSO)**.
      1. Cliquez sur **Modifier les paramètres.**
      1. Cliquez sur **Modifier la configuration**, puis sélectionnez **SAML 2.0** dans le **Type** liste déroulante.
      1. Copiez le **URL de métadonnées**, qui doit être similaire à ce qui suit :

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Sur le serveur ADFS, cliquez avec le bouton droit de la souris sur l’approbation de la partie de confiance que vous avez précédemment configurée, puis cliquez sur **Propriétés.**
   1. Cliquez sur le bouton **Surveillance** , puis collez l’URL copiée à partir de Workfront dans la **URL des métadonnées de fédération de l’utilisateur de confiance** champ .
   1. Cochez les options pour **Surveiller le partenaire de confiance** et **Mettre automatiquement à jour le partenaire de confiance**.
   1. Cliquez sur **OK**.
   1. Sélectionnez la confiance de la partie de confiance que vous avez précédemment configurée pour être utilisée avec Workfront, puis, dans le panneau de droite, cliquez sur **Mise à jour à partir des métadonnées de fédération.**

1. Cliquez sur **OK** pour ignorer le message concernant une partie du contenu des métadonnées de fédération non prises en charge par ADFS 2.0.
1. Cliquez sur **Mettre à jour** pour terminer la mise à jour des métadonnées de votre fédération.

Utilisateurs autorisés à accéder à Workfront via l’écran de connexion natif à l’aide des informations de connexion de Workfront (ces informations peuvent être configurées à partir de la page de profil de chaque utilisateur dans la variable **Accès** ) peuvent se connecter à l’aide de leur nom d’utilisateur et de leur mot de passe Workfront en accédant à l’URL suivante : `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Utilisation d’autres fournisseurs d’identité

Lorsque vous utilisez des fournisseurs d’identité autres que ADFS (tels que Ping, Okta ou Centrify), vous devez charger à nouveau les métadonnées Workfront sur votre fournisseur d’identité.

Pour plus d’informations sur la manière d’obtenir une nouvelle URL de métadonnées Workfront, voir [Mise à jour de vos métadonnées ADFS](#update-your-adfs-metadata).

Pour plus d’informations sur l’utilisation des services de fédération Active Directory (ADFS) avec SAML 2.0 dans Workfront, voir [Configuration d’Adobe Workfront avec SAML 2.0 à l’aide d’ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
