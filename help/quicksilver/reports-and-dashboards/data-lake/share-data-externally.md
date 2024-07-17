---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data lake
title: Établissement d’une connexion au lac de données Workfront
description: Le lac de données Workfront vous permet d’utiliser les données Workfront de votre entreprise avec les outils de renseignements commerciaux les plus courants ou de les stocker dans un entrepôt de données externe.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 91371c862be6f3b99f0450ff359f601dc913dc0c
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 1%

---

# Établissement d’une connexion au lac de données Workfront

Le lac de données Workfront vous permet d’utiliser les données Workfront de votre entreprise avec des outils de Business Intelligence ou de les stocker dans un entrepôt de données externe.

Pour connecter vos données de lac de données Workfront à un produit externe, vous devez d’abord ajouter toutes les adresses IP requises à la liste autorisée, comme décrit dans la section [Ajout d’adresses IP à la liste autorisée](#add-ips-to-the-allowlist) ci-dessous. En outre, la plupart des produits nécessiteront des informations supplémentaires sur votre lac de données pour établir une connexion :

| Nom du champ | Valeur |
|---------------|-------------|
| Serveur | URL de la connexion, sans la partie `https://` (disponible sur la page **Data access** dans Workfront*) |
| Port | `443` |
| Base | `WORKFRONT` |
| Entrepôt | `READER_WH` |
| Schéma | `WF` |
| Rôle | `READER_ROLE` |
| Nom d’utilisateur | Nom d’utilisateur choisi lors de la création de la connexion (trouvé sur la page **Accès aux données** dans Workfront*) |
| Mot de passe | Mot de passe choisi lors de la première connexion du Snowflake* |

*Pour plus d’informations sur l’emplacement de la page **Data access** contenant vos connexions de lac de données, voir [Création d’un compte de lecteur (service) pour Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Une fois qu’une entrée est ajoutée à la liste autorisée IP, toutes les autres adresses IP ne sont plus autorisées. Assurez-vous d’avoir saisi toutes les adresses IP requises (pour les expériences de création et de lecture de votre outil de visualisation) avant de tenter d’utiliser l’outil. Dans le cas contraire, vous risquez de rencontrer une erreur concernant les informations d’identification incorrectes.
>
>Si vous ne disposez d’aucune adresse IP incluse dans votre liste autorisée mais que vous rencontrez toujours des problèmes de connexion à un outil de BI, vérifiez la configuration du serveur proxy pour l’outil de BI.


## Ajout d’adresses IP à la liste autorisée

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Accès aux données**.

1. Cliquez sur l’onglet **IP autorisées** , puis sur le bouton **Ajouter une adresse IP à votre Liste autorisée** .

1. Saisissez un nom pour l’adresse IP dans **Description de l’adresse IP** et saisissez l’adresse IP (ou bloc CIDR) de l’outil que vous souhaitez utiliser dans **Adresse IP**, puis cliquez sur **Ajouter une adresse IP à la Liste autorisée**.

   ![Ajouter une adresse IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Suppression d’une adresse IP de la liste autorisée

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Accès aux données**.

1. Cliquez sur l’onglet **IP autorisées** , puis sur l’icône de corbeille ![Icône Supprimer](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) située à droite de l’adresse IP que vous souhaitez supprimer.

1. Dans la fenêtre qui s&#39;affiche, cochez la case pour confirmer, puis cliquez sur **Supprimer**.

## Partage de données avec les outils de Business Intelligence

Vous trouverez ci-dessous un certain nombre d’outils de Business Intelligence courants ; les liens vous conduiront au site de documentation du service pour en savoir plus sur la connexion à votre lac de données.

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Domo](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## Stockage des données dans un entrepôt de données externe

Vous trouverez ci-dessous un certain nombre d’entrepôts de données courants. Les liens vous conduiront au site de documentation de chaque service, où vous pourrez en savoir plus sur la connexion à votre lac de données.

* [Databricks](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
