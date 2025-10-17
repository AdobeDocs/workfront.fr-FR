---
title: Importer des utilisateurs
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Vous pouvez importer des utilisateurs et utilisatrices sur le site Adobe Workfront en synchronisant les utilisateurs et utilisatrices à partir d’un service de répertoire réseau (Active Directory ou un autre répertoire LDAP, par exemple) ou importer des utilisateurs et utilisatrices à l’aide d’un fichier d’import de feuille de calcul.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 72%

---

# Importer des utilisateurs et utilisatrices

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/fr/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Vous pouvez importer des utilisateurs et utilisatrices à l’aide d’un fichier d’import de feuille de calcul.

Avant de créer un utilisateur ou une utilisatrice, assurez-vous d’abord d’avoir créé tous les objets que vous souhaitez lui associer. Par exemple, si vous n’avez pas créé de planning, vous ne pouvez pas en affecter un au nouvel utilisateur ou utilisatrice, et le champ que vous utilisez pour associer un planning au nouvel utilisateur ou utilisatrice n’apparaît pas dans l’écran Nouvel utilisateur ou utilisatrice.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès de l’administrateur système. </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utiliser un fichier d’import de feuille de calcul pour importer des utilisateurs et utilisatrices

{{step-1-to-users}}

1. Cliquez sur la flèche déroulante **Nouvel utilisateur ou utilisatrice**, puis sur **Importer des utilisateurs et utilisatrices**.

1. Dans la zone **Importer des utilisateurs** qui s’affiche, téléchargez l’exemple de fichier, puis mettez à jour l’exemple de fichier pour inclure les informations personnelles de votre propre utilisateur.

   Chaque ligne comprend les champs suivants :

   * **Prénom**
   * **Nom**
   * **Adresse e-mail**

     Les adresses e-mail doivent être uniques.

   * **Niveau d’accès**

     Les niveaux d’accès respectent la casse.

   * **ID de connexion SSO**

     Ce champ est inclus uniquement si la connexion SSO est activée dans votre système. Vous devez ajouter l’ID de fédération dans ce champ pour chaque utilisateur et utilisatrice. Lorsque vous créez un utilisateur ou une utilisatrice à partir de l’onglet Personnes, vous pouvez configurer un mot de passe pour l’utilisateur ou l’utilisatrice si vous souhaitez permettre aux utilisateurs et utilisatrices de se connecter sans SSO. Toutefois, la fonctionnalité d’import ne vous permet pas de laisser l’ID de connexion SSO vide.

   * Assurez-vous qu’il n’existe aucun espace avant ou après l’adresse e-mail d’un utilisateur ou d’une utilisatrice.

   Lorsque vous avez terminé avec une ligne, elle doit se présenter comme suit :

   ![importing-new-users.png](assets/importing-new-users.png)

1. Enregistrez le fichier à un emplacement de votre poste de travail.
1. Cliquez sur **Choisir un fichier** dans la zone **Importer des utilisateurs**.

1. Accédez au fichier que vous avez enregistré et sélectionnez-le.

<!--
1. (Optional) Select the **Send an invite email to this user** option to send an email invitation to the user, notifying them that a Workfront account has been created and prompting them to set their password.

   Deselect this option if you want to set the password for the user.

-->

1. Cliquez sur **Importer**.

   Un message de confirmation s’affiche en haut de l’écran pour confirmer que l’importation des utilisateurs a réussi.

>[!NOTE]
>
>Les utilisateurs sont créés avec le statut Désactivé et Approbation en attente .
> 
>Si un utilisateur ou une utilisatrice ne quitte pas le statut Désactivé et Approbation en attente dans les minutes qui suivent, et qu’une actualisation de l’écran ne supprime pas le badge Approbation en attente , vous pouvez ajouter directement le lot d’utilisateurs ou d’utilisatrices au Adobe Admin Console.
>
>Pour obtenir des instructions, voir la section [Gérer plusieurs utilisateurs et utilisatrices | Chargement CSV en masse](https://helpx.adobe.com/fr/enterprise/using/bulk-upload-users.html?lang=fr) dans la documentation Adobe.
