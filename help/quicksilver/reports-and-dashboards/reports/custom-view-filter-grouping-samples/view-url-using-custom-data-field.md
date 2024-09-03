---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vue : URL externe utilisant un champ de données personnalisé'
description: Vous pouvez afficher un lien vers une URL personnalisée interne à l’aide d’un champ personnalisé calculé nommé « URL personnalisée » dans une vue de tâche.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 97%

---

# Vue : URL externe utilisant un champ de données personnalisé

Vous pouvez afficher un lien vers une URL personnalisée interne à l’aide d’un **Champ personnalisé calculé** nommé « URL personnalisée » dans une **Vue de tâche**.

Vous pouvez ainsi créer rapidement des liens à partir de certains objets d’une vue vers certaines zones de l’application, directement depuis vos rapports.

Lors de la création d’un champ personnalisé calculé, vous devez d’abord créer le champ, puis créer la Vue.

Les sections suivantes constituent un exemple de champ personnalisé calculé pour les tâches. Le champ personnalisé est appelé URL personnalisée. La vue personnalisée affiche la valeur du champ ainsi que le champ **URL** pour les tâches.

En suivant les mêmes étapes, vous pouvez créer des champs personnalisés et des vues personnalisées calculés similaires pour tous les objets du système qui possèdent un formulaire personnalisé.

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
   <td> <p>Demander la modification d’un affichage </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Créer le champ personnalisé calculé « URL personnalisée »

Pour plus d’informations sur la création d’un champ personnalisé calculé, voir [Ajout de champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Si vous avez accès à la création d’un formulaire personnalisé, vous pouvez créer un champ personnalisé calculé pour les tâches appelé « URL personnalisée ». Ce champ est directement lié au sous-onglet **Vue d’ensemble** de l’onglet **Détails de la tâche**.

1. Créez un champ personnalisé calculé.
1. Dans le champ Calcul , saisissez le code suivant :

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;)

1. Remplacer « `<domain>` » par votre nom de domaine réel, sans les crochets.

   Le/la/les

   ```
   /overview
   ```

   partie de cette URL redirige le lien vers la section **Vue d’ensemble** dans le panneau de gauche de la tâche.

1. Après avoir créé votre **champ personnalisé calculé**, attachez ce **formulaire personnalisé** avec ce champ à plusieurs tâches dans Adobe Workfront que vous souhaitez afficher dans votre nouvelle vue.

## Créez la vue qui affiche les champs « URL personnalisée » et « URL » de la tâche.

La **Vue** de tâche dans l’exemple ci-dessous, affiche le **Champ personnalisé calculé** appelé « URL personnalisée » en tant que lien direct vers le sous-onglet **Vue d’ensemble** de l’onglet **Détails** de la tâche, ainsi que le champ **URL** de la tâche.

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Pour personnaliser cette vue :

1. Accédez à une liste de tâches.
1. Développez le menu déroulant **Vue** en haut de la liste des tâches.
1. Cliquez sur **Personnaliser la vue**.
1. Supprimez toutes les colonnes dans la vue, à l’exception de la première colonne.
1. Cliquez sur l’en-tête de la première colonne.
1. Cliquez sur **Passer en mode Texte** dans le coin supérieur droit de l’interface.
1. Cliquez sur **Cliquer pour modifier le texte**.
1. Collez le mode Texte ci-dessous dans votre colonne.\
   Dans cet exemple, la colonne « column.1 ». affiche la valeur du champ « URL personnalisée » sous la forme d’un lien dans la **Vue d’ensemble** de la tâche. « Column.2. » affiche la valeur stockée dans le **champ d’URL** de la tâche.
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Custom URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString(URL personnalisée)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(URL personnalisée)<br>column.1.name=Custom URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=Custom URL<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. Cliquez sur **Enregistrer la vue**.
