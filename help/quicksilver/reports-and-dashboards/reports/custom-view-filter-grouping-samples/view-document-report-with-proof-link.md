---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : rapport de document avec lien vers un BAT'
description: 'Afficher : rapport de document avec lien vers un BAT'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 43%

---

# Vue : rapport de document avec lien vers une épreuve

Dans cette vue de document, vous pouvez insérer un lien vers un BAT de la version actuelle du document.

![](assets/view-document-with-proof-link-350x92.png)

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

## Afficher un rapport de document avec un lien vers un BAT

Pour appliquer cette vue :

1. Accédez à une liste de documents.
1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Passer en mode Texte**.
1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Remplacez &quot;Votre domaine&quot; par votre domaine Workfront réel. Par exemple, si l’URL Workfront de votre société est *Company.my.workfront.com*, votre domaine est &quot;Société&quot;.

1. Cliquez sur **Enregistrer**, puis sur **Enregistrer la vue**.
1. Saisissez le nom de la vue, puis cliquez sur **Enregistrer la vue**.
1. (Facultatif) Pour n’afficher que les documents avec BAT, ajoutez un filtre en procédant comme suit :

   1. Cliquez sur le menu déroulant **Filtre**, puis sur **Nouveau filtre**.
   1. Cliquez sur **Ajouter une règle de filtre** et commencez à saisir Propriétaire du BAT, puis sélectionnez **ID de propriétaire du BAT** lorsqu’il s’affiche dans la liste.
   1. Sélectionnez **N’est pas vierge** pour le modificateur de filtre.
   1. Cliquez sur **Enregistrer le filtre**, saisissez le nom du filtre, puis cliquez sur **Enregistrer le filtre**.

1. Cliquez sur le lien de la colonne Lien du bon à tirer pour accéder au BAT de la dernière version du document.
