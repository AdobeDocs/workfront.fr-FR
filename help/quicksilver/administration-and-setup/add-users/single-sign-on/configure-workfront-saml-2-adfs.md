---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configuration d’Adobe Workfront avec SAML 2.0 avec ADFS
description: Vous pouvez activer l’authentification vers Workfront avec SAML 2.0.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 11%

---

# Configurer Adobe Workfront avec SAML 2.0 à l’aide d’ADFS

{{important-admin-console-onboard}}

En tant qu’administrateur Adobe Workfront, vous pouvez intégrer Workfront à une solution SAML 2.0 Security Assertion Markup Language (SAML) pour l’authentification unique lors de l’utilisation des services de fédération Active Directory (ADFS).

Ce guide se concentre sur la configuration d’ADFS sans mise en service automatique ni mappages d’attributs. Nous vous recommandons de terminer la configuration et de la tester avant de configurer toute configuration automatique.

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

## Activation de l’authentification vers Workfront avec SAML 2.0

Pour activer l’authentification à l’application web Workfront et à l’application mobile Workfront avec SAML 2.0, renseignez les sections suivantes :

* [Récupération du fichier de métadonnées SSO Workfront](#retrieve-the-workfront-sso-metadata-file)
* [Configurer des approbations de tiers de confiance](#configure-relying-party-trusts)
* [Configurer des règles de revendication](#configure-claim-rules)
* [Chargement du fichier de métadonnées et test de la connexion](#upload-the-metadata-file-and-test-the-connection)

### Récupération du fichier de métadonnées SSO Workfront {#retrieve-the-workfront-sso-metadata-file}

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système** > **Connexion unique (SSO)**.
1. Dans le menu déroulant **Type**, cliquez sur **SAML 2.0** pour afficher des informations et des options supplémentaires.
1. Copiez l’URL qui s’affiche après **URL de métadonnées**.
1. Passez à la section suivante, [Configurer les approbations de tiers de confiance](#configure-relying-party-trusts).

### Configuration des approbations de tiers de confiance {#configure-relying-party-trusts}

1. Ouvrez le **gestionnaire ADFS** à l’aide du serveur Windows 2008 R2 (la version peut varier).
1. Accédez à **Start.**
1. Cliquez sur **Outils d’administration.**
1. Cliquez sur **Gestion ADFS 2.0.**
1. Sélectionnez **ADFS** et développez **relation de confiance**.
1. Cliquez avec le bouton droit de la souris sur **Fidélisation des membres**, puis sélectionnez **Ajouter la confiance des membres du groupe de confiance** pour lancer l’assistant Ajouter la confiance des membres du groupe de confiance.
1. Dans la **page de bienvenue**, sélectionnez **Démarrer**.
1. Dans la section **Select Date Source** , collez l’URL des métadonnées à partir de Workfront.
1. Cliquez sur **Suivant**.
1. Cliquez sur **OK** pour reconnaître le message d&#39;avertissement.
1. Dans la section **Définir le nom d&#39;affichage**, ajoutez un **nom d&#39;affichage** et des **notes** pour distinguer l&#39;approbation, puis cliquez sur **Suivant**.
1. Sélectionnez **Autoriser tous les utilisateurs à accéder à cette partie de confiance** (ou **Aucun** si vous souhaitez la configurer ultérieurement).
1. Cliquez sur **Suivant**.

   Vous accédez alors à la section **Ready to Add Trust** (Prêt à ajouter une approbation).

1. Passez à la section suivante [Configuration des règles de réclamation](#configure-claim-rules).

### Configuration des règles de demande {#configure-claim-rules}

1. Cliquez sur **Suivant** dans la section **Ready to Add Trust** (Prêt à ajouter une approbation), puis assurez-vous que l’option **de la boîte de dialogue  Modifier les règles de réclamation** est sélectionnée.

   Vous pourrez ainsi modifier les règles de réclamation à une prochaine étape.

1. Cliquez sur **Fermer**.
1. Cliquez sur **Ajouter une règle.**
1. Sélectionnez **Envoyer l’attribut LDAP en tant que revendications**.
1. Cliquez sur **Suivant** pour afficher l’étape **Configurer la règle de revendication** .
1. Spécifiez les exigences minimales suivantes pour configurer la règle de demande : (Cela se passera dans l’ **ID de fédération** sur la configuration de l’utilisateur et sert à distinguer qui se connecte.)


   <table >                
      <tbody>
            <tr>
               <td>Demander le nom de la règle
               </td>
               <td>Indiquez un nom pour la règle de revendication. Par exemple, "Workfront".</td>
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
               <td>Type de demande sortante</td>
               <td>Vous devez sélectionner <b>Name ID</b> comme type de demande sortante.</td>
            </tr>
      </tbody>
   </table>

1. (Facultatif) Pour établir la configuration automatique, ajoutez les revendications supplémentaires suivantes dans l’attribut LDAP et le type de revendication sortante :

   * Prénom
   * Nom
   * Adresse électronique

1. Cliquez sur **Terminer**, puis sur **OK** dans l’écran suivant.
1. Cliquez avec le bouton droit de la souris sur le nouvel **Approbation de partie de confiance**, puis sélectionnez **Propriétés**.
1. Sélectionnez l’**onglet avancé**. Et sous **Secure Hash Algorithm**, sélectionnez SHA-1 ou SHA-256.

   >[!NOTE]
   >
   >L’option que vous sélectionnez sous Algorithme de hachage sécurisé doit correspondre au champ Algorithme de hachage sécurisé de Workfront sous Configuration > Système > Connexion unique (SSO).

1. Passez à la section suivante [Téléchargez le fichier de métadonnées et testez la connexion](#upload-the-metadata-file-and-test-the-connection).

### Chargement du fichier de métadonnées et test de la connexion {#upload-the-metadata-file-and-test-the-connection}

1. Ouvrez un navigateur et accédez à `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   Cela doit télécharger un fichier de métadonnées FederationMetadata.xml .

1. Cliquez sur **Choisir le fichier** sous **Renseigner les champs à partir des métadonnées du fournisseur d’identité**, puis sélectionnez le fichier **FederationMetadata.xml**.

1. (Facultatif) Si les informations sur le certificat n’ont pas été renseignées avec le fichier de métadonnées, vous pouvez charger un fichier séparément. Sélectionnez **Choose File** dans la section **Certificate** .

1. Cliquez sur **Tester la connexion**. Si la configuration est correcte, une page similaire à celle illustrée ci-dessous s’affiche :

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Si vous souhaitez configurer le mappage des attributs, veillez à copier les attributs de Test Connection dans l’attribut de répertoire. Pour plus d’informations, voir Mappage des attributs utilisateur.

1. Sélectionnez **Exception d’administration** pour permettre aux administrateurs Workfront de se connecter à l’aide des informations d’identification Workfront avec l’URL de contournement.

   Les signets pointant vers `<yourdomain>`.my.workfront.com/login contournent la redirection.

1. Sélectionnez la zone **Activer** pour activer la configuration.
1. Cliquer sur **Enregistrer**.

## À propos de la mise à jour des utilisateurs pour SSO

Suivant ce guide, le **nom d’utilisateur SSO** sera leur **nom d’utilisateur Active Directory**.

En tant qu’administrateur Workfront, vous pouvez mettre à jour les utilisateurs en masse pour la connexion unique. Pour plus d’informations sur la mise à jour des utilisateurs pour la SSO, voir [Mettre à jour les utilisateurs et utilisatrices pour l’authentification unique](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

En tant qu’administrateur Workfront, vous pouvez également affecter manuellement un ID de fédération en modifiant le profil de l’utilisateur et en remplissant le champ ID de fédération . Pour plus d’informations sur la modification d’un utilisateur, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>Lors de la modification des profils des utilisateurs pour inclure un ID de fédération, la sélection de l’option **Autoriser uniquement l’authentification SAML 2.0** supprime la possibilité de se connecter à Workfront à l’aide de l’URL de contournement (`<yourdomain>`.my.workfront.com/login).
