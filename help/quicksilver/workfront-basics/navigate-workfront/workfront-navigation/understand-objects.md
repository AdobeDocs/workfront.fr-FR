---
content-type: overview;reference
navigation-topic: workfront-navigation
title: Vue d’ensemble des objets [!DNL Adobe Workfront]
description: Les informations affichées dans  [!DNL Adobe Workfront]  sont représentées par des objets stockés dans la base  [!DNL Workfront]  données. Les objets sont à la base des informations contenues dans  [!DNL Workfront]. En savoir plus sur ces objets dans cet article.
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '2508'
ht-degree: 95%

---

# Vue d’ensemble des objets [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

Les informations que vous affichez dans [!DNL Adobe Workfront] sont représentées par des objets qui sont stockés dans la base de données [!DNL Workfront]. Les objets sont à la base des informations contenues dans [!DNL Workfront].

Pour une utilisation efficace des ressources, il est essentiel de bien comprendre la nature des objets [!DNL Workfront], en vue de répondre aux exigences spécifiques de votre entreprise.

Par exemple, lorsque vous planifiez une grande quantité de travail, vous devez utiliser l’objet [!UICONTROL Projet] pour définir ce travail. Pour répartir ce travail en petits incréments prévus, vous pouvez utiliser l’objet [!UICONTROL Tâche]. Pour un travail moins important qui n’est pas prévu et qui peut survenir de manière inattendue, vous pouvez utiliser l’objet Problème. Pour suivre la progression et le respect du budget et du calendrier d’un groupe de projets, vous pouvez les organiser dans [!UICONTROL Portfolios] et [!UICONTROL Programmes]. Pour définir d’autres éléments qui vous aident à accomplir votre travail, vous pouvez utiliser d’autres objets stockés sous [!UICONTROL Projets], [!UICONTROL Tâches], [!UICONTROL Problèmes], ou [!UICONTROL Portfolios], comme [!UICONTROL Documents], [!UICONTROL Mises à jour], [!UICONTROL Heures], [!UICONTROL Utilisateurs et Utilisatrices], ou [!UICONTROL Fonctions].

[!UICONTROL Rapports] et [!UICONTROL Tableaux de bord] sont un autre exemple d’objets qui peuvent vous aider à organiser visuellement la quantité de données dans [!DNL Workfront], pour la rendre facilement accessible à tous les utilisateurs et à toutes les utilisatrices.

Pour obtenir la liste complète des objets de [!DNL Workfront], consultez la section [Explorateur d’API](../../../wf-api/general/api-explorer.md).

## Interdépendance et hiérarchie des objets

Les objets sont liés les uns aux autres dans [!UICONTROL Workfront]. Par exemple, une tâche ou un problème ne peut jamais exister indépendamment en dehors d’un projet. [!UICONTROL Tâches] et [!UICONTROL Problèmes] sont des exemples d’objets stockés dans l’objet [!UICONTROL Projet]. [!UICONTROL Tâches] et [!UICONTROL Problèmes] sont considérés comme des objets enfants des projets.

Voici quelques-uns des objets les plus couramment utilisés dans [!DNL Workfront] et leurs objets parents et enfants respectifs :

| **Objet** | **Objets parent** | **Objets enfant** |
|---|---|---|
| [!UICONTROL Portefeuilles] |  | [!UICONTROL Programmes], [!UICONTROL Projets], [!UICONTROL Documents], [!DNL Notes], [!UICONTROL Utilisateurs et Utilisatrices] |
| [!UICONTROL Programmes] | [!UICONTROL Portefeuilles] | [!UICONTROL Projets], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Utilisateurs et Utilisatrices] |
| [!UICONTROL Projets] | [!UICONTROL Portfolios], [!UICONTROL Programmes] | [!UICONTROL Tâches], [!UICONTROL Problèmes], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Heures], [!UICONTROL Utilisateurs et Utilisatrices] |
| [!UICONTROL Tâches] | [!UICONTROL Projets] | [!UICONTROL Problèmes], [!UICONTROL Tâches enfant], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Heures], [!UICONTROL Utilisateurs et Utilisatrices] |
| [!UICONTROL Événements] | [!UICONTROL Tâches], [!UICONTROL Projets] | [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Heures], [!UICONTROL Utilisateurs et Utilisatrices] |
| [!UICONTROL Tableaux de bord] |  | [!UICONTROL Rapports], Pages externes |
| [!UICONTROL Rapports] | [!UICONTROL Tableaux de bord] |  |
| [!UICONTROL Groupes] |  | [!UICONTROL Utilisateurs ou utilisatrices] |
| [!UICONTROL Équipes] |  | [!UICONTROL Utilisateurs ou utilisatrices] |
| [!UICONTROL Utilisateurs ou utilisatrices] | [!UICONTROL Groupes], [!UICONTROL Équipes], [!UICONTROL Entreprises] | [!UICONTROL Fonctions] |
| [!UICONTROL Entreprises] |  | [!UICONTROL Utilisateurs et utilisatrices] |
| [!UICONTROL Documents] | [!UICONTROL Tâches], [!UICONTROL Problèmes], [!UICONTROL Projets], [!UICONTROL Portfolios], [!UICONTROL Programmes], [!UICONTROL Utilisateurs et utilisatrices] |  |
| [!UICONTROL Plans]* |  | [!UICONTROL Initiatives] |
| [!DNL Goals]* |  | [!UICONTROL Résultats], [!UICONTROL Activités] |

Pour obtenir la liste complète des objets dans [!DNL Workfront], consultez la section [Explorateur d’API](../../../wf-api/general/api-explorer.md).

*Les plans sont les objets du [!DNL Adobe Workfront Scenario Planner]. Pour plus d’informations sur le [!DNL Scenario Planner], consultez la section [Vue d’ensemble du [!UICONTROL Planificateur de scénarios &#x200B;]](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Objectifs] sont les objets d’[!DNL Adobe Workfront Goals]. Pour plus d’informations sur [!DNL Workfront Goals], consultez la section Vue d’ensemble d’[[!DNL Adobe Workfront Goals] &#x200B;](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Personnaliser les noms d’objet

En tant qu’administrateur ou administratrice [!DNL Workfront], vous pouvez personnaliser les noms d’objet dans [!DNL Workfront] en utilisant un [!UICONTROL modèle de mise en page].

Pour plus d’informations sur la personnalisation des noms d’objet à l’aide d’un [!UICONTROL modèle de mise en page], consultez la section [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Après la personnalisation d’un modèle de mise en page et son affectation, les utilisateurs et les utilisatrices peuvent voir les noms personnalisés des objets. Les utilisateurs et les utilisatrices à qui le modèle de mise en page a été affecté ne voient plus les noms par défaut des objets, peu importe leur emplacement dans l’application web.

Par exemple, si le volume de travail le plus important dans votre organisation est appelé « Engagement », vous pouvez remplacer le nom « [!UICONTROL Projet] » par « Engagement ». Votre interface [!DNL Workfront] affiche « Engagement » au lieu de « [!UICONTROL Projet] » partout où le nom « [!UICONTROL Projet] » apparaît.

>[!NOTE]
>
>Afin que vos utilisateurs et vos utilisatrices puissent voir les nouveaux noms des objets, ils doivent se déconnecter et se reconnecter à [!DNL Workfront] après avoir sauvegardé le [!UICONTROL modèle de mise en page].

>[!IMPORTANT]
>
>La documentation [!DNL Workfront] fait toujours référence aux noms par défaut des objets. Vous devez, en tant qu’administrateur ou administratrice [!DNL Workfront], veiller à informer les utilisateurs et les utilisatrices des modifications apportées aux noms des objets, pour leur permettre de comprendre comment utiliser la documentation [!DNL Workfront], ainsi que les parties des applications qui ne reflètent pas les modifications apportées aux noms des objets.

* [Noms d’objets qui peuvent être personnalisés à l’aide d’un [!UICONTROL modèle de mise en page].](#object-names-that-can-be-customized-using-a-layout-template)
* [Zones  [!DNL Workfront]  qui reflètent les noms d’objets personnalisés.](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Zones  [!DNL Workfront]  qui ne reflètent pas les noms d’objets personnalisés.](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Noms d’objets qui peuvent être personnalisés à l’aide d’un [!UICONTROL modèle de mise en page].

En tant qu’administrateur ou administratrice [!DNL Workfront], vous pouvez personnaliser les noms des objets suivants pour qu’ils correspondent à la terminologie en vigueur dans votre organisation :

* [!UICONTROL Portfolio]
* [!UICONTROL Programme]
* [!UICONTROL Projet]
* [!UICONTROL Tâche]
* [!UICONTROL Problème]
* [!UICONTROL Objectif]*
* [!UICONTROL Résultat]*
* [!UICONTROL Activité]*

  * [!UICONTROL Objectifs], [!UICONTROL Résultats], et [!UICONTROL Activités] ne sont disponibles que si votre société a acheté [!DNL Workfront Goals]. Pour plus d’informations sur [!DNL Workfront Goals], consultez la section [[!DNL Adobe Workfront Goals] Vue d’ensemble](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Initiative]**
* [!UICONTROL Scénario]**
* [!UICONTROL Plan]**

  ** [!UICONTROL Initiatives], [!UICONTROL Scénarios], et [!UICONTROL Plans] ne sont disponibles que si votre société a acheté le [!DNL Workfront Scenario Planner]. Pour plus d’informations sur le [!DNL Scenario Planner], consultez la section [Commencer avec le  [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).



Pour plus d’informations sur la personnalisation des noms d’objets à l’aide des [!UICONTROL modèles de mise en page], consultez la section [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Vous ne pouvez pas personnaliser les noms d’un autre objet dans Workfront. Pour obtenir la liste complète des objets de [!DNL Workfront], consultez la section [Explorateur d’API](../../../wf-api/general/api-explorer.md).

Lorsque vous personnalisez le nom d’un objet, le nouveau nom s’affiche dans la plupart des zones de l’application [!DNL Workfront] dans lesquelles ce nom d’objet s’affiche.

### Zones [!DNL Workfront] qui reflètent les noms d’objets personnalisés.

Les zones suivantes indiquent le nom actualisé des objets :

* Barre de navigation supérieure
* Toutes les sections dans la navigation du panneau de gauche
* Tous les menus
* Notifications in-app
* Report Builder et éléments de rapport (vues, filtres et regroupements)
* Boutons [!UICONTROL Enregistrer]
* Fichiers exportés
* E-mails
* Applications mobiles

### Zones [!DNL Workfront] qui ne reflètent pas les noms d’objet personnalisés.

Les zones suivantes n’affichent pas le nom mis à jour des objets :

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* Module complémentaire [!DNL Outlook]

### Implications de la personnalisation des noms d’objet

Lorsque vous personnalisez des noms d’objet dans [!DNL Workfront], vous devez tenir compte des éléments suivants :

* Vous pouvez rencontrer des erreurs de syntaxe ou de grammaire dans les affichages du système. Par exemple, si vous renommez « [!UICONTROL Problème] » par « Requête » et que vous voyez n’importe où dans le système la phrase « Un requête », le système fonctionne comme prévu et vous ne devez pas la considérer comme un bug.
* Les noms personnalisés des objets ne sont pas traduisibles. Seuls les noms par défaut [!DNL Workfront] peuvent être traduits dans les langues prises en charge. Pour plus d’informations sur les langues prises en charge dans [!DNL Workfront], consultez la section [Langues prises en charge dans  [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). Les champs de noms d’objets personnalisés prennent en charge les caractères étrangers afin que vous puissiez saisir la terminologie dans n’importe quelle langue.
* Nous vous recommandons d’affecter vos [!UICONTROL modèles de mise en page] en fonction de vos unités opérationnelles (équipes ou groupes) lorsque vous personnalisez les noms d’objets à l’aide d’un [!UICONTROL modèle de mise en page].\
   Nous vous recommandons d’utiliser des noms clairement compris par les utilisateurs et les utilisatrices de ces unités opérationnelles, afin d’éviter toute confusion.
* Les notifications par e-mail et les rapports remis contiennent toujours des noms d’objets tels que définis par le [!UICONTROL modèle de mise en page] de l’utilisateur ou de l’utilisatrice qui génère l’e-mail. Vos utilisateurs et vos utilisatrices doivent se préparer à voir apparaître dans leurs e-mails des noms d’objets qui ne sont pas liés à leur groupe ou à leur équipe, s’ils reçoivent des notifications par e-mail de la part d’utilisateurs ou d’utilisatrices d’autres équipes ou groupes.\
   En tant qu’administrateur ou administratrice de [!DNL Workfront], conseillez aux utilisateurs et aux utilisatrices de faire attention aux icônes associées à chaque objet. Les icônes restent cohérentes entre les différents noms d’objets et correspondent à l’objet par défaut, tel qu’il apparaît dans la base de données. Pour une liste de toutes les icônes [!DNL Workfront] associées aux objets, consultez la section [Icônes des objets](#object-icons).

  >[!TIP]
  >
  >Pour les tâches courantes dans votre organisation, envisagez de créer une documentation personnalisée pour refléter votre terminologie.

## Icônes d’objets

La documentation de [!DNL Workfront] fait toujours référence aux noms par défaut des objets. Si les noms de vos objets ont été personnalisés, vous pouvez vous fier à l’icône qui leur est associée pour savoir quel objet personnalisé correspond à quel objet [!DNL Workfront] par défaut.

Pour plus d’informations sur les objets dont les noms peuvent être personnalisés dans [!DNL Workfront], consultez la section [Noms d’objets pouvant être personnalisés à l’aide d’un [!UICONTROL modèle de mise en page]](#object-names-that-can-be-customized-using-a-layout-template).

Voici une liste des objets et de leurs icônes correspondantes dans Workfront.

| **Objet** | **Icône** | **Nom d’objet personnalisable** |
|---|---|---|
| [!UICONTROL Entreprise] | ![Icône d’entreprise](assets/company-icon-nwe.png) , ![Icône d’entreprise bleue](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Tableau de bord] | ![Icône Tableau de bord](assets/dashboard-icon-nwe.png) , ![Icône Tableaux de bord bleue](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Objectif] | ![Icône Objectif](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Groupe] | ![Icône Groupes](assets/groups-icon-nwe.png) , ![Icône Groupe](assets/nwe-group-icon.png) |  |
| [!UICONTROL Problème] | ![Icône Événement](assets/issue-icon-nwe.png) , ![Icône Événement rose](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Fonction] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![Icône de fonction](assets/job-role-nwe-no-color.png), ![Couleur de l’icône de fonction](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plan] | ![Icône Plan](assets/plan-icon.png), ![Icône Plan bleue](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![Portfolio](assets/portfolio-icon-nwe.png) , ![icône Portfolio bleue](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Programme] | ![Icône de programme](assets/program-icon-nwe.png) , ![Icône de programme orange](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Projet] | ![Icône Projet](assets/project-icon-nwe.png) , ![Icône Projet violette](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Rapport] | ![Icône de rapport](assets/report-icon-nwe.png) , ![Icône de rapport verte](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Tâche] | ![Icône de tâche](assets/task-icon-new.png) , ![Icône de tâche verte](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Équipe] | ![Icône Équipe](assets/team-icon-nwe.png), ![Icône Équipe ronde](assets/team-icon-nwe-color.png) , ![Icône Équipes](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Modèle] | ![Icône Modèle](assets/template-icon-nwe.png) , ![Icône Modèle verte](assets/nwe-templates-icon.png) |  |
| [!UICONTROL Utilisateur ou utilisatrice] | ![Icône utilisateur grise](assets/users-icon-gray.png) , ![Icône utilisateur bleue](assets/user-icon-blue.png) , ![Icône utilisateur avec initiales](assets/user-icon-initials.png) , ![Avatar](assets/user-avatar.png) , ![Menu principal Icône utilisateur](assets/user-main-menu-area.png) |  |

## Numéros de référence des objets

Chaque objet créé dans [!DNL Workfront] se voit affecter un numéro de référence unique. Les numéros de référence sont utiles pour distinguer deux objets similaires (par exemple, des tâches portant le même nom). Vous pouvez rechercher des objets à l’aide de leur numéro de référence et vous pouvez inclure des numéros de référence dans les rapports.

Pour plus d’informations sur la recherche d’objets par numéro de référence, consultez la section [Utiliser le numéro de référence des objets](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Recherches spécifiques à un objet

Vous pouvez effectuer une recherche parmi tous les objets consultables sur [!DNL Workfront], ou sélectionner un objet spécifique à rechercher dans vos recherches de base et avancées.

Tous les objets ne peuvent pas faire l’objet d’une recherche sur [!DNL Workfront]. Vous pouvez effectuer des recherches de base et des recherches avancées sur les objets suivants dans [!DNL Workfront] :

| **Objet** | **Recherche simple** | **Recherche avancée** |
|---|---|---|
| [!UICONTROL Projets] | ✓ | ✓ |
| [!UICONTROL Tâches] | ✓ | ✓ |
| [!UICONTROL Événements] | ✓ | ✓ |
| [!UICONTROL Rapports] | ✓ | ✓ |
| [!UICONTROL Utilisateurs ou utilisatrices] | ✓ | ✓ |
| [!UICONTROL Modèles] | ✓ | ✓ |
| [!UICONTROL Documents] | ✓ | ✓ |
| [!UICONTROL Portefeuilles] | ✓ | ✓ |
| [!UICONTROL Programmes] | ✓ | ✓ |
| [!UICONTROL Tableaux de bord] | ✓ | ✓ |
| [!UICONTROL Entreprises] | ✓ | ✓ |
| [!UICONTROL Notes] (ou [!UICONTROL Mises à jour]) | ✓ |  |

Pour plus d’informations sur l’exécution de recherches de base et de recherches avancées dans [!DNL Workfront], voir [Recherche [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).


## Accès limité aux objets

Lorsqu’une personne n’a pas accès à un objet, le message « Pas d’accès » s’affiche partout où le nom de l’objet s’affiche dans Workfront.

L’accès aux objets peut être limité au niveau d’accès ou dans les autorisations d’un objet spécifique.

Cela s’applique à tous les objets et aux objets enfant répertoriés dans la section [Interdépendance et hiérarchie des objets](#interdependency-and-hierarchy-of-objects) de cet article. Cela ne s’applique pas aux objets Équipe et Utilisateur et utilisatrice.

## Rapport sur les objets

Il est extrêmement important de comprendre la hiérarchie et l’interdépendance des objets avant de commencer à créer des rapports dans [!DNL Workfront]. Les rapports sont spécifiques à un objet. Vous devez sélectionner l’objet correct pour votre rapport avant de pouvoir afficher les données que vous souhaitez.

>[!IMPORTANT]
>
>Vous ne pouvez établir un rapport que sur l’objet que vous sélectionnez et sur les objets parent dans le même rapport. Il n’est pas possible d’avoir des informations sur les objets enfants dans un rapport sur l’objet parent. Par exemple, vous pouvez afficher des informations sur le projet dans un rapport de tâche, mais pas des informations sur les tâches dans un rapport de projet.

Vous pouvez établir des rapports sur tous les objets de la base de données à l’aide de notre API ouverte. Pour obtenir une liste complète de tous les objets de la base de données, voir [Explorateur d’API](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
> * Si vous avez personnalisé les noms de vos objets à l’aide d’un modèle de mise en page, les noms des objets dans Report Builder ont également été personnalisés. Assurez-vous de savoir quels objets ont été personnalisés et recherchez le nom personnalisé dans Report Builder. Pour plus d’informations sur les objets dont les noms peuvent être personnalisés dans [!DNL Workfront], voir [Noms d’objets pouvant être personnalisés à l’aide d’un [!UICONTROL modèle de mise en page]](#object-names-that-can-be-customized-using-a-layout-template) dans cet article.
> * Lorsque vous utilisez le mode texte dans vos rapports, les noms des objets dans les expressions en mode texte sont les noms standard dans [!DNL Workfront], et non les noms d’objets personnalisés. Pour plus d’informations sur l’utilisation du mode texte dans les rapports, voir [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Pour plus d’informations sur notre API, voir [Explorateur d’API](../../../wf-api/general/api-explorer.md).

### Objets disponibles pour les rapports

Vous pouvez créer des rapports sur les objets suivants lorsque vous utilisez Report Builder dans l’application web [!DNL Workfront]. Les puces en retrait donnent plus d’informations sur l’objet et ne représentent pas d’objets supplémentaires.

* [!UICONTROL Projet]
* [!UICONTROL Tâche]
* [!UICONTROL Heure]
* [!UICONTROL Problème]
* [!UICONTROL Utilisateur ou utilisatice]
* Niveau [!UICONTROL d’accès]
* [!UICONTROL Approbation]
* [!UICONTROL Processus d’approbation]
* [!UICONTROL Affectation]
* [!UICONTROL Référence]
* [!UICONTROL Tâche de référence]
* [!UICONTROL Enregistrement de facturation]
* [!UICONTROL Heure budgétée]
   * Il s’agit des [!UICONTROL Heures budgétées], telles qu’elles apparaissent dans les outils de gestion des ressources plus anciens et obsolètes.
   * Le champ « Heures bugétées» du rapport [!UICONTROL Heures bugétées] fait référence aux heures budgétées pour les fonctions dans le [!UICONTROL planificateur de ressources]. Pour plus d’informations, voir [Comprendre le [!UICONTROL Coût budgété de la main d’œuvre] et les [!UICONTROL Heures budgétées] pour les projets](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Événement sur le calendrier]
* [!UICONTROL Entreprise]
* [!UICONTROL Formulaire personnalisé]
* [!UICONTROL Tableau de bord]
* [!UICONTROL Document]
* [!UICONTROL Approbation du document]
* [!UICONTROL Version du document]
   * Vous pouvez afficher des informations sur la version du document, le document auquel la version est associée, la personne ayant créé la version et celle ayant créé l’épreuve sur la version du document, le cas échéant (Personne ayant créé l’épreuve).
* [!UICONTROL Modèle d’e-mail]
* [!UICONTROL Dépense]
* [!UICONTROL Type de dépense]
* [!UICONTROL Page externe]
* [!UICONTROL Favori]
* [!UICONTROL Filtre]
* [!UICONTROL Objectif]
   * Vous pouvez créer un rapport pour les objectifs stratégiques ou afficher des informations relatives aux objectifs dans un rapport de projet lorsque les projets sont associés aux objectifs en tant qu’activités d’objectifs. Vous ne pouvez créer des objectifs stratégiques et les connecter à des projets que si votre organisation a acheté une licence [!DNL Workfront Goals]. Pour plus d’informations sur [!DNL Workfront Goals], voir Vue d’ensemble des [[!DNL Workfront Goals] &#x200B;](../../../workfront-goals/goal-management/wf-goals-overview.md). Pour plus d’informations sur la connexion des projets aux objectifs stratégiques, voir [Ajouter des projets aux objectifs dans Objectifs Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).
* Vous ne pouvez pas établir de rapport sur les objectifs du projet qui sont associés à un [!UICONTROL business case]. Pour plus d’informations sur les objectifs de projet et les objectifs stratégiques, voir [Glossaire de la terminologie  [!DNL Adobe Workfront] &#x200B;](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Groupe]
* [!UICONTROL Regroupement]
* [!UICONTROL Type d’heure]
* [!UICONTROL Initiative]
   * Vous ne pouvez créer un rapport pour les initiatives qui sont les objets enfant d’un plan que si votre entreprise a acheté une licence [!DNL Workfront Scenario Planner]. Pour plus d’informations sur les initiatives, voir [Vue d’ensemble des initiatives dans le  [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).

* Fonction d&#39;initiative
   * Vous ne pouvez créer un rapport sur les fonctions associées aux initiatives d’un plan que si votre entreprise a acheté une licence [!DNL Workfront Scenario Planner]. Pour plus d’informations sur la création d’initiatives et leur association à des fonctions, voir [Créer et modifier des initiatives dans le  [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).

* [!UICONTROL Itération]
* [!UICONTROL Fonction]
* [!UICONTROL Entrée du journal]
   * Vous pouvez établir un rapport sur les mises à jour du système suivies dans la zone [!UICONTROL Mises à jour] d’objets tels que les tâches, les projets, les problèmes, etc. Pour plus d&#39;informations, voir [Rapport sur la zone Mises à jour avec un rapport Entrée de journal](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Modèles de mise en page]
* [!UICONTROL Jalon]
* [!UICONTROL Chemin jalonné]
* [!UICONTROL Note] ou [!UICONTROL Mises à jour]
   * Vous pouvez établir un rapport sur les commentaires ajoutés par des personnes individuelles.

* [!UICONTROL Paramètre] (ou [!UICONTROL Champ personnalisé])
* [!UICONTROL Groupe de paramètres] (ou [!UICONTROL Saut de section])
* [!UICONTROL Portfolio]
* [!UICONTROL Programme]
* [!UICONTROL Projet (données financières)]
   * Les informations financières ne figurent dans les rapports [!UICONTROL Projet (données financières)] que si les données qui y sont associées datent de moins de 5 ans. Par exemple, si une fonction a été affectée à une tâche en janvier 2015 et que nous sommes aujourd’hui en septembre 2021, un fichier financier tel que [!UICONTROL Date d’attribution] pour la fonction n’apparaît pas dans le rapport [!UICONTROL Projet (données financières)].

  >[!CAUTION]
  >
  >L’exécution d’un rapport Projet (données financières) permet de recalculer les données financières, ce qui peut écraser les données financières précédentes et nécessiter un temps important. Pour plus d’informations sur les conséquences du recalcul des données financières, voir [Recalculer les finances du projet](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md).

* [!UICONTROL Approbation d’épreuve]
   * Permet d’afficher diverses informations sur l’approbation d’une épreuve, notamment : l’épreuve soumise à approbation, des informations sur [!UICONTROL l’approbateur ou l’approbatrice], des informations sur le demandeur ou la demandeuse (s’il s’agit d’une personne disposant d’une licence [!DNL Workfront]), des informations sur la version, l’ID de l’épreuve et la date de création de l’épreuve.\
      Les rapports sur l’[!UICONTROL approbation des épreuves] n’incluent que les épreuves disponibles dans les espaces « Mon travail » des utilisateurs et utilisatrices et pour lesquelles aucune décision n’a encore été prise.\
   * Les approbations d’épreuves sont attribuées dans [!DNL Workfront] comme décrit dans [Ajouter des personnes à une épreuve](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) dans [Partager une épreuve dans  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL File d’attente]
* [!UICONTROL Rubrique de file d’attente]
* [!UICONTROL Taux] (ceci affiche les informations de [!UICONTROL Taux de facturation] de la fonction).
* [!UICONTROL Notification de rappel]
* [!UICONTROL Rapport]
* [!UICONTROL Groupe de ressources]
* [!UICONTROL Risque]
* [!UICONTROL Type de risque]
* [!UICONTROL Planning]
* [!UICONTROL Carte de performance]
* [!UICONTROL Équipe]
* [!UICONTROL Modèle]
* [!UICONTROL Tâche de modèle]
* [!UICONTROL Congés]
   * Vous pouvez faire un rapport sur les congés d’une personne tels qu’ils sont indiqués par la personne dans son profil.

* [!UICONTROL Feuille de temps]
* [!UICONTROL Profil de feuille de temps]
* [!UICONTROL Groupe de rubriques]
* [!UICONTROL Approbation de la personne]
* [!UICONTROL Délégation d’utilisateurs et d’utilisatrices]

   * Vous pouvez établir des rapports sur les personnes qui ont été chargées d’exécuter les tâches et les problèmes des autres personnes lorsque celles-ci ne sont pas au bureau. Ce rapport affiche la personne absente du bureau ainsi que celle qui remplit ses fonctions pendant son absence.

* [!UICONTROL Décisions des utilisateurs et utilisatrices]

   * Vous pouvez indiquer le nombre de décisions prises par les personnes sur les épreuves et les documents pendant le mois en cours.

* [!UICONTROL Afficher]
* [!UICONTROL Élément de travail] (produit un rapport sur les tâches et les problèmes).
