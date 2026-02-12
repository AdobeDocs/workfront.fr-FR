---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Créer un compte de lecteur pour Snowflake
description: Pour accéder aux données de Data Connect, vous devez d’abord créer un compte de lecteur Snowflake.
author: Nolan
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 9cf221bda04614856a6a3670100742340fb73aee
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 6%

---

# Créer un compte de lecteur ou une connexion pour Snowflake

Pour accéder aux données Data Connect, vous devez d’abord créer un compte de lecteur (ou de service) Snowflake pour votre organisation, puis établir une nouvelle connexion pour chaque utilisateur ou outil que vous souhaitez voir accéder à Data Connect.

Après avoir créé une connexion, vous pouvez trouver l’URL et le nom d’utilisateur associés en cliquant dessus sur la page Data Connect (menu principal > Configuration > Système > Data Connect) sous l’onglet Connexions existantes .

Pour plus d’informations sur l’utilisation d’une nouvelle connexion avec un produit externe, voir [Établir une connexion à Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un compte de lecteur

Vous devez créer un compte de lecteur Snowflake pour votre organisation avant de pouvoir commencer à créer des connexions.

>[!IMPORTANT]
>
>Ce processus ne doit être effectué qu’une seule fois par organisation. Si le bouton **Créer un compte Reader** n’apparaît pas à l’emplacement décrit ci-dessous, cela signifie que votre compte de lecteur a déjà été créé.

Pour créer un compte de lecteur :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Connexion aux données**.

1. Cliquez sur le bouton **Créer un compte Reader** pour commencer à créer le compte de lecteur de votre organisation. Le processus est automatique, mais peut prendre jusqu’à 24 heures.

1. Une fois l’opération terminée, une boîte de dialogue s’affiche pour expliquer que votre compte de lecteur est désormais actif. Actualisez la page du navigateur pour accéder au bouton **Créer une connexion**.

Boîte de dialogue de création du compte Reader ![](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-reader-account-created.png)

## Créer une connexion

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Connexion aux données**.

1. Cliquez sur **Créer une connexion**

1. Dans la fenêtre qui s’affiche, saisissez un nom pour votre connexion dans **Description de la référence de connexion** et un nom d’utilisateur dans **Utilisateur de la connexion**, puis cliquez sur **Générer la connexion**.

   ![Créer une connexion](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Un **mot de passe par défaut** sera généré, ainsi qu’une URL où vos données peuvent être consultées via Snowflake. Vous devrez utiliser le mot de passe conjointement avec le nom d’utilisateur que vous avez choisi pour vous connecter pour la première fois à Snowflake. Veillez donc à conserver un enregistrement de celui-ci ainsi que l’URL. Cochez la case indiquant que vous l’avez fait, puis cliquez sur **Fermer**.

   ![Mot de passe de compte par défaut](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Ouvrez Snowflake à l’aide d’un navigateur pour accéder à l’URL de l’étape précédente, saisissez le nom d’utilisateur que vous avez sélectionné et le mot de passe par défaut de l’étape précédente, puis cliquez sur **Se connecter**.

1. Après vous être connecté pour la première fois, vous serez invité à choisir un nouveau mot de passe. Saisissez un mot de passe de votre choix dans les champs **Nouveau mot de passe** et **Confirmer le mot de passe**, puis cliquez sur **Envoyer**.

   ![Réinitialiser le mot de passe Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Vous pouvez maintenant utiliser votre nom d’utilisateur et votre nouveau mot de passe pour accéder à votre lac de données Data Connect dans Snowflake ou à l’outil de visualisation d’entreprise de votre choix.

## Révoquer un compte de lecteur

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Accès aux données**.

1. Cliquez sur l’icône de corbeille ![icône de suppression](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à droite du compte que vous souhaitez révoquer.

1. Dans la fenêtre qui s&#39;affiche, cochez la case pour confirmer, puis cliquez sur **Supprimer**.
