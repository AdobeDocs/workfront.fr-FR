---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Mettre à jour les utilisateurs et utilisatrices pour l’authentification unique
description: Vous pouvez mettre à jour les utilisateurs pour l’authentification unique dans Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 7%

---

# Mettre à jour les utilisateurs et utilisatrices pour l’authentification unique

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

Lorsque l’authentification unique (SSO) est activée dans votre instance Adobe Workfront, vos utilisateurs peuvent se connecter à Workfront avec leurs informations d’identification SSO.

Si vous disposez d’un système déjà rempli d’utilisateurs associés aux informations d’identification d’authentification unique, vous pouvez importer les ID des utilisateurs dans Workfront en important un fichier de valeurs séparées par des virgules (CSV) dans Workfront.

Pour plus d’informations sur l’intégration de Workfront à un système SSO, voir [Présentation de l’authentification unique dans Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td><p>Nouveau : Standard</p><p>Ou</p><p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Noms d’utilisateur SSO

Selon la solution SSO que vous utilisez, le nom d’utilisateur de votre environnement SSO peut être appelé comme suit :

* Nom d’utilisateur SSO
* ID de fédération
* Nom d’utilisateur de la fédération

Quel que soit le nom d’utilisateur appelé dans votre environnement SSO, la valeur du champ est stockée dans le champ Nom d’utilisateur SSO, sur l’objet User .

Pour que vos utilisateurs puissent utiliser leurs informations d’identification d’authentification unique pour se connecter à Workfront, vous devez mettre à jour leur profil afin d’inclure leur nom d’utilisateur d’authentification unique, en plus de leur nom d’utilisateur Workfront.

En tant qu’administrateur Workfront, vous pouvez mettre à jour en masse le champ Nom d’utilisateur de l’authentification unique pour vos utilisateurs Workfront en important une liste de noms d’utilisateur dans Workfront. Cette liste doit :

* Contenir l’identifiant utilisateur Workfront (GUID) ainsi que le nom d’utilisateur d’authentification unique correspondant pour chaque utilisateur
* Enregistrez-le au format CSV ou TSV.

Ce processus met à jour les noms d’utilisateur SSO existants dans Workfront ou ajoute un nouveau nom d’utilisateur SSO, si celui-ci est absent pour les utilisateurs.

## Préparation du fichier d’importation {#prepare-the-import-file}

Vous pouvez commencer à préparer votre fichier d’importation en créant un rapport de tous les utilisateurs de Workfront qui doivent avoir leurs champs Nom d’utilisateur SSO mis à jour.

1. Créez un rapport utilisateur dans Workfront.

   Pour plus d’informations sur la création de rapports utilisateur dans Workfront, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Sélectionnez les champs suivants dans votre rapport :

   | champ | Explication |
   |---|---|
   | Nom | Nom complet de l’utilisateur Workfront. |
   | ID | L’ID est le GUID alphanumérique Workfront. |
   | Nom d’utilisateur SSO | Ajout du champ Nom d’utilisateur de l’authentification unique pour vous assurer qu’il n’existe aucun nom d’utilisateur que vous remplacez par votre importation. Ce champ doit être vide pour tous les utilisateurs, si vos utilisateurs n’ont pas encore été mis à jour pour SSO. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Enregistrez le rapport.
1. Cliquez sur **Exporter** dans la partie supérieure du rapport et exportez le rapport vers Excel.
1. Ouvrez le fichier Excel exporté et ajoutez vos noms d’utilisateur SSO pour chaque utilisateur du rapport dans la colonne Nom d’utilisateur SSO.

   >[!IMPORTANT]
   >
   >Les noms d’utilisateur SSO sont sensibles à la casse.

1. Supprimez toutes les colonnes du fichier Excel, à l’exception des colonnes **ID** et la variable **Nom d’utilisateur SSO** colonnes.

1. Supprimez les en-têtes de colonne et assurez-vous qu’il n’y a aucune ligne vide en haut du rapport.

   Le fichier que vous utilisez pour mettre à jour vos utilisateurs Workfront avec les noms d’utilisateur SSO **must** contenir uniquement 2 colonnes, dans cet ordre :

   * La première colonne doit afficher l’ID utilisateur Workfront (le GUID utilisateur tel qu’il est défini dans Workfront).
   * La deuxième colonne doit contenir le nom d’utilisateur de l’authentification unique, tel qu’il s’affiche dans votre système d’authentification unique.
   * Les colonnes ne doivent pas comporter d’en-têtes et aucune ligne vide ne doit se trouver en haut de la liste des noms.

     ![](assets/update-users-for-sso-csv-file-for-import.png)

1. Enregistrez le rapport au format CSV ou TSV sur votre ordinateur.

## Mise à jour de vos utilisateurs pour la SSO {#update-your-users-for-sso}

Le processus de mise à jour des utilisateurs pour SSO permet d’ajouter le champ Nom d’utilisateur de SSO à vos utilisateurs Workfront s’il n’y en a pas, ou de mettre à jour la valeur de ce champ si une valeur est déjà associée aux utilisateurs.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur, **Système** puis sélectionnez **Mise à jour des utilisateurs pour la connexion unique**.

1. Cliquez sur **Choisir un fichier** pour rechercher le fichier que vous avez préparé.

   Pour plus d’informations sur la préparation de ce fichier, voir [Préparation du fichier d’importation](#prepare-the-import-file).

1. Sélectionnez le fichier sur lequel il est enregistré sur votre ordinateur, puis cliquez sur **Ouvrir**.

   Cela insère les informations d’identification SSO à Workfront, ce qui permet à tous les utilisateurs de se connecter à Workfront à l’aide de leurs informations d’identification SSO.

   La variable **Autoriser uniquement `<SSO Configuration>` Authentification** est activé pour tous les utilisateurs inclus dans le fichier CSV. Cela garantit que les utilisateurs doivent se connecter via SSO.

## Vérification de l’authentification unique par rapport aux noms d’utilisateur Workfront de vos utilisateurs

Pour obtenir des instructions sur la création d’un rapport utilisateur contenant des informations sur le nom d’utilisateur SSO, voir [Préparation du fichier d’importation](#prepare-the-import-file).

1. Exécutez un rapport utilisateur contenant des informations de nom d’utilisateur SSO.

   Notez que la colonne SSO Username est renseignée pour chaque utilisateur.

1. Assurez-vous que les valeurs de la colonne SSO Username correspondent au nom d’utilisateur SSO sur votre serveur SSO.
1. Si la colonne Nom d’utilisateur d’authentification unique est vide, mettez à jour les noms d’utilisateur d’authentification unique de vos utilisateurs.

   ![](assets/users-with-sso-field-updated.png)

   Pour plus d’informations sur la mise à jour de vos utilisateurs pour SSO, voir [Mise à jour de vos utilisateurs pour la SSO](#update-your-users-for-sso).
