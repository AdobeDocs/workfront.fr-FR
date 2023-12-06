---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configuration d’Adobe Workfront avec SAML 2.0
description: En tant qu’administrateur Adobe Workfront, vous pouvez configurer les applications web et mobiles Workfront pour les intégrer à une solution SAML 2.0 (Security Assertion Markup Language) pour l’authentification unique (SSO).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: b4fe4dd38bca513f1ce932a8474c06192d97d760
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 6%

---

# Configuration d’Adobe Workfront avec SAML 2.0

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

{{important-admin-console-onboard}}

En tant qu’administrateur Adobe Workfront, vous pouvez configurer les applications web et mobiles Workfront pour les intégrer à une solution SAML 2.0 (Security Assertion Markup Language) pour l’authentification unique (SSO).

Après avoir configuré SAML 2.0 dans Workfront, comme décrit dans les sections suivantes, vous pouvez conserver la configuration, comme décrit dans la section [Mise à jour des métadonnées SAML 2.0 dans votre fournisseur d’identité](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

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
   <td><p>Nouveau plan : Standard </p>
       <p>ou</p> 
       <p>Formule actuelle : Formule </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Activation de l’authentification vers Workfront avec SAML 2.0

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Connexion unique (SSO).**

1. Dans le **Type** liste déroulante, sélectionnez **SAML 2.0.**

1. Dans la partie supérieure des options qui s’affichent, cliquez sur **Téléchargement des métadonnées SAML 2.0** pour télécharger le fichier sur votre ordinateur.

   Votre fournisseur d’identité SAML 2.0 requiert un fichier XML avec les informations générées dans votre instance Workfront. Après avoir téléchargé le fichier, vous devez accéder à votre serveur de fournisseur d’identité SAML 2.0 et y charger le fichier XML de métadonnées SAML 2.0 de Workfront.

1. Spécifiez les informations suivantes dans Workfront :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">ID de fournisseur de services </td>
      <td> Cette URL, déjà renseignée pour vous, identifie Workfront à votre fournisseur d’identité. Par exemple : <code>&lt;yourcompany&gt;.com/SAML2</code>.</td>
     </tr>
     <tr>
      <td role="rowheader">Type de liaison</span> </td>
      <td> <p>Sélectionnez la méthode prise en charge par votre serveur IDP pour envoyer les informations d’authentification :</p>
       <ul>
       <li>POST</li>
       <li>REDIRECT</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">Champs remplis à partir des métadonnées de fournisseurs d'identité </td> 
      <td>Dans votre solution de fournisseur d’identité SAML 2.0, exportez un fichier XML de métadonnées du fournisseur de services et enregistrez-le à un emplacement temporaire sur votre ordinateur. Sélectionner <strong>Choisir un fichier</strong>, puis recherchez et sélectionnez le fichier que vous avez enregistré pour l’ajouter à votre configuration Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL du portail de connexion</span> </td> 
      <td>Saisissez le portail de connexion commun de votre entreprise. Il s’agit de l’URL à laquelle les utilisateurs se connectent pour accéder à Workfront et à toutes les autres applications intégrées à SAML 2.0.</td> 
     </tr>
     <tr>
      <td role="rowheader">URL de déconnexion</span> </td> 
      <td> <p>Saisissez l’URL de déconnexion du serveur IDP. Workfront envoie une requête HTTP à cette URL avant de se déconnecter de Workfront. La session de l’utilisateur se ferme sur le serveur distant à la fermeture de la session Workfront.</p> <p><b>REMARQUE</b>: vous n’êtes redirigé vers l’URL de déconnexion que si vous avez la possibilité <strong>Autoriser uniquement l’authentification SAML 2.0</strong> activée dans votre profil utilisateur.</p> </td>
     </tr>
     <tr>
      <td role="rowheader">Modifier l'URL de mot de passe </td> 
      <td> <p> Spécifiez l’URL vers laquelle les utilisateurs seront redirigés pour modifier leurs mots de passe. </p> <p>Les informations d’identification SAML 2.0 étant utilisées pour accéder à Workfront, les utilisateurs doivent être redirigés vers une page où ils peuvent modifier leur mot de passe SAML 2.0 au lieu de terminer cette activité via Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Algorithme de hachage sécurisé </td> 
      <td> <p>Sélectionnez l’algorithme de hachage sécurisé (SHA) pris en charge par votre fournisseur d’identité :</p> 
       <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuration automatique des utilisateurs</span> </td> 
      <td> <p>Cette option crée automatiquement un utilisateur dans le système lorsqu’un nouvel utilisateur avec un nom d’utilisateur d’annuaire et un mot de passe tente de se connecter à Workfront pour la première fois.</p> <p>Pour créer des utilisateurs dans Workfront, vous devez mapper les attributs de données Workfront avec les attributs de données utilisateur suivants dans votre fournisseur d’annuaire :</p> 
       <ul> 
       <li>Prénom</li> 
       <li>Nom de famille</li> 
       <li>Adresse e-mail</li> 
       </ul> 
       <p>Lorsque vous cochez la case, les options suivantes s’affichent :</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>Sélectionnez l’ attribut utilisateur Workfront que vous souhaitez mapper dans la liste déroulante, puis spécifiez l’ attribut de répertoire correspondant dans le répertoire utilisateur.</p> 
       <p>La variable <strong>Attribut de répertoire</strong> doit contenir le Nom d’attribut de répertoire de la table Attribut utilisateur que vous avez enregistrée lors du test de votre configuration SAML 2.0.</p> 
       <p>Vous pouvez définir une valeur Workfront par défaut dans la variable <strong>Valeur par défaut</strong> champ . Vous pouvez également définir des règles basées sur les valeurs de votre fournisseur d’identité SAML 2.0.</p> 
       <p><b>Avertissement</b>: Workfront tente de mapper les attributs répertoriés ci-dessous chaque fois qu’un utilisateur se connecte au système. Pour cette raison, nous vous déconseillons de mapper les niveaux d’accès. Vous pouvez facilement supprimer l’accès administrateur si un attribut n’est pas mappé correctement. Cliquez sur <strong>Ajouter un mappage</strong> pour ajouter des règles supplémentaires.
       </p> 
       <p>Vous pouvez mapper les attributs Workfront suivants :</p> 
      <ul> 
      <li> <p>Niveau d'accès</p> </li> 
      <li> <p>Adresse</p> </li> 
      <li> <p>Adresse2</p> </li> 
      <li> <p>Facturation par heure</p> </li> 
      <li> <p>Ville</p> </li> 
      <li> <p>Entreprise</p> </li> 
      <li> <p>Coût par heure</p> </li> 
      <li> <p>Adresse e-mail</p> </li> 
      <li> <p>Extension</p> </li> 
      <li> <p>Prénom</p> </li> 
      <li> <p>Groupe principal</p> </li> 
      <li> <p>Équipe interne</p> </li> 
      <li> <p>Fonction</p> </li> 
      <li> <p>Nom de famille</p> </li> 
      <li> <p>Modèles de mise en page</p> </li> 
      <li> <p>Gestionnaire</p> </li> 
      <li> <p>Téléphone portable</p> </li> 
      <li> <p>Numéro de téléphone</p> </li> 
      <li> <p>Code postal</p> </li> 
      <li> <p>Planning</p> </li> 
      <li> <p>Département</p> </li> 
      <li> <p>Profil de feuille de temps</p> </li> 
      <li> <p>Titre</p> </li> 
      </ul>
      <p>Cliquez sur <strong>Enregistrer</strong> lorsque vous avez terminé de mapper les attributs utilisateur.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Certificat </td> 
      <td> <p>Téléchargez un certificat SSL valide pour garantir une connexion sécurisée entre le service d’authentification et Workfront. Pour les comptes OnDemand, un certificat est toujours requis. Vous pouvez obtenir ce certificat auprès de votre administrateur système SAML 2.0.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exemption admin </td> 
      <td> <p>Permet aux administrateurs Workfront d’accéder à Workfront à l’aide de leur connexion Workfront. Si cette option n’est pas sélectionnée, les administrateurs Workfront doivent utiliser leur nom d’utilisateur et mot de passe SAML 2.0.</p> 
      <p>Workfront tente pour la première fois de se connecter à Workfront via SAML 2.0 pour les utilisateurs disposant du niveau d’accès Administrateur système Workfront. Si l’authentification SAML 2.0 échoue, Workfront utilise l’authentification locale pour les administrateurs Workfront.</p> 
      <p>Nous vous recommandons de toujours sélectionner cette option afin que votre administrateur Workfront puisse se connecter à Workfront si votre fournisseur SAML 2.0 est temporairement hors service.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Activer </td> 
      <td> <p>Active la connexion unique sur le système Workfront. Assurez-vous que vous avez communiqué les instructions de connexion à vos utilisateurs.</p> <p>Après avoir activé votre configuration SSO dans Workfront, vous devez activer la fonction <strong>Autoriser uniquement l’authentification SAML 2.0</strong> pour tous les utilisateurs afin qu’ils puissent utiliser SSO.</p> <p>Pour plus d’informations sur la mise à jour des utilisateurs pour SSO, voir <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Mise à jour des utilisateurs pour l’authentification unique</a>.</p> <p>Pour plus d’informations sur les paramètres utilisateur, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Confirmer la configuration </td> 
      <td> 
      <p>Cliquez sur <strong>Tester la connexion</strong> pour vérifier que Workfront et le fournisseur d’identité SAML 2.0 peuvent communiquer entre eux. Cette connexion n'est réussie que si vous avez échangé les fichiers XML.
      </p> 
      <p>Une fois le lien entre votre fournisseur d’identité SAML 2.0 et Workfront testé, un écran similaire à l’image ci-dessous s’affiche.</p>
      <p><b>REMARQUE</b>: cet écran s’affiche dans une fenêtre contextuelle de navigateur. Veillez donc à désactiver le blocage des fenêtres contextuelles dans votre navigateur.</p>
      <p>Enregistrez les informations affichées dans le tableau en vue d’une utilisation ultérieure.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer** pour enregistrer la configuration SAML 2.0.
