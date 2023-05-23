---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : rapport de document avec lien vers un BAT'
description: '"Affichage : rapport de document avec lien vers un BAT'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Afficher : rapport de document avec lien vers un BAT

Dans cette vue de document, vous pouvez insérer un lien vers un BAT de la version actuelle du document.

![](assets/view-document-with-proof-link-350x92.png)

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

## Afficher un rapport de document avec un lien vers un BAT

Pour appliquer cette vue :

1. Accédez à une liste de documents.
1. Dans la **Affichage** menu déroulant, sélectionnez **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Passer en mode Texte**.
1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Remplacez &quot;Votre domaine&quot; par votre domaine Workfront réel. Par exemple, si l’URL Workfront de votre entreprise est *Company.my.workfront.com*, votre domaine est &quot;Société&quot;.

1. Cliquez sur **Enregistrer**, puis **Enregistrer la vue**.
1. Saisissez le nom de la vue, puis cliquez sur **Enregistrer la vue**.
1. (Facultatif) Pour n’afficher que les documents avec BAT, ajoutez un filtre en procédant comme suit :

   1. Cliquez sur le bouton **Filtrer** menu déroulant, puis cliquez sur **Nouveau filtre**.
   1. Cliquez sur **Ajouter une règle de filtre** et commencez à saisir Propriétaire du BAT, puis sélectionnez **Identifiant du propriétaire du BAT** lorsqu’il s’affiche dans la liste.
   1. Sélectionner **N’est pas vierge** pour le modificateur de filtre.
   1. Cliquez sur **Enregistrer le filtre**, saisissez le nom du filtre, puis cliquez sur **Enregistrer le filtre**.

1. Cliquez sur le lien de la colonne Lien du bon à tirer pour accéder au BAT de la dernière version du document.
