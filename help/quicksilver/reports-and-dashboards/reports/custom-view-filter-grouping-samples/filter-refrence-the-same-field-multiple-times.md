---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtre : créer plusieurs règles de filtrage qui référencent le même champ (’instructions AND’)"
description: Dans l’interface en mode standard, lorsque vous essayez de créer plusieurs filtres qui font référence au même champ (en utilisant le qualificateur AND), l’un des filtres est supprimé lorsque vous enregistrez le rapport et que vous quittez Report Builder.
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 89%

---

# Filtre : créer plusieurs règles de filtrage qui font référence au même champ (instructions « AND »)

<!--Audited: 10/2024-->

Dans l’interface en mode standard, lorsque vous essayez de créer plusieurs filtres qui font référence au même champ (en utilisant le qualificateur AND), l’un des filtres est supprimé lorsque vous enregistrez le rapport et que vous quittez Report Builder.

**Exemple :** vous souhaitez afficher uniquement les tâches dont le nom contient le mot « vert » mais pas le mot « rouge ». Adobe Workfront ne vous permet pas d’enregistrer les règles de filtrage suivantes à l’aide de l’interface en mode standard car elles font référence au même champ (Nom de la tâche), mais utilisent des modificateurs différents et se réfèrent à des valeurs différentes :

* Nom de la tâche > Contient > Vert
* Nom de la tâche > Ne contient pas > Rouge

Toutefois, vous pouvez créer ce filtre en mode texte.

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

## Créer plusieurs règles de filtrage faisant référence au même champ

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Filtre**, sélectionnez **Nouveau filtre**.
1. Cliquez sur **Text Mode**.
1. Dans la zone qui s&#39;affiche, ajoutez le code suivant :

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Pour créer des filtres similaires, créez d’abord la première instruction. Par exemple :
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Copiez et collez l’instruction autant de fois que nécessaire. Vous pouvez ensuite ajouter autant d’instructions que nécessaire pour référencer le même champ (dans notre cas, « nom ») et apporter les modifications suivantes aux déclarations supplémentaires :
   >
   >1. Ajoutez « AND:1: », « AND:2: », « AND:3: », etc. au début des deux lignes copiées pour chaque nouvelle valeur possible du champ.
   >1. Remplacez la ligne du champ par la nouvelle valeur du champ (après le signe « = »).
   >1. Remplacez la ligne du modificateur (_Mod) par le nouveau modificateur.
   >   
   >Ces instructions respectent la casse.

1. Cliquez sur **Apply**, puis sur **Save as new**.
