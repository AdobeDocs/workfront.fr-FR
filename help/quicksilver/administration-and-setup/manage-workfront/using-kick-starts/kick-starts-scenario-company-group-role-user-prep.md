---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: 'Scénario Kickstart : préparation Kickstart pour les entreprises, groupes, rôles et utilisateurs et utilisatrices'
description: Lorsque vous commencez à implémenter Adobe Workfront, plutôt que de saisir manuellement des données, vous pouvez importer la liste de vos clientes et clients, les services internes, les fonctions et les informations relatives aux utilisateurs et utilisatrices.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 59431354076a0909fb1878d68cf266f08d2114b3
workflow-type: tm+mt
source-wordcount: '1216'
ht-degree: 53%

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

| Entreprises | Groupes | Rôles |
|---|---|---|
| Acme, Co <p>Workfront, Inc. <p>_Votre entreprise_ <p>XYZ, Inc. | Finances <p>IT <p>Marketing <p>Ventes | Personne chargée de l’analyse d’affaires <p>Personne responsable de la création <p>Designer <p>Gestionnaire des ressources <p>Personnes maîtresse Scrum <p>Personne chargée de la rédaction technique <p>Personne chargée du développement web |

{style="table-layout:auto"}

Les noms de rôle doivent être uniques. Les fonctions existantes ne peuvent pas être importées.

Les tableaux suivants présentent les utilisateurs et utilisatrices à importer et plusieurs attributs utilisateur pour chacun d’eux :

### Utilisateur 1

| Attribut | Valeur |
|---|---|
| **Prénom** | Chris |
| **Nom** | Manning |
| **Nom d’utilisateur/Adresse e-mail** | mailto:cmanning@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Membre d&#39;équipe |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Marketing |
| **Fonction** | Personne chargée de l’analyse d’affaires |

{style="table-layout:auto"}

### Utilisatrice 2

| Attribut | Valeur |
|---|---|
| **Prénom** | Jennifer |
| **Nom** | Campbell |
| **Nom d’utilisatrice/Adresse e-mail** | jcampbell@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de projet |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Marketing |
| **Fonction** | Gestionnaire de projet |

{style="table-layout:auto"}

### Utilisatrice 3

| Attribut | Valeur |
|---|---|
| **Prénom** | Jill |
| **Nom** | Sullivan |
| **Nom d’utilisatrice/Adresse e-mail** | jsullivan@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Help Desk |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Ventes |
| **Fonction** | Personne chargée de la représentation commerciale |

{style="table-layout:auto"}

### Utilisateur 4

| Attribut | Valeur |
|---|---|
| **Prénom** | Marc |
| **Nom** | Lewis |
| **Nom d’utilisateur/Adresse e-mail** | mlewis@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de portefeuille |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Finances |
| **Fonction** | Contrôleur |

{style="table-layout:auto"}

### Utilisatrice 5

| Attribut | Valeur |
|---|---|
| **Prénom** | Pam |
| **Nom** | Reynolds |
| **Nom d’utilisatrice/Adresse e-mail** | preynolds@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de projet |
| **Entreprise** | *Votre entreprise>* |
| **Groupe principal** | Marketing |
| **Fonction** | IT |

{style="table-layout:auto"}

### Utilisateur 6

| Attribut | Valeur |
|---|---|
| **Prénom** | Ray |
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
1. Cliquez sur **Télécharger**.

## Saisir les informations sur l’entreprise

1. Ouvrez le fichier **Workfront.xlsx** que vous venez de télécharger.

   >[!TIP]
   >
   >Lorsque vous utilisez des feuilles de données très volumineuses, vous pouvez utiliser l’outil « Figer les données » (ou équivalent) de votre éditeur de feuille de calcul pour faciliter l’utilisation de la feuille de calcul.

1. Accédez à la fiche **Société CMPY**.

   Il devrait être vide à moins que des entreprises soient déjà dans le système.

   ![Feuille de société](assets/cmpysheet-350x16.png) ![ID de société](assets/companyid--1--350x78.png)

1. Saisissez **TRUE** dans la colonne **isNew**.

   Répétez cette action pour chaque entreprise ajoutée. (Dans cet exemple, exécutez cette action pour les lignes 3 à 6, car quatre entreprises sont ajoutées.)

   ![La société est nouvelle](assets/cmpyisnew-350x86.png)

1. Saisissez un **ID** unique.

   Vous devez saisir un ID pour chaque ligne. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![La société est nouvelle](assets/cmpyisnew-350x86.png)

1. Saisissez les noms de chaque client dans la colonne **setName**.

   ![Identifiant de la société](assets/companyid-350x78.png)

1. Accédez à la feuille **Groupe**.

   Sauf si vous avez déjà créé des groupes dans Workfront, cette feuille ne doit afficher que le groupe par défaut configuré avec chaque compte de Workfront.

   ![Feuille de groupement](assets/groupsheet-350x15.png) ![Feuille de groupement vide](assets/emptygroupsheet-350x85.png)

1. Saisissez **TRUE** dans la colonne **isNew**.

   Selon le scénario, 4 groupes seront importés. Entrez donc **TRUE** dans la colonne **isNew** pour les lignes 4 à 7.

1. Saisissez un **ID** unique.

   Vous devez saisir un ID pour chaque ligne. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![ID de groupe](assets/groupids-350x85.png)

1. Saisissez les noms de chaque service dans la colonne **setName**.

   ![Noms de groupe](assets/groupnames-350x85.png)

1. Accédez à la feuille **Rôle**.

   À moins que vous n’ayez déjà créé ou supprimé des rôles dans votre compte, cette feuille doit afficher 8 rôles configurés avec chaque compte de Workfront.

   ![Noms de groupe](assets/groupnames-350x85.png)

1. Saisissez **TRUE** dans la colonne **isNew**.

   Selon le scénario, 7 fonctions seront importées. Saisissez donc **TRUE** dans la colonne **isNew** pour les lignes 12 à 18.

   ![Rôle nouveau](assets/roleisnew-350x104.png)

1. Saisissez un **ID** unique.

   Vous devez saisir un ID pour chaque ligne. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![Rôle nouveau](assets/roleisnew--1--350x104.png)

1. Attribuez un nom à chaque rôle de la colonne **setName**.

   ![Rôle nouveau](assets/roleisnew-350x104.png)

1. Indiquez des détails supplémentaires si nécessaire.

   Incluez les taux de facturation, les taux de coûts et les descriptions des rôles que vous créez, si nécessaire.

1. Accédez à la feuille **Utilisateur**.

   Sauf si vous avez déjà créé des utilisateurs et utilisatrices dans votre compte, cette feuille ne doit afficher que l’utilisateur ou utilisatrice Admin de chaque compte de Workfront.

   ![Feuille utilisateur](assets/usersheet-350x16.png) ![Feuille utilisateur vide](assets/emptyusersheet-350x52.png)

1. Saisissez **TRUE** dans la colonne **isNew**.

   Selon le scénario, 6 utilisateurs seront importés. Entrez donc **TRUE** dans la colonne **isNew** pour les lignes 4 à 9.

   ![L’utilisateur est nouveau](assets/userisnew-350x52.png)

1. Saisissez un **ID** unique.

   Vous devez saisir un ID pour chaque ligne. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![L’utilisateur est nouveau](assets/userisnew-350x52.png)

1. Saisissez les noms de chaque utilisateur dans les colonnes **setFirstName** et **setLastName**.

   ![Noms d’utilisateur](assets/usernames-350x52.png)

1. Définissez les valeurs détaillées en saisissant des valeurs dans les colonnes **setEmail**, **setPassword** et **setUsername**.

   ![Informations d’identification utilisateur](assets/usercredentials-350x52.png)

1. Indiquez les valeurs du niveau d’accès.

   Par exemple, Chris Manning est un membre d’équipe. Recherchez l’ID sur la feuille **Niveau d’accès ACSLVL** pour le niveau d’accès Membre de l’équipe. Copiez l’ID et, sur la feuille **Utilisateur**, collez-le dans la colonne **setAccessLevelID** de la ligne correspondant à cet utilisateur.

   Répétez cette étape pour chaque personne et niveau d’accès.

   ![Copier l’ID de niveau d’accès](assets/copyalid-350x171.png) ![Coller l’ID de niveau d’accès](assets/pastealid-350x59.png)

1. Saisissez les détails du groupe principal de l’utilisateur.

   Selon le scénario, Chris Manning appartient au groupe Marketing. Dans la feuille **GROUP**, recherchez l’ID du groupe marketing, copiez-le et, dans la feuille **USER**, collez-le dans la colonne **setHomeGroupID** de la ligne de l’utilisateur. &#x200B;Répétez cette étape pour chaque affectation de personne et de groupe.

   ![Copier l’ID de groupe](assets/copygroupid-1-350x133.png) ![Coller l’ID de groupe](assets/pastegroupid-350x59.png)

1. Saisissez les informations d’entreprise de l’utilisateur.

   Tous les utilisateurs de ce scénario appartiennent à la même société. Dans la feuille **Société CMPY**, recherchez l’ID de la société **Votre propre société**, copiez l’ID, puis, dans l’onglet **Utilisateur utilisateur**, collez cette valeur dans chaque ligne de la colonne **setCompanyID**&#x200B;

   Répétez cette étape pour chaque affectation de personne et de groupe.

   ![ID de la société](assets/companyid--1--350x78.png) ![Coller l’ID de la société](assets/pastecompanyid-350x84.png)

1. Saisissez les détails de la fonction de l’utilisateur.

   Selon le scénario, Chris Manning aura le rôle de personne chargée de l’analyse d’affaires. Dans la feuille **Rôle**, localisez l’ID du rôle Analyste métier, copiez-le et, dans la feuille **Utilisateur**, collez-le dans la colonne **setRoleID** sur la ligne de l’utilisateur. &#x200B;Répétez cette étape pour chaque affectation de personne et de groupe.

   ![Copier l’ID du rôle](assets/copyroleid-350x149.png) ![Coller l’ID du rôle](assets/pasteroleid-350x95.png)

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
