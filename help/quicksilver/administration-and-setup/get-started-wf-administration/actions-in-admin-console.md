---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)
description: Si votre entreprise a été intégrée à Adobe Business Platform, vos utilisateurs utilisent Adobe Business Platform pour accéder à Adobe Workfront. Cela signifie que la gestion des utilisateurs s’effectue en grande partie via Adobe Admin Console et que l’authentification unique (SSO) est gérée via Adobe Business Platform plutôt que par Workfront. En tant qu’administrateur Adobe Workfront, vos responsabilités et procédures d’administration diffèrent selon que votre entreprise a été intégrée à Adobe Business Platform. Cet article répertorie les procédures qui doivent être gérées différemment et fournit des liens vers des instructions pour Workfront et Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 1%

---

# Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)

Si votre entreprise a été intégrée à Adobe Business Platform, vos utilisateurs utilisent Adobe Business Platform pour accéder à Adobe Workfront. Cela signifie que :

* La gestion des utilisateurs s’effectue principalement via Adobe Admin Console.
* L’authentification unique (SSO) est gérée via Adobe Business Platform plutôt que par Workfront.

En tant qu’administrateur Adobe Workfront, vos responsabilités et procédures d’administration diffèrent selon que votre entreprise a été intégrée à Adobe Business Platform. Cet article répertorie les procédures qui doivent être gérées différemment et fournit des liens vers des instructions pour Workfront et Adobe Admin Console.

## Utilisateurs

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Action</th> 
   <th>Pour obtenir des instructions dans Workfront, voir</th> 
   <th>Pour obtenir des instructions sur la console d’administration Adobe, voir</th> 
  </tr> 
 </thead> 
 <tbody> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Octroi d’un accès administrateur utilisateur</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La section "Modifier les détails de l’utilisateur" dans <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gérer les utilisateurs individuellement</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ajout d’un utilisateur à Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Ajouter des utilisateurs</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Gestion des utilisateurs dans Adobe Admin Console</a> </p> </li> 
     <li> <p>La section "Ajouter des utilisateurs" de la section <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gérer les utilisateurs individuellement</a></p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Désactivation d’un utilisateur</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactivation ou réactivation d’un utilisateur</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La section "Suppression d’utilisateurs" de la section <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gérer les utilisateurs individuellement</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Suppression d’un utilisateur</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Suppression d’utilisateurs</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La section "Suppression définitive des utilisateurs" dans <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Gestion des utilisateurs d’annuaire</a>
     </p><p>Remarque : Suppression d’un utilisateur de l’événement [!DNL Adobe Admin Console] désactive l’utilisateur dans [!DNL Workfront], mais ne les supprime pas de [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Modification d’un profil utilisateur</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La section "Modifier les détails de l’utilisateur" dans <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Gérer les utilisateurs individuellement</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Modification en masse de profils utilisateur</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Modification en masse des profils utilisateur</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La section "Modifier les détails de l’utilisateur" dans <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Chargement CSV en masse</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Importer des utilisateurs </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importer des utilisateurs</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La section "Ajouter des utilisateurs" dans <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Chargement CSV en masse</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connexion en tant qu’autre utilisateur</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Connexion en tant qu’autre utilisateur</a> </p> </li> 
    </ul> </td> 
   <td>non disponible</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Renouvellement du certificat SAML</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renouvellement du certificat de métadonnées Adobe Workfront SAML 2.0</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>La section "La signature numérique dans la réponse SAML n’a pas été validée..." in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Federated ID de dépannage</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO (authentification unique)

Comme Adobe Business Platform contrôle l’authentification unique (SSO) pour les utilisateurs, les actions et fonctionnalités suivantes sont gérées automatiquement par l’intermédiaire d’Adobe Business Platform. Si votre entreprise n’a pas encore été intégrée à Adobe Business Platform, vous devez effectuer ces actions dans Workfront.


* [Configuration d’Adobe Workfront avec SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Configuration d’Adobe Workfront avec SAML 2.0 à l’aide d’ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Désactivation de l’authentification unique dans Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [Mise à jour des métadonnées SAML 2.0 dans votre fournisseur d’identité](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Mise à jour des utilisateurs pour l’authentification unique](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [Configuration des stratégies de mot de passe pour l’authentification](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [Configuration des préférences de sécurité système](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
