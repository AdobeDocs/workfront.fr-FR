---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Affichage : modification permanente de la largeur d’une colonne'
description: Vous pouvez temporairement modifier la largeur des colonnes en les faisant glisser et en les déposant sur les marges correspondant à la largeur souhaitée. Pour plus d’informations, consultez la section « Modifier la largeur et l’ordre des colonnes ».
author: Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 90%

---

# Vue : modifier définitivement la largeur d’une colonne

<!-- Audited: 11/2024 -->

Vous pouvez temporairement modifier la largeur des colonnes en les faisant glisser et en les déposant sur les marges correspondant à la largeur souhaitée. Pour plus d’informations, consultez la section [Modifier la largeur et l’ordre des colonnes](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Pour modifier définitivement la largeur d’une colonne dans une vue, vous devez utiliser le mode texte dans la colonne lorsque vous modifiez celle-ci.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou demande de modification d’une vue </p>
   <p>Standard ou Plan pour modifier un rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier définitivement la largeur d’une colonne

>[!IMPORTANT]
>
>Après avoir modifié la largeur d’une colonne de façon définitive, si vous modifiez manuellement la largeur d’une colonne comme décrit dans la section [Modifier temporairement la largeur et l’ordre des colonnes](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) de l’article [Modifier la largeur et l’ordre des colonnes](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md), la largeur de la colonne est préservée en fonction de votre redimensionnement manuel. Dans ce cas, la largeur de la colonne actualisée selon les étapes suivantes est écrasée. Vous pouvez afficher la colonne selon la largeur définie dans les étapes suivantes après avoir effacé votre cache ou ouvert une session à partir d’un autre navigateur.
>
>Pour plus d’informations sur la personnalisation de la largeur des colonnes lors de l’utilisation de l’interface en mode texte, consultez les définitions des termes « largeur » et « étirer » dans la section [Glossaire de la terminologie Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Accédez à une liste d’objets.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne** pour ajouter une nouvelle colonne.

   Ou

   Cliquez sur l’en-tête de colonne d’une colonne existante.

1. Cliquez sur **Basculer en mode texte**.
1. Cliquez Sur **Modifier Le Mode Texte**.T
1. Ajoutez le code suivant au mode texte de la colonne :

   ```
   width=200
   usewidths=true
   ```

   Pour la ligne intitulée **largeur**, indiquez un nombre quelconque (en pixels) représentant la largeur de la colonne à afficher dans la vue.

1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.


