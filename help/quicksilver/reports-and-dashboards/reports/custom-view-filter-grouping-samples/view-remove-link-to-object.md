---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : supprimer le lien vers un objet dans une colonne'
description: Certains objets que vous affichez dans une vue sont associés par défaut à la page Détails de l’objet. Par exemple, la colonne qui affiche le nom d’un projet est un lien vers le projet ; la colonne Nom d’un utilisateur est un lien vers la page de profil de l’utilisateur.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Afficher : Suppression d’un lien vers un objet dans une colonne

Certains objets que vous affichez dans une vue sont associés par défaut à la page Détails de l’objet. Par exemple, la colonne qui affiche le nom d’un projet est un lien vers le projet ; la colonne Nom d’un utilisateur est un lien vers la page de profil de l’utilisateur.

Vous pouvez supprimer ce lien en mode texte dans les colonnes qui s’affichent dans toutes les vues.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Exemple : Supprimez le lien vers une tâche de la colonne Nom de la tâche dans une vue de tâche :

1. Accédez à une liste de tâches.
1. Dans la **Affichage** menu déroulant, cliquez sur **Nouvelle vue** pour créer une vue.

   Ou

   Cliquez sur le bouton **Icône Modifier** ![](assets/edit-icon.png)

   pour modifier une vue existante, sélectionnez-la.

1. Cliquez sur **Ajouter une colonne** pour ajouter une nouvelle colonne.

   Ou

   Cliquez sur une colonne existante avec un lien vers un objet.

1. Cliquez sur **Passer en mode Texte**.
1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :

   <pre>displayname=Task Name<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >Vous pouvez utiliser le même code pour d’autres objets en ajustant les éléments suivants :
   >
   >   
   >   
   >   * Remplacez la variable **valuefield** de la ligne de code avec **valeur expression** et conserver le même nom entre accolades après le signe égal.
   >   
   >   
   >
   >   
   >   
   >   * Éliminez toutes les lignes commençant par >

      >   
      >     ```>   
      >     link.
      >     ```   >   
      >   
      >     
      from the original text of the column. For example, eliminate all the following lines:
      >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
      >   
      >   
      >



1. Cliquez sur **Enregistrer**, puis **Enregistrer la vue**.
