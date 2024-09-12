---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Création d’un compte de lecteur (service) pour Snowflake
description: Pour accéder aux données de Data Connect, vous devez d’abord créer un compte de lecteur de Snowflake.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: c3e18716aa74ed91e21e542437a017586a58d0b3
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 10%

---

# Création d’un compte de lecteur (service) pour Snowflake

Pour accéder aux données de Data Connect, vous devez d’abord créer un compte de lecteur (ou service) de Snowflake pour chaque nouvelle connexion. Après la création d’une connexion, vous pouvez trouver son URL et son nom d’utilisateur associés en cliquant dessus sur la page **Accès aux données** (**Menu principal** > **Configuration** > **Système** > **Accès aux données**) sous l’onglet **Connexions existantes**.

Pour plus d’informations sur l’utilisation d’une nouvelle connexion avec un produit externe, voir [Établissement d’une connexion à Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td><p>Inclus dans les plans suivants :</p>
    <ul>
        <li>Final</li> 
    </ul>    
   <p>Peuvent être achetées sous la forme d’un module complémentaire pour les forfaits suivants :</p> 
    <ul>
        <li>Sélectionner</li> 
        <li>Principal</li>
    </ul> 
    <p>Workfront Data Connect n’est pas disponible pour les plans Workfront hérités.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un compte de lecteur

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Accès aux données**.

1. Cliquez sur **Créer une connexion**

1. Dans la fenêtre qui s&#39;affiche, saisissez un nom pour votre connexion dans **Description de référence de connexion** et un nom d&#39;utilisateur dans **Utilisateur de connexion**, puis cliquez sur **Générer la connexion**.

   ![Créer un compte de lecteur](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Un **mot de passe par défaut** sera généré, ainsi qu’une URL permettant de visualiser vos données par l’intermédiaire de Snowflake. Vous devrez utiliser le mot de passe conjointement avec le nom d’utilisateur que vous avez choisi de vous connecter pour la première fois à Snowflake. Veillez donc à en conserver un enregistrement ainsi qu’avec l’URL. Cochez la case affirmant que vous l’avez fait, puis cliquez sur **Fermer**.

   ![Mot de passe du compte par défaut](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Ouvrez Snowflake à l’aide d’un navigateur pour accéder à l’URL de l’étape précédente, saisissez le nom d’utilisateur que vous avez sélectionné et le mot de passe par défaut de l’étape précédente, puis cliquez sur **Se connecter**.

1. Après la première connexion, vous serez invité à choisir un nouveau mot de passe. Saisissez un mot de passe de votre choix dans les champs **Nouveau mot de passe** et **Confirmer le mot de passe** , puis cliquez sur **Envoyer**.

   ![Réinitialiser le mot de passe du Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Vous pouvez désormais utiliser votre nom d’utilisateur et votre nouveau mot de passe pour accéder à votre lac de données Data Connect en Snowflake ou à l’outil de visualisation d’entreprise de votre choix.

## Révocation d’un compte de lecteur

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Accès aux données**.

1. Cliquez sur l’icône de corbeille ![Icône Supprimer](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) située à droite du compte que vous souhaitez révoquer.

1. Dans la fenêtre qui s&#39;affiche, cochez la case pour confirmer, puis cliquez sur **Supprimer**.
