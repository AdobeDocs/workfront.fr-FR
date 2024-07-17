---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Groupement : éditez le nom d'affichage dans un groupement"
description: Vous pouvez renommer les groupes dans les listes et les rapports en un élément plus familier pour vos utilisateurs.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 138181de2ad8257785773a5296bc5bcfc144a801
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 33%

---

# Regroupement : modifier le nom d’affichage dans un regroupement

<!--Audited: 01/2024-->

Vous pouvez renommer les regroupements en un élément plus familier à vos utilisateurs.

Par exemple, lorsque vous appliquez le regroupement Nom de Portfolio standard à une liste de projets, le nom du regroupement apparaît sous la forme *Portfolio : Nom :`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

Vous pouvez modifier ce regroupement en mode texte pour afficher un nom plus facile à lire.

![](assets/grouping-edited-name-350x160.png)

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
   <td>

<p>Nouveau : </p>
   <ul>
   <li> <p>Contributeur à la modification d’un groupement </p></li>
   <li><p>Standard pour modifier un rapport</p></li></ul>

<p> Actuel :</p>
   <ul>  
   <li><p>Demande de modification d’un groupement </p></li>
   <li><p>Prévoir la modification d’un rapport</p></li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Editer l'accès aux Filtres, Vues, Groupements pour modifier un groupement</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Editer le nom d&#39;affichage dans un groupement

Pour modifier le nom d’affichage dans un regroupement de projet :

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Groupement**, sélectionnez **Nouveau groupement**.

1. Cliquez sur **Ajouter un groupement** et commencez à saisir &quot;Nom du Portfolio&quot; dans le champ **First by :** , puis sélectionnez-le lorsqu’il s’affiche dans la liste.

1. Cliquez sur **Passer en mode Texte**.
1. Effectuez l’une des opérations suivantes :

   * Ajoutez le code suivant au texte existant disponible dans la zone **Regrouper votre rapport** :


     `group.0.displayname=Your Value`


     Ou, dans ce cas :

     `group.0.displayname=Portfolio`

   * Supprimez toutes les lignes dans l&#39;interface du mode texte du groupement contenant le mot &quot;name&quot;, puis ajoutez la ligne :

     `group.0.name=Your Value`

     Ou, dans ce cas :

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >Vous pouvez également laisser les lignes `group.0.name=` et `group.0.displayname=` vides, auquel cas le regroupement affiche la valeur par laquelle vous effectuez le regroupement.


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. Cliquez sur **Terminé**, puis sur **Enregistrer le groupement**.

   Le nom par défaut du groupement est modifié en fonction de vos informations de mode texte.
