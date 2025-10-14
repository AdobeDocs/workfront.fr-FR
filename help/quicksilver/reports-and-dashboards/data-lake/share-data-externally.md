---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Établir une connexion à Workfront Data Connect
description: Workfront Data Connect vous permet d’utiliser les données Workfront de votre organisation avec des outils de Business Intelligence ou de les stocker dans un entrepôt de données externe.
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 9%

---

# Établir une connexion à Workfront Data Connect

Workfront Data Connect vous permet d’utiliser les données Workfront de votre organisation avec des outils de Business Intelligence ou de les stocker dans un entrepôt de données externe.

Pour connecter votre lac de données Data Connect à un produit externe, vous devez d’abord créer une connexion comme décrit dans la section [Création d’un compte de lecteur ou d’une connexion pour Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). Vous devez ensuite ajouter les adresses IP requises à la place sur la liste autorisée de données, comme décrit dans la section [Ajouter des adresses IP à la liste autorisée &#x200B;](#add-ips-to-the-allowlist) ci-dessous.

La plupart des produits nécessitent les informations suivantes sur votre lac de données pour établir une connexion :

| Nom du champ | Valeur |
|---------------|-------------|
| Serveur | URL de la connexion, sans la partie `https://` (sur la page **Data Connect** dans Workfront*) |
| Port | `443` |
| Base de données | `WORKFRONT` |
| Entrepôt de données | `READER_WH` |
| Schéma | `WF` |
| Rôle | `READER_ROLE` |
| Nom d’utilisateur | Nom d’utilisateur choisi lors de la création de la connexion (sur la page **Data Connect** de Workfront*) |
| Mot de passe | Mot de passe choisi lors de la première connexion à Snowflake* |

*Pour plus d’informations sur l’emplacement de la page **Data Connect** contenant vos connexions, voir [Création d’un compte de lecteur ou d’une connexion pour Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Une fois qu’une entrée est ajoutée à la place sur la liste autorisée IP, toutes les autres adresses IP ne sont plus autorisées. Assurez-vous d’avoir saisi toutes les adresses IP requises (pour les expériences de création et de lecture de votre outil de visualisation) avant d’essayer d’utiliser l’outil. Si ce n’est pas le cas, vous pouvez rencontrer une erreur concernant des informations d’identification non valides.
>
>Si aucune adresse IP n’est incluse dans votre liste autorisée, mais que vous rencontrez toujours des problèmes pour vous connecter à un outil BI, vérifiez la configuration du serveur proxy de l’outil BI.

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
        <li><p>Final</p></li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect n’est pas disponible pour les plans Workfront hérités.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter des adresses IP à la place sur la liste autorisée

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Connexion aux données**.

1. Placer sur la liste autorisée Cliquez sur l’onglet **Adresses IP autorisées**, puis sur le bouton **Ajouter une adresse IP à votre**.

1. Saisissez le nom de l’adresse IP dans **Description de l’adresse IP** et saisissez l’adresse IP (ou le bloc CIDR) de l’outil que vous souhaitez utiliser dans **Adresse IP**, puis cliquez sur **Ajouter une adresse IP pour Placer sur la liste autorisée**.

   ![Ajouter une adresse IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Supprimer une adresse IP de la place sur la liste autorisée

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Connexion aux données**.

1. Cliquez sur l’onglet **Adresses IP autorisées**, puis sur l’icône de corbeille ![icône de suppression](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à droite de l’adresse IP que vous souhaitez supprimer.

1. Dans la fenêtre qui s&#39;affiche, cochez la case pour confirmer, puis cliquez sur **Supprimer**.

## Partage de données avec des outils de Business Intelligence

Vous trouverez ci-dessous un certain nombre d’outils courants de Business Intelligence. Consultez leurs sites de documentation pour en savoir plus sur la connexion à votre lac de données.

* Tableau
* Power BI
* Domo
* SAP HANA

## Stocker les données dans un entrepôt de données externe

Vous trouverez ci-dessous un certain nombre d’entrepôts de données courants ; consultez leurs sites de documentation pour en savoir plus sur la connexion à votre lac de données.

* Briques de données
* AWS Redshift
