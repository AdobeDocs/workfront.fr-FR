---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: "Scénario de démarrage : entreprise, groupe, rôle et préparation du lancement de l’utilisateur"
description: Lorsque vous commencez à implémenter Adobe Workfront, plutôt que de saisir manuellement des données, vous pouvez importer la liste de vos clients, les services internes, les rôles de tâche et les informations sur les utilisateurs.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 11%

---

# Scénario de démarrage : société, groupe, rôle et utilisateur - Démarrage de la préparation

Lorsque vous commencez à implémenter Adobe Workfront, plutôt que de saisir manuellement des données, vous pouvez importer la liste de vos clients, les services internes, les rôles de tâche et les informations sur les utilisateurs.

## Conditions d’accès

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

## Éléments que vous pouvez importer

Le tableau suivant affiche les sociétés, groupes et rôles à importer :

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
   <td valign="top"> <p valign="top" rowspan="7">Finances</p> <p valign="top" rowspan="7">Informatique </p> <p valign="top" rowspan="7">Marketing </p> <p valign="top" rowspan="7">Ventes</p> </td> 
   <td valign="top"> <p valign="top">Analyste métier</p> <p valign="top">Créatif du contrôleur</p> <p valign="top">Designer</p> <p valign="top">Gestionnaire des ressources</p> <p valign="top">Principal de script</p> <p valign="top">Rédacteur technique</p> <p valign="top">Développeur web</p> </td> 
  </tr> 
 </tbody> 
</table>

Les noms des rôles doivent être uniques, les rôles de tâche existants ne peuvent pas être importés.

Les tableaux suivants présentent les utilisateurs à importer et plusieurs attributs utilisateur pour chacun d’eux :

### Utilisateur 1

| **Prénom** | Chris |
|---|---|
| **Nom** | Manning |
| **Nom d’utilisateur/Adresse électronique** | mailto:cmanning@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Membre d&#39;équipe |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe d’accueil** | Marketing |
| **Rôle de tâche** | Analyste métier |

{style="table-layout:auto"}

### Utilisateur 2

| **Prénom** | Jennifer |
|---|---|
| **Nom** | Campbell |
| **Nom d’utilisateur/Adresse électronique** | jcampbell@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de projet |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe d’accueil** | Marketing |
| **Rôle de tâche** | Gestionnaire de projet |

{style="table-layout:auto"}

### Utilisateur 3

| **Prénom** | Jill |
|---|---|
| **Nom** | Sullivan |
| **Nom d’utilisateur/Adresse électronique** | jsullivan@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Help Desk |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe d’accueil** | Ventes |
| **Rôle de tâche** | représentant commercial |

{style="table-layout:auto"}

### Utilisateur 4

| **Prénom** | Marc |
|---|---|
| **Nom** | Lewis |
| **Nom d’utilisateur/Adresse électronique** | mlewis@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de portefeuille |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe d’accueil** | Finances |
| **Rôle de tâche** | Contrôleur |

{style="table-layout:auto"}

### Utilisateur 5

| **Prénom** | Pam |
|---|---|
| **Nom** | Reynolds |
| **Nom d’utilisateur/Adresse électronique** | preynolds@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de projet |
| **Entreprise** | *Votre entreprise>* |
| **Groupe d’accueil** | Marketing |
| **Rôle de tâche** | Informatique |

{style="table-layout:auto"}

### Utilisateur 6

| **Prénom** | Ray |
|---|---|
| **Nom** | Andrews |
| **Nom d’utilisateur/Adresse électronique** | randrews@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Administrateur |
| **Entreprise** | *Votre entreprise>* |
| **Groupe d’accueil** | Gestionnaire des ressources |
| **Rôle de tâche** | none |

{style="table-layout:auto"}

## Téléchargement d’un modèle de démarrage rapide

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **System** > **Kick-Starts** > **Import Data.**

1. Cliquez sur **Plus d’options** pour afficher la liste complète des options d’importation.
1. Sélectionnez les objets Niveau d’accès, Société, Groupe, Rôle de tâche et Utilisateur à importer.

## Informations sur la société de saisie

1. Ouvrez le fichier **Workfront.xlsx** que vous venez de télécharger.

   >[!TIP]
   >
   >Lorsque vous utilisez des feuilles de données très volumineuses, vous pouvez utiliser l’outil Volet de congélation (ou équivalent) de votre éditeur de feuille de calcul pour faciliter l’utilisation de la feuille de calcul.

1. Accédez à la feuille &quot;Société CMPY&quot;.

   Il devrait être vide, à moins que les entreprises ne soient déjà dans le système. ![](assets/cmpysheet-350x16.png)

   ![](assets/companyid--1--350x78.png)

1. Spécifiez TRUE dans la colonne **isNew**.
1. Répétez cette action pour chaque société ajoutée. (Dans cet exemple, exécutez cette action pour les lignes 3 à 6, car quatre sociétés sont ajoutées.)

   ![](assets/cmpyisnew-350x86.png)

1. Spécifiez un identifiant unique.

   Cela doit être effectué pour chaque ligne de la colonne ID. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![](assets/cmpyisnew-350x86.png)

1. Définissez un Nom.

   Indiquez les noms de chaque client dans la colonne **setName**.

   ![](assets/companyid-350x78.png)

1. Accédez à la feuille Groupe de GROUPE .

   Sauf si vous avez déjà créé des groupes dans Workfront, cette feuille ne doit afficher que le groupe par défaut configuré avec chaque compte de Workfront.

   ![](assets/groupsheet-350x15.png) ![](assets/emptygroupsheet-350x85.png)

1. Définissez la colonne **isNew**. Selon le scénario, 4 groupes seront importés. Par conséquent, spécifiez TRUE dans les lignes 4 à 7 pour la colonne &quot;isNew&quot;.
1. Spécifiez un identifiant unique.

   Cela doit être effectué pour chaque ligne de la colonne ID. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![](assets/groupids-350x85.png)

1. Définissez un Nom.

   Indiquez les noms de chaque service dans la colonne **setName**.

   ![](assets/groupnames-350x85.png)

   Spécifiez les informations de rôle. Accédez à la feuille Rôle du RÔLE .

1. À moins que vous n’ayez déjà créé ou supprimé des rôles dans votre compte, cette feuille doit afficher 8 rôles configurés avec chaque compte de Workfront.

   ![](assets/groupnames-350x85.png)

1. Définissez l’instruction True .

   Sept rôles de tâche sont en cours d’importation, saisissez TRUE dans les lignes 12 à 18 pour la colonne &quot;isNew&quot;.

   ![](assets/roleisnew-350x104.png)

1. Spécifiez un identifiant unique.

   Cela doit être effectué pour chaque ligne de la colonne ID. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![](assets/usersheet-350x16.png)

   ![](assets/roleisnew--1--350x104.png)

1. Attribuez des noms à chaque rôle en le tapant dans la colonne setName .

   ![](assets/roleisnew-350x104.png)

1. Fournissez des détails supplémentaires si nécessaire.

   Incluez les taux de facturation, les taux de coût et les descriptions des rôles que vous créez, si nécessaire.

1. Accédez à la feuille utilisateur USER pour saisir les informations utilisateur.

   Sauf si vous avez déjà créé des utilisateurs dans votre compte, cette feuille ne doit afficher que l’ utilisateur administrateur fourni avec chaque compte de Workfront.

   ![](assets/rolenames-350x104.png) ![](assets/emptyusersheet-350x52.png)

1. Définissez la valeur True en spécifiant TRUE dans les lignes 4 à 9 pour la colonne &quot;isNew&quot;, puisque 6 utilisateurs sont importés.

   ![](assets/userisnew-350x52.png)

1. Définissez un identifiant unique en spécifiant un identifiant unique dans chaque ligne pour la colonne ID. Généralement, les entiers commençant à 1 fonctionnent bien pour les nouveaux enregistrements.

   ![](assets/userisnew-350x52.png)

1. Saisissez les noms de chaque utilisateur dans les colonnes &#39;setFirstName&#39; et &#39;setLastName&#39;.

   ![](assets/usernames-350x52.png)

1. Définissez des valeurs détaillées en spécifiant des valeurs dans les colonnes &#39;setEmail&#39;, &#39;setPassword&#39; et &#39;setUsername&#39;.

   ![](assets/usercredentials-350x52.png)

1. Spécifiez les valeurs du niveau d’accès.

   Par exemple, Chris Manning, qui est membre de l’équipe, recherche l’identifiant sur la feuille Niveau d’accès ACSLVL pour le niveau d’accès Membre de l’équipe. Copiez l’ID dans votre presse-papiers, puis collez-le dans la feuille utilisateur de la colonne **setAccessLevelID** de la ligne Chris.

   Répétez cette étape pour chaque utilisateur et niveau d’accès.

   ![](assets/copyalid-350x171.png) ![](assets/pastealid-350x59.png)

1. Spécifiez les détails du groupe d’accueil.

   Selon le scénario, Chris Manning appartient au groupe Marketing. Dans la feuille Groupe GROUP, recherchez l’identifiant du groupe Marketing, copiez-le dans le Presse-papiers, puis, dans la feuille Utilisateur, collez-le dans la colonne **setHomeGroupID** de la ligne Chris. &#x200B;Répétez cette étape pour chaque affectation d’utilisateur et de groupe.

   ![](assets/copygroupid-1-350x133.png) ![](assets/pastegroupid-350x59.png)

1. Spécifiez les détails de la société.

   Tous les utilisateurs de ce scénario appartiennent à la même société. Dans la feuille Société CMPY, recherchez l’ID de la société *Votre propre entreprise*, copiez l’ID dans le presse-papiers, puis, dans l’onglet Utilisateur, collez cette valeur dans chaque ligne de la colonne &quot;setCompanyID&quot;. &#x200B;

   Répétez cette étape pour chaque affectation d’utilisateur et de groupe.

   ![](assets/companyid--1--350x78.png)

   ![](assets/pastecompanyid-350x84.png)

1. Spécifiez les détails du rôle de tâche.

   Selon le scénario, Chris Manning aura le rôle Analyste métier . Dans la feuille Rôle du RÔLE, recherchez l’ID du rôle Analyste métier, copiez-le dans le Presse-papiers, puis, dans la feuille Utilisateur de l’UTILISATEUR, collez-le dans la colonne &quot;setRoleID&quot; de la ligne Chris. &#x200B;Répétez cette étape pour chaque affectation d’utilisateur et de groupe.

   ![](assets/copyroleid-350x149.png)

   ![](assets/pasteroleid-350x95.png)

1. Renseignez d’autres informations sur l’utilisateur, si nécessaire, puis enregistrez le fichier.
1. Importez le fichier Excel.

   Suivez les instructions de la section **Importation de fichiers de démarrage de ick** de cet article.
