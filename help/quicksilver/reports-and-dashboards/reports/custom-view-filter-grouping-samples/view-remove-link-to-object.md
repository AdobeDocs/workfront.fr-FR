---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : supprimer le lien vers un objet dans une colonne »'
description: Certains objets affichés dans une vue renvoient par défaut à la page Détails de l’objet. Par exemple, la colonne qui affiche le nom d’un projet est un lien vers le projet ; la colonne qui affiche le nom d’un utilisateur ou d’une utilisatrice est un lien vers la page de profil de cette personne.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 100%

---

# Vue : supprimer le lien vers un objet dans une colonne

Certains objets affichés dans une vue renvoient par défaut à la page Détails de l’objet. Par exemple, la colonne qui affiche le nom d’un projet est un lien vers le projet ; la colonne qui affiche le nom d’un utilisateur ou d’une utilisatrice est un lien vers la page de profil de cette personne.

Vous pouvez supprimer ce lien en mode texte dans les colonnes qui s’affichent dans toutes les vues.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demander la modification d’un affichage </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Exemple : Supprimer le lien vers une tâche de la colonne Nom de la tâche dans une vue de la tâche :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue** pour créer une nouvelle vue.

   Ou

   Cliquez sur l’**icône de notification** ![](assets/edit-icon.png)

   pour modifier une vue existante, puis sélectionnez la vue.

1. Cliquez sur **Ajouter une colonne** pour ajouter une nouvelle colonne.

   Ou

   Cliquez sur une colonne existante avec un lien vers un objet.

1. Cliquez sur **Basculer en mode texte**.
1. Survolez la zone du mode texte et cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte qui se trouve dans la zone **Mode texte** et remplacez-le par le code suivant :
   <pre>displayname=Task Name<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >Vous pouvez utiliser un code similaire pour d’autres objets en procédant aux ajustements suivants :
   >
   >* Remplacez la ligne de code **valuefield** par **valueexpression** et conservez le même nom entre crochets après le signe égal.
   >* Éliminez toutes les lignes commençant par `link.` du texte original de la colonne. Par exemple, éliminez toutes les lignes suivantes :
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Cliquez sur **Enregistrer**, puis sur **Enregistrer l’affichage**.
