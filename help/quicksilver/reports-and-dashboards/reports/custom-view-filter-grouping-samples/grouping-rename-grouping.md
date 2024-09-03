---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Regroupement : modifier le nom d’affichage dans un regroupement »'
description: Vous pouvez renommer les regroupements dans les listes et les rapports et leur donner un nom que vos utilisateurs et utilisatrices connaissent mieux.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 138181de2ad8257785773a5296bc5bcfc144a801
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 100%

---

# Regroupement : modifier le nom d’affichage dans un regroupement

<!--Audited: 01/2024-->

Vous pouvez renommer les regroupements et leur donner un nom que vos utilisateurs et utilisatrices connaissent mieux.

Par exemple, lorsque vous appliquez le regroupement Nom de portfolio standard à une liste de projets, le nom du regroupement apparaît comme *Portfolio : nom :`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

Vous pouvez modifier ce regroupement en mode texte pour afficher un nom plus facile à lire.

![](assets/grouping-edited-name-350x160.png)

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
   <td>

<p>Nouveau : </p>
   <ul>
   <li> <p>Personne contributrice pour modifier un regroupement </p></li>
   <li><p>Standard pour modifier un rapport</p></li></ul>

<p> Actuel :</p>
   <ul>  
   <li><p>Demander à modifier un regroupement </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et regroupements pour modifier un regroupement</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Modifier le nom d’affichage dans un regroupement

Pour modifier le nom d’affichage dans un regroupement de projet, procédez comme suit :

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.

1. Cliquez sur **Ajouter un regroupement**, puis commencez à saisir « Nom du portfolio » dans le champ **D’abord par :** puis sélectionnez-le lorsqu’il s’affiche dans la liste.

1. Cliquez sur **Basculer en mode texte**.
1. Effectuez l’une des opérations suivantes :

   * Ajoutez le code suivant au texte existant disponible dans la case **Grouper votre rapport** :


     `group.0.displayname=Your Value`


     Ou, dans ce cas, effectuez ce qui suit :

     `group.0.displayname=Portfolio`

   * Supprimez toutes les lignes dans l’interface du mode texte du regroupement contenant le mot « nom », puis ajoutez la ligne :

     `group.0.name=Your Value`

     Ou, dans ce cas, effectuez ce qui suit :

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >Vous pouvez également laisser le `group.0.name=` et les lignes `group.0.displayname=` vides, auquel cas le regroupement affiche la valeur pour laquelle vous effectuez le regroupement.


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. Cliquez sur **Terminé**, puis sur **Enregistrer le regroupement**.

   Le nom par défaut du regroupement est modifié en fonction de vos informations de mode texte.
