---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: 'Scénario Kickstart : préparation Kickstart pour les entreprises, groupes, rôles et utilisateurs et utilisatrices'
description: Lorsque vous commencez à implémenter Adobe Workfront, plutôt que de saisir manuellement des données, vous pouvez importer la liste de vos clientes et clients, les services internes, les fonctions et les informations relatives aux utilisateurs et utilisatrices.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: a8faf4aa1a0a1b60f61c0c981c3be1b0d9d033a4
workflow-type: tm+mt
source-wordcount: '1218'
ht-degree: 84%

---

# Scénario Kick-Starts : préparation Kick-Starts de l’entreprise, du groupe, du rôle et de l’utilisateur

Lorsque vous commencez à implémenter Adobe Workfront, plutôt que de saisir manuellement des données, vous pouvez importer la liste de vos clientes et clients, les services internes, les fonctions et les informations relatives aux utilisateurs et utilisatrices.

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
   <td>
   <p> Nouveau : Standard</p>
   ou
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Éléments que vous pouvez importer

Le tableau suivant répertorie les sociétés, les groupes et les rôles à importer :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Entreprises</strong> </th> 
   <th><strong>Groupes</strong> </th> 
   <th><strong>Rôles</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>Acme, Co</p> <p>Workfront, Inc.</p> <p><em>Votre entreprise</em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">Finances</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">Marketing </p> <p valign="top" rowspan="7">Ventes</p> </td> 
   <td valign="top"> <p valign="top">Personne chargée de l’analyse d’affaires</p> <p valign="top">Personne responsable de la création</p> <p valign="top">Designer</p> <p valign="top">Gestionnaire des ressources</p> <p valign="top">Personnes maîtresse Scrum</p> <p valign="top">Personne chargée de la rédaction technique</p> <p valign="top">Personne chargée du développement web</p> </td> 
  </tr> 
 </tbody> 
</table>

Les noms de rôle doivent être uniques. Les fonctions existantes ne peuvent pas être importées.

Les tableaux suivants présentent les utilisateurs et utilisatrices à importer et plusieurs attributs utilisateur pour chacun d’eux :

### Utilisateur 1

| **Prénom** | Chris |
|---|---|
| **Nom** | Manning |
| **Nom d’utilisateur/Adresse e-mail** | mailto:cmanning@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Membre d&#39;équipe |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Marketing |
| **Fonction** | Personne chargée de l’analyse d’affaires |

{style="table-layout:auto"}

### Utilisatrice 2

| **Prénom** | Jennifer |
|---|---|
| **Nom** | Campbell |
| **Nom d’utilisatrice/Adresse e-mail** | jcampbell@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de projet |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Marketing |
| **Fonction** | Gestionnaire de projet |

{style="table-layout:auto"}

### Utilisatrice 3

| **Prénom** | Jill |
|---|---|
| **Nom** | Sullivan |
| **Nom d’utilisatrice/Adresse e-mail** | jsullivan@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Help Desk |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Ventes |
| **Fonction** | Personne chargée de la représentation commerciale |

{style="table-layout:auto"}

### Utilisateur 4

| **Prénom** | Marc |
|---|---|
| **Nom** | Lewis |
| **Nom d’utilisateur/Adresse e-mail** | mlewis@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de portefeuille |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Finances |
| **Fonction** | Contrôleur |

{style="table-layout:auto"}

### Utilisatrice 5

| **Prénom** | Pam |
|---|---|
| **Nom** | Reynolds |
| **Nom d’utilisatrice/Adresse e-mail** | preynolds@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de projet |
| **Entreprise** | *Votre entreprise>* |
| **Groupe principal** | Marketing |
| **Fonction** | IT |

{style="table-layout:auto"}

### Utilisateur 6

| **Prénom** | Ray |
|---|---|
| **Nom** | Andrews |
| **Nom d’utilisateur/Adresse e-mail** | randrews@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Administrateur ou administratrice |
| **Entreprise** | *Votre entreprise>* |
| **Groupe principal** | Gestionnaire des ressources |
| **Fonction** | Aucune |

{style="table-layout:auto"}

## Télécharger un modèle Kickstart

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Kickstarts** > **Importer des données.**

1. Cliquez sur **Plus d’options** pour afficher la liste complète des options d’import.
1. Sélectionnez les objets Niveau d’accès, Entreprise, Groupe, Fonction et Utilisateur ou utilisatrice à importer.

## Saisir les informations sur l’entreprise

1. Ouvrez le fichier **Workfront.xlsx** que vous venez de télécharger.

   >[!TIP]
   >
   >Lorsque vous utilisez des feuilles de données très volumineuses, vous pouvez utiliser l’outil « Figer les données » (ou équivalent) de votre éditeur de feuille de calcul pour faciliter l’utilisation de la feuille de calcul.

1. Accédez à la feuille « Entreprise CMPY ».

   Il devrait être vide à moins que des entreprises soient déjà dans le système. ![Feuille de la société](assets/cmpysheet-350x16.png)

   ![Identifiant de la société](assets/companyid--1--350x78.png)

1. Indiquez TRUE dans la colonne **isNew**.
1. Répétez cette action pour chaque entreprise ajoutée. (Dans cet exemple, exécutez cette action pour les lignes 3 à 6, car quatre entreprises sont ajoutées.)

   ![La société est nouvelle](assets/cmpyisnew-350x86.png)

1. Indiquez un identifiant unique.

   Cela doit être effectué pour chaque ligne de la colonne Identifiant. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![La société est nouvelle](assets/cmpyisnew-350x86.png)

1. Définissez un nom.

   Indiquez les noms de chaque client et cliente dans la colonne **setName**.

   ![Identifiant de la société](assets/companyid-350x78.png)

1. Accédez à la feuille de groupe GROUP.

   Sauf si vous avez déjà créé des groupes dans Workfront, cette feuille ne doit afficher que le groupe par défaut configuré avec chaque compte de Workfront.

   ![Feuille de groupement](assets/groupsheet-350x15.png) ![Feuille de groupement vide](assets/emptygroupsheet-350x85.png)

1. Définissez la colonne **isNew**. Selon le scénario, 4 groupes seront importés. Par conséquent, indiquez TRUE dans les lignes 4 à 7 pour la colonne « isNew ».
1. Indiquez un identifiant unique.

   Cela doit être effectué pour chaque ligne de la colonne Identifiant. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![ID de groupe](assets/groupids-350x85.png)

1. Définissez un nom.

   Indiquez les noms de chaque département dans la colonne **setName**.

   ![Noms de groupe](assets/groupnames-350x85.png)

   Indiquez les informations de rôle. Accédez à la feuille de rôle ROLE.

1. À moins que vous n’ayez déjà créé ou supprimé des rôles dans votre compte, cette feuille doit afficher 8 rôles configurés avec chaque compte de Workfront.

   ![Noms de groupe](assets/groupnames-350x85.png)

1. Définissez l’instruction True.

   Sept fonctions sont en cours d’import, saisissez TRUE dans les lignes 12 à 18 pour la colonne « isNew ».

   ![Rôle nouveau](assets/roleisnew-350x104.png)

1. Indiquez un identifiant unique.

   Cela doit être effectué pour chaque ligne de la colonne Identifiant. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![Feuille utilisateur](assets/usersheet-350x16.png)

   ![Rôle nouveau](assets/roleisnew--1--350x104.png)

1. Indiquez des noms pour chaque rôle en le saisissant dans la colonne setName.

   ![Rôle nouveau](assets/roleisnew-350x104.png)

1. Indiquez des détails supplémentaires si nécessaire.

   Incluez les taux de facturation, les taux de coûts et les descriptions des rôles que vous créez, si nécessaire.

1. Accédez à la feuille utilisateur USER pour saisir les informations des utilisateurs et utilisatrices.

   Sauf si vous avez déjà créé des utilisateurs et utilisatrices dans votre compte, cette feuille ne doit afficher que l’utilisateur ou utilisatrice Admin de chaque compte de Workfront.

   ![Noms de rôle](assets/rolenames-350x104.png) ![Feuille d’utilisation vide](assets/emptyusersheet-350x52.png)

1. Définissez la valeur True en spécifiant TRUE dans les lignes 4 à 9 pour la colonne « isNew », puisque 6 personnes sont importées.

   ![L’utilisateur est nouveau](assets/userisnew-350x52.png)

1. Définissez un identifiant unique en spécifiant un identifiant unique dans chaque ligne pour la colonne Identifiant. Généralement, les entiers commençant à 1 fonctionnent bien pour les nouveaux enregistrements.

   ![L’utilisateur est nouveau](assets/userisnew-350x52.png)

1. Saisissez les noms de chaque utilisateur et utilisatrice dans les colonnes « setFirstName » et « setLastName ».

   ![Noms d’utilisateur](assets/usernames-350x52.png)

1. Définissez des valeurs détaillées en indiquant des valeurs dans les colonnes « setEmail », « setPassword » et « setUsername ».

   ![Informations d’identification utilisateur](assets/usercredentials-350x52.png)

1. Indiquez les valeurs du niveau d’accès.

   Par exemple, Chris Manning, qui est membre de l’équipe, recherche l’identifiant sur la feuille de niveau d’accès ACSLVL pour le niveau d’accès Personne membre de l’équipe. Copiez l’identifiant dans le presse-papiers, puis collez-le dans la feuille utilisateur USER dans la colonne **setAccessLevelID** sur la ligne de Chris.

   Répétez cette étape pour chaque personne et niveau d’accès.

   ![Copier l’ID de niveau d’accès](assets/copyalid-350x171.png) ![Coller l’ID de niveau d’accès](assets/pastealid-350x59.png)

1. Indiquez les détails du groupe principal.

   Selon le scénario, Chris Manning appartient au groupe Marketing. Dans la feuille de groupe GROUP, recherchez l’identifiant du groupe marketing, copiez-le dans le presse-papiers, puis, dans la feuille utilisateur USER, collez-le dans la colonne **setHomeGroupID** sur la ligne de Chris.Répétez cette étape pour chaque affectation de personne et de groupe.

   ![Copier l’ID de groupe](assets/copygroupid-1-350x133.png) ![Coller l’ID de groupe](assets/pastegroupid-350x59.png)

1. Indiquez les détails de l’entreprise.

   Tous les utilisateurs et utilisatrices de ce scénario appartiennent à la même entreprise. Dans la feuille d’entreprise CMPY, recherchez l’identifiant de l’entreprise *Votre propre entreprise*, copiez l’identifiant dans le presse-papiers, puis, dans l’onglet Utilisateur USER, collez cette valeur dans chaque ligne de la colonne « setCompanyID ».

   Répétez cette étape pour chaque affectation de personne et de groupe.

   ![Identifiant de la société](assets/companyid--1--350x78.png)

   ![Coller l’ID d’entreprise](assets/pastecompanyid-350x84.png)

1. Indiquez les détails de la fonction.

   Selon le scénario, Chris Manning aura le rôle de personne chargée de l’analyse d’affaires. Dans la feuille de rôle ROLE, recherchez l’identifiant du rôle Personne chargée de l’analyse d’affaires, copiez-le dans le presse-papiers, puis, dans la feuille utilisateur USER, collez-le dans la colonne « setRoleID » de la ligne Chris.Répétez cette étape pour chaque affectation de personne et de groupe.

   ![Copier l’ID de rôle](assets/copyroleid-350x149.png)

   ![Coller l’ID de rôle](assets/pasteroleid-350x95.png)

1. Renseignez d’autres informations sur l’utilisateur ou l’utilisatrice, si nécessaire, puis enregistrez le fichier.
1. Importez le fichier Excel.

   Suivez les instructions fournies dans [Importer des données dans Adobe Workfront à l’aide d’un modèle Kickstart](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).



>[!NOTE]
>
>Les utilisateurs importés dans Workfront ont le statut Désactivé et Approbation en attente .
> 
>Si votre organisation a été migrée vers Adobe Admin Console et qu’un utilisateur ne quitte pas le statut Désactivé et Approbation en attente dans les minutes qui suivent, vous pouvez ajouter directement le lot d’utilisateurs au Adobe Admin Console.
>
>Pour obtenir des instructions, voir [Gérer plusieurs utilisateurs | Chargement CSV en masse](https://helpx.adobe.com/fr/enterprise/using/bulk-upload-users.html) dans la documentation d’Adobe.
