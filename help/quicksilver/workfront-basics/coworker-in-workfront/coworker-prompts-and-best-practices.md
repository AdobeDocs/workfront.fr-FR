---
title: Invites et bonnes pratiques du collaborateur CX
content-type: reference
description: Découvrez les bonnes pratiques relatives à l’utilisation de Coworker dans Workfront et consultez une liste d’exemples d’invites.
author: Becky
feature: Get Started with Workfront
source-git-commit: 01de260893e5bbf7a228479df2f3fc6a1337d31d
workflow-type: tm+mt
source-wordcount: '2247'
ht-degree: 2%

---

# Invites et bonnes pratiques du collaborateur CX

&lt;!—NE PAS UTILISER CELA—Liez plutôt à l&#39;exemple d&#39;article MCP, assurez-vous qu&#39;il est mis à jour avec les versions récentes de MCP—>

>[!IMPORTANT]
>
>CX Coworker n’est actuellement pas disponible pour les organisations du secteur des soins de santé, de la finance ou de certains autres secteurs disposant de données sensibles. AI Assistant est disponible pour ces organisations. Pour plus d’informations, voir [ Présentation de l’assistant AI ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

Avec CX Coworker, vous pouvez utiliser le langage naturel pour interagir avec Workfront Workflow et Workfront Planning.

Coworker fait partie d’Adobe Experience Cloud Agent Orchestrator.

Pour plus d’informations sur Agent Orchestrator, voir [Adobe Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/fr/docs/experience-cloud-ai/experience-cloud-ai/agents/agent-orchestrator).

## Conditions d’accès

<!--Add info about how to qualify for agent orchestrator stuff-->

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Select, Prime ou Ultimate </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard ou Léger</p>
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td><p>Pour toute fonctionnalité en dehors des compétences de base, votre entreprise doit avoir acheté Adobe Agent Orchestrator.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td><p>Vous devez disposer des autorisations appropriées pour interagir avec n’importe quel objet via Coworker.</p> <p>Par exemple, pour recevoir des informations sur un projet par l'intermédiaire de Coworker, vous devez au moins disposer de l'autorisation Afficher sur ce projet.</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

* Votre administrateur Workfront doit avoir activé l’assistant AI pour votre organisation.

  Pour plus d’informations, consultez [Conditions préalables pour l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant) dans la présentation de l’assistant AI.
* Votre administrateur Workfront doit avoir activé AI Assistant pour votre niveau d’accès.

  Pour plus d’informations, voir [Activer ou désactiver l’assistant IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Considérations

Tenez compte des contraintes suivantes lors de l’utilisation de CX Coworker :

### Réversibilité

Certaines actions peuvent être annulées. Par exemple, si un objet est créé, cette création peut être inversée.

Cependant, certaines actions, telles que la suppression d’objet, ne peuvent **pas** être inversées. Nous vous recommandons de garder cela à l’esprit lors de l’exécution d’actions sur vos données par l’intermédiaire de Coworker.

### Contraintes de couverture des données/objets

* L’interrogation et le compte rendu des performances des champs personnalisés en sont aux premières étapes et certaines compétences (telles que les assistants d’interrogation basés sur les API) ne gèrent pas encore les champs personnalisés arbitraires pour l’agrégation et le filtrage.

### Limites d’interaction/d’expérience utilisateur

* Actuellement, CX Coworker n’« apprend » pas à long terme à partir du style ou des préférences d’un utilisateur individuel. Chaque conversation utilise uniquement la conversation actuelle et les connaissances sur les produits.
* Le contexte de la conversation est conservé au sein d’une seule session de conversation. L&#39;ouverture d&#39;une nouvelle page ou la fermeture de l&#39;assistant réinitialise l&#39;historique des conversations.
* Si les procédures d’approbation résident dans une application externe telle que Confluence ou SharePoint et sont uniquement liées par des champs d’URL, Coworker ne récupère pas et ne raisonne pas actuellement sur ces pages.

### Stockage des données / Clés gérées par le client

* Étant donné que CX Coworker fait partie de Adobe Experience Platform Agent Orchestrator, les données de vos interactions avec Coworker sont stockées dans Adobe Experience Platform, et non dans Workfront. Par conséquent, ces données ne sont pas couvertes par les accords BYOK (Customer Managed Keys) de Workfront.

## Compétences fondamentales générales en IA

>[!IMPORTANT]
>
>Ces fonctionnalités d’utilisation générale sont disponibles pour tous les utilisateurs dont l’organisation a enregistré un contrat Adobe AI signé.

Pour connaître les bonnes pratiques et les invites pour ces compétences d&#39;utilisation générale, voir [Invites et bonnes pratiques de l&#39;assistant AI](/help/quicksilver/workfront-basics/ai-assistant/ai-prompts-best-practices.md).

<!--Follow up with Oznur-->

### Connaissances du produit

CX Coworker peut fournir des instructions ou des informations de référence extraites de la documentation de Workfront.

Pour plus d’informations sur l’extraction d’informations à partir de la documentation de Workfront, voir [Obtenir de l’aide de l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

Exemple : comment modifier le type de durée d&#39;une tâche ?

### Résumé des projets, tâches et événements

Un collègue CX peut résumer un projet, une tâche ou un problème<!--, or documents--> qui a été chargé dans Workfront.

Pour plus d’informations sur les résumés de projets, de tâches et de problèmes, voir [Résumer à l’aide de l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

Exemple : résumez le projet appelé Campagne d’automne 2026.

<!--

### Locate work items

CX Coworker can find work items like projects, tasks, and issues

Example: Find all tasks assigned to me that are due this week.

For more information on using AI Assistant to locate project, tasks, and issues, see [se AI Assistant to work with projects, tasks, and issues](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

-->

<!--

Follow up on this to see if it's going away or what

### Catch Me Up 

Catch Me Up summarizes updates, uploaded documents, and other notable changes that have about your projects that have occurred in the last 24 hours, 3 days, or 7 days.  

For more information on Catch me up, see [Catch up on work in Priorities](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).

-->

<!--

### Smart filters

You can use natural language filters in Priorities to replace status, pre-built views to help you filter your work.

For more information on using Smart Filters, see [Filter your work with Smart filters](/help/quicksilver/workfront-basics/priorities/filter-group-work-priorities.md) in the article Filter and group your work with Priorities.

-->

## Collègue CX dans Workfront

* [Informations sur le projet, la tâche et l&#39;événement](#project-task-and-issue-information)
* [Gestion de projet et de travail](#project-and-work-management)
* [Contenu et approbations](#content-and-approvals)

### Informations sur le projet, la tâche et l&#39;événement

CX Coworker peut vous donner des informations sur les projets, les tâches et les problèmes, y compris des résumés et l’intégrité du projet.

Consultez des exemples d’invites pour les approbations de documents et de ressources dans les zones suivantes :

* [Obtenir des informations sur des projets, des tâches ou des événements](#find-information-about-projects-tasks-or-issues)
* [Résumer des projets, des tâches ou des événements](#summarize-projects-tasks-or-issues)
* [Afficher l&#39;intégrité du projet pour les projets, programmes ou portefeuilles](#show-project-health-for-projects-programs-or-portfolios) <!--remove any mention of project health-->

#### Obtenir des informations sur des projets, des tâches ou des événements

* Projets
  * Afficher tous les projets actifs de l’équipe Brand Marketing
  * Vous avez besoin d&#39;une liste de projets dans le portefeuille Campagnes du 4e trimestre, sous la catégorie « Numérique ».
  * Montrez-moi les projets gérés par des utilisateurs qui sont chefs de projet dans la société de services Creative.
* Tâches
  * Donne-moi toutes les tâches assignées à Joan Harris.
  * Me montrer les tâches de la catégorie « Conception » affectées à l&#39;équipe Expérience utilisateur.
  * J&#39;ai besoin de tâches affectées aux rédacteurs dans le programme Promotions des vacances.
* Problèmes
  * Montrez-moi tous les numéros du projet « Website Redesign » sous la catégorie « Technical ».
  * Récupérez tous les problèmes non résolus signalés par le groupe d’assurance qualité.
  * J’ai besoin de problèmes affectés aux développeurs de la société Global Tech.

#### Résumer des projets, des tâches ou des événements

* « Résumer ce projet »
* « Résumer la semaine dernière pour ce projet »

#### Afficher l&#39;intégrité du projet pour les projets, programmes ou portefeuilles

>[!NOTE]
>
>Votre organisation doit être inscrite à la version Beta de l’intégrité du projet pour pouvoir utiliser cette fonctionnalité.

* « Montrez-moi la santé de mes projets actifs »
* « Montrez-moi l&#39;état de ce programme »

### Gestion de projet et de travail

Vous pouvez utiliser CX Coworker pour créer et gérer des projets, y compris des tâches et des affectations.

Consultez des exemples d&#39;invites pour la gestion de projet et de travail dans les domaines suivants :

* [Créer, mettre à jour ou supprimer des projets](#create-update-or-delete-projects)
* [Identifier le modèle de projet approprié en fonction de l’invite utilisateur](#identify-the-right-project-template-based-on-user-prompt)
* [Ajouter, modifier ou personnaliser des tâches dans un projet](#add-edit-or-customize-tasks-in-a-project)
  <!--* [Create, update, or delete assignments](#create-update-or-delete-assignments)-->
  <!--* [Recommend best matching user assignments for the task based on users' job role and availability](#recommend-best-matching-user-assignments-for-the-task-based-on-users-job-role-and-availability)-->

#### Créer, mettre à jour ou supprimer des projets

Vous pouvez créer des projets à partir de zéro ou de modèles, mettre à jour des projets et les supprimer.

* Créez un projet vierge appelé Sandbox d’innovation du 2e trimestre, du 10 mars au 30 avril. Définissez-moi comme propriétaire.
* Créez un projet appelé Lucent AI Launch - NA à l’aide du modèle Campagne marketing intégrée . Démarrez le 5 février et définissez-le sur Actuel.
* Créez un projet appelé Website Redesign - EMEA du 1er mars au 15 juin. Il s&#39;agit d&#39;une priorité élevée, détenue par EMEA Marketing, parrainée par le vice-président marketing, budgétée à 250 000 $ avec environ 1 200 heures planifiées, axée sur l&#39;Europe dans le but d&#39;améliorer les conversions.
* Pour le projet Lucent AI Launch - NA, déplacez-le au 2e trimestre, changez l&#39;objectif de conduire des essais gratuits, repoussez l&#39;arrivée à la mi-avril, augmentez le budget à 150 000 $ et marquez-le comme urgent.
* Afficher tous les projets marketing en cours se terminant au T2 qui sont hautement ou urgents, triés par date de fin au plus tôt.

#### Ajouter ou modifier des tâches

Vous pouvez ajouter ou modifier des tâches dans un projet et vous pouvez personnaliser la liste des tâches du modèle que vous utilisez pour créer un projet.

* Ajoutez au projet une nouvelle tâche appelée Assurance qualité de la page de destination et planifiez-la du 22 au 26 avril.
* Mettez à jour la tâche de Révision de la conception afin qu’elle se termine le 18 avril et affectez-la à l’équipe créative.
* Supprimez la tâche Imprimer la production de ressources du projet.
* Afficher toutes les tâches de ce projet qui ne sont pas terminées et dont le début est prévu entre le 1er et le 30 avril.
* Définissez Approbation juridique comme prédécesseur de la tâche Campaign Launch.
* Ajoutez une nouvelle tâche appelée Final Copy Poland planifiée du 15 au 16 avril, déplacez la tâche Copy Review au 10 avril, supprimez la tâche Extra Review Round et définissez Final Copy Poland comme prédécesseur de Email Build.
* Lors du flux de création du projet, essayez de fournir autant d’informations que possible sur les livrables qui doivent idéalement devenir des tâches dans le cadre du projet.

#### Créer, mettre à jour ou supprimer des affectations

Vous pouvez créer, mettre à jour et supprimer des affectations d’utilisateurs ou de fonctions.

* Pour le projet « Concevoir une page de destination pour le lancement du produit », identifiez les fonctions appropriées et les heures planifiées recommandées pour toutes les tâches actuellement non affectées.
* Plusieurs tâches ne me sont pas affectées, notamment « Implémenter le suivi GA4 pour le site de campagne », « Configurer les événements de conversion » et « Valider les données d’analyse ». Pouvez-vous suggérer les fonctions appropriées et une estimation des heures pour chacune d’elles ?
* Pour les tâches de création « Créer 3 variantes de bannière pour les publicités display EMEA », « Appliquer les révisions » et « Exporter les ressources finales », attribuez les meilleures fonctions et estimez l’effort requis pour chaque tâche.
* Dans les projets « Lancement de produit 2e trimestre », « Reconception de site web - EMEA » et « Campagne média payante - NA », identifiez toutes les tâches non affectées et attribuez les fonctions appropriées avec les heures planifiées recommandées pour chacune.

<!--

#### Identify the right project template based on user prompt

* We're launching a new product feature with a landing page, emails, paid ads, and social posts. Which project template should we use?
* Create a project for a global marketing campaign with multiple channels and regional rollouts. (should suggest a template if provided more info)
* For Website Redesign – EMEA project, recommend and attach the correct project template.

-->

<!--

#### Recommend best matching user assignments for the task based on users' job role and availability

* Who is the best available user to assign to 'Design Landing Page Hero', considering who still has capacity today?
* Who should be assigned to 'Backend API integration for campaign reporting', considering engineering role alignment?
* For all unassigned tasks in this project, recommend the best users based on job role match and daily availability.
* Recommend users for the tasks 'QA testing for website launch' and 'Content review', prioritizing users whose job roles match and who are not over-allocated today.

-->

### Contenu et approbations

Un collègue CX peut vous aider à gérer les approbations de documents et de ressources dans Workfront.

Tenez compte des points suivants lorsque vous utilisez les approbations de documents et de ressources :

* Les approbations de contenu doivent être activées pour votre organisation avant de pouvoir utiliser cette fonctionnalité dans Coworker.
* L’IA ne peut pas approuver ni rejeter au nom des humains. Les décisions reposent sur les utilisateurs, à l’exception du réviseur de l’IA dédiée à Workfront.

  Pour plus d’informations sur le réviseur de l’IA dédiée à Workfront, voir [Prise en main du réviseur de l’IA dédiée à Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).
* Cette fonctionnalité existe dans Workfront et ne peut pas être utilisée pour interagir avec des outils ou des fournisseurs de documents externes.
* Pour une expérience optimale, utilisez cette fonctionnalité avec l’expérience Validations unifiées .

  Pour plus d&#39;informations sur les validations unifiées, voir [Présentation des validations unifiées](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

Consultez des exemples d’invites pour les approbations de documents et de ressources dans les zones suivantes :

* [Ajouter ou supprimer des participants à l&#39;approbation](#add-or-remove-approval-participants)
* [Rappeler aux parties prenantes qu’une seule ressource est en attente de révision](#remind-stakeholders-of-a-single-asset-waiting-for-review)
* [Ajouter, mettre à jour ou appliquer des modèles d’approbation pour une seule ressource](#add-update-or-apply-approval-templates-for-a-single-asset)

#### Ajouter ou supprimer des participants à l&#39;approbation

* Ajouter Sarah Chen et Miguel Alvarez en tant qu&#39;approbateurs sur le document actuel.
* Supprimer Jennifer Otto de cette approbation.
* Supprimez toute personne qui n’a pas encore pris de décision d’approbation.
* Ajoutez une nouvelle étape au fichier spring-campaign.pdf appelée « Révision finale ».
* Ajoutez Mark et Sarah en tant qu’approbateurs et Phil en tant que réviseur pour la deuxième étape de la campagne d’hiver.pdf
* Pour la campagne d&#39;hiver.pdf, donnez à la première étape une date limite pour aujourd&#39;hui à 17h, et à la revue finale une date limite pour demain à 17h
* Ajoutez une étape de vérification finale au fichier fall-campaign.png avec une date limite de jeudi à 17h et incluez Jim et Pam en tant qu’approbateurs, ainsi qu’Oscar en tant que réviseur
* Ajoutez Mark Jones au fichier fall-campaign.png aux première et dernière étapes en tant que réviseur/réviseuse.
* Créons une validation en plusieurs étapes pour le fichier fall-campaign.png avec 3 étapes, 1 conception 2 rédaction et 3 juridiques. Je n&#39;ai besoin que d&#39;une seule décision pour chaque étape. Ajoutez Mike, Sally, Jane au design, Chris, Richard, Mark à la rédaction et Phil, Tom et Sarah à Legal.

#### Rappeler aux parties prenantes qu’une seule ressource est en attente de révision

* Envoyez un rappel aux approbateurs de la ressource « Vidéo de campagne de printemps » qui n’ont pas répondu.
* Rappelez à toutes les personnes qui n’ont pas approuvé cette ressource « Vidéo de campagne de printemps ».
* Qui n’a pas encore pris de décision sur la ressource « Brand Guidelines PDF » ? Rappelez-leur.

#### Ajouter, mettre à jour ou appliquer des modèles d’approbation pour une seule ressource

* Appliquez le modèle d’approbation « Lancement marketing » à la ressource nommée « Vidéo de campagne de printemps ».
* Créez un modèle d’approbation en 3 étapes : Révision de Creative, Approbation juridique et Approbation finale.
* Ajouter Julia Santos et Shane Baker à l&#39;étape 1.
* Modifiez le modèle « Lancement du produit » pour ajouter Elizabeth Peterson à l’étape d’approbation finale.
* Créez un modèle appelé « Révision urgente » en une seule étape et affectez-le à Olivia Kim.
* Mettez à jour le modèle « Creative Review » en supprimant Rick Kuvec et en ajoutant Karen Sterling à l’étape 2.


## Collaborateur CX dans la planification Workfront

### Utiliser les enregistrements Planning

* [Créer, supprimer, dupliquer ou restaurer des enregistrements](#create-delete-duplicate-or-restore-records)
* [Lier des enregistrements à d&#39;autres enregistrements](#link-records-to-other-records)
* [Modifier, mettre à jour ou ajouter un champ à un enregistrement](#edit-update-or-append-a-field-to-a-record)
* [Accéder à l’historique des modifications d’enregistrement](#access-record-change-history)

#### Créer, supprimer, dupliquer ou restaurer des enregistrements

* Créez un nouvel enregistrement de campagne appelé Vente d’été 2026.
* Ajoutez un nouvel enregistrement de produit avec le nom Widget Pro et le prix $299
* Pouvez-vous créer un nouvel enregistrement de prospect pour John Smith ?
* Supprimez l’enregistrement de la campagne nommé Ancienne promotion
* Supprimer l&#39;enregistrement de test que je viens de créer
* Pouvez-vous supprimer l’ID d’enregistrement Rc123abc456 ?
* Dupliquer l’enregistrement de la campagne T1
* Pouvez-vous copier cette campagne pour en créer une nouvelle ?
* Effectuer une copie de la campagne de promotion des vacances
* Restaurer la campagne que j’ai supprimée accidentellement
* Pouvez-vous récupérer l’enregistrement du projet supprimé ?
* Si j’ai supprimé un enregistrement par erreur, pouvez-vous le restaurer ?

#### Lier des enregistrements à d&#39;autres enregistrements

* Lier l’enregistrement de la campagne d’été à l’initiative T2
* Pouvez-vous connecter ce produit aux campagnes marketing associées ?
* Je dois associer ces trois prospects à l’enregistrement Compte d’entreprise

#### Modifier, mettre à jour ou ajouter un champ à un enregistrement

* Mettez à jour le champ Budget dans la campagne d’été sur 75 000 $
* Pouvez-vous changer le statut de cet enregistrement de projet en Terminé ?
* Ajoutez John Doe au champ Membres de l’équipe pour cette initiative.

#### Accéder à l’historique des modifications d’enregistrement

* Afficher l&#39;historique des modifications de l&#39;enregistrement Campagne d&#39;été
* Pouvez-vous indiquer qui a modifié ce projet et ce qu’il a changé ?
* J&#39;ai besoin de voir toutes les mises à jour de ce record la semaine dernière

### Utilisation de System Designer dans Workfront Planning

* [Création et configuration des espaces de travail](#create-and-configure-workspaces)
* [Définition des types d’enregistrements](#define-record-types)
* [Champs de conception et champs de formule](#design-fields-and-formula-fields)
* [Créer des vues personnalisées](#build-custom-views)


#### Création et configuration des espaces de travail

* Créez un espace de travail Planning appelé Campagnes marketing 2026
* Mettre à jour mon espace de travail de planification des produits pour appliquer la couleur bleue et ajouter une description
* Afficher tous les espaces de travail Planning auxquels j&#39;ai accès

#### Définition des types d’enregistrements

* Créer un nouveau type d&#39;enregistrement appelé Campagnes dans mon espace de travail Planning
* Mettez à jour le type d’enregistrement Initiatives pour modifier son icône et sa description
* Afficher tous les types d&#39;enregistrements dans mon espace de travail Marketing Planning

#### Champs de conception et champs de formule

* Ajouter un champ Budget à mon type d&#39;enregistrement Campagnes Planning avec le type de devise
* Créez un champ de formule dans Planning qui calcule les jours restants avant la date de fin de la campagne
* Mettre à jour le champ Priorité dans mon espace de travail Planning pour ajouter d&#39;autres options de liste déroulante

#### Créer des vues personnalisées

* Créez une vue chronologique dans Planning pour afficher le planning de mes campagnes par dates de début et de fin
* Ajouter une nouvelle vue de tableau à mes initiatives de planification qui filtre uniquement le statut actif
* Dupliquez ma vue Campagnes actives Planning et modifiez le tri.
