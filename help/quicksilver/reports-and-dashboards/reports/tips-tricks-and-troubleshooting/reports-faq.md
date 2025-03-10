---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Questions fréquentes sur les rapports
description: Questions fréquentes sur les rapports
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1519'
ht-degree: 99%

---

# Questions fréquentes sur les rapports

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

Vous trouverez ci-dessous les questions fréquentes sur les rapports.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan, Travail</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Pourquoi mon calcul personnalisé pour la différence d’une heure n’affiche-t-il pas le résultat correct dans une colonne ?

Sur un rapport de projet, j’ai un calcul qui soustrait les heures effectives (2) du nombre d’heures prévues (4). Le résultat que j’obtiens est 120 alors qu’il devrait être 2.\
Mon calcul est le suivant :
<pre>valueexpression=SUB(workRequired,actualWorkRequired)</pre>

### Réponse

Les champs utilisant les heures dans Workfront sont stockés en minutes. Lorsque vous utilisez le champ dans un calcul, le résultat sera exprimé en minutes. Pour obtenir le résultat en heures, vous devez diviser le résultat du calcul par 60.

Le calcul correct est le suivant :

<pre>valueexpression=SUB(workRequired,actualWorkRequired)/60</pre>

## Pourquoi la valeur de chacun de mes éléments de graphique dans un rapport ne s’affiche-t-elle pas sur le graphique ?

### Réponse

Si un graphique de rapport contient plus de 50 éléments de graphique, la valeur de chaque élément ne s’affiche pas dans le graphique.

Lorsque le graphique contient moins de 50 éléments, la valeur de chaque élément s’affiche dans le graphique. Envisagez d’ajouter un filtre ou de modifier les regroupements dans le rapport afin de limiter la quantité d’éléments affichés dans chaque élément du graphique.

## Pourquoi mon rapport renvoie-t-il trop de résultats pour afficher le graphique ?

Lorsque je lance un rapport avec un graphique, le message d’erreur suivant s’affiche : « Attention...Ce a retourné UNE GRANDE QUANTITÉ de données qui rendent le graphique illisible. Vous devez encisager de limiter vos résultats en ajoutant un filtre ou en modifiant les regroupements dans votre graphique. »

### Réponse

Cette erreur signifie que votre graphique contient jusqu’à 618 résultats distincts, par exemple plus de 618 barres dans un graphique à barres. Pour résoudre le problème d’affichage, vous devez affiner les résultats en modifiant le filtre actuel et les sélections de regroupement.

Pour plus d’informations sur la modification des filtres et des regroupements, voir les articles [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) et [Vue d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Pourquoi mes tâches (ou mes problèmes) apparaissent-elles lorsque j’accède au même rapport (ou calendrier) que la personne avec qui je travaille et qu’elle voit ses tâches à la place ?

### Réponse

Le rapport ou le calendrier peut comporter une variable de filtre de caractères génériques qui pointe vers la personne connectée. Dans ce cas, le rapport affiche des informations en fonction de la personne connectée. Réglez le filtre pour supprimer le caractère générique qui pointe vers la personne connectée.\
![Variable de filtre de l’ID utilisateur](assets/qs--user.id-filter-variable-350x79.png)

Pour obtenir la liste complète des variables de filtrage des caractères génériques basées sur la personne, voir [Vue d’ensemble des variables de filtrage des caractères génériques](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Pourquoi les données de mon rapport semblent-elles incomplètes ?

### Réponse

Cela peut se produire dans la plupart des cas si vous disposez d’un accès limité qui vous empêche de voir des éléments du système. De plus, les éléments que vous souhaitez voir ne sont pas partagés avec vous.

Le créateur ou la créatrice du rapport peut le modifier pour l’exécuter avec les droits d’accès d’un administrateur ou administratrice système ou de toute personne utilisant le Plan ayant accès aux données.

Pour plus d’informations, voir [Exécuter et diffuser un rapport avec les droits d’accès d’une autre personne](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## Comment puis-je créer un rapport sur les tâches (ou les problèmes) qui me sont affectées, que je sois ou non propriétaire de ces tâches ?

### Réponse

Pour afficher toutes les tâches ou tous les problèmes qui vous sont affectés, que vous soyez propriétaire (ou personne cessionnaire principale) ou non, utilisez le filtre suivant dans un rapport de tâche ou de problème :

1. Accédez à un rapport de tâche ou de problème.
1. Sur l’onglet **Filtres**, cliquez sur **Ajouter une règle de filtre**.

1. Dans le champ **Commencez à saisir le nom du champ...**, commencer à saisir **Nom d’utilisateurs et utilisatrices de l’affectation**, puis sélectionnez-le lorsqu’il apparaît dans la liste.

   >[!NOTE]
   >
   >N’utilisez pas le champ **Nom attribué**, car ce filtre s’applique uniquement aux tâches et problèmes pour lesquels vous êtes la personne cessionnaire principale ou la personne propriétaire.

1. Sélectionnez le modificateur **Égal**.
1. Commencez à saisir *$$USER.ID* dans la zone de texte et sélectionnez-le dans la liste déroulante qui s’affiche.\
   Vous affichez ainsi toutes les tâches et tous les problèmes affectés à la personne connectée. Vous pouvez remplacer le caractère générique par un nom de personne spécifique.\
   ![Tâches qui me sont affectées](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Cliquez sur **Enregistrer + Fermer**.

## Pourquoi les liens Ajouter des problèmes/Ajouter des tâches n’apparaissent-ils pas au bas de mes listes de problèmes et de tâches sur un projet ?

### Réponse

Tout d’abord, assurez-vous que vous disposez des droits d’accès et des autorisations appropriés pour ajouter des problèmes et des tâches à un projet. Dans ce cas, vous devriez voir les liens **Ajouter des problèmes** et **Ajouter des tâches** au bas des listes **Problèmes** et **Tâches**.

Toutefois, certains éléments peuvent empêcher l’affichage de ces liens :

* Si le filtre rapide est appliqué à ces listes, les liens ne s’affichent pas. Supprimez le filtre rapide et les liens devraient s’afficher pour que vous puissiez ajouter des problèmes et des tâches à vos projets.\
  Pour plus d’informations sur le filtre rapide, voir [Commencer avec les listes dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Si un **Regroupement** est appliqué à ces listes, les liens ne s’affichent pas. Supprimez le **Regroupement** et les liens devraient s’afficher afin que vous puissiez ajouter des problèmes et des tâches à vos projets.\
  Pour plus d’informations sur la création de regroupements, voir [Vie d’ensemble des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Si vous avez un **Vue** appliquée à ces listes dans lesquelles une devise est sélectionnée autre que la devise par défaut du projet, les liens ne s’affichent pas. Modifiez la **Vue** en **Devise originale du projet** et les liens devraient s’afficher afin que vous puissiez ajouter des problèmes et des tâches à vos projets.\
  Pour plus d’informations sur la modification de la devise dans votre vue, voir [Créer des rapports de données financières avec des taux de change uniques](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![Devise du projet ](assets/nwe-project-original-currency-350x229.png)

## Les informations de mon rapport ou de mon tableau de bord sont-elles actualisées automatiquement ?

### Réponse

Les informations contenues dans les rapports ou les tableaux de bord ne sont pas automatiquement actualisées.

Les informations peuvent être actualisées manuellement dans un rapport mis en cache.\
Pour plus d’informations sur l’actualisation d’un rapport mis en cache, voir [Exécuter un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

Les informations peuvent être actualisées manuellement dans un tableau de bord mis en cache.\
Pour plus d’informations sur l’actualisation d’un tableau de bord mis en cache, voir la section [Afficher les tableaux de bord](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) dans l’article [Commencer avec les tableaux de bord](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Puis-je modifier la personne propriétaire d’un rapport ?

### Réponse

Vous ne pouvez pas modifier la personne propriétaire d’un rapport. Cependant, la personne qui a créé le rapport peut permettre à d’autres personnes de le modifier. La manière dont vous pouvez autoriser les personnes à modifier un rapport dépend du type d’utilisateur ou utilisatrice que vous êtes.

* Les administrateurs et administratrices système peuvent autoriser les personnes disposant d’une licence Plan à modifier les rapports en configurant l’option Modifier de la ligne Rapports afin d’inclure l’accès à Créer un rapport.\
  Pour plus d’informations, voir [Accorder l’accès aux rapports, aux tableaux de bord et aux calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Tout utilisateur final ou toute utilisatrice finale ayant accès à la création et au partage de rapports peut permettre à d’autres personnes de modifier des rapports individuels en les partageant et en leur accordant des autorisations de gestion.\
  Pour plus d’informations, voir [Partager un rapport dans Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Si vous disposez des autorisations nécessaires pour afficher ou gérer un rapport, vous pouvez également en faire une copie, dont vous serez alors la personne propriétaire par défaut. Pour en savoir plus sur la copie d’un rapport, voir [Créer une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Pourquoi ne puis-je pas accéder à un rapport détenu par une personne désactivée ?

### Réponse

Parfois, la personne propriétaire du rapport est également celle indiquée dans le.champ **Exécuter ce rapport avec les droits d’accès de :** sur le rapport. Si la personne de l’option **Exécuter ce rapport avec les droits d’accès suivants :** est désactivée, le rapport ne s’affiche plus pour les personnes avec lesquelles le rapport est partagé.Dans ce cas, vous pouvez rendre le rapport accessible à nouveau en laissant le champ **Exécuter ce rapport avec les droits d’accès suivants :** vide ou en y saisissant une personne active.

Pour en savoir plus sur le champ **Exécuter ce rapport avec les droits d’accès suivants :**, voir [Exécuter et diffuser un rapport avec les droits d’accès d’une autre personne](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Pour plus d’informations sur l’identification de tous les rapports détenus par des personnes désactivées, voir [Créer un rapport sur les activités de reporting](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## Comment accéder à un tableau de bord contenant un rapport détenu par une personne supprimée ?

### Réponse

Lorsque vous supprimez une personne, vous pouvez toujours accéder aux rapports qu’elle a créés. Toutefois, les tableaux de bord qui incluaient le rapport sont également supprimés. Cela signifie que vous ne pouvez plus accéder aux éléments suivants :

* Tableau de bord contenant le rapport
* Section personnalisée contenant un tableau de bord du rapport

Pour en savoir plus sur les implications de la suppression d’une personne, voir [Supprimer des personnes](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Si vous disposez de l’accès Afficher au rapport, vous pouvez effectuer les opérations suivantes :

1. Créez une copie du rapport.\
   Pour savoir comment créer une copie d’un rapport, voir [Créer une copie d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Mettez à jour le tableau de bord pour inclure le rapport copié.\
   Pour savoir comment modifier un tableau de bord, voir [Modifier un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
