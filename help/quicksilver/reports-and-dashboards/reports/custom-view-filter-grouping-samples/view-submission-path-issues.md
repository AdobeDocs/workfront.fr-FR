---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Affichage : chemin d’envoi pour les problèmes"
description: Vous pouvez afficher le chemin à travers lequel un problème a été envoyé dans l’affichage d’un rapport de problème. Le chemin d’accès indique la file d’attente, le groupe de rubriques et la rubrique de la file d’attente où le problème a été envoyé initialement.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bee1e066-c3f4-4d74-92b0-ab7f43d52a50
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 46%

---

# Vue : chemin de soumission des problèmes

Vous pouvez afficher le chemin à travers lequel un problème a été envoyé dans l’affichage d’un rapport de problème. Le chemin d’accès indique la file d’attente, le groupe de rubriques et la rubrique de la file d’attente où le problème a été envoyé initialement.

![issue_submission_path.png](assets/issue-submission-path-350x66.png)

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

## Afficher le chemin d’envoi pour les problèmes

1. Accédez à une liste de problèmes.
1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, cliquez sur **Ajouter une colonne**.

1. Cliquez sur l’en-tête de la nouvelle colonne, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode Texte, puis cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :
   <pre>displayname= Issue Path<br>linkedname=direct <br>namekey=displayQueueBreadcrumb <br>valuefield=displayQueueBreadcrumb <br>valueformat=HTML<br></pre>

1. Cliquez sur **Enregistrer la vue**.
