---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configuration d’Adobe Workfront avec SAML 2.0 à l’aide d’ADFS
description: Vous pouvez activer l’authentification vers Workfront avec SAML 2.0.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# Configuration d’Adobe Workfront avec SAML 2.0 à l’aide d’ADFS

{{important-admin-console-onboard}}

En tant qu’administrateur Adobe Workfront, vous pouvez intégrer Workfront à une solution SAML 2.0 Security Assertion Markup Language (SAML) pour l’authentification unique tout en utilisant les services de fédération Principale Directory (ADFS).

Ce guide se concentre sur la configuration d’ADFS sans mise en service automatique ni mappages d’attributs. Nous vous recommandons de terminer la configuration et de la tester avant de configurer toute configuration automatique.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Activation de l’authentification vers Workfront avec SAML 2.0

Pour activer l’authentification à l’application web Workfront et à l’application mobile Workfront avec SAML 2.0, renseignez les sections suivantes :

* [Récupération du fichier de métadonnées SSO Workfront](#retrieve-the-workfront-sso-metadata-file)
* [Configuration des approbations de tiers de confiance](#configure-relying-party-trusts)
* [Configuration des règles de demande](#configure-claim-rules)
* [Chargement du fichier de métadonnées et test de la connexion](#upload-the-metadata-file-and-test-the-connection)

### Récupération du fichier de métadonnées SSO Workfront {#retrieve-the-workfront-sso-metadata-file}

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).
1. Dans le panneau de gauche, cliquez sur **Système** > **Authentification unique (SSO)**.
1. Dans le **Type** menu déroulant, cliquez sur **SAML 2.0** pour afficher des informations et des options supplémentaires.
1. Copiez l’URL qui s’affiche après **URL de métadonnées**.
1. Passez à la section suivante, [Configuration des approbations de tiers de confiance](#configure-relying-party-trusts).

### Configuration des approbations de tiers de confiance {#configure-relying-party-trusts}

1. Ouvrez le **Gestionnaire ADFS** en utilisant le serveur Windows 2008 R2 (la version peut varier).
1. Accédez à **Démarrez.**
1. Cliquez sur **Outils d’administration.**
1. Cliquez sur **Gestion ADFS 2.0.**
1. Sélectionner **ADFS** et développer **Relations de confiance**.
1. Clic droit **Confiance des parties**, puis sélectionnez **Ajouter la confiance du parti de confiance** pour lancer l’assistant Ajouter une approbation de partie de confiance.
1. Dans la **Page de bienvenue**, sélectionnez **Début**.
1. Dans le **Sélectionner la source de date** , collez l’URL des métadonnées à partir de Workfront.
1. Cliquez sur **Suivant**.
1. Cliquez sur **OK** pour reconnaître le message d’avertissement.
1. Dans le **Nom d’affichage** , ajoutez une **Nom d’affichage** et **Remarques** pour distinguer l’approbation, cliquez sur **Suivant**.
1. Sélectionner **Autoriser tous les utilisateurs à accéder à cette partie de confiance** (Ou **Aucun** si vous souhaitez le configurer ultérieurement).
1. Cliquez sur **Suivant**.

   Vous accédez alors au **Prêt à ajouter de la confiance** .

1. Passez à la section suivante [Configuration des règles de demande](#configure-claim-rules).

### Configuration des règles de demande {#configure-claim-rules}

1. Cliquez sur **Suivant** dans le **Prêt à ajouter de la confiance** , puis assurez-vous que la variable **Ouvrez la boîte de dialogue Modifier les règles de réclamation .** est sélectionnée.

   Vous pourrez ainsi modifier les règles de réclamation à une prochaine étape.

1. Cliquez sur **Fermer**.
1. Cliquez sur **Ajouter une règle.**
1. Sélectionner **Envoyer l’attribut LDAP en tant que revendications**.
1. Cliquez sur **Suivant** pour afficher la variable **Configuration de la règle de demande** étape .
1. Définissez les conditions minimales suivantes pour configurer la règle de demande : (Cela se répercutera dans la variable **ID de fédération** sur la configuration de l’utilisateur et sert à distinguer qui se connecte.)


   <table >                
      <tbody>
            <tr>
               <td>Demander le nom de la règle
               </td>
               <td>Indiquez un nom pour la règle de revendication. Par exemple, "Workfront".</td>
            </tr>
            <tr>
               <td>Magasin d’attributs</td>
               <td >Sélectionner <b>Principal Directory</b> dans le menu déroulant.</td>
            </tr>
            <tr>
               <td>Attribut LDAP</td>
               <td>Il peut s’agir de n’importe quel type d’attribut. Nous vous recommandons d’utiliser <b>SAM-Account-Name</b> pour cet attribut.</td>
            </tr>
            <tr>
               <td>Type de demande sortante</td>
               <td>Vous devez sélectionner <b>ID de nom</b> comme type de demande sortante</td>
            </tr>
      </tbody>
   </table>

1. (Facultatif) Pour établir la configuration automatique, ajoutez les revendications supplémentaires suivantes dans l’attribut LDAP et le type de revendication sortante :

   * Prénom
   * Nom
   * Adresse électronique

1. Cliquez sur **Terminer**, puis cliquez sur **OK** sur l’écran suivant.
1. Cliquez avec le bouton droit de la souris sur la nouvelle **Confiance du parti de confiance**, puis sélectionnez **Propriétés**.
1. Sélectionnez la **Onglet Avancé**. Et sous **Algorithme de hachage sécurisé** sélectionnez SHA-1 ou SHA-256.

   >[!NOTE]
   >
   >L’option que vous sélectionnez sous Algorithme de hachage sécurisé doit correspondre au champ Algorithme de hachage sécurisé de Workfront sous Configuration > Système > Connexion unique (SSO).

1. Passez à la section suivante [Chargement du fichier de métadonnées et test de la connexion](#upload-the-metadata-file-and-test-the-connection).

### Chargement du fichier de métadonnées et test de la connexion {#upload-the-metadata-file-and-test-the-connection}

1. Ouvrez un navigateur et accédez à `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   Cela doit télécharger un fichier de métadonnées FederationMetadata.xml .

1. Cliquez sur **Choisir un fichier** under **Renseignement des champs à partir des métadonnées du fournisseur d’identité**, puis sélectionnez la variable **FederationMetadata.xml** fichier .

1. (Facultatif) Si les informations sur le certificat n’ont pas été renseignées avec le fichier de métadonnées, vous pouvez charger un fichier séparément. Sélectionner **Choisir un fichier** dans le **Certificat** .

1. Cliquez sur **Tester la connexion**. Si la configuration est correcte, une page similaire à celle illustrée ci-dessous s’affiche :

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Si vous souhaitez configurer le mappage des attributs, veillez à copier les attributs de Test Connection dans l’attribut de répertoire. Pour plus d’informations, voir Mappage des attributs utilisateur.

1. Sélectionner **Exonération pour les administrateurs** pour permettre aux administrateurs Workfront de se connecter à l’aide des informations d’identification Workfront avec l’URL de contournement.

   Signets pointant vers `<yourdomain>`.my.workfront.com/login contournez la redirection.

1. Sélectionnez la **Activer** pour activer la configuration.
1. Cliquer sur **Enregistrer**.

## À propos de la mise à jour des utilisateurs pour SSO

En suivant ce guide, la variable **Nom d’utilisateur SSO** seront leurs **Nom d’utilisateur principale Directory**.

En tant qu’administrateur Workfront, vous pouvez mettre à jour les utilisateurs en masse pour la connexion unique. Pour plus d’informations sur la mise à jour des utilisateurs pour SSO, voir [Mise à jour des utilisateurs pour l’authentification unique](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

En tant qu’administrateur Workfront, vous pouvez également affecter manuellement un ID de fédération en modifiant le profil de l’utilisateur et en remplissant le champ ID de fédération . Pour plus d’informations sur la modification d’un utilisateur, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>Lors de la modification des profils d’utilisateur pour inclure un ID de fédération, en sélectionnant **Autoriser uniquement l’authentification SAML 2.0** supprime la possibilité de se connecter à Workfront à l’aide de l’URL de contournement (`<yourdomain>`.my.workfront.com/login).
