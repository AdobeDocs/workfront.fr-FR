---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Vue : afficher les objets qui ne sont pas inclus dans l’interface standard"
description: Vous pouvez afficher dans une vue des objets qui ne sont pas inclus dans l’interface de mode standard. Pour ce faire, vous pouvez uniquement les référencer en mode texte.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Vue : affiche les objets qui ne sont pas inclus dans l’interface standard

Vous pouvez afficher dans une vue des objets qui ne sont pas inclus dans l’interface de mode standard. Pour ce faire, vous pouvez uniquement les référencer en mode texte.\
Vous pouvez déterminer les champs qui peuvent être inclus dans une vue de l’une des façons suivantes :

* Utilisez la variable [Explorateur d’API](../../../wf-api/general/api-explorer.md) pour découvrir d’autres objets qui peuvent être référencés via le mode texte.\
  Tous les champs documentés dans l’explorateur d’API ne sont pas des champs valides pour le mode texte. Certains champs ne sont reportables que par le biais de l’API.

* Recherchez le champ ID de l’objet dans une colonne. La plupart des objets ayant un identifiant de champ ont également un nom de colonne ou de champ correspondant qui peut ne pas être accessible par le biais de l’interface de mode standard.

  Vous pouvez utiliser le mode texte pour inclure dans une vue le nom de la colonne ou du champ au lieu de l’identifiant en remplaçant la variable `fieldnameID` avec la propriété `fieldname:name`.

  Par exemple, dans l’interface du mode standard, la variable **Identifiant du propriétaire du Portfolio** est disponible pour une vue de projet, mais le champ **Nom du propriétaire du Portfolio** ne l’est pas. Vous pouvez utiliser le mode texte pour afficher la variable **Nom du propriétaire du Portfolio** dans la colonne d’une vue.

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

## Exemple : ajoutez la colonne Nom du propriétaire du Portfolio à une vue de projet.

1. Accédez à une liste de projets.
1. Dans la **Affichage** menu déroulant, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne** puis commencez à saisir &quot;Identifiant du propriétaire du Portfolio&quot; dans la variable **Afficher dans cette colonne** puis sélectionnez-la lorsqu’elle s’affiche dans la liste.

1. Cliquez sur **Passer en mode Texte**.
1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Remplacez la variable `valuefield` ligne (`valuefield=portfolio:ownerID`) avec la ligne suivante :

   ```
   valuefield=portfolio:owner:name
   ```

   Ou

   Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   Dans cet exemple particulier, le rapport triera le rapport selon l’identifiant du propriétaire du Portfolio, comme indiqué par la variable `querysort` ligne.

   >[!TIP]
   >
   >Pour remplacer un champ `ID` avec le champ `name` en mode texte, toujours remplacer `ID` avec `:name` dans le `valuefield` ligne.

1. Cliquez sur **Enregistrer**, puis **Enregistrer la vue**.
