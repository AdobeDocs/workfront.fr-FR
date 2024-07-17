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
source-git-commit: 5d4434d090c4b6cdefc9c313fecccf6d6e9a510b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)

En tant qu’administrateur d’Adobe Workfront, vos responsabilités et procédures d’administration peuvent varier selon que votre entreprise a été intégrée à Adobe Business Platform ou non. Cet article répertorie les procédures qui sont gérées différemment et fournit des liens vers des instructions pour Workfront et Adobe Admin Console.

Si votre entreprise a été intégrée à Adobe Business Platform, vos utilisateurs utilisent Adobe Business Platform pour accéder à Adobe Workfront. Cela signifie que :

* Les administrateurs système sont créés via Adobe Admin Console
* Le renouvellement d’un certificat SAML est géré via Adobe Admin Console.
* L’authentification unique (SSO) est gérée via Adobe Business Platform plutôt que par Workfront.

## Création d’administrateurs système Workfront dans Adobe Admin Console

>[!NOTE]
>
>Nous vous recommandons d’ajouter des utilisateurs qui ne sont pas administrateurs système directement dans Workfront. Il est possible d’ajouter des utilisateurs dans Adobe Admin Console, mais de les ajouter dans Workfront permet de définir leur niveau d’accès lors de leur création, ce qui peut vous faire gagner du temps.

Pour obtenir des instructions sur la création des administrateurs système Workfront, voir [Gestion des administrateurs système dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Action</th> 
   <th>For instructions in Workfront, see</th> 
   <th>For instructions in the Adobe Admin console, see</th> 
  </tr> 
 </thead> 
 <tbody> 
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
  <tr> 
   <td role="rowheader">Grant a user admin access</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Add a user to Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
     <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
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
  <tr> 
   <td role="rowheader">Deactivate a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Remove users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Delete a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Delete users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Permanently delete users" in <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Manage directory users</a>
     </p><p>Note: Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Edit a user profile</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bulk edit user profiles</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Edit user profiles in bulk</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Import users </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Add users" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Log in as another user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Log in as another user</a> </p> </li> 
    </ul> </td> 
   <td>Not available</td> 
  </tr> 
  <tr> 
    -->

## Renouvellement du certificat SAML

Pour obtenir des instructions sur le renouvellement du certificat SAML sur Adobe Admin Console, reportez-vous à la section &quot;La signature numérique dans la réponse SAML n’a pas été validée..&quot; dans [Federated ID de dépannage](https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html).

<!--

   <td role="rowheader">Renew SAML certificate</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renew the Adobe Workfront SAML 2.0 metadata certificate</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "The digital signature in the SAML response did not validate..." in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Troubleshooting Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

-->

## SSO (authentification unique)

Comme Adobe Business Platform contrôle l’authentification unique (SSO) pour les utilisateurs, les actions et fonctionnalités suivantes sont gérées automatiquement par l’intermédiaire d’Adobe Business Platform. Si votre entreprise n’a pas encore été intégrée à Adobe Business Platform, vous devez effectuer ces actions dans Workfront.


* [Configuration d’Adobe Workfront avec SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [Configuration d’Adobe Workfront avec SAML 2.0 à l’aide d’ADFS](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Désactiver l’authentification unique dans Adobe Workfront](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [Mise à jour des métadonnées SAML 2.0 dans votre fournisseur d’identité](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [Mettre à jour les utilisateurs pour l’authentification unique](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [ Configuration des stratégies de mot de passe pour l’authentification ](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [ Configuration des préférences de sécurité système ](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
