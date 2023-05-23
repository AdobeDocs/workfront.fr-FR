---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : éléments de reporting utilisés dans les rapports'
description: Cette vue affiche la Vue, le Filtre et le Groupement utilisés pour créer chaque rapport dans Adobe Workfront lorsque vous l’utilisez dans une liste de rapports.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 67f86523-e136-4768-af93-586a107b106f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Afficher : éléments de reporting utilisés dans les rapports

Cette vue affiche la Vue, le Filtre et le Groupement utilisés pour créer chaque rapport dans Adobe Workfront lorsque vous l’utilisez dans une liste de rapports.

Vous pouvez voir la variable

```
valuefields
```

ou

```
valueexpressions
```

utilisé dans chaque élément du rapport.

![report_with_elements_definitions.png](assets/report-with-elements-definitions-350x130.png)

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

## Afficher les éléments de rapport utilisés dans les rapports

1. Accédez à une liste de rapports.
1. Dans la **Affichage** menu déroulant, sélectionnez **Nouvelle vue**.

1. Dans le **Aperçu des colonnes** , éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=string<br>column.0.link.lookup=link.run<br>column.0.link.value=val(objCode)<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.descriptionkey=objecttype<br>column.1.listsort=nested(view).string(uiObjCode)<br>column.1.namekey=objecttype.abbr<br>column.1.querysort=uiObjCode<br>column.1.valuefield=uiObjCode<br>column.1.valueformat=objCodeMessage<br>column.1.width=80<br>column.2.descriptionkey=enter<br>column.2.listsort=nested(embeddedBy).string(lastName)<br>column.2.namekey=enter.by.abbr<br>column.2.querysort=entryBy:lastName<br>column.2.valuefield=entryBy:name<br>column.2.valueformat=HTML<br>column.2.width=130<br>column.3.displayname=Définition du filtre<br>column.3.textmode=true<br>column.3.valuefield=filter:definition<br>column.3.value.format=HTML<br>column.4.displayname=Définition de la vue<br>column.4.textmode=true<br>column.4.valuefield=view:definition<br>column.4.valueformat=HTML<br>column.5.displayname=Définition du groupement<br>column.5.textmode=true<br>column.5.valuefield=groupBy:definition<br>column.5.valueformat=HTML<br></pre>

1. Cliquez sur **Enregistrer la vue**.
