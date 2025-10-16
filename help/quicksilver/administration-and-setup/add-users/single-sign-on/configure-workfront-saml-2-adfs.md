---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configuration d’Adobe Workfront avec SAML 2.0 à l’aide d’ADFS
description: Vous pouvez activer l’authentification à Workfront avec SAML 2.0.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 98%

---

# Configurer Adobe Workfront avec SAML 2.0 à l’aide d’ADFS

{{important-admin-console-onboard}}

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez intégrer Workfront à une solution SAML 2.0 pour une authentification unique à l’aide d’ADFS.

Ce guide aborde la configuration d’ADFS sans approvisionnement automatique ni mappage d’attributs. Nous vous recommandons de terminer la configuration et de la tester avant de mettre en place l’approvisionnement automatique.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Activer l’authentification à Workfront avec SAML 2.0

Pour activer l’authentification à l’application web Workfront et à l’application mobile Workfront avec SAML 2.0, accomplissez les sections suivantes :

* [Récupérer le fichier de métadonnées Workfront SSO](#retrieve-the-workfront-sso-metadata-file)
* [Configurer les parties de confiance](#configure-relying-party-trusts)
* [Configurer les règles de revendication](#configure-claim-rules)
* [Charger le fichier de métadonnées et tester la connexion](#upload-the-metadata-file-and-test-the-connection)

### Récupérer le fichier de métadonnées Workfront SSO {#retrieve-the-workfront-sso-metadata-file}

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système** > **Authentification unique (SSO)**.
1. Dans le menu déroulant **Type**, cliquez sur **SAML 2.0** pour afficher des informations et des options supplémentaires.
1. Copiez l’URL qui s’affiche après **URL de métadonnées**.
1. Poursuivez vers la section suivante, [Configurer les parties de confiance](#configure-relying-party-trusts).

### Configurer les parties de confiance {#configure-relying-party-trusts}

1. Ouvrez le **Gestionnaire ADFS** via Windows Server 2008 R2 (la version peut varier).
1. Accédez à **Démarrer.**
1. Cliquez sur **Outils d’administration.**
1. Cliquez sur **Gestion d’ADFS 2.0.**
1. Sélectionnez **ADFS** et développez **Relations de confiance**.
1. Cliquez avec le bouton droit de la souris sur **Parties de confiance**, puis sélectionnez **Ajouter une partie de confiance** pour lancer l’assistant d’ajout de partie de confiance.
1. À partir de la **Page d’accueil**, sélectionnez **Démarrer**.
1. Dans la section **Sélectionner une source de données**, collez l’URL de métadonnées de Workfront.
1. Cliquez sur **Suivant**.
1. Cliquez sur **OK** pour confirmer le message d’avertissement.
1. Dans la section **Spécifier le nom d’affichage**, ajoutez un **Nom d’affichage** et des **Notes** pour pouvoir distinguer la partie de confiance, puis cliquez sur **Suivant**.
1. Sélectionnez **Autoriser tous les utilisateurs et utilisatrices à accéder à cette partie de confiance** (ou **Aucun** si vous souhaitez configurer cette option ultérieurement).
1. Cliquez sur **Suivant**.

   Vous accédez alors à la section **Partie de confiance prête à être ajoutée**.

1. Poursuivez vers la section suivante [Configurer les règles de revendication](#configure-claim-rules).

### Configurer les règles de revendication {#configure-claim-rules}

1. Cliquez sur **Suivant** dans la section **Partie de confiance prête à être ajoutée**, puis vérifiez que l’option **Ouvrir la boîte de dialogue Modifier les règles de revendication** est sélectionnée.

   Cela vous permet de modifier les règles de revendication lors d’une étape ultérieure.

1. Cliquez sur **Fermer**.
1. Cliquez sur **Ajouter une règle.**
1. Sélectionnez **Envoyer les attributs LDAP en tant que revendications**.
1. Cliquez sur **Suivant** pour afficher l’étape **Configurer une règle de revendication**.
1. Spécifiez les conditions minimales requises suivantes pour configurer la règle de revendication : (celles-ci vont dans l’**ID de fédération** dans la configuration de l’utilisateur ou de l’utilisatrice et sont utilisées pour identifier la personne qui se connecte).


   <table >                
      <tbody>
            <tr>
               <td>Nom de la règle de revendication
               </td>
               <td>Spécifiez un nom pour la règle de revendication. Par exemple, « Workfront ».</td>
            </tr>
            <tr>
               <td>Magasin d’attributs</td>
               <td >Sélectionnez <b>Active Directory</b> dans le menu déroulant.</td>
            </tr>
            <tr>
               <td>Attribut LDAP</td>
               <td>Il peut s’agir de n’importe quel type d’attribut. Nous vous recommandons d’utiliser <b>SAM-Account-Name</b> pour cet attribut.</td>
            </tr>
            <tr>
               <td>Type de revendication sortante</td>
               <td>Vous devez sélectionner <b>Identifiant de nom</b> comme type de revendication sortante.</td>
            </tr>
      </tbody>
   </table>

1. (Facultatif) Afin de mettre en place l’approvisionnement automatique, ajoutez les revendications supplémentaires suivantes dans l’attribut LDAP et dans le type de revendication sortante :

   * Prénom
   * Nom
   * Adresse e-mail

1. Cliquez sur **Terminé**, puis sur **OK** sur l’écran suivant.
1. Cliquez avec le bouton droit de la souris sur la nouvelle **Partie de confiance**, puis sélectionnez **Propriétés**.
1. Sélectionnez l’**onglet Avancé**. Puis, dans **Algorithme de hachage sécurisé**, sélectionnez SHA-1 ou SHA-256.

   >[!NOTE]
   >
   >L’option que vous sélectionnez pour l’algorithme de hachage sécurisé doit correspondre au champ Algorithme de hachage sécurisé dans Workfront situé dans Configuration > Système > Authentification unique (SSO).

1. Poursuivez vers la section suivante [Charger le fichier de métadonnées et tester la connexion](#upload-the-metadata-file-and-test-the-connection).

### Charger le fichier de métadonnées et tester la connexion {#upload-the-metadata-file-and-test-the-connection}

1. Ouvrez un navigateur et accédez à `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml`.

   Cela doit lancer le téléchargement d’un fichier de métadonnées nommé FederationMetadata.xml.

1. Cliquez sur **Choisir un fichier** dans **Renseigner les champs à partir des métadonnées du fournisseur d’identité** et sélectionnez le fichier **FederationMetadata.xml**.

1. (Facultatif) Si les informations relatives au certificat n’ont pas été renseignées à l’aide du fichier de métadonnées, vous pouvez charger un autre fichier séparément. Sélectionnez **Choisir un fichier** dans la section **Certificat**.

1. Cliquez sur **Tester la connexion**. Si la configuration est correcte, vous devez voir apparaître une page similaire à celle présentée ci-dessous :

   ![Message de réussite SAML 2](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Si vous souhaitez mettre en place un mappage d’attributs, veillez à copier les attributs de la connexion de test dans le répertoire Attributs. Pour plus d’informations, voir Mappage des attributs des utilisateurs et des utilisatrices.

1. Sélectionnez **Exception pour les administrateurs et les administratrices** pour permettre aux administrateurs et aux administratrices Workfront de se connecter à l’aide des informations d’identification de Workfront via l’URL de contournement.

   Les marque-pages qui dirigent vers `<yourdomain>`.my.workfront.com/login contournent la redirection.

1. Cochez la case **Activer** pour activer la configuration.
1. Cliquer sur **Enregistrer**.

## À propos de la mise à jour des utilisateurs et des utilisatrices pour l’authentification unique

En suivant ce guide, le **nom d’utilisateur ou d’utilisatrice pour l’authentification unique** devient le **nom d’utilisateur ou d’utilisatrice pour Active Directory**.

En tant qu’administrateur ou administratrice Workfront, vous pouvez mettre à jour en masse les utilisateurs et les utilisatrices pour l’authentification unique. Pour plus d’informations sur la mise à jour des utilisateurs et des utilisatrices pour l’authentification unique, voir [Mettre à jour les utilisateurs et les utilisatrices pour l’authentification unique](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

En tant qu’administrateur ou administratrice Workfront, vous pouvez également attribuer manuellement un identifiant de fédération en modifiant le profil de l’utilisateur ou de l’utilisatrice et en renseignant le champ ID de fédération. Pour plus d’informations sur la modification d’un utilisateur ou d’une utilisatrice, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>Lorsque vous modifiez des profils d’utilisateurs et d’utilisatrices pour inclure un ID de fédération, sélectionner **Autoriser uniquement l’authentification SAML 2.0** supprime la possibilité de se connecter à Workfront en utilisant l’URL de contournement (`<yourdomain>`.my.workfront.com/login).
