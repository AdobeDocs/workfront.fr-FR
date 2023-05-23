---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Affichage : vue de projet à plusieurs lignes"
description: 'Dans cette vue de projet, vous pouvez : MODIFIER MOI.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 3c6028c0-2c9f-4f86-aa6c-bf089844bac8
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Afficher : vue de projet à plusieurs lignes

Dans cette vue de projet, vous pouvez :

* Affichez les informations du projet dans un format multiligne.\
   La vue utilise la variable

   ```
   sharecol=true
   ```

   pour combiner plusieurs champs sous le même en-tête de colonne. Pour en savoir plus sur cette balise, voir [Afficher : fusionner les informations de plusieurs colonnes dans une seule colonne partagée](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

* Utilisez une colonne d’espace réservé qui contient une balise de saut de ligne de HTML (

   ```
   <br>
   ```

   ) pour forcer l’affichage de la description sous le nom du projet, par exemple.
* Affichez le propriétaire du projet entre parenthèses après le nom du projet.
* Affichez le nom du projet comme lien vers le projet.

![](assets/project-multi-row-stacked-view-350x219.png)

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

## Création d’une vue de projet de plusieurs lignes

1. Créez une vue de projet. Pour plus d’informations sur la création d’une vue, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
1. Lorsque vous créez la vue, supprimez toutes les colonnes sauf une.
1. Sélectionnez la colonne restante et cliquez sur **Passer en mode texte**.
1. Copiez et collez le mode texte ci-dessous dans la colonne :
   <pre>column.0.linkedname=direct<br>column.0.link.valueformat=val<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.valuefield=objCode<br>column.0.link.lookup=link.view<br>column.0.sharecol=true<br>column.0.descriptionkey=name<br>column.0.width=150<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.name=Nom du projet / Gestionnaire / Description<br>column.0.shortview=false<br>column.0.étich=100<br>column.0.textmode=true<br>column.0.listsort=string(name)<br>column.0.valueformat=HTML<br>column.1.valueexpression=CONCAT(" (",{owner}).{name},")")<br>column.1.listsort=nested(owner).string(name)<br>column.1.width=1<br>column.1.linkedname=direct<br>column.1.querysort=owner:name<br>column.1.textmode=true<br>column.1.shortview=false<br>column.1.étich=0<br>column.1.valueformat=HTML<br>column.1.sharecol=true<br>column.2.width=1<br>column.2.value=<br><br>column.2.shortview=false<br>column.2.sharecol=true<br>column.2.étich=0<br>column.2.textmode=true<br>column.2.valueformat=HTML<br>column.3.styledef.style=font-color:#ccc;<br>column.3.descriptionkey=description<br>column.3.linkedname=direct<br>column.3.valuefield=description<br>column.3.listsort=string(description)<br>column.3.querysort=description<br>column.3.namekey=description.abbr<br>column.3.textmode=true<br>column.3.sharecol=true<br>column.3.étirement=0<br>column.3.shortview=false<br>column.3.value.format=HTML<br>column.3.width=1<br>column.4.shortview=false<br>column.4.value=<br><br>column.4.sharecol=true<br>column.4.width=1<br>column.4.textmode=true<br>column.4.valueformat=HTML\<br>column.4.étich=0<br>column.5.name=Dates / Durée planifiées<br>column.5.width=150<br>column.5.querysort=scheduledStartDate<br>column.5.sharecol=true<br>column.5.étich=0<br>column.5.textmode=true<br>column.5.shortview=false<br>column.5.linkedname=direct<br>column.5.listsort=atDateAsAtDate(scheduledStartDate)<br>column.5.valuefield=scheduledStartDate<br>column.5.valueformat=atDate<br>column.6.sharecol=true<br>column.6.étich=0<br>column.6.width=1<br>column.6.textmode=true<br>column.6.value=-<br>column.6.valueformat=HTML<br>column.6.shortview=false<br>column.7.namekey=plannedcomplete.abbr<br>column.7.width=1<br>column.7.sharecol=true<br>column.7.shortview=false<br>column.7.étich=0<br>column.7.listsort=atDateAsAtDate(scheduledCompletionDate)<br>column.7.linkedname=direct<br>column.7.descriptionkey=plannedcompletiondate<br>column.7.textmode=true<br>column.7.querysort=scheduledCompletionDate<br>column.7.valueformat=atDate<br>column.7.valuefield=scheduledCompletionDate<br>column.8.value=<br><br>column.8.width=1<br>column.8.textmode=true<br>column.8.sharecol=true<br>column.8.valueformat=HTML<br>column.8.étich=0<br>column.9.textmode=true<br>column.9.listsort=intAsInt(durationMinutes)<br>column.9.étich=0<br>column.9.valuefield=durationFieldLong<br>column.9.descriptionkey=duration<br>column.9.viewalias=duration<br>column.9.querysort=durationMinutes<br>column.9.sharecol=true<br>column.9.width=100<br>column.9.shortview=false<br>column.9.namekey=duration.abbr<br>column.9.linkedname=direct<br>column.9.valueformat=composé<br>column.10.textmode=true<br>column.10.étich=0</pre>

1. Cliquez sur **Enregistrer la vue**.
