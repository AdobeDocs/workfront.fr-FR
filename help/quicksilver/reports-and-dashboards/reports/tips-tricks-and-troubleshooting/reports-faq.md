---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Questions fréquentes sur les rapports
description: Questions fréquentes sur les rapports
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 04818bc054c3bab6e6208b6678365549664d1594
workflow-type: tm+mt
source-wordcount: '1500'
ht-degree: 88%

---

# Questions fréquentes sur les rapports

<!--Audited: 05/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

Vous trouverez ci-dessous les questions fréquentes sur les rapports.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td><p>Nouveau : Standard</p> 
   <p>Actuellement : Travail ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux rapports, tableaux de bord et calendriers</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pourquoi mon calcul personnalisé pour la différence d’une heure n’affiche-t-il pas le résultat correct dans une colonne ?

<!--this section is linked from the Actual Hours article for Tasks in the Task Information folder; edit the links or do not delete or change this section-->

Dans un rapport de projet, j&#39;ai un calcul qui soustrait les heures effectives héritées des heures prévues.

Le résultat que j&#39;obtiens est erroné.

<!--this changed with this issue in May 2025; Actual Hours changed from actualWorkRequired to actualWorkRequiredDouble: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/68108e860000120e90a79cb82e5811c2/updates : On a project report I have a calculation that subtracts Actual Hours (2) from Planned Hours (4). The result I am getting is 120 when it should be 2.  -->

Mon calcul est le suivant :

`valueexpression=SUB(workRequired,actualWorkRequired)`

### Réponse

La plupart des champs utilisant des heures dans Workfront sont stockés en minutes. Lorsque vous utilisez ces champs dans un calcul, le résultat est le plus souvent exprimé en minutes. Pour obtenir le résultat en heures, vous devez diviser le résultat du calcul ou le champ que vous référencez par 60.

Le calcul correct est le suivant :

`valueexpression=SUB(workRequired,actualWorkRequired)/60`

>[!NOTE]
>
>Si vous utilisez des heures réelles dans votre calcul, utilisez `actualWorkRequiredDouble` pour le champ de valeur. Les heures réelles sont stockées en heures. Les heures planifiées sont stockées en minutes.
>
>Le calcul correct pour les heures réelles est le suivant :
>>`valueexpression=SUB(workRequired/60,actualWorkRequiredDouble)`


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

Parfois, la personne propriétaire du rapport est également celle indiquée dans le.champ **Exécuter ce rapport avec les droits d’accès de :** sur le rapport. Si l&#39;utilisateur **Exécuter ce rapport avec les droits d&#39;accès de:** est désactivé, le rapport ne s&#39;affiche plus pour les utilisateurs avec lesquels il est partagé. Dans ce cas, vous pouvez rendre à nouveau le rapport accessible en laissant vide le champ **Exécuter ce rapport avec les droits d’accès de :** ou en entrant un utilisateur actif dans le champ.

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
