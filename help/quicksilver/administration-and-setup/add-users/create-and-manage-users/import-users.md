---
title: Importer des utilisateurs et utilisatrices
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Vous pouvez importer des utilisateurs sur le site Adobe Workfront en synchronisant les utilisateurs à partir d’un service d’annuaire réseau (Active Directory ou un autre annuaire LDAP, par exemple) ou importer des utilisateurs à l’aide d’un fichier d’importation de feuille de calcul.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 1949a0bb213553f1f1f252c4382a90514fcd0b5b
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 27%

---

# Importer des utilisateurs et utilisatrices

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Vous pouvez importer des utilisateurs à l’aide d’un fichier d’importation de feuille de calcul.

Avant de créer un utilisateur, assurez-vous d’abord d’avoir créé tous les objets que vous souhaitez associer à l’utilisateur. Par exemple, si vous n’avez pas créé de planning, vous ne pouvez pas en attribuer un au nouvel utilisateur, et le champ que vous utilisez pour associer un planning au nouvel utilisateur n’apparaît pas dans l’écran Nouvel utilisateur.

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

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
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur ou administratrice système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à un utilisateur ou une utilisatrice</a>. </p> </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Parmi ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être administrateur ou administratrice d’un groupe dont l’utilisateur est membre.</p> <p>Pour plus d’informations sur le paramètre <b>Utilisateurs et utilisatrices</b> dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Utiliser un fichier d’importation de feuille de calcul pour importer des utilisateurs

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Utilisateurs et utilisatrices** ![](assets/users-icon-in-main-menu.png).

1. Cliquez sur la flèche de liste déroulante **Nouvel utilisateur**, puis sur **Importer des utilisateurs**.

1. Dans la zone **Importer des utilisateurs** qui s’affiche, téléchargez le fichier d’exemple, puis mettez à jour le fichier d’exemple afin d’inclure les informations personnelles de votre propre utilisateur.

   Chaque ligne comprend les champs suivants :

   * **Prénom**
   * **Nom**
   * **Adresse de courriel**

     Les adresses électroniques doivent être uniques.

   * **Niveau d’accès**

     Les niveaux d’accès sont sensibles à la casse.

   * **Identifiant de connexion SSO**

     Ce champ est inclus uniquement si SSO est activé dans votre système. Vous devez ajouter l&#39;ID de fédération dans ce champ pour chaque utilisateur. Lorsque vous créez un utilisateur à partir de l’onglet Personnes, vous pouvez configurer un mot de passe pour l’utilisateur si vous souhaitez permettre aux utilisateurs de se connecter sans authentification unique. Toutefois, la fonction d’importation ne vous permet pas de laisser l’identifiant de connexion SSO vide.

   * Assurez-vous qu’il n’existe aucun espace avant ou après l’adresse électronique d’un utilisateur.

   Lorsque vous avez terminé avec une ligne, elle doit se présenter comme suit :

   ![import-new-users.png](assets/importing-new-users.png)

1. Enregistrez le fichier à un emplacement de votre poste de travail.
1. Cliquez sur **Choose File** dans la zone **Import Users**.

1. Accédez au fichier que vous avez enregistré et sélectionnez-le.
1. (Facultatif) Sélectionnez l’option **Envoyer un courrier électronique d’invitation à cet utilisateur** pour envoyer une invitation par courrier électronique à l’utilisateur, lui indiquant qu’un compte Workfront a été créé et lui demandant de définir son mot de passe.

   Désélectionnez cette option pour définir le mot de passe de l’utilisateur.

1. Cliquez sur **Importer**.

   Un message de confirmation s’affiche en haut de l’écran pour confirmer que l’utilisateur a bien été importé.
