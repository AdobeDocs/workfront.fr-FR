---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Vue : supprimer le lien vers un objet d’une colonne"
description: Certains objets que vous affichez dans une vue sont associés par défaut à la page Détails de l’objet. Par exemple, la colonne qui affiche le nom d’un projet est un lien vers le projet ; la colonne qui affiche le nom d’un utilisateur est un lien vers la page de profil de l’utilisateur.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 36%

---

# Vue : supprimer le lien vers un objet dans une colonne

Certains objets que vous affichez dans une vue sont associés par défaut à la page Détails de l’objet. Par exemple, la colonne qui affiche le nom d’un projet est un lien vers le projet ; la colonne qui affiche le nom d’un utilisateur est un lien vers la page de profil de l’utilisateur.

Vous pouvez supprimer ce lien en mode texte dans les colonnes qui s’affichent dans toutes les vues.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demander la modification d’une vue </p>
   <p>Prévoir la modification d’un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier une vue</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Exemple : supprimez le lien vers une tâche de la colonne Nom de la tâche dans une vue de tâche :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Afficher**, cliquez sur **Nouvelle vue** pour créer une vue.

   Ou

   Cliquez sur l’ **icône Modifier** ![](assets/edit-icon.png)

   pour modifier une vue existante, sélectionnez-la.

1. Cliquez sur **Ajouter une colonne** pour ajouter une nouvelle colonne.

   Ou

   Cliquez sur une colonne existante avec un lien vers un objet.

1. Cliquez sur **Passer en mode Texte**.
1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :
   <pre>displayname=Task Name<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >Vous pouvez utiliser le même code pour d’autres objets en ajustant les éléments suivants :
   >
   >* Remplacez la ligne **valuefield** du code par **valueexpression** et conservez le même nom entre accolades après le signe égal.
   >* Éliminez toutes les lignes commençant par `link.` du texte d’origine de la colonne. Supprimez par exemple toutes les lignes suivantes :
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Cliquez sur **Enregistrer**, puis sur **Enregistrer la vue**.
