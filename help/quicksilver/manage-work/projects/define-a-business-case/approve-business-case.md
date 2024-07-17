---
navigation-topic: business-case-and-scorecards
title: Approuver une analyse de rentabilité
description: Une fois que vous avez terminé et envoyé l’analyse de cas pour une demande de projet, l’analyse de cas doit être approuvée. Cela dépend du workflow de votre organisation. Un projet peut commencer sans que l’analyse de cas ne doive être approuvée, mais votre administrateur Adobe Workfront et vos propriétaires de projet peuvent ne pas la considérer comme idéale.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 14%

---

# Approuver une analyse de rentabilité

Une fois que vous avez terminé et envoyé l’analyse de cas pour une demande de projet, l’analyse de cas doit être approuvée. Cela dépend du workflow de votre organisation. Un projet peut commencer sans que l’analyse de cas ne doive être approuvée, mais votre administrateur Adobe Workfront et vos propriétaires de projet peuvent ne pas la considérer comme idéale. 

Pour plus d’informations sur l’exécution et l’envoi d’un cas d’entreprise, consultez l’article [Créer un cas d’entreprise pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion d’un projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Présentation de l’approbation des dossiers métier

Tenez compte des points suivants lors de l’approbation d’un cas d’entreprise d’un projet :

* Vous devez disposer des autorisations de gestion pour un projet afin d’approuver l’analyse de cas pour celui-ci. 
* Vous ne pourrez pas voir les projets en attente de l’approbation de l’analyse de cas par vos validations dans votre site Web.
* Vous devez accéder manuellement aux différents projets nécessitant l’approbation de Business Case pour vérifier qu’ils sont en attente d’approbation. Il n’existe aucun mécanisme de notification Workfront qui avertit une personne qu’elle doit approuver l’analyse de cas d’un projet.
* Vous pouvez retrouver les projets en attente de validation de l’Analyse de cas, soit en créant un rapport de projet, soit en accédant au portefeuille auquel ils sont associés. 

  Pour plus d’informations sur les Portfolios, consultez l’article [Présentation des Portfolios dans Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## Approuver l’analyse de cas en créant un rapport de projet

Vous pouvez créer un rapport pour les projets afin de déterminer les projets pour lesquels l’analyse de cas des projets doit être approuvée. 

Pour créer un rapport sur les projets en attente de validation de leurs dossiers d’activité :

1. Créez un rapport pour les projets.

   Pour plus d’informations sur la création de rapports, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Sélectionnez l&#39;onglet **Afficher** du rapport, puis cliquez sur **Ajouter une colonne**.

1. Commencez à saisir &quot;Status&quot; dans le champ **Afficher dans cette colonne**, puis sélectionnez ce champ lorsqu’il apparaît dans la liste.

    Cette colonne affiche le statut des projets.

1. Sélectionnez l’onglet **Filtres** du rapport, puis cliquez sur **Ajouter une règle de filtre**.

1. Commencez à saisir &quot;Status&quot; dans le champ **Afficher uniquement les projets dans lequel le champ ...** et sélectionnez-le lorsqu’il apparaît dans la liste.
1. Sélectionnez **Equal** pour le modificateur de filtre.
1. Commencez à saisir &quot;Demandé&quot; dans le champ disponible. 

   Cela permet de s’assurer que le rapport inclut uniquement les projets dont le statut est Demandé .

     ![}essed_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. (Facultatif) Cliquez sur **Ajouter une autre règle de filtre**.

   Vous pouvez ajouter d’autres filtres pour n’afficher que les projets dont vous êtes le propriétaire du projet, le parrain du projet ou le propriétaire du Portfolio.

   Par exemple, vous pouvez utiliser les instructions de filtre suivantes : 

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   pour afficher les projets pour lesquels vous êtes désigné comme responsable du projet

   ```
   Project Owner ID Equals $$USER.ID
   ```

   pour afficher les projets pour lesquels vous êtes désigné comme propriétaire du projet.

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   pour afficher l’emplacement où vous avez été désigné comme Gestionnaire de Portfolios. 

1. Cliquez sur **Enregistrer+Fermer**.

   Notez que tous les projets du rapport sont dans l’état **Demandé**.

1. Cliquez sur le nom d’un projet dans le rapport pour l’ouvrir.
1. Cliquez sur **Business Case** dans le panneau de gauche.
1. Cliquez sur **Approuver** ou **Rejeter** dans la zone Résumé de l&#39;analyse de cas pour approuver ou rejeter l&#39;analyse de cas.

   ![](assets/business-case-summary-with-rp-information--1-.png)

   Le statut du projet passe à **Approuvé** si l’analyse de cas est approuvée.

   L’état du projet est remplacé par **Rejected** si le dossier Business est rejeté.

   >[!NOTE]
   >
   >Aucune notification n’avertit l’utilisateur qui a soumis l’approbation de l’analyse de cas si sa demande de projet a été approuvée ou rejetée.

## Approuver l’analyse de cas en accédant aux projets demandés dans un portfolio

Pour plus d’informations sur la révision des projets demandés, consultez l’article [Révision des projets demandés](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
