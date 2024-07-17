---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Vue d’ensemble des domaines de l’analyse de rentabilité
description: Cet article décrit les domaines de l’analyse de cas d’un projet.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1605'
ht-degree: 4%

---

# Vue d’ensemble des domaines de l’analyse de rentabilité

Cet article décrit les domaines de l’analyse de cas d’un projet.

Pour plus d’informations sur la création d’un dossier de recherche pour un projet, voir [Création d’un dossier de recherche pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

L’administrateur ou l’administrateur de groupe Adobe Workfront doit activer toutes les sections de l’Analyse de cas avant qu’elles ne soient visibles sur le projet, à l’exception de la section Informations sur le projet . La section Informations sur le projet est activée par défaut.

Pour plus d’informations sur l’activation des zones de l’analyse de cas, reportez-vous à la section &quot;Analyses de cas&quot; de la section  [ Configurez les préférences du projet à l’échelle du système ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Voici les domaines de l’analyse de cas d’un projet :

* Informations sur le projet
* Objectifs
* Frais
* Établissement du budget de ressources
* Risques
* Carte de score
* Formulaires personnalisés
* Récapitulatif du business case

## Informations sur le projet

La zone **Informations sur le projet** de l’analyse de cas n’est pas configurable par l’administrateur Workfront. Tous les projets comportent une zone Informations sur le projet dans l’Analyse de cas. 

La section Informations sur le projet de l’Analyse de cas inclut les informations de base d’un projet, avant même que le projet n’ait réellement commencé.

Envisagez de modifier les champs suivants :

* **Description** : décrivez votre projet.
* **Propriétaire du projet**

  Par défaut, l’utilisateur qui crée le projet est également le propriétaire du projet. Vous pouvez modifier ce champ et indiquer un autre utilisateur actif comme propriétaire du projet.

* **Sponsor du projet**

  Envisagez d’ajouter une autre personne que le propriétaire du projet en tant que parrain du projet. Le parrain reçoit l&#39;approbation de l&#39;Analyse de cas. 

* **Portfolio** : spécifiez un Portfolio pour le projet. Vous devez créer le Portfolio et le placer dans l’état **Actif** avant de pouvoir le sélectionner dans ce menu déroulant.

  Pour plus d’informations sur les portefeuilles, consultez la [présentation des Portfolios dans Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

  Pour plus d’informations sur la création de Portfolios, voir [Création d’un portfolio](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **Avantage planifié** : estimez l’avantage financier prévu pour votre organisation une fois ce projet terminé. Il peut s’agir de n’importe quelle devise et il doit s’agir d’une valeur positive. Par exemple, 10 000 $.
* **Status** : par défaut, l’état d’une requête de projet est défini sur **Idée**.

  Si vous définissez le statut sur autre chose que Idée ou Planification, le bouton **Envoyer** disparaît de la zone Résumé de l’analyse de cas opérationnelle et vous ne pouvez plus soumettre l’analyse de cas pour approbation. 

* **Date de début fixe** : indiquez une date de début du projet.
* **Date de fin fixe** : spécifiez une date de fin du projet.

  >[!NOTE]
  >
  >Les dates de début et de fin fixes de l’analyse de cas n’ont aucune incidence sur les dates de début et de fin planifiées du projet. Elles représentent les dates demandées par le créateur du projet pour lesquelles le projet se développerait idéalement. Au lieu de cela, les dates de début et de fin planifiées du projet indiquent la chronologie planifiée du projet, basée sur les tâches du projet.

## Objectifs

Les objectifs définissent les objectifs du projet. Cette zone est activée par défaut dans l’Analyse de cas, mais l’administrateur de Workfront peut choisir de ne pas l’afficher. Ce champ affiche les objectifs par ordre de priorité.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>Vous pouvez créer des objectifs stratégiques pour votre organisation qui ne sont pas liés à l’analyse de cas individuelle d’un projet. Vous devez avoir accès aux objectifs Adobe Workfront pour pouvoir créer des objectifs stratégiques. Vous pouvez ensuite les connecter à des projets en dehors de leurs analyses de cas. Pour plus d’informations sur la création d’objectifs à l’aide des objectifs Workfront, voir [Présentation des objectifs Adobe Workfront](../../../workfront-goals/goal-management/wf-goals-overview.md).

La définition des objectifs est facultative pour que le projet reçoive un score dans Portfolio Optimizer. Cette section est la seule section facultative de l’Analyse de cas. Toutes les autres sections de l’analyse de cas doivent être terminées avant que le projet ne soit noté dans Portfolio Optimizer. Vous pouvez indiquer un niveau de priorité pour un objectif au fur et à mesure de sa création.

Pour plus d’informations sur les objectifs, voir  [Créer des objectifs de Business Case](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Frais

Les dépenses représentent les frais non liés au travail qui pourraient être engagés pendant la durée de vie d&#39;un projet. Cette zone est activée par défaut dans l’Analyse de cas, mais l’administrateur de Workfront peut choisir de ne pas l’afficher. 

Les dépenses que vous indiquez dans l&#39;Analyse de cas sont également renseignées dans l&#39;onglet Dépenses du projet, sous la forme Dépenses prévues.

Les dépenses affectent les champs suivants du projet :

* Coût budgété
* Valeur nette

Pour plus d’informations sur les coûts budgétaires et les valeurs nettes, voir [Présentation des champs financiers de Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Pour plus d’informations sur les dépenses, voir  [Gérer les dépenses de projet](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

Votre administrateur Workfront peut configurer des types de dépenses personnalisés.

Pour plus d’informations sur la création de types de dépenses personnalisés, voir [Création de types de dépenses personnalisés](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## Établissement du budget de ressources

Vous pouvez effectuer les actions suivantes dans la zone Ressource/Budget de l’Analyse de cas :

* Associez les groupes de ressources au projet.
* Planifiez vos ressources au niveau du projet.

Les heures budgétisées pour les ressources du projet s’affichent dans la zone Ressource/Budget de l’analyse de cas, générant le Coût de la main-d’oeuvre budgétisé du projet. Cette zone de l’Analyse de cas est activée par défaut.

Pour plus d’informations sur la planification des ressources pour le projet dans l’Analyse de cas, voir [Ressources budgétaires dans l’Analyse de cas](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

Tenez compte des points suivants lors de l’affichage de la section Ressource/Budget de l’Analyse de cas :

* Vous pouvez y inscrire des informations sur les ressources de budget à l’aide des outils suivants :

   * Le planificateur de ressources

     Pour plus d’informations, voir [Ressources de budget dans l’analyse de cas à l’aide du planificateur de ressources](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * Le planificateur de scénario , si votre société a acheté une licence supplémentaire pour le planificateur de scénario d’Adobe

     Pour plus d’informations, voir [Ressources budgétaires dans l’analyse de cas à l’aide du planificateur de scénario](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     Le planificateur de scénarios n’est disponible que dans la nouvelle expérience Adobe Workfront et nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénarios Workfront, voir [Vue d’ensemble du planificateur de scénarios](../../../scenario-planner/scenario-planner-overview.md).

* Les informations affichées ici s’affichent également dans le planificateur de ressources au niveau du système ou dans le planificateur de scénario. 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* Une fois vos ressources budgétisées, le coût de la main-d’oeuvre Budget du projet s’affiche dans la zone Budget des ressources si les rôles sont associés aux taux de coût par heure. Le Coût de la main-d’oeuvre budgété s’affiche dans la devise du projet.

  >[!IMPORTANT]
  >
  >Le coût de la main-d’oeuvre budgété est le coût associé aux rôles sur le projet, et non aux utilisateurs. La somme de tous les coûts de main-d’oeuvre budgétés pour les utilisateurs peut ou non correspondre au coût de main-d’oeuvre budgété du rôle de travail associé aux utilisateurs. 

  Pour plus d’informations sur le coût de la main-d’oeuvre budgété, voir [Présentation des champs financiers de Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

  Pour plus d’informations sur la création de rôles de tâche et l’association des taux de coût par heure avec eux, voir [Création et gestion des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Risques

Les risques sont des facteurs qui peuvent empêcher un projet de se terminer à temps ou sur le budget. La définition de ces facteurs est importante pour le responsable de Portfolio ou le parrain de projet afin de prendre une décision éclairée sur l’approbation du projet. Cette zone est activée par défaut dans l’Analyse de cas, mais l’administrateur de Workfront peut choisir de ne pas l’afficher.

Vous pouvez associer un coût potentiel aux risques que vous définissez en cas de besoin. Le coût des risques sur un projet affecte la valeur nette du projet. 

Pour plus d’informations sur le projet Net Value, voir [Présentation des champs financiers de Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Pour plus d’informations sur la création de risques, voir  [Créer et modifier des risques sur les projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

Votre administrateur Workfront peut configurer des types de risque personnalisés.

Pour plus d’informations sur la création et la modification des types de risque personnalisés, voir [Modification et création de types de risque](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Carte de score

Les Fiches d’évaluation mesurent l’alignement du projet. Cette zone est activée par défaut dans l’Analyse de cas, mais l’administrateur de Workfront peut choisir de ne pas l’afficher.

Pour plus d’informations sur l’application d’une fiche d’évaluation à un projet et la génération d’un score d’alignement, voir [Application d’une fiche d’évaluation à un projet et génération d’un score d’alignement](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Pour appliquer une fiche d’évaluation, votre administrateur Workfront doit en créer une. La zone **Fiche d’évaluation** de l’Analyse de cas ne s’affiche pas, sauf si une Fiche d’évaluation est créée.

Pour plus d’informations sur la création d’une fiche d’évaluation, voir  [Créez une fiche d’évaluation](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Formulaires personnalisés

Vous pouvez associer des Forms personnalisées à un projet lors de la définition d’un cas d’entreprise. Cette zone n’est pas activée par défaut dans l’Analyse de cas. L’administrateur Workfront doit l’activer pour l’afficher dans l’Analyse de cas.

Pour plus d’informations sur l’activation des zones de l’analyse de cas, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Pour appliquer un formulaire personnalisé, votre administrateur Workfront doit d’abord créer un formulaire personnalisé.

Pour plus d’informations sur la création d’un formulaire personnalisé, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

Vous pouvez utiliser des formulaires personnalisés pour collecter des informations supplémentaires qui ne s’affichent pas dans les autres champs de l’Analyse de cas.

Pour plus d’informations sur l’application d’un formulaire personnalisé, voir [Joindre un formulaire personnalisé à un cas d’entreprise](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## Récapitulatif du business case

* [Présentation du résumé de l’analyse de cas ](#overview-of-the-business-case-summary)
* [Exporter l’analyse de cas](#export-the-business-case)

### Présentation de la synthèse des analyses de cas {#overview-of-the-business-case-summary}

Vous pouvez voir un résumé des finances principales du projet et si un projet est aligné ou non avec une Fiche d’évaluation dans le panneau Résumé de l’analyse de cas, dans le coin supérieur droit de l’ analyse de cas .

Vous ne pouvez pas modifier le résumé des affaires. Il ne s’agit que d’un aperçu rapide de l’état du projet en ce qui concerne les champs financiers et la Fiche d’évaluation. \
 

Les champs suivants s’affichent dans le récapitulatif des cas d’entreprise :

* Valeur nette du projet
* Le coût du projet budgété
* Le coût potentiel du risque
* Les avantages prévus
* Score d’alignement

Pour plus d’informations sur ces champs, voir [Présentation des champs financiers de Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### Exporter l’analyse de cas {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

Vous pouvez exporter le Business Case vers un fichier de PDF, au cas où vous auriez besoin de l’imprimer ou de le joindre à un email dans un format plus condensé. 

Pour plus d’informations, voir [Export the Business Case of a project](../../../manage-work/projects/define-a-business-case/export-business-case.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it.&nbsp;</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.&nbsp; The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>
--&gt;
