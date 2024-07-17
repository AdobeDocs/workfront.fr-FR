---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtre : créez plusieurs règles de filtrage qui référencent le même champ ('instructions AND')"
description: Dans l’interface de mode standard, lorsque vous tentez de créer plusieurs filtres qui référencent le même champ (à l’aide du qualificateur ET), l’un des filtres est supprimé lorsque vous enregistrez le rapport et quittez le créateur de rapports.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 28%

---

# Filtre : créer plusieurs règles de filtrage qui font référence au même champ (instructions « AND »)

Dans l’interface de mode standard, lorsque vous tentez de créer plusieurs filtres qui référencent le même champ (à l’aide du qualificateur ET), l’un des filtres est supprimé lorsque vous enregistrez le rapport et quittez le créateur de rapports.

**Exemple :** Vous pouvez afficher uniquement les tâches qui contiennent le mot &quot;vert&quot; mais ne contiennent pas le mot &quot;rouge&quot; dans le nom. Adobe Workfront ne vous permet pas d’enregistrer les règles de filtrage suivantes à l’aide de l’interface de mode standard, car elle fait référence au même champ (Nom de la tâche), mais utilise des modificateurs différents et fait référence à des valeurs différentes :

* Nom de la tâche > Contient > Vert
* Nom de la tâche > Ne contient pas > Rouge

Vous pouvez toutefois créer ce filtre en mode texte.

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
   <td> <p>Demande de modification d’un filtre </p>
   <p>Prévoir la modification d’un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier un filtre</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Créer plusieurs règles de filtrage qui référencent le même champ

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Filtre**, sélectionnez **Nouveau filtre**.
1. Cliquez sur **Passer en mode Texte**.
1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Dans la zone Définir les règles de filtrage pour votre rapport, ajoutez le code suivant :

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Pour créer des filtres similaires, vous devez d’abord créer la première instruction . Par exemple :
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Copiez et collez l’instruction autant de fois que nécessaire. Vous pouvez ensuite ajouter autant d’instructions que nécessaire pour référencer le même champ (dans notre cas, &quot;name&quot;) et apporter les modifications suivantes aux instructions supplémentaires :
   >
   >1. Précisez les deux lignes copiées avec &quot;AND:1:&quot;, &quot;AND:2:&quot;, &quot;AND:3:&quot;, etc. pour chaque nouvelle valeur de champ possible.
   >1. Remplacez la ligne du champ par la nouvelle valeur du champ (après le signe &quot;=&quot;).
   >1. Remplacez la ligne de modification (_Mod) par le nouveau modificateur .
   >   
   >Ces instructions sont sensibles à la casse.

1. Cliquez sur **Terminé**, puis sur **Enregistrer le filtre**.
