---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : modifier définitivement la largeur d’une colonne ;'
description: Vous pouvez temporairement modifier la largeur des colonnes en les faisant glisser et en les déposant sur les marges correspondant à la largeur souhaitée. Pour plus d’informations, voir Modification de la largeur et de l’ordre des colonnes.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Afficher : modifier définitivement la largeur d’une colonne ;

Vous pouvez temporairement modifier la largeur des colonnes en les faisant glisser et en les déposant sur les marges correspondant à la largeur souhaitée. Pour plus d’informations, voir [Modification de la largeur et de l’ordre des colonnes](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Vous pouvez modifier la largeur de n’importe quelle colonne de n’importe quelle vue de manière permanente en utilisant le mode texte dans la colonne au fur et à mesure que vous modifiez la vue.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demande de modification d’une vue </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification d’un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier une vue</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Modification permanente de la largeur d’une colonne

>[!IMPORTANT]
>
>Si vous modifiez manuellement la largeur d’une colonne comme décrit dans la section &quot;Modifier temporairement la largeur et l’ordre des colonnes&quot; de l’article [Modification de la largeur et de l’ordre des colonnes](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) une fois la largeur de la colonne modifiée de manière permanente, elle est conservée en fonction de votre redimensionnement manuel et la largeur de la colonne mise à jour selon les étapes suivantes est écrasée. Vous pouvez afficher la colonne en fonction de la largeur définie dans les étapes suivantes après avoir vidé le cache ou vous être connecté à partir d’un autre navigateur.
>
>Pour plus d’informations sur la personnalisation de la largeur des colonnes lors de l’utilisation de l’interface du mode Texte, voir les définitions &quot;largeur&quot; et &quot;étirement&quot; dans la section [Glossaire de la terminologie Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Accédez à une liste d’objets.
1. Dans la **Affichage** menu déroulant, cliquez sur **Nouvelle vue**.

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

   Pour le **width** ligne, spécifiez un nombre (en pixels) représentant la largeur de la colonne à afficher dans la vue.

1. Cliquez sur **Enregistrer**, puis **Enregistrer la vue**.


