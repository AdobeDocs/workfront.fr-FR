---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: 'Scénario de démarrage : Lancement de la préparation de la mise en route de l’entreprise, du groupe, du rôle et de l’utilisateur"'
description: Lorsque vous commencez à implémenter Adobe Workfront, plutôt que de saisir manuellement des données, vous pouvez importer la liste de vos clients, les services internes, les rôles de tâche et les informations sur les utilisateurs.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 10%

---

# Scénario de démarrage : Préparation du coup d’envoi de l’entreprise, du groupe, du rôle et de l’utilisateur

Lorsque vous commencez à implémenter Adobe Workfront, plutôt que de saisir manuellement des données, vous pouvez importer la liste de vos clients, les services internes, les rôles de tâche et les informations sur les utilisateurs.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
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
   <td valign="top"> <p valign="top" rowspan="7">Finances</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">Marketing </p> <p valign="top" rowspan="7">Ventes</p> </td> 
   <td valign="top"> <p valign="top">Analyste métier</p> <p valign="top">Créatif du contrôleur</p> <p valign="top">Dessinateur</p> <p valign="top">Gestionnaire des ressources</p> <p valign="top">Principal de script</p> <p valign="top">Rédacteur technique</p> <p valign="top">Développeur web</p> </td> 
  </tr> 
 </tbody> 
</table>

Les noms des rôles doivent être uniques, les rôles de tâche existants ne peuvent pas être importés.

Les tableaux suivants présentent les utilisateurs à importer et plusieurs attributs utilisateur pour chacun d’eux :

### Utilisateur 1

| **Prénom** | Chris |
|---|---|
| **Nom de famille** | Manning |
| **Nom d’utilisateur/Adresse électronique** | mailto:cmanning@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Membre d&#39;équipe |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Marketing |
| **Fonction** | Analyste métier |

{style=&quot;table-layout:auto&quot;}

### Utilisateur 2

| **Prénom** | Jennifer |
|---|---|
| **Nom de famille** | Campbell |
| **Nom d’utilisateur/Adresse électronique** | jcampbell@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de projet |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Marketing |
| **Fonction** | Gestionnaire de projet |

{style=&quot;table-layout:auto&quot;}

### Utilisateur 3

| **Prénom** | Jill |
|---|---|
| **Nom de famille** | Sullivan |
| **Nom d’utilisateur/Adresse électronique** | jsullivan@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Help Desk |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Ventes |
| **Fonction** | représentant commercial |

{style=&quot;table-layout:auto&quot;}

### Utilisateur 4

| **Prénom** | Marc |
|---|---|
| **Nom de famille** | Lewis |
| **Nom d’utilisateur/Adresse électronique** | mlewis@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de portefeuille |
| **Entreprise** | &lt;*Votre entreprise>* |
| **Groupe principal** | Finances |
| **Fonction** | Contrôleur |

{style=&quot;table-layout:auto&quot;}

### Utilisateur 5

| **Prénom** | Pam |
|---|---|
| **Nom de famille** | Reynolds |
| **Nom d’utilisateur/Adresse électronique** | preynolds@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Gestionnaire de projet |
| **Entreprise** | *Votre entreprise>* |
| **Groupe principal** | Marketing |
| **Fonction** | IT |

{style=&quot;table-layout:auto&quot;}

### Utilisateur 6

| **Prénom** | Ray |
|---|---|
| **Nom de famille** | Andrews |
| **Nom d’utilisateur/Adresse électronique** | randrews@foo.com |
| **Mot de passe** | updateMe |
| **Accès** | Administrateur |
| **Entreprise** | *Votre entreprise>* |
| **Groupe principal** | Gestionnaire des ressources |
| **Fonction** | none |

{style=&quot;table-layout:auto&quot;}

## Téléchargement d’un modèle de démarrage rapide

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Démarrages** > **Importer des données.**

1. Cliquez sur **Plus d’options** pour afficher la liste complète des options d’importation.
1. Sélectionnez les objets Niveau d’accès, Société, Groupe, Rôle de tâche et Utilisateur que vous souhaitez importer.

## Informations sur la société de saisie

1. Ouvrez le **Workfront.xlsx** que vous venez de télécharger.

   >[!TIP]
   >
   >Lorsque vous utilisez des feuilles de données très volumineuses, vous pouvez utiliser l’outil Volet de gel (ou équivalent) de votre éditeur de feuille de calcul pour faciliter l’utilisation de la feuille de calcul.

1. Accédez à la feuille &quot;Société CMPY&quot;.

   Il devrait être vide, à moins que les entreprises ne soient déjà dans le système. ![](assets/cmpysheet-350x16.png)

   ![](assets/companyid--1--350x78.png)

1. Spécifiez TRUE dans la variable **isNew** colonne .
1. Répétez cette action pour chaque société ajoutée. (Dans cet exemple, exécutez cette action pour les lignes 3 à 6, car quatre sociétés sont ajoutées.)

   ![](assets/cmpyisnew-350x86.png)

1. Spécifiez un identifiant unique.

   Cela doit être effectué pour chaque ligne de la colonne ID. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![](assets/cmpyisnew-350x86.png)

1. Définissez un Nom.

   Indiquez les noms de chaque client dans la variable **setName** colonne .

   ![](assets/companyid-350x78.png)

1. Accédez à la feuille Groupe de GROUPE .

   Sauf si vous avez déjà créé des groupes dans Workfront, cette feuille ne doit afficher que le groupe par défaut configuré avec chaque compte de Workfront.

   ![](assets/groupsheet-350x15.png) ![](assets/emptygroupsheet-350x85.png)

1. Définissez la variable **isNew** column. Selon le scénario, 4 groupes seront importés. Par conséquent, spécifiez TRUE dans les lignes 4 à 7 pour la colonne &quot;isNew&quot;.
1. Spécifiez un identifiant unique.

   Cela doit être effectué pour chaque ligne de la colonne ID. Les entiers commençant à 1 fonctionnent bien lors de la création de nouveaux enregistrements.

   ![](assets/groupids-350x85.png)

1. Définissez un Nom.

   Indiquez les noms de chaque service dans la variable **setName** colonne .

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

   Par exemple, Chris Manning, qui est membre de l’équipe, recherche l’identifiant sur la feuille Niveau d’accès ACSLVL pour le niveau d’accès Membre de l’équipe. Copiez l’identifiant dans le presse-papiers, puis collez-le dans la feuille utilisateur de l’utilisateur du Presse-papiers. **setAccessLevelID** sur la ligne de Chris.

   Répétez cette étape pour chaque utilisateur et niveau d’accès.

   ![](assets/copyalid-350x171.png) ![](assets/pastealid-350x59.png)

1. Spécifiez les détails du groupe d’accueil.

   Selon le scénario, Chris Manning appartient au groupe Marketing. Dans la feuille Groupe de groupes, recherchez l’identifiant du groupe marketing, copiez-le dans le Presse-papiers, puis, dans la feuille Utilisateur, collez-le dans le **setHomeGroupID** sur la ligne de Chris. &#x200B;Répétez cette étape pour chaque affectation d’utilisateur et de groupe.

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

   Suivez les instructions de la section **Importation de fichiers de démarrage rapide** de cet article.
