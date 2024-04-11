---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Création d’un compte de lecteur (service) pour Snowflake
description: Pour accéder aux données du lac de données Workfront, vous devez d’abord créer un compte de lecteur pour Snowflake.
author: Nolan
feature: Reports and Dashboards
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 7d24659833f0ac0ceeecb245358f2ade8bd08a17
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# Création d’un compte de lecteur (service) pour Snowflake

Pour accéder aux données de lac de données Workfront, vous devez d’abord créer un compte de lecteur pour Snowflake. En outre, vous devez ajouter des adresses IP à la liste autorisée pour tout outil externe que vous prévoyez de connecter aux données.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Final</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Créer un compte de lecteur

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Accès aux données**.

1. Cliquez sur **Créer une connexion**

1. Dans la fenêtre qui s’affiche, saisissez le nom de votre connexion dans **Description de la référence de connexion** et un nom d’utilisateur dans **Utilisateur de connexion**, puis cliquez sur **Générer une connexion**.

   ![Créer un compte de lecteur](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **Mot de passe par défaut** sera générée, ainsi qu’une URL permettant de visualiser vos données via Snowflake. Vous devrez utiliser le mot de passe conjointement avec le nom d’utilisateur que vous avez choisi de vous connecter pour la première fois à Snowflake. Veillez donc à en conserver un enregistrement ainsi qu’avec l’URL. Cochez la case indiquant que vous l’avez fait, puis cliquez sur **Fermer**.

   ![Mot de passe du compte par défaut](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Ouvrez Snowflake à l’aide d’un navigateur pour accéder à l’URL de l’étape précédente, saisissez le nom d’utilisateur que vous avez sélectionné et le mot de passe par défaut de l’étape précédente, puis cliquez sur **Se connecter**.

1. Après la première connexion, vous serez invité à choisir un nouveau mot de passe. Saisissez le mot de passe de votre choix dans la **Nouveau mot de passe** et **Confirmer le mot de passe** champs, puis cliquez sur **Envoyer**.

   ![Réinitialisation du mot de passe du Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Vous pouvez désormais utiliser votre nom d’utilisateur et votre nouveau mot de passe pour accéder à votre lac de données Workfront en Snowflake.

## Ajout d’adresses IP à la liste autorisée

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Accès aux données**.

1. Cliquez sur le bouton **Adresses IP autorisées** , puis cliquez sur le bouton **Ajout d’une adresse IP à votre Liste autorisée** bouton .

   ![Ajouter une adresse IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

1. Saisissez le nom de l’adresse IP dans **Description de l’adresse IP** et saisissez l’adresse IP de l’outil que vous souhaitez utiliser dans **Adresse IP**, puis cliquez sur **Ajout d’une adresse IP à la Liste autorisée**.

## Révocation d’un compte de lecteur ou suppression d’une adresse IP de la liste autorisée

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Accès aux données**.

1. Cliquez sur l’icône de la corbeille ![Icône Supprimer](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à droite du compte que vous souhaitez révoquer.

   OU

   Cliquez sur le bouton **Adresses IP autorisées** , puis cliquez sur l’icône de la corbeille ![Icône Supprimer](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à droite de l’adresse IP que vous souhaitez supprimer.

1. Dans la fenêtre qui s’affiche, cochez la case pour confirmer, puis cliquez sur **Supprimer**.
