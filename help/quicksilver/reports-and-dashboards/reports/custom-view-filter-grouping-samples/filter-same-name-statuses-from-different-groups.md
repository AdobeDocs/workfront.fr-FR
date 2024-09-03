---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Filtre : afficher les éléments par statut de même nom lorsque les statuts sont associés à des groupes différents »'
description: Vous pouvez avoir un statut de tâche affecté au groupe A nommé Nouveau statut avec la clé à 3 lettres « NST ». Un autre statut de tâche peut être affecté au groupe B, également nommé Nouveau statut, avec la clé à 3 lettres « NES ». Bien que les noms des deux statuts puissent être identiques, le code à 3 lettres est toujours unique. Pour plus d’informations sur les statuts de groupe, voir Créer ou modifier un statut de groupe.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 100%

---

# Filtre : afficher les éléments par statut de même nom lorsque les statuts sont associés à des groupes différents

Vous pouvez avoir un statut de tâche affecté au groupe A nommé *Nouveau statut* avec la clé à 3 lettres *« NST »*. Un autre statut de tâche peut être affecté au groupe B, également nommé *Nouveau statut* avec la clé à 3 lettres *« NES ».* Bien que les noms des deux statuts puissent être identiques, le code à 3 lettres est toujours unique.\
Pour plus d’informations sur les statuts de groupe, voir [Créer ou modifier un statut de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Le créateur de filtres ne vous permet pas de différencier deux statuts qui portent le même nom. Vous devez utiliser le mode texte pour faire la distinction entre les deux statuts.

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

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher les éléments par statut de même nom lorsque les statuts sont associés à des groupes différents

1. Accédez au filtre que vous souhaitez personnaliser pour une liste de tâches, par exemple.\
   Cela s’applique également aux projets et aux problèmes.
1. Cliquez sur **Ajouter une règle de filtre** pour le champ **Statut** de l’objet de votre liste.\
   Par exemple, dans un rapport de tâches, ajoutez **Statut égal à Nouveau statut**, si vous souhaitez n’afficher que les tâches dont le statut est **Nouveau statut**.

   >[!TIP]
   >
   >Notez que vous ne disposez que d’une seule option pour un statut nommé Nouveau statut.

1. Cliquez sur **Basculer en mode texte**.\
   Le code suivant doit s’afficher :
   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Un seul statut s’affiche ici. La ligne du statut affiche l’une des clés à 3 lettres correspondant à l’un des statuts.

1. Ajoutez les deux lignes de code suivantes pour ajouter le statut qui manque dans le filtre :
   <pre>OR:1:status=NES<br>OR:1:status_Mod=in</pre>

1. Cliquez sur **Terminé**, puis sur **Enregistrer le filtre**.

   La liste affiche les tâches au statut « Nouveau statut » du groupe A et au statut « Nouveau statut » du groupe B.
