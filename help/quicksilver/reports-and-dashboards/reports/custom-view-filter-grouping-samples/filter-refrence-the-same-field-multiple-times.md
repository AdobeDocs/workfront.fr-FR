---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Filtre : créer plusieurs règles de filtrage qui font référence au même champ (instructions AND) »'
description: Dans l’interface en mode standard, lorsque vous essayez de créer plusieurs filtres qui font référence au même champ (en utilisant le qualificateur AND), l’un des filtres est supprimé lorsque vous enregistrez le rapport et que vous quittez Report Builder.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 100%

---

# Filtre : créer plusieurs règles de filtrage qui font référence au même champ (instructions « AND »)

Dans l’interface en mode standard, lorsque vous essayez de créer plusieurs filtres qui font référence au même champ (en utilisant le qualificateur AND), l’un des filtres est supprimé lorsque vous enregistrez le rapport et que vous quittez Report Builder.

**Exemple :** vous souhaitez afficher uniquement les tâches dont le nom contient le mot « vert » mais pas le mot « rouge ». Adobe Workfront ne vous permet pas d’enregistrer les règles de filtrage suivantes à l’aide de l’interface en mode standard car elles font référence au même champ (Nom de la tâche), mais utilisent des modificateurs différents et se réfèrent à des valeurs différentes :

* Nom de la tâche > Contient > Vert
* Nom de la tâche > Ne contient pas > Rouge

Toutefois, vous pouvez créer ce filtre en mode texte.

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
   <td> <p>Demande de modification d’un filtre </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Créer plusieurs règles de filtrage faisant référence au même champ

1. Accédez à une liste de tâches.
1. Cliquez sur le menu déroulant **Filtre** et sélectionnez **Nouveau filtre**.
1. Cliquez sur **Basculer en mode texte**.
1. Pointez sur la zone du mode texte et cliquez sur **Cliquez pour modifier le texte**.
1. Dans la zone Définir les règles de filtrage de la zone Rapport, insérez le code suivant :

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

1. Cliquez sur **Terminé**, puis sur **Enregistrer le filtre**.
