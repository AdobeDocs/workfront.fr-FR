---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Groupement : modifiez le nom d’affichage dans un groupement"
description: Vous pouvez renommer les regroupements dans les listes et les rapports et leur donner un nom que vos utilisateurs et utilisatrices connaissent mieux.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 77%

---

# Regroupement : modifier le nom d’affichage dans un regroupement

<!--Audited: 01/2024-->

Vous pouvez renommer les regroupements et leur donner un nom que vos utilisateurs et utilisatrices connaissent mieux.

Par exemple, lorsque vous appliquez le regroupement Nom de portfolio standard à une liste de projets, le nom du regroupement apparaît comme *Portfolio : nom :`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

Vous pouvez modifier ce regroupement en mode texte pour afficher un nom plus facile à lire.

![](assets/grouping-edited-name-350x160.png)

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
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur à la modification d’un filtre </p></li>
   <li><p>Standard pour modifier un rapport</p></li> </ul>

<p>Actuel :</p>
   <ul><li><p>Demande de modification d’un filtre </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </ul></td> 
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

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier le nom d’affichage dans un regroupement

Pour modifier le nom d’affichage dans un regroupement de projet, procédez comme suit :

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.

1. Cliquez sur **Ajouter un groupement** et commencez à saisir &quot;Nom du Portfolio&quot; dans le champ **Group by:** , puis sélectionnez-le lorsqu&#39;il s&#39;affiche dans la liste.

1. Cliquez sur **Basculer en mode texte**.
1. Effectuez l’une des opérations suivantes :

   * Ajoutez le code suivant au texte existant disponible dans la case **Grouper votre rapport** :


     `group.0.displayname=Your Value`


     Par exemple, ajoutez le code suivant pour remplacer le nom d’affichage par &quot;Portfolio&quot; :

     `group.0.displayname=Portfolio`

   * Supprimez toutes les lignes dans l’interface du mode texte du regroupement contenant le mot « nom », puis ajoutez la ligne :

     `group.0.name=Your Value`

     Par exemple, ajoutez le code suivant pour remplacer le nom d’affichage par &quot;Portfolio&quot; :

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >Vous pouvez également laisser le `group.0.name=` et les lignes `group.0.displayname=` vides, auquel cas le regroupement affiche la valeur pour laquelle vous effectuez le regroupement.


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. Cliquez sur **Terminé**, puis sur **Enregistrer le regroupement**.
1. (Facultatif) Mettez à jour le nom du groupement, puis cliquez sur **Enregistrer le groupement**.

   Le nom par défaut du regroupement est modifié en fonction de vos informations de mode texte.
