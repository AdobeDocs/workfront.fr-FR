---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Affichage : modifiez définitivement la largeur d’une colonne"
description: Vous pouvez temporairement modifier la largeur des colonnes en les faisant glisser et en les déposant sur les marges correspondant à la largeur souhaitée. Pour plus d’informations, voir Modification de la largeur et de l’ordre des colonnes.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 27%

---

# Vue : modifier de manière permanente la largeur d’une colonne

<!-- Audited: 1/2024 -->

Vous pouvez temporairement modifier la largeur des colonnes en les faisant glisser et en les déposant sur les marges correspondant à la largeur souhaitée. Pour plus d’informations, voir [Modification de la largeur et de l’ordre des colonnes](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Pour modifier définitivement la largeur d’une colonne d’un mode, vous devez utiliser le mode texte dans la colonne au fur et à mesure que vous modifiez la vue.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau :<ul><li>Contributeur à la modification d’une vue</li><li>Standard pour modifier un rapport</li></ul></p><p>Ou</p>Actuel :<ul><li>Demander la modification d’une vue</li><li>Prévoir la modification d’un rapport</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier une vue</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modification permanente de la largeur d’une colonne

>[!IMPORTANT]
>
>Si vous modifiez manuellement la largeur d’une colonne comme décrit dans la section [Modifier temporairement la largeur et l’ordre des colonnes](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) de l’article [Modifier la largeur et l’ordre des colonnes](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) après avoir modifié définitivement la largeur de la colonne, la largeur de la colonne est conservée en fonction de votre redimensionnement manuel. Dans ce cas, la largeur de la colonne mise à jour selon les étapes suivantes est écrasée. Vous pouvez afficher la colonne en fonction de la largeur définie dans les étapes suivantes après avoir vidé le cache ou vous être connecté à partir d’un autre navigateur.
>
>Pour plus d’informations sur la personnalisation de la largeur des colonnes lors de l’utilisation de l’interface du mode Texte, voir les définitions &quot;largeur&quot; et &quot;extension&quot; dans le [Glossaire de la terminologie Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Accédez à une liste d’objets.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne** pour ajouter une nouvelle colonne.

   Ou

   Cliquez sur l’en-tête de colonne d’une colonne existante.

1. Cliquez sur **Passer en mode Texte**.
1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Ajoutez le code suivant au mode texte de la colonne :

   ```
   width=200
   usewidths=true
   ```

   Pour la ligne **width**, spécifiez tout nombre (en pixels) représentant la largeur de la colonne à afficher dans la vue.

1. Cliquez sur **Enregistrer**, puis sur **Enregistrer la vue**.


