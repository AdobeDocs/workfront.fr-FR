---
title: Importer des utilisateurs
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Vous pouvez importer des utilisateurs et utilisatrices sur le site Adobe Workfront en synchronisant les utilisateurs et utilisatrices à partir d’un service de répertoire réseau (Active Directory ou un autre répertoire LDAP, par exemple) ou importer des utilisateurs et utilisatrices à l’aide d’un fichier d’import de feuille de calcul.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 93%

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
   <td><p>Nouveau : Standard</p><p>Ou</p><p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès de l’administrateur système. </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utiliser un fichier d’import de feuille de calcul pour importer des utilisateurs et utilisatrices

{{step-1-to-users}}

1. Cliquez sur la flèche déroulante **Nouvel utilisateur ou utilisatrice**, puis sur **Importer des utilisateurs et utilisatrices**.

1. Dans la zone **Importer des utilisateurs et utilisatrices** qui s’affiche, téléchargez le fichier d’exemple, puis mettez-le à jour afin d’inclure les informations personnelles de votre utilisateur ou utilisatrice.

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
1. Cliquez sur **Choisir un fichier** dans la zone **Importer des utilisateurs et utilisatrices**.

1. Accédez au fichier que vous avez enregistré et sélectionnez-le.
1. (Facultatif) Sélectionnez l’option **Envoyer un e-mail d’invitation à cet utilisateur ou à cette utilisatrice** pour envoyer une invitation par e-mail à l’utilisateur ou à l’utilisatrice, l’informant qu’un compte Workfront a été créé et lui demandant de définir son mot de passe.

   Désélectionnez cette option pour définir le mot de passe de l’utilisateur ou de l’utilisatrice.

1. Cliquez sur **Importer**.

   Vous recevez un message de confirmation en haut de l’écran pour confirmer que l’utilisateur ou l’utilisatrice a bien été importé.
