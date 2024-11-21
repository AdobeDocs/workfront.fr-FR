---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Établissement d’une connexion à Workfront Data Connect
description: Workfront Data Connect vous permet d’utiliser les données Workfront de votre entreprise avec des outils de Business Intelligence ou de les stocker dans un entrepôt de données externe.
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 7b50876f1be16473704eddeb3157dacfacd96e90
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 9%

---

# Établissement d’une connexion à Workfront Data Connect

Workfront Data Connect vous permet d’utiliser les données Workfront de votre entreprise avec des outils de Business Intelligence ou de les stocker dans un entrepôt de données externe.

Pour connecter votre lac de données Data Connect à un produit externe, vous devez d’abord créer une connexion comme décrit dans la section [Création d’un compte de lecteur ou d’une connexion pour Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). Ensuite, vous devez ajouter toutes les adresses IP requises à la liste autorisée, comme décrit dans la section [Ajouter des adresses IP à la liste autorisée](#add-ips-to-the-allowlist) ci-dessous.

La plupart des produits auront besoin des informations suivantes sur votre lac de données pour établir une connexion :

| Nom du champ | Valeur |
|---------------|-------------|
| Serveur | URL de la connexion, sans la partie `https://` (disponible sur la page **Data Connect** dans Workfront*) |
| Port | `443` |
| Base | `WORKFRONT` |
| Entrepôt | `READER_WH` |
| Schéma | `WF` |
| Rôle | `READER_ROLE` |
| Nom d’utilisateur | Nom d’utilisateur choisi lors de la création de la connexion (trouvé sur la page **Data Connect** dans Workfront*) |
| Mot de passe | Mot de passe choisi lors de la première connexion du Snowflake* |

*Pour plus d’informations sur l’emplacement de la page **Data Connect** contenant vos connexions, voir [Création d’un compte de lecteur ou d’une connexion pour Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Une fois qu’une entrée est ajoutée à la liste autorisée IP, toutes les autres adresses IP ne sont plus autorisées. Assurez-vous d’avoir saisi toutes les adresses IP requises (pour les expériences de création et de lecture de votre outil de visualisation) avant de tenter d’utiliser l’outil. Dans le cas contraire, vous risquez de rencontrer une erreur concernant les informations d’identification incorrectes.
>
>Si vous ne disposez d’aucune adresse IP incluse dans votre liste autorisée mais que vous rencontrez toujours des problèmes de connexion à un outil de BI, vérifiez la configuration du serveur proxy pour l’outil de BI.

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

## Ajout d’adresses IP à la liste autorisée

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Connexion aux données**.

1. Cliquez sur l’onglet **IP autorisées** , puis sur le bouton **Ajouter une adresse IP à votre Liste autorisée** .

1. Saisissez un nom pour l’adresse IP dans **Description de l’adresse IP** et saisissez l’adresse IP (ou bloc CIDR) de l’outil que vous souhaitez utiliser dans **Adresse IP**, puis cliquez sur **Ajouter une adresse IP à la Liste autorisée**.

   ![Ajouter une adresse IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Suppression d’une adresse IP de la liste autorisée

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Connexion aux données**.

1. Cliquez sur l’onglet **IP autorisées** , puis sur l’icône de corbeille ![Icône Supprimer](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) située à droite de l’adresse IP que vous souhaitez supprimer.

1. Dans la fenêtre qui s&#39;affiche, cochez la case pour confirmer, puis cliquez sur **Supprimer**.

## Partage de données avec les outils de Business Intelligence

Vous trouverez ci-dessous un certain nombre d’outils de Business Intelligence courants ; consultez leurs sites de documentation pour en savoir plus sur la connexion à votre lac de données.

* Tableau
* Power BI
* Domo
* SAP HANA

## Stockage des données dans un entrepôt de données externe

Vous trouverez ci-dessous un certain nombre d’entrepôts de données courants. Consultez leurs sites de documentation pour en savoir plus sur la connexion à votre lac de données.

* Balises de données
* AWS Redshift
