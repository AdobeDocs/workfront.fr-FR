---
product-area: reporting
navigation-topic: text-mode-reporting
title: Référencer des collections dans un rapport
description: Référencer des collections dans un rapport
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '2598'
ht-degree: 4%

---

# Référencer des collections dans un rapport

La création d&#39;un rapport dans Adobe Workfront permet d&#39;afficher un ensemble d&#39;objets, leurs champs respectifs ou les objets liés sous la forme d&#39;une liste, d&#39;une grille ou d&#39;un graphique.

Pour plus d’informations sur la création d’un rapport dans Workfront, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Gestion des autorisations d’un affichage, d’un filtre ou d’un regroupement </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

+++

## Présentation des collections

Une collection est une liste d’objets liés à un autre objet.

Vous avez les deux relations suivantes entre les objets dans Workfront :

* **Une relation un-à-un** : un objet ne peut être lié qu’à un seul autre objet à la fois.\
  Par exemple, un projet ne peut être lié qu’à un portefeuille à la fois.

* **Une relation un-à-multiple** : un objet peut être lié à plusieurs autres objets à la fois.\
  Par exemple, un projet peut comporter plusieurs tâches. Dans ce cas, la liste des tâches forme une collection pour le projet.

>[!IMPORTANT]
>
>Vous pouvez créer un rapport montrant la relation un-à-un entre les objets à l’aide du créateur de rapports standard. Cependant, vous pouvez uniquement créer un rapport montrant la relation un-à-plusieurs entre les objets à l’aide de l’interface du mode texte du créateur de rapports.

Pour plus d’informations sur la création d’un rapport dans le créateur de rapports standard, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour plus d’informations sur la création d’un rapport à l’aide de l’interface du mode texte, voir :

* [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Présentation des utilisations courantes du mode Texte](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Vue d’ensemble de la syntaxe du mode texte](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Recherche d’objets de collection et de leurs champs dans l’explorateur d’API {#find-collection-objects-and-their-fields-in-the-api-explorer}

Toutes les collections ne peuvent pas faire l’objet de rapports.

Pour comprendre les objets qui peuvent être associés à une collection d’autres objets, vous devez utiliser l’explorateur d’API.\
Pour plus d’informations sur la table de l’explorateur d’API, voir l’ [ explorateur d’API](../../../wf-api/general/api-explorer.md).

Pour savoir sur quelles collections peuvent faire l’objet de rapports :

1. Accédez à l’ [API Explorer](../../../wf-api/general/api-explorer.md).
1. Recherchez l’objet de votre rapport.
1. Sélectionnez l’onglet **collections** .

   >[!NOTE]
   >
   >Seuls les objets répertoriés dans cet onglet peuvent être représentés en tant que collection dans un rapport pour l’objet que vous avez sélectionné.

1. Développez l’objet de votre collection en cliquant dessus.
1. Cliquez sur le lien affiché pour accéder à l’objet de votre collection.\
   Cela ouvre l’onglet **fields** pour l’objet de votre collection.

   >[!NOTE]
   >
   >Seuls les champs répertoriés dans cet onglet peuvent être référencés dans le rapport de collection, ou les champs associés aux objets répertoriés dans cet onglet.

## Collections de référence dans les rapports

Vous pouvez référencer des objets d’une collection dans les éléments de rapport suivants :

* Vues
* Filtres
* Invites

Vous ne pouvez pas référencer des objets d’une collection dans les éléments de rapport suivants :

* Regroupements
* Graphique

Par exemple, vous pouvez référencer la tâche ou publier des collections à partir d’un rapport de projet pour afficher des informations sur la tâche ou la publication au niveau du projet.

* [Référencer une collection dans l’affichage d’un rapport](#reference-a-collection-in-the-view-of-a-report)
* [Référencer une collection dans le filtre d’un rapport](#reference-a-collection-in-the-filter-of-a-report)
* [Référencer une collection dans l’invite personnalisée d’un rapport](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Référencer une collection dans l’affichage d’un rapport {#reference-a-collection-in-the-view-of-a-report}

Vous pouvez référencer une collection d’objets dans la vue d’un rapport pour afficher les attributs des objets associés à l’objet du rapport.

Vous pouvez, par exemple, afficher les informations sur une tâche ou un problème dans un rapport de projet en créant une colonne de collection pour les tâches ou les problèmes dans l’affichage du rapport.

Vous pouvez afficher des informations sur les tâches ou les problèmes, tels que les noms, les dates, les personnes désignées principales, le pourcentage d’achèvement, etc. dans la vue Collection.

L’affichage affiche les informations sur les tâches ou les problèmes sous la forme d’une liste, chaque ligne de la liste représentant des informations sur une tâche ou un problème. La liste des tâches ou des problèmes et de leurs champs s’affiche sur la même ligne que le projet auquel appartiennent les tâches ou les problèmes.\
![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [Ajouter une colonne de collection dans une vue de rapport](#add-a-collection-column-in-a-report-view)
* [Comprendre les lignes d’une vue de collection en mode texte](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Limites de la vue d’une collection](#limitations-of-a-collection-view)

### Ajout d’une colonne de collection dans une vue de rapport {#add-a-collection-column-in-a-report-view}

Pour ajouter une colonne de collection dans une vue de rapport :

1. Cliquez sur le menu **Main** ![](assets/main-menu-icon.png), puis sur **Rapports**.
1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez l’objet de votre rapport.
1. Quittez votre rapport et, à l’aide de l’[API Explorer](../../../wf-api/general/api-explorer.md), déterminez les collections disponibles pour l’objet que vous avez sélectionné pour votre rapport.

   Pour plus d’informations sur la sélection de l’objet de votre collection, reportez-vous à la section [Rechercher des objets de collection et leurs champs dans l’API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) de cet article.\
   Notez le nom de l’objet de la collection.

1. À l’aide de l’[ API Explorer](../../../wf-api/general/api-explorer.md), accédez à la liste des champs de l’objet que vous souhaitez afficher dans la collection.

   Pour plus d’informations sur la recherche des champs de l’objet de votre collection, reportez-vous à la section [Rechercher des objets de collection et leurs champs dans l’API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) de cet article.

   Notez le nom du champ que vous souhaitez afficher dans la collection.

1. Revenez à votre rapport et, dans l’onglet **Colonnes (vues)**, cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Passer en mode Texte**.
1. Pointez sur la boîte de dialogue, puis cliquez sur **Cliquez pour modifier le texte**.
1. Sélectionnez tout le texte dans la boîte de dialogue **Text Mode** et supprimez-le, puis collez le code suivant si vous référencez un champ de l’objet de collection :

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. Remplacez **Column Name** par le nom de votre colonne dans la ligne `displayname`.
1. Remplacez **nom de l’objet de collection** par le nom de votre objet de collection dans la ligne `listmethod`, tel qu’il apparaît dans l’ [API Explorer](../../../wf-api/general/api-explorer.md).

1. Remplacez **champ d’objet de collection** par le nom du champ de votre objet de collection dans la ligne `valuefield`, tel qu’il apparaît dans l’ [API Explorer](../../../wf-api/general/api-explorer.md).

   Vous pouvez remplacer **valuefield** par **valueexpression** si vous souhaitez créer une expression personnalisée dans votre vue.

   Pour plus d’informations sur les expressions personnalisées calculées, voir [Présentation des expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Par exemple, si vous souhaitez afficher une liste des tâches dans un rapport de projet. Cette collection utilise une ligne `valuefield` pour référencer les noms des tâches.

   Utilisez l’une des méthodes suivantes :

   * Utilisez le code suivant pour créer votre colonne :

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Project Tasks Names
     listmethod=nested(tasks).lists
     valuefield=name
     ```

   * Utilisez le code suivant pour afficher la liste des problèmes du rapport :

     ```
     displayname=Project Issues Names
     listdelimiter=<p>
     listmethod=nested(issues).lists
     textmode=true
     type=iterate
     valuefield=name
     valueformat=HTML
     ```

     Notez que dans une collection, vous devez utiliser **issues** pour la ligne **listmethod**, au lieu de **opTasks** qui est le nom de base de données pour les problèmes. Pour plus d’informations sur le moment où utiliser **issue** et le moment où utiliser **opTask** en cas de problèmes, voir [Utiliser &quot;opTask&quot; et &quot;issue&quot; en cas de problèmes](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Si vous souhaitez afficher une liste des tâches dans un rapport de projet avec leur responsable principal, vous utiliserez une ligne **valueexpression** pour référencer les noms des tâches adjacentes aux noms de leurs principaux responsables au lieu de **valuefield**.

     Utilisez le code suivant pour créer votre colonne :

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Tasks Names - Primary Assignee
     listmethod=nested(tasks).lists
     valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
     ```

1. La colonne suivante s’affiche dans le rapport de projet, répertoriant toutes les tâches de chaque projet avec leurs principaux responsables :

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png)

1. Cliquer sur **Enregistrer**.
1. (Facultatif) Poursuivez la modification du rapport.

   Ou

   Cliquez sur **Enregistrer + Fermer** pour enregistrer le rapport.

#### Présentation des lignes d’une vue de collection en mode Texte

Les lignes d’une collection en mode texte sont décrites dans le tableau suivant :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Exemple de ligne</strong> </th> 
   <th><strong>Description</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>Vous pouvez utiliser différentes valeurs pour cette ligne, mais nous recommandons que le <code style="font-weight: normal;">valueformat</code> pour une liste de collections soit <strong>HTML.</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>Cette ligne indique que la colonne a été paramétrée en mode texte. Si vous supprimez cette ligne, Workfront la réajoute par défaut.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>Le <code>type</code> d'une liste est toujours <code>iterate</code>, lors de la création d'une vue.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>Il s’agit du délimiteur utilisé pour séparer les valeurs de votre liste.<br>Nous vous recommandons d’utiliser <code>&lt;p&gt;</code> qui ajoute un saut de ligne entre les valeurs.</p> <p>Vous pouvez également utiliser les éléments suivants :</p> <p><code>&amp;zwj;</code> (jointure à largeur nulle). Les valeurs de la collection ne sont pas séparées entre elles.<br><strong>,</strong> =séparateur virgule. Les valeurs de la collection sont séparées par une virgule suivie d’un espace vide.<br><strong>/</strong> = séparateur de barre oblique. Les valeurs de la collection sont séparées par une barre oblique.<br><strong>-</strong> = séparateur de tiret. Les valeurs de la collection sont séparées par un tiret.<br> Si vous laissez cette ligne vide, une virgule est ajoutée, suivie par un espace entre les valeurs de la collection, par défaut.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Nom de colonne</em> </td> 
   <td> <p>Remplacez <strong>Nom de colonne</strong> par le nom réel de votre nouvelle colonne.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Cette ligne définit la collection à laquelle vous faites référence.</p> <p>Remplacez <strong>nom de l’objet de collection</strong> par le nom de l’objet que vous référencez dans votre collection, tel qu’il apparaît dans l’ <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. Cette valeur correspond généralement à la forme plurielle du nom de l’objet de collection.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Cette ligne définit le champ que vous référencez à partir de l’objet de collection.</p> <p>Remplacez <strong>champ d’objet de collection</strong> par le nom du champ de l’objet que vous référencez dans votre collection, tel qu’il apparaît dans l’ <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>Vous pouvez remplacer cette ligne par :</p> <p><strong>valeur expression</strong>=champ/champs d’objet de collection calculé</p> <p>En utilisant <strong>valueexpression</strong>, vous pouvez  afficher une expression personnalisée calculée dans la colonne.</p> <p>Pour plus d’informations sur la façon de formater les lignes <strong>value expression</strong>, voir <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Présentation de la syntaxe du mode texte</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Limites de la vue d’une collection {#limitations-of-a-collection-view}

Tenez compte des restrictions suivantes lorsque vous créez une vue de collection :

* Vous ne pouvez pas contrôler l’ordre d’affichage des données de collection.
* Vous ne pouvez pas appliquer de mise en forme conditionnelle à une vue de collection.
* Vous ne pouvez pas faire d’un objet d’une collection un lien cliquable.
* Vous ne pouvez pas créer une vue de collection d’une autre collection.\
  Par exemple, vous ne pouvez pas afficher tous les personnes désignées pour chaque tâche dans un rapport de projet. Vous ne pouvez afficher que la personne désignée principale pour chaque tâche dans une vue de projet.

### Référencer une collection dans le filtre d’un rapport {#reference-a-collection-in-the-filter-of-a-report}

Vous pouvez référencer une collection d’objets dans le filtre d’un rapport afin de filtrer les attributs des objets associés à l’objet du rapport.

Vous pouvez, par exemple, filtrer les informations de tâche ou de problème dans un rapport de projet en utilisant une référence aux attributs des tâches ou des problèmes du projet dans l’instruction de filtre.

Pour ajouter une référence à une collection dans un filtre de rapport :

1. Cliquez sur le menu **Main** ![](assets/main-menu-icon.png), puis sur **Rapports**.
1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez l’objet de votre rapport.
1. Quittez votre rapport et, à l’aide de l’[API Explorer](../../../wf-api/general/api-explorer.md), déterminez les collections disponibles pour l’objet que vous avez sélectionné pour votre rapport.

   Pour plus d’informations sur la sélection de l’objet de votre collection, reportez-vous à la section [Rechercher des objets de collection et leurs champs dans l’API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) de cet article.

   Notez le nom de l’objet de la collection.

1. À l’aide de l’[ API Explorer](../../../wf-api/general/api-explorer.md), accédez à la liste des champs de l’objet que vous souhaitez afficher dans la collection.

   Pour plus d’informations sur la recherche des champs de l’objet de votre collection, reportez-vous à la section [Rechercher des objets de collection et leurs champs dans l’API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) de cet article.

   Notez le champ que vous souhaitez afficher dans la collection.

1. Revenez à votre rapport et, dans l’onglet **Filtres**, cliquez sur **Passer en mode texte**.

1. Dans la zone **Définir des règles de filtrage pour votre rapport**, collez le code suivant :

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Remplacez **nom de l’objet de collection** par le nom de votre objet de collection tel qu’il apparaît dans l’ [explorateur d’API](../../../wf-api/general/api-explorer.md). Cette valeur correspond généralement à la forme plurielle du nom de l’objet de collection.

1. Remplacez **champ d’objet de collection** par le nom du champ de votre objet de collection dans, tel qu’il apparaît dans l’[ Explorateur API](../../../wf-api/general/api-explorer.md).

1. Remplacez **la valeur de l’objet de collection** par la valeur de l’objet de collection tel qu’il apparaît dans Workfront.
1. Remplacez la valeur **du modificateur** par un modificateur valide.

   Pour obtenir une liste des modificateurs, voir [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   Par exemple, pour créer un rapport de projet qui affiche uniquement les projets dont le nom contient &quot;Marketing&quot;, utilisez le code suivant :

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   Ce rapport affiche uniquement les projets dont le nom contient au moins une tâche portant le mot &quot;marketing&quot;.

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png)

1. Pour filtrer le nom d’un problème, utilisez le code suivant :

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >Notez que vous devez utiliser `issues` pour le nom de l’objet de collection, au lieu de `optask`, qui est la manière dont les problèmes apparaissent dans l’explorateur d’API.

1. Cliquez sur **Terminé**.
1. (Facultatif) Poursuivez la modification du rapport.

   Ou

   Cliquez sur **Enregistrer + Fermer** pour enregistrer le rapport.

### Référencer une collection dans l’invite personnalisée d’un rapport {#reference-a-collection-in-the-custom-prompt-of-a-report}

Vous pouvez référencer une collection d’objets dans l’invite personnalisée d’un rapport afin de filtrer les résultats du rapport en fonction des attributs des objets associés à l’objet du rapport.

Par exemple, vous pouvez demander des informations sur la tâche dans un rapport de projet en utilisant une référence aux attributs des tâches du projet dans l’invite personnalisée du rapport.

>[!NOTE]
>
>Vous ne pouvez pas référencer des collections dans une invite standard.

Une invite personnalisée est un filtre personnalisé où les instructions sont jointes par des symboles d’esperluette. Nous vous recommandons de créer votre instruction dans un filtre, d’abord, puis de joindre les lignes des instructions avec des esperluettes.

Pour plus d’informations sur la création d’une instruction de filtre avec une référence de collection, reportez-vous à la section [Référence d’une collection dans le filtre d’un rapport](#reference-a-collection-in-the-filter-of-a-report) de cet article.

Pour ajouter une référence à une collection dans l’invite personnalisée d’un rapport :

1. Cliquez sur le menu **Main** ![](assets/main-menu-icon.png), puis sur **Rapports**.
1. Cliquez sur **Nouveau rapport**.
1. Sélectionnez l’objet de votre rapport.
1. Créez un filtre avec une référence de collection comme décrit dans la section [Référencer une collection dans le filtre d&#39;un rapport](#reference-a-collection-in-the-filter-of-a-report) de cet article.
1. Cliquez sur **Paramètres de rapport**.
1. Cliquez sur **Report Prompts**.
1. Cliquez sur **Ajouter une invite**.
1. Cliquez sur **Invite personnalisée**.
1. Indiquez le nom de l’invite dans le champ **Field****name**.

1. Spécifiez un **libellé d’élément de liste déroulante**.
1. Spécifiez les éléments suivants dans le champ **Condition** :

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Facultatif) Indiquez si ce choix est affiché par défaut dans l’invite.
1. Remplacez **nom de l’objet de collection** par le nom de votre objet de collection tel qu’il apparaît dans l’ [explorateur d’API](../../../wf-api/general/api-explorer.md). Cette valeur correspond généralement à la forme plurielle du nom de l’objet de collection.
1. Remplacez **champ d’objet de collection** par le nom du champ de votre objet de collection, tel qu’il apparaît dans l’[ Explorateur d’API](../../../wf-api/general/api-explorer.md).
1. Remplacez **la valeur de l’objet de collection** par la valeur de l’objet de collection tel qu’il apparaît dans Workfront.

   Par exemple, si vous filtrez les projets dont le nom de la tâche contient &quot;Marketing&quot;, remplacez **valeur d’objet de collection** par **marketing**.

1. Remplacez la valeur **du modificateur** par un modificateur valide.

   Pour obtenir la liste des modificateurs, voir  [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Exemple :** Par exemple, pour créer un rapport de projet avec une invite personnalisée dans laquelle vous souhaitez afficher uniquement les projets pour lesquels au moins une tâche est affectée à un utilisateur spécifique, utilisez le code ci-dessous :

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Cela génère un rapport dans lequel tous les projets répertoriés comportent au moins une tâche affectée à l’utilisateur dont le GUID est 57cf1b7a000077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   >Vous ne pouvez pas référencer le nom de la personne désignée principale (champ &quot;Affectée à&quot;) d’une tâche, selon l’ [API Explorer](../../../wf-api/general/api-explorer.md). Vous ne pouvez référencer que l’ID de la personne désignée principale.

   Par exemple, pour filtrer les projets pour lesquels l’un des problèmes de projet est assigné à un utilisateur spécifique, utilisez le code suivant pour votre invite personnalisée :

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Cela génère un rapport dans lequel tous les projets répertoriés comportent au moins un problème assigné à l’utilisateur dont le GUID est 57cf1b7a000077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   >Notez que vous devez utiliser **issues** pour le nom de l’objet de collection. L’explorateur API  ne propose pas de nom d’objet de collection pour les problèmes en ce moment.

1. Cliquez sur **Terminé**.
1. (Facultatif) Poursuivez la modification du rapport.

   Ou

   Cliquez sur **Enregistrer + Fermer** pour enregistrer le rapport.
