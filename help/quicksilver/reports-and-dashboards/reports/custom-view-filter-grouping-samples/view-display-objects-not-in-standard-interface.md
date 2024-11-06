---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Affichage : affiche les objets qui ne sont pas inclus dans l’interface standard"
description: Vous pouvez afficher dans une vue des objets qui ne sont pas inclus dans l’interface de mode standard. Pour ce faire, vous pouvez uniquement les référencer en mode Texte.
author: Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 87%

---

# Vue : affichez les objets qui ne sont pas inclus dans l’interface standard.

Vous pouvez afficher dans une vue des objets qui ne sont pas inclus dans l’interface de mode standard. Pour ce faire, vous pouvez uniquement les référencer en mode Texte.\
Vous pouvez déterminer les champs qui peuvent être inclus dans une vue de l’une des façons suivantes :

* Utilisez l’[Explorateur d’API](../../../wf-api/general/api-explorer.md) pour découvrir d’autres objets qui peuvent être référencés via le mode Texte.\
  Tous les champs documentés dans l’explorateur d’API ne sont pas des champs valides pour le mode Texte. Certains champs ne sont reportables que par le biais de l’API.

* Recherchez le champ Identifiant de l’objet dans une colonne. La plupart des objets ayant un identifiant de champ ont également un nom de colonne ou de champ correspondant qui peut ne pas être accessible par le biais de l’interface de mode standard.

  Vous pouvez utiliser le mode Texte pour inclure dans une vue le nom de la colonne ou du champ au lieu de l’identifiant en remplaçant l’`fieldnameID` par le `fieldname:name`.

  Par exemple, dans l’interface du mode standard, le champ **Identifiant de la personne propriétaire du portfolio** est disponible pour une vue de projet, mais le champ **Nom de la personne propriétaire du portfolio** ne l’est pas. Vous pouvez utiliser le mode Texte pour afficher le **Nom de la personne propriétaire du portfolio** dans la colonne d’une vue.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur à la modification d’un filtre </p></li>
   <li><p>Standard pour modifier un rapport</p></li> </ul>

<p>Actuel :</p>
   <ul><li><p>Demande de modification d’un filtre </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exemple : ajoutez la colonne Nom de la personne propriétaire du portfolio à une vue de projet.

1. Accédez à une liste de projets.
1. Dans le menu déroulant de la **Vue**, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**, commencez à saisir « Identifiant de la personne propriétaire du portfolio » dans le champ **Afficher dans cette colonne**, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

1. Cliquez sur **Passer en mode Texte**, puis **Modifier le mode Texte**.
1. Remplacez la ligne `valuefield` (`valuefield=portfolio:ownerID`) par la ligne suivante :

   `valuefield=portfolio:owner:name`

   Ou

   Supprimez le texte que vous trouvez dans la zone **Edit Text Mode** et remplacez-le par le code suivant :

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   Dans cet exemple particulier, le rapport triera le rapport selon l’identifiant de la personne propriétaire du portfolio, comme indiqué par la ligne `querysort`.

   >[!TIP]
   >
   >Pour remplacer un champ `ID` avec le champ `name` en mode Texte, remplacez toujours `ID` par `:name` dans la ligne `valuefield`.

1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.
