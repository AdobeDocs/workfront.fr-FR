---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtre : affiche les éléments selon les états du même nom lorsque les états sont associés à différents groupes'
description: Un état de tâche peut être affecté au groupe A nommé New Status avec la clé NST à 3 lettres. Un autre état de tâche peut également être affecté au groupe B, nommé Nouveau statut avec la clé 3 lettres NN. Bien que les noms des deux états puissent être identiques, le code à 3 lettres est toujours unique. Pour plus d’informations sur les états d’un groupe, voir Création ou modification de l’état d’un groupe.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 25%

---

# Filtre : afficher les éléments par statut de même nom lorsque les statuts sont associés à des groupes différents

Un état de tâche peut être attribué au groupe A nommé *New Status* avec la clé à 3 lettres *NST*. Un autre état de tâche peut être affecté au groupe B, également appelé *New Status* avec la clé à 3 lettres *NES.* Bien que les noms des deux états puissent être identiques, le code à 3 lettres est toujours unique.\
Pour plus d’informations sur les états d’un groupe, voir [Création ou modification d’un état d’un groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Avec le créateur de filtres, vous ne pouvez pas identifier les deux états portant le même nom. Vous devez utiliser le mode Texte pour faire la distinction entre les deux états.

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

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher les éléments par états du même nom lorsque les états sont associés à différents groupes

1. Accédez au filtre que vous souhaitez personnaliser pour une liste de tâches, par exemple.\
   Cela fonctionne de la même manière pour les projets et les problèmes.
1. Cliquez sur **Ajouter une règle de filtre** pour le champ **État** de l’objet de votre liste.\
   Par exemple, dans un rapport de tâche, ajoutez **Status Equal New Status**, si vous souhaitez afficher uniquement les tâches dont l’état est **New Status**.

   >[!TIP]
   >
   >Notez que vous n’avez qu’une seule option pour un état nommé New Status.

1. Cliquez sur **Passer en mode Texte**.\
   Le code suivant doit s’afficher :
   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Un seul état s’affiche ici. La ligne d’état affiche l’une des clés à 3 lettres pour l’un des états.

1. Ajoutez les 2 lignes de code suivantes pour ajouter l’état manquant dans le filtre :
   <pre>OR:1:status=NES<br>OR:1:status_Mod=in</pre>

1. Cliquez sur **Terminé**, puis sur **Enregistrer le filtre**.

   La liste affiche les deux tâches avec le statut &quot;Nouveau statut&quot; du groupe A et le statut &quot;Nouveau statut&quot; du groupe B.
