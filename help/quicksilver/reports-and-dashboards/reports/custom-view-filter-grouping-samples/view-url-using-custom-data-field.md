---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vue : URL externe utilisant le champ de données personnalisé'
description: Vous pouvez afficher un lien vers une URL personnalisée interne à l’aide d’un champ personnalisé calculé nommé « URL personnalisée » dans une vue de tâche.
author: Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 6a1152bb86a856d60585db7d6ffd43a59a212a72
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 81%

---

# Vue : URL externe utilisant un champ de données personnalisé

<!--Audited: 11/2024-->

Vous pouvez afficher un lien vers une URL personnalisée interne à l’aide d’un **Champ personnalisé calculé** nommé « URL personnalisée » dans une **Vue de tâche**.

Vous pouvez ainsi créer rapidement des liens à partir de certains objets d’une vue vers certaines zones de l’application, directement depuis vos rapports.

Lors de la création d’un champ personnalisé calculé, vous devez d’abord créer le champ, puis créer la Vue.

Les sections suivantes constituent un exemple de champ personnalisé calculé pour les tâches. Le champ personnalisé est appelé URL personnalisée. La vue personnalisée affiche la valeur du champ ainsi que le champ **URL** pour les tâches.

En suivant les mêmes étapes, vous pouvez créer des champs personnalisés et des vues personnalisées calculés similaires pour tous les objets du système qui possèdent un formulaire personnalisé.

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
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p> Actuel : 
   <ul>
   <li>Demander la modification d’un affichage</li> 
   <li>Prévoir de modifier un rapport</li>
   </ul>
     </p>
     <p> Nouveau : 
   <ul>
   <li>Contributeur à la modification d’une vue</li> 
   <li>Standard pour modifier un rapport</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer le champ personnalisé calculé « URL personnalisée »

Pour plus d’informations sur la création d’un champ personnalisé calculé, voir [Ajouter des champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Si vous avez accès à la création d’un formulaire personnalisé, vous pouvez créer un champ personnalisé calculé pour les tâches appelé « URL personnalisée ». Ce champ est directement lié au sous-onglet **Vue d’ensemble** de l’onglet **Détails de la tâche**.

1. Créez un champ personnalisé calculé.
1. Dans le champ Calcul , saisissez le code suivant :

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;)

1. Remplacez « `<domain>` » par votre nom de domaine réel, sans les crochets. La partie `/overview` de cette URL dirige le lien vers la section **Aperçu** dans le panneau de gauche de la tâche.

1. Après avoir créé votre **champ personnalisé calculé**, attachez ce **formulaire personnalisé** avec ce champ à plusieurs tâches dans Adobe Workfront que vous souhaitez afficher dans votre nouvelle vue.

## Créez la vue qui affiche les champs « URL personnalisée » et « URL » de la tâche.

La **Vue** de tâche dans l’exemple ci-dessous, affiche le **Champ personnalisé calculé** appelé « URL personnalisée » en tant que lien direct vers le sous-onglet **Vue d’ensemble** de l’onglet **Détails** de la tâche, ainsi que le champ **URL** de la tâche.

(assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Pour personnaliser cette vue :

1. Accédez à une liste de tâches.
1. Développez le menu déroulant **Vue** en haut de la liste des tâches.
1. Cliquez sur **Personnaliser la vue**.
1. Supprimez toutes les colonnes dans la vue, à l’exception de la première colonne.
1. Cliquez sur l’en-tête de la première colonne.
1. Cliquez sur **Passer en mode Texte** > **Modifier le mode Texte**.
1. Supprimez le texte de la zone **Modifier le mode texte** et remplacez-le par le code suivant :


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat= int
   column.0.link.lookup=link.view
   column.0.link.valuefield= objCode
   column.0.link.valueformat= val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.description=Custom URL
   column.1.link.isnewwindow=true
   column.1.link.url=customDataLabelsAsString(Custom URL)
   column.1.linkedname=direct
   column.1.listsort=customDataLabelsAsString(Custom URL)
   column.1.name=Custom URL
   column.1.querysort=URL
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=Custom URL
   column.1.valueformat=customDataLabelsAsString
   column.1.width=150
   column.2.descriptionkey=url
   column.2.linkedname=direct
   column.2.listsort=string(URL)
   column.2.namekey=url.abbr
   column.2.querysort=URL
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=URL
   column.2.valueformat=HTML
   column.2.width=150
   ```

   Dans cet exemple, la colonne « column.1 ». Les lignes affichent la valeur dans le champ « URL personnalisée » sous la forme d’un lien vers la section **Aperçu** de la tâche ; « colonne.2. » affiche la valeur stockée dans le **champ d’URL** de la tâche.

1. Cliquez sur **Terminé** > **Enregistrer la vue**.
