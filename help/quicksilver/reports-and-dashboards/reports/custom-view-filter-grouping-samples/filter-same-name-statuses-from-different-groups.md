---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtre : afficher les éléments par états du même nom lorsque les états sont associés à différents groupes"
description: Vous pouvez avoir un statut de tâche affecté au groupe A nommé Nouveau statut avec la clé à 3 lettres « NST ». Un autre statut de tâche peut être affecté au groupe B, également nommé Nouveau statut, avec la clé à 3 lettres « NES ». Bien que les noms des deux statuts puissent être identiques, le code à 3 lettres est toujours unique. Pour plus d’informations sur les statuts de groupe, voir Créer ou modifier un statut de groupe.
author: Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 65%

---

# Filtre : afficher les éléments par statut de même nom lorsque les statuts sont associés à des groupes différents

<!--Audited: 10/2024-->

Vous pouvez avoir un statut de tâche affecté au groupe A nommé *Nouveau statut* avec la clé à 3 lettres *« NST »*. Un autre statut de tâche peut être affecté au groupe B, également nommé *Nouveau statut* avec la clé à 3 lettres *« NES ».* Bien que les noms des deux statuts puissent être identiques, le code à 3 lettres est toujours unique.

Pour plus d’informations sur les statuts de groupe, voir [Créer ou modifier un statut de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Le créateur de filtres ne vous permet pas de différencier deux statuts qui portent le même nom. Vous devez utiliser le mode Texte dans un filtre personnalisé pour faire la distinction entre les 2 états.

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

## Afficher les éléments par statut de même nom lorsque les statuts sont associés à des groupes différents

1. Accédez à la liste déroulante **Filtre** pour le filtre que vous souhaitez personnaliser pour une liste de tâches, par exemple.\
   Cela s’applique également aux projets et aux problèmes.
1. Cliquez sur **Nouveau filtre**.
1. Dans la première liste déroulante du coin supérieur gauche, sélectionnez Tâche > Statut.
1. Sélectionnez **Égal à** pour le modificateur, puis sélectionnez l’un des états sur lesquels vous souhaitez créer un rapport.

   Par exemple, dans un rapport de tâche, ajoutez **Status Equals New Status**, si vous souhaitez afficher uniquement les tâches dont l’état est **New Status**.

   >[!TIP]
   >
   >Notez que vous ne disposez que d’une seule option pour un statut nommé Nouveau statut.

1. Cliquez sur **Text Mode**.\
   Le code suivant doit s’afficher dans l’espace fourni :

   <pre>OR:1:status=NST<br>OR:1:status_Mod=in </pre>

   >[!NOTE]
   >
   >Un seul statut s’affiche ici. La ligne du statut affiche l’une des clés à 3 lettres correspondant à l’un des statuts.

1. Ajoutez les deux lignes de code suivantes pour ajouter le statut qui manque dans le filtre :

   <pre>OR:2:status=NES<br>OR:2:status_Mod=in</pre>

1. Cliquez sur **Apply**, puis sur **Save as new**.

   La liste affiche les deux tâches avec le statut &quot;Nouveau statut&quot; du groupe A et le statut &quot;Nouveau statut&quot; du groupe B.
