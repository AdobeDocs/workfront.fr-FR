---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Mettre à jour les métadonnées SAML 2.0 dans votre fournisseur d’identité
description: Vous pouvez mettre à jour des métadonnées SAML 2.0 dans votre fournisseur d’identité.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 97%

---

# Mettre à jour des métadonnées SAML 2.0 dans votre fournisseur d’identité

{{important-admin-console-onboard}}

Les sections suivantes décrivent comment mettre à jour vos métadonnées SAML (Security Assertion Markup Language) 2.0 lorsque vous utilisez Active Directory Federation Services (ADFS) comme fournisseur d’identité.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Utiliser ADFS comme fournisseur d’identité

Vous pouvez mettre à jour vos métadonnées ADFS avant qu’Adobe Workfront ne mette à jour le certificat SAML 2.0 ou après. Si vous choisissez de mettre à jour les métadonnées ADFS avant que Workfront ne mette à jour le certificat SAML 2.0, des étapes supplémentaires sont nécessaires.

* [Mettre à jour vos métadonnées ADFS](#update-your-adfs-metadata)
* [Forcer la mise à jour de vos métadonnées ADFS](#force-your-adfs-metadata-to-update)

### Mettre à jour vos métadonnées ADFS {#update-your-adfs-metadata}

Pour configurer vos métadonnées ADFS afin qu’elles soient mises à jour automatiquement, suivez les étapes de cette section.

Par défaut, ADFS est configuré pour vérifier automatiquement les mises à jour de toutes les métadonnées de ses parties de confiance ; cependant, la valeur par défaut est définie sur une interrogation toutes les 24 heures seulement. Vous pouvez modifier cette valeur à l’aide de commandes PowerShell.

1. Connectez-vous au serveur ADFS et ouvrez la console de gestion ADFS.
1. Dans le panneau de gauche, développez **ADFS 2.0**, puis développez **Relations de confiance**.

1. Cliquez sur le dossier **Parties de confiance**.
1. Sélectionnez la partie de confiance que vous avez précédemment configurée pour être utilisée avec Workfront, puis, dans le panneau de droite, cliquez sur **Mettre à jour à partir des métadonnées de fédération**.
1. (Le cas échéant) Si cette option est désactivée (ce qui signifie que la partie de confiance a été précédemment configurée à l’aide d’un fichier de métadonnées), procédez comme suit.

   1. Cliquez sur l’icône **Menu principal** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![Icône des paramètres d’engrenage](assets/gear-icon-settings.png).

   1. Cliquez sur **Système** > **Authentification unique (SSO)**.

   1. Cliquez sur **Modifier les paramètres**.
   1. Cliquez sur **Modifier la configuration**, puis sélectionnez **SAML 2.0** dans la liste déroulante **Type**.

   1. Copiez l’**URL des métadonnées**, qui doit ressembler à ce qui suit :

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Sur le serveur ADFS, cliquez avec le bouton droit sur la partie de confiance que vous avez configurée précédemment, puis cliquez sur **Propriétés**.
   1. Cliquez sur l’onglet **Surveillance**, puis collez l’URL que vous avez copiée depuis Workfront dans le champ **URL des métadonnées de fédération de la partie de confiance**.

   1. Cochez les options **Surveiller la partie de confiance** et **Mettre à jour automatiquement la partie de confiance**.

   1. Cliquez sur **OK**.
   1. Sélectionnez la partie de confiance que vous avez précédemment configurée pour être utilisée avec Workfront ; puis, dans le panneau de droite, cliquez sur **Mettre à jour depuis les métadonnées de fédération**.

1. Cliquez sur **OK** pour ignorer le message indiquant que certains contenus des métadonnées de fédération ne sont pas pris en charge par ADFS 2.0.
1. Ouvrez **Modules Windows PowerShell**.
1. Après le chargement de tous les modules, exécutez la commande suivante dans PowerShell :

   `Get-ADFSProperties`

1. Recherchez la valeur à côté de l’**Intervalle de surveillance**.

   Il s’agit d’un nombre qui représente le nombre de minutes entre les interrogations. La valeur par défaut est 1 440 (1 440 minutes = 24 heures).

1. Définissez une nouvelle valeur en exécutant la commande suivante dans PowerShell :

   `Set-ADFSProperties -MonitoringInterval 1`

   Avec cette commande, l’intervalle de surveillance passe de toutes les 24 heures à toutes les minutes. Vous pouvez remplacer la valeur 1 par une valeur plus élevée si vous souhaitez que les interrogations soient moins fréquentes.

1. Pour vérifier que cela fonctionne correctement, utilisez l’**Observateur d’événements** pour rechercher les informations suivantes dans les journaux d’ADFS2.0 :

   **Identifiant d’événement 156 et 157**

### Forcer la mise à jour de vos métadonnées ADFS {#force-your-adfs-metadata-to-update}

Pour mettre à jour vos métadonnées ADFS, suivez les étapes de la section suivante.

Pour forcer l’échange de métadonnées entre Workfront et votre fournisseur SAML 2.0 lors de l’utilisation d’Active Directory Federation Services (ADFS), procédez comme suit :

>[!NOTE]
>
>Certaines de ces modifications peuvent devoir être effectuées par votre service informatique.

1. Connectez-vous au serveur ADFS et ouvrez la **console de gestion ADFS**.
1. Dans le panneau de gauche, développez **ADFS 2.0**, puis développez **Relations de confiance**.

1. Cliquez sur le dossier **Parties de confiance**.
1. Sélectionnez la partie de confiance que vous avez précédemment configurée pour être utilisée avec Workfront, puis dans le panneau de droite, cliquez sur **Mettre à jour à partir des métadonnées de fédération**.

   Si cette option est grisée et ne peut être sélectionnée, procédez comme suit :

   (L’option n’est désactivée que si la partie de confiance a été configurée précédemment à l’aide d’un fichier de métadonnées.)

   1. Dans Workfront, dans la zone de configuration, copiez l’**URL des métadonnées** à partir de l’écran de configuration de l’authentification unique de Workfront.

      Pour accéder aux informations relatives à l’**URL des métadonnées**, procédez comme suit :

      1. Cliquez sur **Configuration** dans le coin supérieur droit d’Adobe Workfront sur la barre de navigation globale.
      1. Cliquez sur > **Système** > **Authentification unique (SSO)**.
      1. Cliquez sur **Modifier les paramètres**.
      1. Cliquez sur **Modifier la configuration**, puis sélectionnez **SAML 2.0** dans la liste déroulante **Type**.
      1. Copiez l’**URL des métadonnées**, qui doit ressembler à ce qui suit :

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Sur le serveur ADFS, cliquez avec le bouton droit sur la partie de confiance que vous avez configurée précédemment, puis cliquez sur **Propriétés**.
   1. Cliquez sur l’onglet **Surveillance**, puis collez l’URL que vous avez copiée depuis Workfront dans le champ **URL des métadonnées de fédération de la partie de confiance**.
   1. Cochez les options **Surveiller la partie de confiance** et **Mettre à jour automatiquement la partie de confiance**.
   1. Cliquez sur **OK**.
   1. Sélectionnez la partie de confiance que vous avez précédemment configurée pour être utilisée avec Workfront, puis dans le panneau de droite, cliquez sur **Mettre à jour à partir des métadonnées de fédération**.

1. Cliquez sur **OK** pour ignorer le message indiquant que certains contenus des métadonnées de la fédération ne sont pas pris en charge par ADFS 2.0.
1. Cliquez sur **Mettre à jour** pour terminer la mise à jour de vos métadonnées de fédération.

Les personnes autorisées à accéder à Workfront via l’écran de connexion natif en utilisant les informations d’identification de Workfront (cela peut être configuré à partir de la page de profil de chaque personne dans la section **Accès**) peuvent se connecter en utilisant leur nom d’utilisateur ou utilisatrice et leur mot de passe Workfront en se rendant sur l’URL suivante : `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Utiliser d’autres fournisseurs d’identité

Si vous utilisez des fournisseurs d’identité autres qu’ADFS (tels que Ping, Okta ou Centrify), vous devez charger à nouveau les métadonnées de Workfront vers votre fournisseur d’identité.

Pour plus d’informations sur la façon d’obtenir une nouvelle URL de métadonnées Workfront, voir [Mettre à jour vos métadonnées ADFS](#update-your-adfs-metadata).

Pour plus d’informations sur l’utilisation d’Active Directory Federation Services (ADFS) avec SAML 2.0 dans Workfront, voir [Configurer Adobe Workfront avec SAML 2.0 à l’aide d’ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
