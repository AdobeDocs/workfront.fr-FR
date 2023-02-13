---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : ajouter une liste de successeurs de tâches dans une colonne'
description: Vous pouvez ajouter une colonne à un affichage de tâche pour afficher la liste des successeurs des tâches. La colonne Réussites de la tâche comprend le numéro du successeur ainsi que le nom.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Afficher : ajouter une liste de successeurs de tâches dans une colonne

Vous pouvez ajouter une colonne à un affichage de tâche pour afficher la liste des successeurs des tâches. Le **Réussites de la tâche** inclut le numéro du successeur ainsi que le nom.

![task_view_with_a_list_of_succeeded_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Ajouter une liste de successeurs de tâches dans une colonne

Pour ajouter cette colonne à une vue de tâche :

1. Accédez à une vue de tâche existante.
1. Développez le menu déroulant Affichage , puis sélectionnez **Vue Personnaliser**.
1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la **Afficher dans cette colonne** , puis cliquez sur **Cliquer pour modifier le texte**.

1. Supprimez tout le texte de la zone Mode Texte et remplacez-le par le code suivant :

   <pre>displayname=Task Success<br>listsepariter=<br><br>listmethod=nested(succeeded).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({remplacement}).{taskNumber},' - ',{remplacement}.{name})<br>valueformat=HTML</pre>

1. Cliquez sur **Enregistrer la vue**.
