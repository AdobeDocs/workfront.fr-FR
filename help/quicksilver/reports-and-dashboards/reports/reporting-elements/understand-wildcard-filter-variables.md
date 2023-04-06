---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Variables de filtre génériques
description: En utilisant des caractères génériques dans des filtres, vous pouvez référencer un utilisateur ou une date générique au lieu d’un utilisateur ou d’une date spécifique. Ainsi, les éléments que vous créez sont dynamiques et les résultats changent en fonction du contexte dans lequel ils sont utilisés.
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 1%

---

# Variables de filtre génériques

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked to the training self-serve promted articles for user-based and date-based widlcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.) </p>
<p>(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.</p>
<p>&gt;&gt;This was included but it is not supported???:</p>
<p>The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.</p>
<p>For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:</p>
<p>AssignedToID Equals $$USER.roleIDs.)</p>
</div>
-->

Adobe Workfront prend en charge les variables de filtre ou les caractères génériques lors de la création des éléments suivants :

* Filtres dans les listes, les rapports et le planificateur de ressources

   Pour plus d’informations sur les filtres Workfront, voir l’article [Présentation des filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Recherches avancées

   Pour plus d’informations sur les recherches avancées, voir la section [Utiliser la recherche avancée](../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search) dans l’article [Rechercher dans Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

* Colonnes calculées dans les vues
* Mise en forme conditionnelle dans les vues

   Pour plus d’informations sur la mise en forme conditionnelle, voir l’article [Utilisation d’une mise en forme conditionnelle dans les vues](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

* Champs personnalisés calculés

   >[!NOTE]
   >
   >Les variables de filtre générique ne sont pas prises en charge lors du référencement de collections imbriquées dans une colonne calculée.

   Pour plus d’informations sur les champs et colonnes personnalisés calculés, consultez l’article [Champs personnalisés calculés par rapport aux colonnes calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

En utilisant des caractères génériques, vous pouvez référencer un utilisateur ou une date générique au lieu d’un utilisateur ou d’une date spécifique. Ainsi, les éléments que vous créez sont dynamiques et les résultats changent en fonction du contexte dans lequel ils sont utilisés.

Par exemple, le filtrage de $$USER.homeGroupID dans un rapport de projet récupère uniquement les projets associés au groupe d’accueil de l’utilisateur connecté.

Vous pouvez utiliser des variables de filtre par date ou par utilisateur dans Workfront.

## Variables de filtre de caractères génériques basées sur des dates

Les options du caractère générique (date-based) de Workfront peuvent être utilisées en combinaison avec n’importe quel attribut de filtre de date.

Pour plus d’informations sur l’ajout d’un caractère générique basé sur les dates à un rapport, reportez-vous à l’article [Utilisation de caractères génériques basés sur des dates pour généraliser des rapports](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Si vous créez un calcul de date et heure qui n’inclut pas de partie horaire ou qui utilise les caractères génériques $$TODAY ou $$NOW, le système utilise la date selon le fuseau horaire universel coordonné (UTC), et non selon votre fuseau horaire local. Cela peut entraîner un résultat de date inattendu.

Choisissez l’un des caractères génériques suivants basés sur la date :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$AUJOURD’HUI</strong> </p> </td> 
   <td> <p>Nous vous recommandons de créer des filtres sensibles à la date à l’aide de ce caractère générique afin d’éviter de les recréer demain, semaine prochaine ou mois prochain.</p> <p>Par exemple, si vous souhaitez afficher toutes les tâches qui doivent être effectuées avant aujourd’hui, vous pouvez utiliser la règle suivante dans un filtre de tâche : <em>Date de début planifiée inférieure à $$AUJOURD’HUI</em>.</p> <p>$$TODAY est toujours égal à minuit pour le jour en cours.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>Cette opération est similaire au caractère générique $$AUJOURD’HUI , mais inclut la date et l’heure actuelles. $$NOW est égal à la date et l’heure actuelles.</p> <p>Par exemple, si vous souhaitez afficher toutes les entrées d’heure fournies jusqu’à l’heure actuelle, vous pouvez le faire en utilisant la règle suivante dans un filtre d’heure : <em>Date de début planifiée inférieure à $$MAINTENANT</em>.</p> <p>Remarque : Ce caractère générique n’est pas pris en charge dans le planificateur de ressources.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour indiquer différentes périodes et différents points dans le temps (futur ou passé), vous pouvez combiner des caractères génériques avec les éléments suivants :

| Attributs |   |
|---|---|
| **q** | trimestre calendaire |
| **h** | heure |
| **d** | jour |
| **w** | semaine |
| **m** | mois |
| **y** | an |

{style="table-layout:auto"}

| **Qualificateurs** |  |
|---|---|
| **b** | début de la semaine (dimanche) |
| **e** | fin de la semaine (samedi) |

{style="table-layout:auto"}

| **Opérateurs** |  |
|---|---|
| **+** | ajouter une valeur à une valeur de caractère générique |
| **-** | soustraire la valeur de la valeur d’un caractère générique |

{style="table-layout:auto"}

Par exemple, le caractère générique `$$TODAYb+2w` fait référence à &quot;2 semaines à partir du début de la semaine&quot;. Caractère générique *`$$NOW+2h` fait référence à &quot;dans 2 heures&quot;.

## Variables de filtre de caractères génériques basées sur l’utilisateur

>[!IMPORTANT]
>
>Si un filtre ou un rapport contient une variable de filtre générique basée sur un utilisateur, les résultats affichent toujours les informations filtrées par l’utilisateur actuellement connecté. Lorsque vous partagez un tel filtre ou rapport avec un autre utilisateur, le caractère générique récupère les informations destinées à l’utilisateur qui consulte le rapport. Les deux utilisateurs voient des résultats différents.

Pour plus d’informations sur l’ajout d’un caractère générique basé sur l’utilisateur à un rapport, reportez-vous à l’article [Utilisation de caractères génériques basés sur l’utilisateur pour généraliser des rapports](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Workfront fournit les variables basées sur les utilisateurs suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>La variable basée sur l’utilisateur la plus courante est $$USER.ID. Cela renvoie toujours l’identifiant de l’utilisateur connecté. Il s’agit de l’identifiant utilisé pour identifier l’utilisateur qui a créé chaque objet et ses affectations de travail.</p> <p>Lorsqu’il est utilisé dans des rapports, ce caractère générique réduit le nombre de rapports que vous devez créer dans votre système. Vous pouvez créer un rapport et le partager avec plusieurs utilisateurs. Les résultats changent en fonction de l’utilisateur connecté qui consulte le rapport.</p> <p>Par exemple, pour créer un rapport pour tous les problèmes affectés à l’utilisateur connecté, vous pouvez utiliser la règle suivante dans un filtre de problèmes : <em>Attribué À L’ID Égal À $$USER.ID</em>.</p> <p>Workfront utilise cette variable dans les filtres intégrés suivants :</p> 
    <ul> 
     <li>Mes rapports</li> 
     <li>Mes projets</li> 
     <li>Mes tâches</li> 
     <li>Mes événements</li> 
     <li>Mes heures</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>La variable $$USER.categoryID fait référence à un formulaire personnalisé spécifique associé à l’utilisateur connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>La variable $$USER.accessLevelID fait référence à l’identifiant du niveau d’accès associé à l’utilisateur connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>La variable $$USER.accessLevelRank fait référence au rang de niveau d’accès associé à l’utilisateur connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>La variable $$USER.companyID fait référence à la société associée à l’utilisateur connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>La variable $$USER.customerID fait référence à l’ID du compte client associé à votre environnement. Pour votre environnement, il n’existe qu’une seule valeur possible pour cette variable. Elle est généralement utilisée uniquement lors de la création d’intégrations via l’API.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>La variable $$USER.firstName fait référence au prénom de l’utilisateur connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>La variable $$USER.lastName fait référence au nom de l’utilisateur connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>La variable $$USER.name fait référence au nom complet de l’utilisateur connecté.</p> <p>Note:   <p>Cette variable de caractère générique ne fonctionne que lors de la modification d’un filtre en mode texte. Vous ne pouvez pas utiliser ce caractère générique dans les filtres qui ne prennent pas en charge le mode texte. Par exemple, vous ne pouvez pas utiliser ce caractère générique dans les filtres des zones suivantes :</p> 
     <ul> 
      <li> <p>Planificateur de ressources</p> </li> 
      <li> <p>Équilibreur de charge de travail</p> </li> 
      <li> <p>Analytique</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>La variable $$USER.homeGroupID fait référence à l’ID du groupe d’accueil de l’utilisateur connecté. En tant qu’administrateur de groupe, vous pouvez utiliser cette variable pour filtrer uniquement les éléments qui appartiennent aux utilisateurs de votre groupe d’accueil.</p> <p>Par exemple, pour voir toutes les tâches incomplètes sur les projets du groupe des finances, utilisez les règles de filtrage suivantes dans un filtre de tâche :<br><em>Projet : ID de groupe = $$USER.homeGroupID </em><br><em>Pourcentage Terminé inférieur à 100</em></p> <p>Pour afficher toutes les tâches incomplètes affectées à des individus dans un groupe spécifique qui est le Groupe d’accueil de l’utilisateur connecté, utilisez les règles de filtrage suivantes dans un filtre de tâche :</p> <p><em>Affecté à : ID de groupe = $$USER.homeGroupID<br>Pourcentage Terminé inférieur à 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>La variable $$USER.otherGroupIDs fait référence à tous les groupes (y compris le groupe d’accueil) associés au profil de l’utilisateur connecté.</p> <p>La fonctionnalité de cette variable est similaire à celle de la variable $$USER.homeGroupID , sauf que les résultats affichent des informations sur les utilisateurs appartenant à l’un des groupes associés à l’utilisateur connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>La variable $$USER.homeTeamID fait référence à l’identifiant de l’équipe d’accueil de l’utilisateur connecté. En tant que chef d’équipe, vous pouvez utiliser cette variable pour filtrer uniquement les éléments qui appartiennent aux utilisateurs de votre équipe d’accueil.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.TeamIDs</strong> </p> </td> 
   <td> <p>La variable $$USER.TeamIDs renvoie une liste de toutes les équipes associées à l’utilisateur connecté.</p> <p>La fonctionnalité de cette variable est similaire à celle de la variable $$USER.homeTeamID , sauf que les résultats affichent des informations sur l’utilisateur qui appartient à l’une des équipes identifiées dans le filtre.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>La variable $$USER.roleID fait référence au rôle Principal de l’utilisateur connecté. Grâce à cette variable, vous pouvez créer des rapports sur les tâches ou les problèmes affectés à un rôle de tâche spécifique.</p> <p>Par exemple, pour voir toutes les tâches affectées au rôle Principal de l’utilisateur connecté, vous pouvez utiliser la règle de filtrage suivante dans un filtre de tâche :</p> <p><em>Tâche : L’ID de rôle est égal à $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader">$$USER.roleIDs</td> 
   <td> <p>La variable $$USER.roleIDs fait référence à tous les rôles de tâche associés à l’utilisateur connecté. Grâce à cette variable, vous pouvez créer des rapports sur les tâches ou les problèmes affectés à l’un des rôles de tâche associés à l’utilisateur connecté. </p> <p>Par exemple, pour voir toutes les tâches affectées à l’un des rôles associés à l’utilisateur connecté, vous pouvez utiliser la règle de filtrage suivante dans un filtre de tâche :</p> <p><i>Tâche : ID de rôle = $$USERID.roleID<br></i> </p> <p>Conseil : Le <i>Tâche : ID de rôle = $$USERID.roleID</i> la règle de filtre existe dans les filtres intégrés Tâches non assignées dans mon rôle et Problèmes non attribués dans mon rôle. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Variables de filtre génériques basées sur des objets

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>La variable $$OBJCODE fait référence au type d’un objet. </p> 
     <p>Dans un formulaire personnalisé, lorsque les types d’objets sélectionnés du formulaire sont incompatibles avec un champ référencé dans un champ personnalisé calculé, vous pouvez utiliser ce caractère générique pour éviter la solution de création de formulaires en double pour ces types d’objets.</p> 
     <p>Dans le champ personnalisé calculé, vous devez inclure la carte de remplacement dans une expression IF afin que le calcul puisse générer des valeurs différentes pour chacun des types d’objets de votre formulaire. </p> 
     <p>Pour plus d’informations et un exemple, reportez-vous à la section <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">Champs personnalisés calculés dans des formulaires personnalisés à plusieurs objets</a> dans l’article <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Ajout de données calculées à un formulaire personnalisé</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
