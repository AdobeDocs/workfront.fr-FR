---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : rapport de document avec lien vers une épreuve'
description: 'Vue : rapport de document avec lien vers une épreuve'
author: Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 66%

---

# Vue : rapport de document avec lien vers une épreuve

<!--Audited: 11/2024-->

Dans cette vue de document, vous pouvez insérer un lien vers une épreuve de la version actuelle du document.

![Afficher le document avec le lien du BAT](assets/view-document-with-proof-link-350x92.png)

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
   <p>Contributeur ou demande de modification d’un filtre </p>
   <p>Standard ou Plan pour modifier un rapport</p>
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

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualiser un rapport de document avec un lien vers une épreuve

Pour appliquer cet affichage :

1. Accédez à une liste de documents.
1. Dans le menu déroulant **Vue**, sélectionnez **Nouvelle vue**.
1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Basculer en mode texte**, puis **Modifier le mode texte**.
1. Supprimez le texte de la zone **Modifier le mode texte** et remplacez-le par le code suivant :

   ```
   displayname=Proof Link
   shortview=true
   textmode=true
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Remplacez « Your domain » par votre domaine Workfront actuel. Par exemple, si l’URL Workfront de votre entreprise est *Company.my.workfront.com*, votre domaine est « Company ».

1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.
1. (Facultatif) Mettez à jour le nom de la vue, puis cliquez sur **Enregistrer la vue**.
1. (Facultatif) Pour vous assurer que vous n’affichez que les documents avec épreuves, ajoutez un filtre en procédant comme suit :

   1. Cliquez sur le menu déroulant **Filtres**, puis cliquez sur **Nouveau filtre**.
   1. Cliquez sur **Ajouter une règle de filtre** et commencez à saisir « Propriétaire de l’épreuve », puis sélectionnez **ID du propriétaire de l’épreuve** lorsqu’il s’affiche dans la liste.
   1. Sélectionnez **N’est pas vide** pour le modificateur de filtre.
   1. Cliquez sur **Enregistrer le filtre**.
   1. (Facultatif) Mettez à jour le nom du filtre, puis cliquez sur **Enregistrer le filtre**.

1. Cliquez sur le lien dans la colonne Lien de l’épreuve pour accéder à l’épreuve de la dernière version du document.
