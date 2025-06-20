---
navigation-topic: business-case-and-scorecards
title: Appliquer une carte de performance à un projet et générer un score d’alignement
description: Tirez parti des cartes de performance pour mesurer l’alignement d’un projet avec les critères précédemment définis d’un portfolio. Une carte de performance reflète souvent la mission, les valeurs et les objectifs stratégiques d’une organisation.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 98%

---

# Appliquer une carte de performance à un projet et générer un score d’alignement

<!-- Audited: 06/2025 -->

Tirez parti des cartes de performance pour mesurer l’alignement d’un projet avec les critères précédemment définis d’un portfolio. Une carte de performance reflète souvent la mission, les valeurs et les objectifs stratégiques d’une organisation.

Pour plus d’informations sur les cartes de performance et sur leur mode de création, consultez la section [Créer une carte de performance](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>
   <p>Current : Prime ou version ultérieure</p>
   <p>ou</p>
   <p>Hérité : Professionnel ou supérieur</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>
   <p>Actuel : Standard</p>
   <p>ou</p>
   <p>Hérité : plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p> <p>Accès en affichage ou supérieur aux portfolios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td><p>Autorisations de gestion d’un projet</p> <p>Autorisations d’affichage ou supérieures à un portfolio</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cartes de performance du projet {#project-scorecards}

* [Vue d’ensemble des cartes de performance](#scorecards-overview)
* [Appliquer une carte de performance à un projet](#apply-a-scorecard-to-a-project)

### Vue d’ensemble des cartes de performance {#scorecards-overview}

En règle générale, une personne responsable de la gestion de projet complète les informations de la carte de performance afin de produire une valeur d’alignement comprise entre 0 et 100 pour le projet. Cette valeur est ensuite utilisée lorsque la personne chargée de la gestion du portfolio passe en revue les projets dans l’optimisateur de portfolio pour les comparer.

Pour plus d’informations sur l’optimisation du portfolio, consultez la section [Vue d’ensemble de l’optimisateur de portfolio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Appliquer une carte de performance à un projet

En tant qu’utilisateur ou utilisatrice disposant d’une licence standard ou de plan et d’autorisations de gestion pour un projet, vous pouvez joindre une carte de performance au projet.

Pour plus d’informations sur les autorisations de projet, consultez la section [Partager un projet dans Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

Vous pouvez ajouter des cartes de performance à un projet dans le cadre de la création du business case du projet.

Pour plus d’informations sur la création d’un business case, consultez la section [Créer un business case pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

L’administrateur ou l’administrateur de groupes Adobe Workfront doit activer la section Carte de performance dans la zone Business case de vos projets pour vous permettre d’accéder aux cartes de performance à partir du business case. Pour plus d’informations sur la configuration des préférences de projet et l’activation des zones du business case, consultez la section [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Pour appliquer une carte de performance à un projet, procédez comme suit :

1. Accédez au projet pour lequel vous souhaitez appliquer une carte de performance.
1. Cliquez sur **Business case** dans le panneau de gauche.
1. Recherchez la section **Carte de performance** du business case.\
   Vous devez créer une carte de performance pour que la section **Carte de performance** s’affiche sur le business case.

   Pour plus d’informations sur la création d’une carte de performance, consultez la section [Créer une carte de performance](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Sélectionnez une carte de performance dans le menu déroulant.

   ![Nouvelle carte de performance](assets/new-scorecard.png)

1. Saisissez une réponse pour toutes les questions de la carte de performance.

   Workfront applique un score à chaque question à laquelle la réponse est donnée et calcule un score global du projet en fonction du score individuel de chaque question.

   Pour plus d’informations sur la génération du score d’alignement global du projet, consultez la section [Générer un score d’alignement pour un projet](#generate-an-alignment-score-for-a-project).

1. Cliquez sur **Enregistrer** pour enregistrer la carte de performance et attribuer une note au projet.

   La carte de performance est maintenant associée au projet et le projet est noté.

<!--This functionality was removed when we redesigned bulk editing projects with 23.2: 

1. (Conditional) When changes occur in the values of scorecard questions, you must recalculate the scorecard to reflect the new values for the project score. To recaulate the scorecard, do the following: 

   1. Go to a list of projects and select all projects in the list. 
   1. Click the **Edit** icon at the top of the list. 
   1. Click **Settings** in the left panel, then check the **Recalculate Scorecards** option at the end of the Settings area. 
   1. Click Save. This recalculates the score value based on the scorecards attached for all the selected projects.  

      >[!NOTE]
      >
      >   The option to recalculate scorecards has been removed from the Preview environment, when editing projects in bulk. 

-->

## Générer un score d’alignement

* [Générer un score d’alignement pour un projet](#generate-an-alignment-score-for-a-project)
* [Générer un score d’alignement pour un portfolio](#generate-an-alignment-score-for-a-portfolio)

### Générer un score d’alignement pour un projet {#generate-an-alignment-score-for-a-project}

Le score d’alignement est la valeur produite après avoir rempli la carte de performance.

Les cartes de performance contiennent des questions avec des choix de réponses auxquelles ont été attribuées des valeurs numériques, appelées points d’alignement. Ces points permettent de déterminer dans quelle mesure le projet est aligné sur les objectifs de votre entreprise. Les points d’alignement de chaque question contiennent un nombre compris entre 0 et 100.

Une fois la carte de performance terminée, Workfront calcule le score d’alignement du projet sous forme de pourcentage à l’aide de la formule suivante :

`Project Alignment Score = The sum of the question points from the scorecard met at a given time / The sum of the possible points on the scorecard`

Pour plus d’informations, consultez la section [Créer une carte de performance](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Générer un score d’alignement pour un portfolio {#generate-an-alignment-score-for-a-portfolio}

Le score d’alignement du portfolio est une moyenne des scores d’alignement de tous les projets du portfolio.

Lorsque les carte de performance des projets sont terminées, Workfront utilise ces valeurs pour calculer le score d’alignement du portfolio en pourcentage à l’aide de la formule suivante :

`Portfolio Alignment Score = The sum of the percentages of the project alignment scores / Number of projects in the portfolio`

>[!NOTE]
>
>Si un projet n’est associé à aucune carte de performance et n’a donc pas de score d’alignement, il est considéré comme ayant un alignement de 0 % dans le portfolio. Le projet est pris en compte dans le nombre de projets du portfolio.

## Afficher le score d’alignement

Vous pouvez afficher le score d’alignement d’un projet au niveau du projet ou dans l’optimisateur de portfolio.

* [Afficher le score d’alignement sur un projet](#view-the-alignment-score-on-a-project)
* [Afficher les scores d’alignement du projet et du portfolio dans l’optimisateur de portfolio](#view-the-alignment-scores-of-the-project-and-of-the-portfolio-in-the-portfolio-optimizer)

### Afficher le score d’alignement sur un projet

Si vous disposez des droits de contribution au projet, vous pouvez afficher le score d’alignement d’un projet au niveau du projet.

1. Accédez au projet dont vous souhaitez afficher le score d’alignement.
1. Cliquez sur **Business case** dans le panneau de gauche.
1. Accédez au **Récapitulatif du business case** sur le côté droit de l’écran.

   Le score d’alignement se trouve dans le récapitulatif du business case, dans la valeur **Aligné**.

   ![Score d’alignement sur un projet](assets/alignment-score-on-a-project.png)

### Afficher les scores d’alignement du projet et du portfolio dans l’optimisateur de portfolio

Si vous disposez d’un accès en gestion au portfolio, vous pouvez afficher le score d’alignement d’un projet ou d’un portfolio dans l’optimisateur de portfolio.

Pour plus d’informations sur les informations affichées dans l’optimisateur de portfolio, consultez la section [Vue d’ensemble de l’optimisateur de portfolio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Localiser le score d’alignement du projet dans l’optimisateur de portfolio](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Localiser le score d’alignement du portfolio dans l’optimisateur de portfolio](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

  ![Score d’alignement dans dans l’optimisateur de portfolio](assets/alignment-score-in-portfolio-optimizer.png)

#### Localiser le score d’alignement du projet dans dans l’optimisateur de portfolio {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Cliquez sur le nom d’un portfolio.
1. Cliquez sur l’**optimisateur de portfolio** dans le panneau de gauche.

   L’optimisateur de portfolio s’affiche.

   Le score d’alignement d’un projet s’affiche en pourcentage dans la colonne **Alignement** de l’optimisateur de portfolio.

   Il s’agit du score d’alignement du projet, déterminé par la carte de performance associée à celui-ci.

#### Localiser le score d’alignement du portfolio dans l’optimisateur de portfolio  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. Cliquez sur le nom d’un portfolio.
1. Cliquez sur l’**optimisateur de portfolio** dans le panneau de gauche.
1. Dans la partie supérieure de l’optimisateur de portfolio, recherchez la valeur **Aligné**, ainsi que la jauge **Alignement**, qui indique le score d’alignement du portfolio.

   Il s’agit du score d’alignement du portfolio.

   Pour plus d’informations sur la génération du score d’alignement d’un portfolio, consultez la section [Générer un score d’alignement pour un portfolio](#generate-an-alignment-score-for-a-portfolio).

## Vue d’ensemble du score de l’optimisateur de portfolio

Il existe une différence entre le score d’alignement et le score de l’optimisateur de portfolio d’un projet.

Le score d’alignement d’un projet est calculé sur la base des points obtenus après avoir rempli la carte de performance. Ce score est ensuite utilisé pour déterminer le score d’alignement du portfolio. Le score d’alignement est exprimé en pourcentage.

Le score d’alignement d’un projet s’affiche dans la colonne **Alignement** de l’optimisateur de portfolio.

Le score de l’optimisateur de portfolio est un classement calculé automatiquement dans l’organisateur de portfolio selon lequel les projets peuvent être classés par priorité. Le score de l’optimisateur de portfolio s’affiche sous forme d’icône d’indicateur accompagnée d’un nombre et s’affiche dans la colonne **Score** de l’optimisateur de portfolio. Un score de l’optimisateur de portfolio n’est généré que lorsque toutes les sections du business case sont remplies, à l’exception des objectifs.

Pour plus d’informations sur la création d’un business case pour un projet, voir [Créer un business case pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Pour plus d’informations sur le calcul du score de l’optimisateur de portfolio d’un projet, voir [Vue d’ensemble du score de l’optimisateur de portfolio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
