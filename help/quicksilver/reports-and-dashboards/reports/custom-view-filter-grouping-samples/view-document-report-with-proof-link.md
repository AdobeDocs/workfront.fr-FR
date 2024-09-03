---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vue : rapport de document avec lien vers une épreuve'
description: 'Vue : rapport de document avec lien vers une épreuve'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 100%

---

# Vue : rapport de document avec lien vers une épreuve

Dans cette vue de document, vous pouvez insérer un lien vers une épreuve de la version actuelle du document.

![](assets/view-document-with-proof-link-350x92.png)

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

## Visualiser un rapport de document avec un lien vers une épreuve

Pour appliquer cet affichage :

1. Accédez à une liste de documents.
1. Dans le menu déroulant **Vue**, sélectionnez **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Basculer en mode texte**.
1. Survolez la zone du mode texte et cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte qui se trouve dans la zone **Mode texte** et remplacez-le par le code suivant :

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

1. Cliquez sur **Enregistrer**, puis sur **Enregistrer la vue**.
1. Saisissez un nom pour la vue, puis cliquez sur **Enregistrer la vue**.
1. (Facultatif) Pour vous assurer que vous n’affichez que les documents avec épreuves, ajoutez un filtre en procédant comme suit :

   1. Cliquez sur le menu déroulant **Filtres**, puis cliquez sur **Nouveau filtre**.
   1. Cliquez sur **Ajouter une règle de filtre** et commencez à taper Propriétaire d’épreuve, puis sélectionnez **Identifiant de propriétaire d’épreuve** lorsque cela s’affiche dans la liste.
   1. Sélectionnez **N’est pas vide** pour le modificateur de filtre.
   1. Cliquez sur **Enregistrer le filtre**, saisissez le nom du filtre, puis cliquez sur **Enregistrer le filtre**.

1. Cliquez sur le lien dans la colonne Lien de l’épreuve pour accéder à l’épreuve de la dernière version du document.
