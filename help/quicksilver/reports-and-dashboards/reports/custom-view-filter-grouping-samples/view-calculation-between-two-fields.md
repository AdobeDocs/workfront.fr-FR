---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : afficher le résultat d''un calcul entre deux champs d''une colonne'
description: Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Afficher : afficher le résultat d&#39;un calcul entre deux champs d&#39;une colonne ;

Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs.

Par exemple, si vous souhaitez connaître le nombre de jours de semaine écoulés entre deux dates, vous pouvez utiliser la syntaxe du mode texte et les expressions de données pour calculer cette différence.\
Par exemple, vous pouvez calculer la différence hebdomadaire entre la date de fin planifiée et la date de fin réelle d’une tâche et afficher le résultat dans une colonne.

Vous pouvez utiliser deux autres dates dans ce calcul (Début réel, Fin réelle, Début projeté, Fin projetée, etc.).\
Pour plus d’informations sur les expressions de données calculées, voir [Expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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
   <td> <p>Demande de modification d’une vue </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification d’un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier une vue</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Afficher le résultat d&#39;un calcul entre deux champs d&#39;une colonne

Pour ajouter cette colonne à une vue de tâche :

1. Accédez à une liste de tâches.
1. Dans la **Affichage** menu déroulant, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**, puis **Passer en mode Texte**.

1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :
   <pre>displayname=Semaine Différence Jour<br>textmode=true<br>valueexpression=WEEKDAYDIFF({scheduledCompletionDate},{realCompletionDate})<br>valueformat=HTML</pre>

1. (Facultatif) Pour agréger les valeurs affichées dans la vue d’un groupement, procédez comme décrit dans la section [Regroupement : afficher le résultat de l&#39;agrégation de plusieurs valeurs calculées dans un groupement ;](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Cliquez sur **Enregistrer**, puis **Enregistrer la vue**.
