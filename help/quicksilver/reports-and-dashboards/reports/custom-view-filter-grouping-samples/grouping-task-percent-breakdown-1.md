---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groupement : répartition du pourcentage de tâche 1'
description: '"Dans ce regroupement personnalisé de projets, vous pouvez afficher les projets regroupés selon une plage de valeurs de pourcentage de réalisation. Les ventilations présentent une valeur de 25 % d’incréments de point en pourcentage : 0 à 25 %, 25 à 50 %, etc.'''
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 2%

---

# Regroupement : répartition du pourcentage de tâche 1

Dans ce regroupement personnalisé de projets, vous pouvez afficher les projets regroupés selon une plage de valeurs de pourcentage de réalisation. Les ventilations présentent une valeur de 25 % d’incréments de point en pourcentage : 0 à 25 %, 25 à 50 %, etc. 

Le regroupement suivant classe les tâches par pourcentage de valeur complète en 6 regroupements différents :

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![task_25__ventilation_regroupement.png](assets/task-25--breakdown-grouping-350x412.png)

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
   <td> <p>Demande de modification d’un groupement </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification d’un rapport</p> <p>Editer l'accès aux Filtres, Vues, Groupements pour modifier un groupement</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Regroupement par pourcentage de tâche

Pour appliquer ce groupement :

1. Accédez à une liste de tâches.
1. Dans la **Regroupement** menu déroulant, sélectionnez **Nouveau groupement**.

1. Cliquez sur **Passer en mode Texte**.
1. Supprimez le texte de la section **Regrouper votre rapport** zone.
1. Remplacez le texte par le code suivant :

   <pre>group.0.linkedname=direct<br>group.0.name=Répartition en pourcentage<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %", IF({percentComplete}&lt;=26,"0-25 %", IF({percentComplete}&lt;=51,"25-50 %", IF({percentComplete}&lt;=76,"50-75 %",IF({percent} &lt;100,"75-99 %","100 %"))))<br>group.0.valueformat=string</pre>

1. Cliquez sur **Enregistrer le groupement**.
