---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Affichage : supprimer le lien vers un objet d’une colonne"
description: Certains objets affichés dans une vue renvoient par défaut à la page Détails de l’objet. Par exemple, la colonne qui affiche le nom d’un projet est un lien vers le projet ; la colonne qui affiche le nom d’un utilisateur ou d’une utilisatrice est un lien vers la page de profil de cette personne.
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 17a277a5a63a521ec7285e3f5051bfd42fc204bf
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 84%

---

# Vue : supprimer le lien vers un objet dans une colonne

<!--Audited: 11/2024-->

Certains objets affichés dans une vue renvoient par défaut à la page Détails de l’objet. Par exemple, la colonne qui affiche le nom d’un projet est un lien vers le projet ; la colonne qui affiche le nom d’un utilisateur ou d’une utilisatrice est un lien vers la page de profil de cette personne.

Vous pouvez supprimer ce lien en mode texte dans les colonnes qui s’affichent dans toutes les vues.

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
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p> Actuel : 
   <ul>
   <li>Demander la modification d’un affichage</li> 
   <li>Prévoir de modifier un rapport</li>
   </ul>
     </p>
     <p> Nouveau : 
   <ul>
   <li>Contributeur à la modification d’une vue</li> 
   <li>Standard pour modifier un rapport</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Exemple : Supprimer le lien vers une tâche de la colonne Nom de la tâche dans une vue de la tâche :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue** pour créer une nouvelle vue.

   Ou

   Cliquez sur l’**icône de notification** ![](assets/edit-icon.png)

   pour modifier une vue existante, puis sélectionnez la vue.

1. Cliquez sur **Ajouter une colonne** pour ajouter une nouvelle colonne.

   Ou

   Cliquez sur une colonne existante avec un lien vers un objet.

1. Cliquez sur **Passer en mode Texte** > **Modifier le mode Texte**.
1. Supprimez le texte que vous trouvez dans la zone **Edit Text Mode** et remplacez-le par le code suivant :

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
   >* Remplacez la ligne `valuefield` du code par `valueexpression` et conservez le même nom entre accolades après le signe égal.
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

