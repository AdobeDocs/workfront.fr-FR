---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : masquer le contenu d’une colonne »'
description: Vous pouvez masquer les informations dans la colonne d’une vue. Pour ce faire, modifiez le mode texte de la colonne.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 100%

---

# Vue : masquer le contenu d’une colonne

Vous pouvez masquer les informations dans la colonne d’une vue. Pour ce faire, modifiez le mode texte de la colonne.

>[!TIP]
>
>* Vous pouvez utiliser des colonnes masquées pour trier selon un certain objet que vous ne souhaitez pas afficher dans la vue.\
>  Par exemple, vous pouvez trier par numéro de tâche dans une vue de tâche et masquer le numéro de tâche. Dans ce cas, l’objet référencé dans la colonne permet de trier la vue, mais les informations de cet objet ne s’affichent pas dans la vue.
>* Lorsque vous masquez une colonne, notez que les informations qu’elle contient sont masquées, mais que la colonne existe toujours dans la vue.
>

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

## Exemple : triez et masquez la colonne Numéro de tâche dans une vue de tâche :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne** et commencez à saisir « Numéro de la tâche » dans le champ **Afficher dans cette colonne** puis sélectionnez-le lorsqu’il s’affiche dans la liste.

1. Cliquez sur **Basculer en mode texte**.
1. Survolez la zone du mode texte et cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte qui se trouve dans la zone **Mode texte** et remplacez-le par le code suivant :

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>Les modifications importantes apportées à ce code pour masquer la colonne sont les suivantes :

   ```
   displayname
   ```

   cette ligne doit être vide.

   ```
   valuefield
   ```

   Ceci a été remplacé par *value* et doit être vide.

   ```
   width
   ```

   : selon le champ, cette valeur doit être *0* ou *1*.

1. Cliquez sur **Enregistrer**, puis **Enregistrer la vue**.
