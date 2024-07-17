---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Variables de filtrage des caractères génériques
description: En utilisant des caractères génériques dans des filtres, vous pouvez référencer une personne ou une date générique au lieu d’une personne ou d’une date spécifique. Ainsi, les éléments que vous créez sont dynamiques et les résultats changent en fonction du contexte dans lequel ils sont utilisés.
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: d6094d944b7955db8a97b5e1ce0af8cb85f82a9e
workflow-type: tm+mt
source-wordcount: '1466'
ht-degree: 100%

---

# Vue d’ensemble des variables de filtrage des caractères génériques

<!-- Audited: 12/2023 -->

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

Les caractères génériques vous permettent de référencer une personne ou une date générique au lieu d’une personne ou d’une date spécifique. Ainsi, les éléments que vous créez sont dynamiques. Les résultats changent en fonction du contexte dans lequel ils sont utilisés.

Par exemple, le filtrage de $$USER.homeGroupID dans un rapport de projet récupère uniquement les projets associés au groupe principal de la personne connectée.

Vous pouvez utiliser des variables de filtre, également appelées caractères génériques, lors de la création des éléments suivants :

<table>
    <tr>
        <td>Filtres dans les listes, les rapports et le planificateur de ressources</td>
        <td>Pour en savoir plus sur les filtres Workfront, voir l’article <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">Vue d’ensemble des filtres</a>.
</td>
    </tr>
    <tr>
        <td>Recherches avancées</td>
        <td>Pour en savoir plus sur les recherches avancées, voir la section <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">Utiliser la recherche avancée</a> dans l’article <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">Rechercher dans Adobe Workfront</a>.
    </tr>
    <tr>
        <td>Colonnes calculées dans les vues</td>
        <td></td>
    </tr>
    <tr>
        <td>Mise en forme conditionnelle dans les vues</td>
        <td>Pour plus d’informations sur la mise en forme conditionnelle, voir l’article <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">Utiliser une mise en forme conditionnelle dans les vues</a>.
    </tr>
    <tr>
        <td>Champs personnalisés calculés</td>
        <td>Les variables de filtre de caractères génériques ne sont pas prises en charge lors du référencement de collections imbriquées dans une colonne calculée.

Pour en savoir plus sur les champs et colonnes personnalisés calculés, consultez l’article <a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">Champs personnalisés calculés et colonnes calculées</a>.
</td>
    </tr>
</table>

## Variables de filtre de caractères génériques basées sur des dates

Les options de caractères génériques basés sur des dates peuvent être utilisées en combinaison avec n’importe quel attribut de filtre de date. Pour en savoir plus sur l’ajout d’un caractère générique basé sur des dates à un rapport, consultez l’article [Utiliser des caractères génériques basés sur des dates pour généraliser des rapports](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Si vous créez un calcul de date et heure qui n’inclut pas de partie « heure » ou qui utilise les caractères génériques $$TODAY ou $$NOW, le système utilise la date selon le temps universel coordonné (UTC), et non selon votre fuseau horaire local. Cela peut entraîner un résultat de date inattendu.

Vous pouvez choisir parmi les caractères génériques suivants basés des dates :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>Nous vous recommandons de créer des filtres sensibles à la date à l’aide de ce caractère générique afin d’éviter de les recréer le jour suivant, la semaine prochaine ou le mois prochain.</p> <p>Par exemple, si vous souhaitez afficher toutes les tâches qui doivent être effectuées avant aujourd’hui, vous pouvez utiliser la règle suivante dans un filtre de tâche : <em>Date de début prévue inférieure à $$TODAY</em>.</p> <p>$$TODAY correspond toujours à minuit pour le jour en cours.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>Ce caractère générique est similaire à $$TODAY, mais inclut la date et l’heure actuelles. $$NOW correspond à la date et l’heure actuelles.</p> <p>Par exemple, si vous souhaitez afficher toutes les entrées d’heure fournies jusqu’à l’heure actuelle, vous pouvez le faire en utilisant la règle suivante dans un filtre d’heure : <em>Date de début prévue inférieure à $$NOW</em>.</p> <p>Remarque : ce caractère générique n’est pas pris en charge dans le planificateur de ressources.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour indiquer différentes périodes et différents moments donnés (futurs ou passés), vous pouvez combiner les caractères génériques ci-dessus avec les éléments suivants :

| Attributs |   |
|---|---|
| **q** | trimestre calendaire |
| **h** | heure |
| **d** | jour |
| **w** | semaine |
| **m** | mois |
| **y** | an |

{style="table-layout:auto"}

| **Qualificateurs** | |
|---|---|
| **b** | début de la période (sans attribut spécifié, début de la semaine par défaut : dimanche) |
| **e** | fin de la période (sans attribut spécifié, fin de la semaine par défaut : samedi) |

{style="table-layout:auto"}

| **Opérateurs** | |
|---|---|
| **+** | ajouter une valeur à une valeur de caractère générique |
| **-** | soustraire une valeur de la valeur de caractère générique |

{style="table-layout:auto"}

Par exemple, le caractère générique `$$TODAYb+2w` fait référence à « 2 semaines à partir du début de cette semaine ». Le caractère générique *`$$NOW+2h` fait référence à « 2 heures à partir de maintenant ».

## Variables de filtre de caractères génériques basées sur l’utilisateur ou l’utilisatrice

>[!IMPORTANT]
>
>Si un filtre ou un rapport contient une variable de filtre de caractères génériques basée sur l’utilisateur ou l’utilisatrice, les résultats affichent toujours les informations filtrées par l’utilisateur ou l’utilisatrice actuellement connecté. Lorsque vous partagez un tel filtre ou rapport avec un autre utilisateur ou une autre utilisatrice, le caractère générique récupère les informations destinées à l’utilisateur ou l’utilisatrice qui consulte le rapport. Les deux utilisateurs et utilisatrices voient des résultats différents.
>
>Pour plus d’informations sur l’ajout d’un caractère générique basé sur l’utilisateur ou l’utilisatrice à un rapport, voir l’article [Utiliser des caractères génériques basés sur l’utilisateur ou l’utilisatrice pour généraliser les rapports](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Vous pouvez choisir parmi les variables basées sur l’utilisateur ou l’utilisatrice suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>La variable basée sur l’utilisateur ou l’utilisatrice la plus courante est $$USER.ID. Elle renvoie toujours l’ID de l’utilisateur ou l’utilisatrice connecté. Il s’agit de l’ID utilisé pour identifier l’utilisateur ou l’utilisatrice qui a créé chaque objet et ses affectations de travail.</p> <p>Lorsqu’il est utilisé dans des rapports, ce caractère générique réduit le nombre de rapports que vous devez créer dans votre système. Vous pouvez créer un rapport et le partager avec plusieurs utilisateurs et utilisatrices. Les résultats changent en fonction de l’utilisateur ou l’utilisatrice connecté qui consulte le rapport.</p> <p>Par exemple, pour créer un rapport pour tous les problèmes affectés à l’utilisateur ou l’utilisatrice connecté, vous pouvez utiliser la règle suivante dans un filtre de problèmes : <em>Affecté à l’ID égal à $$USER.ID</em>.</p> <p>Workfront utilise cette variable dans les filtres intégrés suivants :</p> 
    <ul> 
     <li>Mes rapports</li> 
     <li>Mes projets</li> 
     <li>Mes tâches</li> 
     <li>Mes problèmes</li> 
     <li>Mes heures</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>La variable $$USER.categoryID fait référence à un formulaire personnalisé spécifique associé à l’utilisateur ou l’utilisatrice connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>La variable $$USER.accessLevelID fait référence à l’ID du niveau d’accès associé à l’utilisateur ou l’utilisatrice connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>La variable $$USER.accessLevelRank fait référence au rang de niveau d’accès associé à l’utilisateur ou l’utilisatrice connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>La variable $$USER.companyID fait référence à l’entreprise associée à l’utilisateur ou l’utilisatrice connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>La variable $$USER.customerID fait référence à l’ID du compte cliente ou client associé à votre environnement. Pour votre environnement, il n’existe qu’une seule valeur possible pour cette variable. Elle n’est généralement utilisée que lors de la création d’intégrations via l’API.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>La variable $$USER.firstName fait référence au prénom de l’utilisateur ou l’utilisatrice connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>La variable $$USER.lastName fait référence au nom de l’utilisateur ou l’utilisatrice connecté.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>La variable $$USER.name fait référence au nom complet de l’utilisateur ou l’utilisatrice connecté.</p> <p>Remarque :   <p>Cette variable de caractère générique ne fonctionne que lors de la modification d’un filtre en mode texte. Vous ne pouvez pas utiliser ce caractère générique dans les filtres qui ne prennent pas en charge le mode texte. Par exemple, vous ne pouvez pas utiliser ce caractère générique dans les filtres des zones suivantes :</p> 
     <ul> 
      <li> <p>Planificateur de ressources</p> </li> 
      <li> <p>Équilibreur de charge de travail</p> </li> 
      <li> <p>Analytique</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>La variable $$USER.homeGroupID fait référence à l’ID du groupe d’accueil de la personne connectée. En tant qu’administrateur ou administratrice de groupe, vous pouvez utiliser cette variable pour filtrer uniquement les éléments qui appartiennent aux membres de votre groupe principal.</p> <p>Par exemple, pour voir toutes les tâches incomplètes des projets du groupe des finances, utilisez les règles de filtrage suivantes dans un filtre de tâche :<br><em>Projet : ID de groupe égal à $$USER.homeGroupID </em><br><em>Pourcentage terminé inférieur à 100</em>.</p> <p>Pour afficher toutes les tâches incomplètes affectées à des membres d’un groupe spécifique qui est le groupe principal de la personne connectée, utilisez les règles de filtrage suivantes dans un filtre de tâche :</p> <p><em>Affecté à : ID de groupe égal à $$USER.homeGroupID<br>Pourcentage terminé inférieur à 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>La variable $$USER.otherGroupIDs fait référence à tous les groupes (y compris le groupe principal) associés au profil de la personne connecté.</p> <p>La fonctionnalité de cette variable est similaire à celle de la variable $$USER.homeGroupID , sauf que les résultats affichent des informations sur les membres de l’un des groupes associés à la personne connectée.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>La variable $$USER.homeTeamID fait référence à l’identifiant de l’équipe interne de la personne connectée. En tant que responsable d’équipe, vous pouvez utiliser cette variable pour filtrer uniquement les éléments qui appartiennent aux membres de votre équipe interne.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>La variable $$USER.teamIDs renvoie une liste de toutes les équipes associées à la personne connectée.</p> <p>La fonctionnalité de cette variable est similaire à celle de la variable $$USER.homeTeamID, sauf que les résultats affichent des informations sur la ou le membre de l’une des équipes identifiées dans le filtre.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>La variable $$USER.roleID fait référence au rôle principal de la personne connectée. Grâce à cette variable, vous pouvez créer des rapports sur les tâches ou les problèmes affectés à une fonction spécifique.</p> <p>Par exemple, pour voir toutes les tâches affectées au rôle pincipal de la personne connectée, vous pouvez utiliser la règle de filtrage suivante dans un filtre de tâche :</p> <p><em>Tâche : ID de rôle égal à $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>La variable $$USER.roleIDs fait référence à toutes les fonctions associées à la personne connectée. Grâce à cette variable, vous pouvez créer des rapports sur les tâches ou les problèmes affectés à l’une des fonctions associées à la personne connectée. </p> <p>Par exemple, pour voir toutes les tâches affectées à l’un des rôles associés à la personne connectée, vous pouvez utiliser la règle de filtrage suivante dans un filtre de tâche :</p> <p><i>Tâche : ID de rôle égal à $$USERID.roleIDs<br></i> </p> <p>Conseil : la règle de filtre <i>Tâche : ID de rôle égal à $$USERID.roleIDs</i> existe dans les filtres intégrés Tâches non affectées dans mon rôle et Problèmes non affectés dans mon rôle. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Variables de filtre de caractères génériques basés sur un objet

Vous pouvez choisir parmi les caractères génériques suivants basés sur un objet :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>La variable $$OBJCODE fait référence au type d’un objet. </p> 
     <p>Dans un formulaire personnalisé, lorsque les types d’objets sélectionnés du formulaire sont incompatibles avec un champ référencé dans un champ personnalisé calculé, vous pouvez utiliser ce caractère générique pour éviter la création de formulaires en double pour ces types d’objets.</p> 
     <p>Dans le champ personnalisé calculé, vous devez inclure le caractère générique dans une expression IF afin que le calcul puisse générer des valeurs différentes pour chacun des types d’objets de votre formulaire. </p> 
     <p>Pour plus d’informations et pour consulter un exemple, rendez-vous dans la section <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">Champs personnalisés calculés dans des formulaires personnalisés à plusieurs objets</a> de l’article <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Ajouter des données calculées à un formulaire personnalisé</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
