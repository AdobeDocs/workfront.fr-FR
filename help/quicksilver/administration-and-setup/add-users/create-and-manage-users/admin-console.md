---
title: Gestion des utilisateurs dans Adobe Admin Console
description: En tant qu’administrateur ou administratrice Adobe, vous pouvez créer des utilisateurs et utilisatrices Adobe Workfront et des administrateurs et administratrices système à l’aide d’Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '1477'
ht-degree: 72%

---

# Gérer les utilisateurs dans Adobe Admin Console

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

En tant qu’administrateur ou administratrice Adobe, vous pouvez créer des administrateurs et administratrices système Adobe Workfront à l’aide d’Adobe Admin Console. La console est un emplacement central pour la gestion des droits d’Adobe dans l’ensemble de votre organisation. Pour plus d’informations, voir [Vue d’ensemble d’Admin Console](https://helpx.adobe.com/fr/enterprise/using/admin-console.html).

>[!NOTE]
>
>* **Les administrateurs Workfront doivent être configurés dans Adobe Admin Console.** Pour plus d’informations et d’instructions, voir [Création d’administrateurs système dans Workfront avec Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console) dans cet article.
>* **Si votre entreprise utilise l’authentification unique (SSO)** nous vous recommandons de créer des utilisateurs et de les affecter à Workfront dans Adobe Admin Console. La création de ces utilisateurs dans Workfront est possible, mais il peut y avoir des problèmes de transfert de ces informations vers Adobe Admin Console, en fonction de la configuration d’Admin Console dans votre organisation.
>  >   Après avoir créé l’utilisateur dans le Adobe Admin Console, vous pouvez configurer ses informations dans Workfront, telles que l’attribution de rôles, de groupes, d’équipes et de niveaux d’accès.
>* **Si votre entreprise n’utilise pas l’authentification unique (SSO)** vous pouvez ajouter des utilisateurs qui ne sont pas administrateurs système directement dans Workfront. Vous pouvez ajouter des utilisateurs et utilisatrices dans Adobe Admin Console, mais les ajouter dans Workfront permet de définir leur niveau d’accès lors de leur création, ce qui peut vous faire gagner du temps.

Lorsque vous apportez des modifications aux profils des utilisateurs à partir d’Admin Console, une mise à jour est ajoutée à l’onglet Activité du système de l’utilisateur dans Workfront. La mise à jour s’affiche comme effectuée par le « Système ». Il s’agit de l’administrateur Adobe Admin Console et non de l’administrateur principal Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Droits d’administration Adobe</td> 
   <td> <p>Vous devez être administrateur de profil de produit des produits Adobe pour votre organisation</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant d’utiliser Admin Console pour Workfront, vous devriez recevoir un e-mail vous invitant à accéder à la console.

1. Si vous découvrez Adobe et que vous avez reçu un e-mail vous indiquant que vous disposez désormais des droits d’administration pour gérer les logiciels et services d’Adobe pour votre organisation, cliquez sur le bouton de l’e-mail pour créer un compte Adobe et ouvrir Admin Console.

   Ou

   Si vous disposez déjà d’un compte Adobe, accédez à la [page Adobe Admin Console](https://adminconsole.adobe.com/).

## Informations supplémentaires sur Adobe Admin Console

* Les administrateurs et administratrices système de Workfront peuvent désactiver un utilisateur ou une utilisatrice Workfront depuis Workfront, mais cela ne désactive pas la personne dans Admin Console.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* Le **groupe interne** de l’utilisateur ou utilisatrice est déterminé en fonction de la personne qui l’a créé. Il n’est pas personnalisable dans Admin Console.
* Le niveau d’accès Administration système Workfront ne peut être modifié que depuis Adobe Admin Console.

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* La modification de l’accès d’une personne par un administrateur ou une administratrice système à tout autre niveau d’accès doit d’abord être effectuée par le biais d’Admin Console .

  <!--
   This is not clear
  -->

* Pour supprimer l’accès Administrateur ou administratrice système d’une personne dans Workfront, vous devez utiliser Adobe Admin Console pour supprimer la personne en tant qu’administrateur ou administratrice de profil de produit. Cela modifie le niveau d’accès Workfront de la personne, d’administrateur ou administratrice système à Demandeur ou demandeuse.

  >[!IMPORTANT]
  >
  >N’apportez aucune modification au profil de produit lui-même.

* Les administrateurs et administratrices de Adobe Admin Console peuvent configurer des règles d’affectation automatique pour automatiser le processus d’attribution de produits Adobe aux utilisateurs et utilisatrices de leur entreprise. Votre organisation doit être migrée vers l’expérience unifiée Adobe pour utiliser cette fonctionnalité. Pour plus d’informations et d’instructions, consultez [Gestion des règles d’affectation automatique](https://helpx.adobe.com/enterprise/using/automatic-assignment-rules.html) dans la documentation d’Adobe.

  >[!NOTE]
  >
  >Si vous sélectionnez une organisation approuvée lors de la configuration des affectations automatiques, cette organisation se trouve dans la zone Utilisateurs dans les répertoires ou domaines sélectionnés. Cliquez sur la flèche de liste déroulante en regard du champ **Sélectionner un répertoire** et sélectionnez les organisations. Les organisations de confiance sont marquées d&#39;un badge de confiance.

## Accéder à la zone utilisateur et administration de votre instance de production Workfront {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. Dans la [page Adobe Admin Console](https://adminconsole.adobe.com/), sélectionnez l’onglet **Produits** dans la barre de navigation supérieure, puis sélectionnez **Workfront**.

   <!--![Admin Console product](assets/admin-product-1.png)-->

1. Dans la liste qui s’affiche, sélectionnez le lien en haut.

   Il s’agit de votre instance de production où travaillent vos utilisateurs et utilisatrices.

   <!--![Admin Console instances](assets/instances-1.png)-->

   >[!TIP]
   >
   >Le deuxième lien de la liste, votre instance de prévisualisation, est un environnement de test qui reproduit votre environnement de production actif. Pour plus d’informations, voir [Environnement de prévisualisation de sandbox Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >Vous pouvez également voir des liens vers des environnements de sandbox dans la liste. Pour plus d’informations, voir [Environnement de prévisualisation de sandbox Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. Dans la liste qui s’affiche, avec l’onglet **Profils de produit** sélectionné, cliquez sur le nom du lien Profil produit Workfront.

   ![Profils de produit](assets/prod-profile-1.png)

   Cette liste comprend toutes les personnes déjà affectées à votre instance de production de Workfront.

   >[!IMPORTANT]
   >
   >N’apportez aucune modification au profil de produit lui-même.

1. Passez à l’une des sections suivantes de cet article :

   * [Créer des utilisateurs et utilisatrices dans Workfront avec Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Créer des administrateurs et administratrices système dans Workfront avec Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Créer des administrateurs et administratrices système dans Workfront avec Adobe Admin Console {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

<!--Audited: 12/2023-->

Le niveau d’accès Administrateur ou administratrice système n’est accordé que sur Adobe Admin Console. Vous ne pouvez pas accorder ou supprimer l’accès administrateur ou administratrice dans Workfront.

Vous devez ajouter un utilisateur ou une utilisatrice à votre instance de production de Workfront avant de pouvoir en faire un administrateur ou une administratrice système Workfront.

1. Accédez à la zone utilisateur/utilisatrice et administrateur/administratrice dans Admin Console, comme décrit dans la section [Accéder à la zone utilisateur/utilisatrice et administrateur/administratrice de votre instance de production de Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) dans cet article.
1. Sélectionnez l’onglet **Administration** au-dessus de la liste des utilisateurs et des utilisatrices.
1. Sélectionnez **Ajouter un administrateur ou une administratrice**.
1. Dans la zone **Ajouter des administrateurs/administratrices de profil de produit**, saisissez les adresses e-mails ou les noms des administrateurs et des administratrices à ajouter, puis sélectionnez **Enregistrer**.

   ![Ajouter un administrateur](assets/add-admin-1.png)

   Les administrateurs et administratrices système sont créés dans Workfront.

   >[!IMPORTANT]
   >
   >N’apportez aucune modification au profil de produit lui-même.


## Créer des utilisateurs et des utilisatrices dans Workfront avec Adobe Admin Console {#create-users-in-workfront-with-the-adobe-admin-console}

>[!NOTE]
>
>Nous vous recommandons d’ajouter les utilisateurs et utilisatrices qui ne sont pas en charge de l’administration système directement dans Workfront. Vous pouvez ajouter des utilisateurs et utilisatrices dans Adobe Admin Console, mais les ajouter dans Workfront permet de définir leur niveau d’accès lors de leur création, ce qui peut vous faire gagner du temps.

* [Créer des utilisateurs et des utilisatrices dans Workfront directement dans Adobe Admin Console](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [Créer des utilisateurs et des utilisatrices dans Workfront et les approuver pour Adobe Admin Console](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### Créer des utilisateurs et des utilisatrices dans Workfront directement dans Adobe Admin Console

1. Accédez à la zone utilisateur/utilisatrice et administrateur/administratrice dans Admin Console, comme décrit dans la section [Accéder à la zone utilisateur/utilisatrice et administrateur/administratrice de votre instance de production de Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) dans cet article.
1. Après avoir sélectionné l’onglet **Utilisateurs et utilisatrices** au-dessus de la liste, sélectionnez **Ajouter un utilisateur/une utilisatrice**.
1. Dans la zone **Ajouter des utilisateurs/utilisatrices à ce profil de produit** , saisissez l’adresse e-mail ou le nom d’un utilisateur ou d’une utilisatrice que vous souhaitez ajouter, puis sélectionnez **Enregistrer**.

   L’utilisateur est créé dans Workfront avec le niveau d’accès Demandeur ou Contributeur , selon le package Workfront de votre entreprise.

   >[!IMPORTANT]
   >
   >N’apportez aucune modification au profil de produit lui-même.

1. Dans Workfront, modifiez le niveau d’accès de l’utilisateur ou de l’utilisatrice.

   Pour obtenir des instructions sur la façon dont un administrateur ou une administratrice Workfront peut modifier le niveau d’accès de l’utilisateur ou de l’utilisatrice, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Répétez les étapes 3 et 4 pour ajouter d’autres utilisateurs et utilisatrices.

   >[!NOTE]
   >
   >Admin Console envoie un e-mail aux nouveaux utilisateurs et aux nouvelles utilisatrices d’Adobe les invitant à terminer le processus d’enregistrement. Tous les utilisateurs et toutes les utilisatrices doivent terminer le processus d’enregistrement pour accéder à toutes les applications Adobe.
   >
   >Pour les utilisateurs et utilisatrices d’Adobe existants, l’utilisateur ou l’utilisatrice peut recevoir ou non un e-mail sur la disponibilité de Workfront. Il s’agit d’une préférence contrôlée par l’administrateur ou l’administratrice d’Adobe pour le produit. Votre administrateur ou administratrice Adobe peut être une personne différente de votre administrateur ou administratrice Workfront.

### Créer des utilisateurs et des utilisatrices dans Workfront et les approuver pour Adobe Admin Console

Ce workflow permet aux administrateurs et aux administratrices de groupe qui n’ont pas accès à Adobe Admin Console de créer des utilisateurs et des utilisatrices.

Tout d’abord, l’administrateur ou l’administratrice de groupe crée l’utilisateur ou l’utilisatrice dans Workfront. L’utilisateur ou l’utilisatrice est ainsi créé avec les status Désactivé et En attente d’approbation.

Ensuite, un administrateur ou une administratrice Workfront approuve l’utilisateur ou l’utilisatrice. L’utilisateur ou l’utilisatrice est ainsi activé dans Workfront et ajouté à Adobe Admin Console.

#### Créer l’utilisateur ou l’utilisatrice dans Workfront (administrateur ou administratrice de groupes)

Pour obtenir des instructions sur la création d’un utilisateur ou d’une utilisatrice dans Workfront, voir [Ajouter des utilisateurs et des utilisatrices](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md).

#### Approuver l’utilisateur ou l’utilisatrice (administrateur ou administratrice Workfront)

Pour approuver un utilisateur ou une utilisatrice :

{{step-1-to-users}}

1. Sélectionnez l’utilisateur, puis cliquez sur l’icône **Plus** ![Plus](assets/more-icon.png).

1. Pour approuver l’utilisateur ou l’utilisatrice, cliquez sur **Approuver**, puis cliquez sur **Soumettre**.

   Ou

   Pour rejeter et supprimer l’utilisateur ou l’utilisatrice de Workfront, cliquez sur **Rejeter**, puis sur **Soumettre**.

   Les utilisateurs et les utilisatrices approuvés sont automatiquement ajoutés à Adobe Admin Console.

   Les utilisateurs et les utilisatrices refusés sont automatiquement supprimés de Workfront.


## Modifier les utilisateurs existants dans le Adobe Admin Console

Vous pouvez modifier les détails de l’utilisateur ci-dessous dans le Adobe Admin Console :

* Groupes d’utilisateurs et produits associés à l’utilisateur
* Droits administratifs
* Pays

Pour plus d’informations sur la modification d’un utilisateur unique dans Adobe Admin Console, consultez la section [Modifier les détails de l’utilisateur](https://helpx.adobe.com/enterprise/using/manage-users-individually.html#edit-user-details) dans l’article Gestion individuelle des utilisateurs dans la documentation d’Adobe.

Pour plus d’informations sur la modification en bloc des utilisateurs dans Adobe Admin Console, voir
[Modifier les détails de l’utilisateur](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html#edit-user-details) dans l’article Gestion de plusieurs utilisateurs dans la documentation d’Adobe.
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>You can create Adobe Workfront users and system administrators with the <a href="https://adminconsole.adobe.com/" alt="Admin Console link">Adobe Admin Console</a>. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the <a href="https://helpx.adobe.com/enterprise/using/admin-console.html" alt="Admin Console Overview">Admin Console Overview</a>.</p>
<p>Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. Click in the invitation to accept it and create an account. You can also use an existing account, if already available.</p>
<h2>Create users</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Create users in WF with the Adobe admin console</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">May need to add something about oging throug WF -- check with Jonah</p>

<p>To create users in Workfront with the Admin Console:</p>
<ol>
<li value="1"> <p>From the <a href="https://adminconsole.adobe.com/">Admin Console page</a>, select the <b>Products</b> tab and then select the <b>Workfront</b> product tile.</p> </li>
<li value="2"> <p>Select the link to the Workfront instance you want to change.</p> </li>
<li value="3"> <p>Select the Product profile link. This shows a list of the currently-assigned users. If the list is very long, you can also search for users in the search field above the list.</p> </li>
<li value="4"> <p>Select the <b>Add User</b> button.</p> </li>
<li value="5"> <p>In the <b>Add users</b> box, enter the email address or name of the user you want to add. Select <b>Save</b>. The administrator is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Create system administrators</h2>
<p>To create system administrators:</p>
<ol>
<li value="1"> <p>Make product profile assignments first. To be a Workfront System Administrator, the user must be assigned the Workfront product profile and be an admin for that product profile.</p> </li>
<li value="2"> <p>From the console, select the <b>Products</b> tab and then select the <b>Admins</b> tab. </p> </li>
<li value="3"> <p>Select <b>Add Admin</b>.</p> </li>
<li value="4"> <p>In the <b>Add product profile administrators</b> box, enter the email address or name of the administrator you want to add. Select <b>Save</b>. The user is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Additional details for the Admin Console</h2>
<ul>
<li> <p>System Administrator access level is granted only on the Admin Console. You cannot grant or remove admin access from within Workfront.</p> </li>
</ul>
<ul>
<li> <p>Creating and deleting users inside Workfront is only possible through the Admin Console.</p> </li>
<li> <p>Workfront System Administrators can deactivate Workfront users from within Workfront, but this does not deactivate the user in the Admin Console.</p> </li>
<li> <p>All new users are are assigned <b>Requestor</b> access level upon creation. Also, the user <b>Home Group</b> is determined based on the user who created them. This is currently not customizable from within the Admin Console.</p> </li>
<li> <p>The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.</p> </li>
<li> <p>Editing a user who is a system admin to any other access level must be done through the Admin Console first.</p> </li>
<li> <p>To remove Workfront system admin access, remove users as Product Profile Administrators. This action changes the user access level in Workfront from a system admin to a <b>Requestor</b>.</p> </li>
</ul>
</div>
-->
