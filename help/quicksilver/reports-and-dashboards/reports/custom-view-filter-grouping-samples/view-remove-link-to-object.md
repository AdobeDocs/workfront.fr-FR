---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : supprimer le lien vers un objet dans une colonne'
description: Certains objets affichés dans une vue renvoient par défaut à la page Détails de l’objet. Par exemple, la colonne qui affiche le nom d’un projet est un lien vers le projet ; la colonne qui affiche le nom d’un utilisateur ou d’une utilisatrice est un lien vers la page de profil de cette personne.
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 75%

---

# Vue : supprimer le lien vers un objet dans une colonne

<!--Audited: 11/2024-->

Certains objets affichés dans une vue renvoient par défaut à la page Détails de l’objet. Par exemple, la colonne qui affiche le nom d’un projet est un lien vers le projet ; la colonne qui affiche le nom d’un utilisateur ou d’une utilisatrice est un lien vers la page de profil de cette personne.

Vous pouvez supprimer ce lien en mode texte dans les colonnes qui s’affichent dans toutes les vues.

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

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++


## Exemple : Supprimer le lien vers une tâche de la colonne Nom de la tâche dans une vue de la tâche :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue** pour créer une nouvelle vue.

   Ou

   Cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) pour modifier une vue existante, puis sélectionnez la vue.

1. Cliquez sur **Ajouter une colonne** pour ajouter une nouvelle colonne.

   Ou

   Cliquez sur une colonne existante avec un lien vers un objet.

1. Cliquez sur **Passer en mode Texte** > **Modifier le mode Texte**.
1. Supprimez le texte de la zone **Modifier le mode texte** et remplacez-le par le code suivant :

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >Vous pouvez utiliser un code similaire pour d’autres objets en procédant aux ajustements suivants :
   >
   >* Remplacez la ligne `valuefield` du code par `valueexpression` et conservez le même nom inclus entre crochets après le signe égal.
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

1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.

