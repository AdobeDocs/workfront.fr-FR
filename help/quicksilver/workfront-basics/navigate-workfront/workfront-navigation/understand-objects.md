---
content-type: overview;reference
navigation-topic: workfront-navigation
title: "[!DNL Adobe Workfront] Présentation des objets"
description: "Les informations que vous affichez dans [!DNL Adobe Workfront] est représenté par des objets stockés dans la variable [!DNL Workfront] base de données. Les objets sont ce qui motive les informations dans [!DNL Workfront]. Pour en savoir plus sur ces objets, consultez cet article."
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 25939493f6ffed31ae1bdaf26d417ce4e5e5c004
workflow-type: tm+mt
source-wordcount: '2419'
ht-degree: 2%

---

# Vue d’ensemble des objets [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

Les informations affichées dans [!DNL Adobe Workfront] est représenté par des objets stockés dans la variable [!DNL Workfront] base de données. Les objets sont ce qui motive les informations dans [!DNL Workfront].

Comprendre la définition des objets dans [!DNL Workfront] est important afin que vous puissiez utiliser l’objet correct en fonction des besoins de votre entreprise.

Par exemple, lorsque vous planifiez une grande quantité de travail, vous devez utiliser la variable [!UICONTROL Projet] pour définir ce travail. Pour diviser ce travail en incréments planifiés plus petits, vous pouvez utiliser la variable [!UICONTROL Tâche] . Pour effectuer un travail plus réduit qui n’est pas planifié et qui peut se produire de manière inattendue, vous pouvez utiliser l’objet Problème . Si vous souhaitez tracker l&#39;avancement et le respect du budget et de la chronologie d&#39;un groupe de projets, vous pouvez les organiser dans [!UICONTROL Portfolios] et [!UICONTROL Programmes]. Pour définir d’autres éléments qui vous aident à résoudre votre travail, vous souhaitez utiliser d’autres objets stockés sous [!UICONTROL Projets], [!UICONTROL Tâche], [!UICONTROL Problèmes], ou [!UICONTROL Portfolios], comme [!UICONTROL Documents], [!UICONTROL Mises à jour], [!UICONTROL Heures], [!UICONTROL Utilisateurs], ou [!UICONTROL Rôles de tâche].

[!UICONTROL Rapports] et [!UICONTROL Tableaux de bord] sont un autre exemple d’objets qui peuvent vous aider à organiser la quantité de données dans [!DNL Workfront] visuellement, pour le rendre facilement accessible à tous les utilisateurs.

Pour obtenir la liste complète des objets de la section [!DNL Workfront], voir [Explorateur d’API](../../../wf-api/general/api-explorer.md).

## Interdépendance et hiérarchie des objets

Les objets sont liés les uns aux autres dans [!UICONTROL Workfront]. Par exemple, une tâche ou un problème ne peut jamais exister indépendamment en dehors d’un projet. [!UICONTROL Tâche] et [!UICONTROL Problèmes] sont des exemples d’objets stockés dans la variable [!UICONTROL project] . [!UICONTROL Tâche] et [!UICONTROL Problèmes] sont considérés comme des objets enfants des projets.

Voici quelques-uns des objets les plus couramment utilisés dans [!DNL Workfront] et leurs objets parents et enfants respectifs :

| **Objet** | **Objets parents** | **Objets enfant** |
|---|---|---|
| [!UICONTROL Portefeuilles] |  | [!UICONTROL Programmes], [!UICONTROL Projets], [!UICONTROL Documents], [!DNL Notes], [!UICONTROL Utilisateurs] |
| [!UICONTROL Programmes] | [!UICONTROL Portefeuilles] | [!UICONTROL Projets], [!UICONTROL Documents], [!UICONTROL Remarques], [!UICONTROL Utilisateurs] |
| [!UICONTROL Projets] | [!UICONTROL Portfolios], [!UICONTROL Programmes] | [!UICONTROL Tâche], [!UICONTROL Problèmes], [!UICONTROL Documents], [!UICONTROL Remarques], [!UICONTROL Heures], [!UICONTROL Utilisateurs] |
| [!UICONTROL Tâches] | [!UICONTROL Projets] | [!UICONTROL Problèmes], [!UICONTROL Tâches Enfants], [!UICONTROL Documents], [!UICONTROL Remarques], [!UICONTROL Heures], [!UICONTROL Utilisateurs] |
| [!UICONTROL Événements] | [!UICONTROL Tâche], [!UICONTROL Projets] | [!UICONTROL Documents], [!UICONTROL Remarques], [!UICONTROL Heures], [!UICONTROL Utilisateurs] |
| [!UICONTROL Tableaux de bord] |  | [!UICONTROL Rapports], Pages externes |
| [!UICONTROL Rapports] | [!UICONTROL Tableaux de bord] |  |
| [!UICONTROL Groupes] |  | [!UICONTROL Utilisateurs ou utilisatrices] |
| [!UICONTROL Équipes] |  | [!UICONTROL Utilisateurs ou utilisatrices] |
| [!UICONTROL Utilisateurs ou utilisatrices] | [!UICONTROL Groupes], [!UICONTROL Équipes], [!UICONTROL Entreprises] | [!UICONTROL Rôles de tâche] |
| [!UICONTROL Entreprises] |  | [!UICONTROL Utilisateurs ou utilisatrices] |
| [!UICONTROL Documents] | [!UICONTROL Tâche], [!UICONTROL Problèmes], [!UICONTROL Projets], [!UICONTROL Portfolios], [!UICONTROL Programmes], [!UICONTROL Utilisateurs] |  |
| [!UICONTROL Formules]* |  | [!UICONTROL Initiatives] |
| [!DNL Goals]* |  | [!UICONTROL Résultats], [!UICONTROL Activités] |

Pour obtenir la liste complète des objets de la section [!DNL Workfront], voir [Explorateur d’API](../../../wf-api/general/api-explorer.md).

*Les plans sont l’objet de la [!DNL Adobe Workfront Scenario Planner]. Pour plus d’informations sur la variable [!DNL Scenario Planner], voir [La variable [!UICONTROL Planification du scénario] aperçu](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Objectifs] sont les objets de [!DNL Adobe Workfront Goals]. Pour plus d’informations sur [!DNL Workfront Goals], voir [[!DNL Adobe Workfront Goals] aperçu](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Personnalisation des noms d’objet

Comme [!DNL Workfront] , vous pouvez personnaliser les noms d’objet dans [!DNL Workfront] en utilisant une [!UICONTROL Modèle de mise en page].

Pour plus d’informations sur la personnalisation des noms d’objet à l’aide d’une  [!UICONTROL Modèle de mise en page], voir [Création et gestion des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Une fois que vous avez personnalisé un modèle de mise en page et que vous l’avez attribué aux utilisateurs, ces derniers voient les noms personnalisés des objets. Les utilisateurs qui ont été affectés au modèle de mise en page ne voient plus les noms par défaut des objets, n’importe où dans l’application web.

Par exemple, si la plus grande partie du travail effectué dans votre organisation est appelée &quot;Engagement&quot;, vous pouvez remplacer le nom &quot;&quot;.[!UICONTROL Projet]&quot; avec &quot;Engagement&quot;. Votre [!DNL Workfront] L’interface affiche &quot;Engagement&quot; au lieu de &quot;[!UICONTROL Projet]&#39; partout où le nom &#39;[!UICONTROL Projet]&quot; s’affiche.

>[!NOTE]
>
>Pour que les nouveaux noms des objets soient visibles par vos utilisateurs, ils doivent se déconnecter et se reconnecter à [!DNL Workfront] après avoir enregistré la variable  [!UICONTROL Modèle de mise en page].

>[!IMPORTANT]
>
>La variable [!DNL Workfront] La documentation fait toujours référence aux noms par défaut des objets. Comme [!DNL Workfront] administrateur, assurez-vous d’informer les utilisateurs des modifications apportées aux noms d’objet afin qu’ils puissent comprendre comment utiliser la variable [!DNL Workfront] la documentation, ainsi que les zones des applications qui ne reflètent pas les modifications apportées au nom des objets.

* [Noms d’objet qui peuvent être personnalisés à l’aide d’une  [!UICONTROL Modèle de mise en page]](#object-names-that-can-be-customized-using-a-layout-template)
* [Zones [!DNL Workfront] qui reflètent les noms d’objet personnalisés](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Zones [!DNL Workfront] qui ne reflètent pas les noms d’objet personnalisés](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Noms d’objet qui peuvent être personnalisés à l’aide d’une [!UICONTROL Modèle de mise en page]

Comme [!DNL Workfront] , vous pouvez personnaliser les noms des objets suivants pour qu’ils correspondent à la terminologie de votre entreprise :

* [!UICONTROL Portfolio]
* [!UICONTROL Programme]
* [!UICONTROL Projet]
* [!UICONTROL Tâche]
* [!UICONTROL Problème]
* [!UICONTROL Objectif]*
* [!UICONTROL Résultat]*
* [!UICONTROL Activité]*

  *[!UICONTROL Objectifs], [!UICONTROL résultats], et [!UICONTROL activités] ne sont disponibles que si votre société a acheté [!DNL Workfront Goals]. Pour plus d’informations sur [!DNL Workfront Goals], voir [[!DNL Adobe Workfront Goals] aperçu](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Initiative]**
* [!UICONTROL Scénario]**
* [!UICONTROL Planifier]**

  **[!UICONTROL Initiatives], [!UICONTROL scénarios], et [!UICONTROL plans] sont disponibles uniquement si votre société a acheté la variable [!DNL Workfront Scenario Planner]. Pour plus d’informations sur la variable [!DNL Scenario Planner], voir [Prise en main de la fonction [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).



Pour plus d’informations sur la personnalisation des noms d’objet à l’aide de  [!UICONTROL Modèles de mise en page], voir [Création et gestion des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Vous ne pouvez pas personnaliser les noms d’un autre objet dans Workfront. Pour obtenir la liste complète des objets de la section [!DNL Workfront], voir [Explorateur d’API](../../../wf-api/general/api-explorer.md).

Lorsque vous personnalisez le nom d’un objet, le nouveau nom s’affiche dans la plupart des zones de la variable [!DNL Workfront] application dans laquelle ce nom d’objet s’affiche.

### Zones [!DNL Workfront] qui reflètent les noms d’objet personnalisés

Les zones suivantes indiquent le nom mis à jour des objets :

* Barre de navigation supérieure
* Toutes les sections dans la navigation du panneau de gauche
* Tous les menus
* Notifications in-app
* Éléments de Report Builder et de rapport (vues, filtres et regroupements)
* [!UICONTROL Enregistrer] boutons
* Fichiers exportés
* E-mails
* Applications mobiles

### Zones [!DNL Workfront] qui ne reflètent pas les noms d’objet personnalisés

Les zones suivantes n’affichent pas le nom mis à jour des objets :

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] Module complémentaire

### Implications de la personnalisation des noms d’objet

Lorsque vous personnalisez des noms d’objet dans [!DNL Workfront]:

* Vous pouvez rencontrer des erreurs de syntaxe ou de grammaire dans les affichages du système. Par exemple, si vous renommez &quot;[!UICONTROL Problème]&quot; à &quot;Requête&quot; et vous voyez partout dans le système l’expression &quot;Une requête&quot;, qui fonctionne comme prévu et ne doit pas être considéré comme un bogue.
* Les noms personnalisés des objets ne sont pas traduisibles. Seule la variable [!DNL Workfront] les noms par défaut peuvent être traduits dans les langues prises en charge. Pour plus d’informations sur les langues prises en charge dans [!DNL Workfront], voir [Langues prises en charge dans [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). Les champs de nom d’objet personnalisé prennent en charge les caractères étrangers afin que vous puissiez saisir la terminologie dans n’importe quelle langue.
* Lorsque vous personnalisez des noms d’objet à l’aide d’une  [!UICONTROL Modèle de mise en page], il est recommandé d’affecter à la variable  [!UICONTROL Modèles de mise en page] en fonction de vos unités opérationnelles (équipes ou groupes).\
   Nous vous recommandons d’utiliser des noms clairement compris par les utilisateurs de ces unités afin d’éviter toute confusion.
* Les notifications électroniques et les rapports distribués contiennent toujours des noms d’objet tels que définis par  [!UICONTROL Modèle de mise en page] de l’utilisateur qui génère l’email. Vos utilisateurs doivent être prêts à voir dans leurs emails des noms d’objet qui ne sont pas liés à leur groupe ou équipe, s’ils reçoivent des notifications par e-mail d’utilisateurs d’autres équipes et groupes.\
   Comme [!DNL Workfront] administrateur, conseille aux utilisateurs de noter les icônes associées à chaque objet. Les icônes restent cohérentes entre les différents noms d’objet et cohérentes avec l’objet par défaut, tel qu’il apparaît dans la base de données. Pour obtenir une liste de tous les [!DNL Workfront] icônes associées aux objets, voir [Icônes d’objet](#object-icons).

  >[!TIP]
  >
  >Pour les tâches courantes de votre entreprise, pensez à créer une documentation personnalisée reflétant votre terminologie.

## Icônes d’objet

La variable [!DNL Workfront] La documentation fait toujours référence aux noms par défaut des objets. Si vos noms d’objet ont été personnalisés, vous pouvez vous fier à l’icône qui leur est associée pour déterminer à quel objet personnalisé correspond ce qui [!DNL Workfront] objet par défaut.

Pour plus d’informations sur les objets qui peuvent avoir des noms personnalisés dans [!DNL Workfront], voir [Noms d’objet qui peuvent être personnalisés à l’aide d’une  [!UICONTROL Modèle de mise en page]](#object-names-that-can-be-customized-using-a-layout-template).

Vous trouverez ci-dessous une liste d’objets et leurs icônes correspondantes dans Workfront.

| **Objet** | **Icône** | **Nom d’objet personnalisable** |
|---|---|---|
| [!UICONTROL Société] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Tableau de bord] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Objectif] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Groupe] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Problème] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Rôle de tâche] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Planifier] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Programme] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Projet] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Rapport] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Tâche] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Équipe] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Modèle] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |
| [!UICONTROL Utilisateur] | ![](assets/users-icon-gray.png) , ![](assets/user-icon-blue.png) , ![](assets/user-icon-initials.png) , ![](assets/user-avatar.png) , ![](assets/user-main-menu-area.png) |  |

## Nombre de références d’objets

Chaque objet créé dans [!DNL Workfront] se voit attribuer un numéro de référence unique. Les numéros de référence sont utiles pour distinguer deux objets similaires (par exemple, des tâches portant le même nom). Vous pouvez rechercher des objets à l’aide de leur numéro de référence et les inclure dans les rapports.

Pour plus d’informations sur la recherche d’objets par numéro de référence, voir [Utilisation du numéro de référence des objets](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Recherches spécifiques à un objet

Vous pouvez rechercher dans tous les objets pouvant faire l’objet de recherches dans [!DNL Workfront]ou vous pouvez sélectionner un objet spécifique à rechercher dans vos recherches de base et avancées.

Tous les objets ne peuvent pas faire l’objet de recherches dans [!DNL Workfront]. Vous pouvez exécuter des recherches de base et avancées pour les objets suivants dans [!DNL Workfront]:

| **Objet** | **Recherche de base** | **Recherche avancée** |
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
| [!UICONTROL Remarques] (ou [!UICONTROL Mises à jour]) | ✓ |  |

Pour plus d’informations sur l’exécution de recherches de base et avancées dans [!DNL Workfront], voir [Rechercher [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).


## Accès limité aux objets

Lorsqu’un utilisateur n’a pas accès à un objet, il voit &quot;Aucun accès&quot; partout où ce nom s’affiche dans Workfront.

L’accès aux objets peut être limité au niveau d’accès ou dans les autorisations d’un objet spécifique.

Cela s’applique à tous les objets et aux objets enfants répertoriés dans la variable [Interdépendance et hiérarchie des objets](#interdependency-and-hierarchy-of-objects) dans cet article. Cela ne s’applique pas aux objets Equipe et Utilisateur.

## Rapport sur les objets

Il est extrêmement important de comprendre la hiérarchie et l’interdépendance des objets avant de commencer à créer des rapports dans [!DNL Workfront]. Les rapports sont spécifiques à un objet. Vous devez sélectionner l’objet correct pour votre rapport avant de pouvoir afficher les données de votre choix.

>[!IMPORTANT]
>
>Vous ne pouvez créer un rapport que sur l’objet sélectionné et les objets parents du même rapport. Vous ne pouvez pas avoir d’informations sur les objets enfants dans un rapport d’objet parent. Vous pouvez, par exemple, afficher les informations d’un projet dans un rapport de tâche, mais pas les informations d’une tâche dans un rapport de projet.

Vous pouvez créer des rapports sur tous les objets de la base de données à l’aide de notre API ouverte. Pour obtenir la liste complète de tous les objets de la base de données, voir [Explorateur d’API](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
> * Si vous avez personnalisé les noms de vos objets à l’aide d’un modèle de mise en page, les noms de l’objet dans le créateur de rapports ont également été personnalisés. Assurez-vous de connaître les objets qui ont été personnalisés et recherchez leur nom dans le créateur de rapports. Pour plus d’informations sur les objets qui peuvent avoir des noms personnalisés dans [!DNL Workfront], voir [Noms d’objet qui peuvent être personnalisés à l’aide d’une  [!UICONTROL Modèle de mise en page]](#object-names-that-can-be-customized-using-a-layout-template) dans cet article.
> * Lorsque vous utilisez le mode texte dans vos rapports, les noms des objets dans les expressions du mode texte sont les noms standard dans [!DNL Workfront], et non les noms d’objet personnalisés. Pour plus d’informations sur l’utilisation du mode texte dans les rapports, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Pour plus d’informations sur notre API, voir [Explorateur d’API](../../../wf-api/general/api-explorer.md).

### Objets disponibles pour les rapports

Vous pouvez créer des rapports sur les objets suivants lors de l’utilisation du créateur de rapports dans la variable [!DNL Workfront] application web. Les puces avec retrait donnent plus d’informations sur l’objet et ne représentent pas d’objets supplémentaires.

* [!UICONTROL Projet]
* [!UICONTROL Tâche]
* [!UICONTROL Heure]
* [!UICONTROL Problème]
* [!UICONTROL Utilisateur]
* [!UICONTROL Accès] Niveau
* [!UICONTROL Validation]
* [!UICONTROL Processus d’approbation]
* [!UICONTROL Attribution]
* [!UICONTROL Ligne de base]
* [!UICONTROL Tâche de ligne de base]
* [!UICONTROL Enregistrement de facturation]
* [!UICONTROL Heure budgétée]
   * Il s’agit de la variable [!UICONTROL Heures budgétées], comme ils apparaissent dans les anciens outils de gestion des ressources obsolètes.
   * Le &quot;Bud. Heures&quot; dans le champ [!UICONTROL Heure budgétée] fait référence aux heures prévues pour les rôles de tâche dans le rapport [!UICONTROL Resource Planner]. Pour plus d’informations, voir [Comprendre [!UICONTROL Coût de la main-d&#39;oeuvre budgétisé] et [!UICONTROL Heures budgétées] pour les projets](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Événement de calendrier]
* [!UICONTROL Société]
* [!UICONTROL Formulaire personnalisé]
* [!UICONTROL Tableau de bord]
* [!UICONTROL Document]
* [!UICONTROL Approbation de document]
* [!UICONTROL Version du document]
   * Vous pouvez afficher des informations sur la version du document, le document auquel la version est associée, qui a créé la version et l’utilisateur qui a créé le BAT sur la version du document, le cas échéant (Créateur de BAT).
* [!UICONTROL Modèle de courrier électronique]
* [!UICONTROL Dépense]
* [!UICONTROL Type de dépense]
* [!UICONTROL Page externe]
* [!UICONTROL Favori]
* [!UICONTROL Filtrer]
* [!UICONTROL Objectif]
   * Vous pouvez créer un rapport pour les objectifs stratégiques ou afficher des informations relatives aux objectifs dans un rapport de projet lorsque les projets sont associés aux objectifs en tant qu’activités d’objectif. Vous pouvez créer des objectifs stratégiques et connecter des projets uniquement si votre entreprise a acheté une [!DNL Workfront Goals] licence. Pour plus d’informations sur [!DNL Workfront Goals], voir [[!DNL Workfront Goals] aperçu](../../../workfront-goals/goal-management/wf-goals-overview.md). Pour plus d’informations sur la connexion des projets aux objectifs stratégiques, voir [Ajout de projets aux objectifs dans les objectifs Adobe Workfront](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).
*Vous ne pouvez pas créer de rapports sur les objectifs de projet associés à un [!UICONTROL Analyse de cas]. Pour plus d’informations sur les objectifs du projet par rapport aux objectifs stratégiques, voir [Glossaire [!DNL Adobe Workfront] terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Groupe]
* [!UICONTROL Regroupement]
* [!UICONTROL Type d’heure]
* [!UICONTROL Initiative]
   * Vous pouvez créer un rapport pour les initiatives qui sont des objets enfants d’un plan uniquement si votre entreprise a acheté un [!DNL Workfront Scenario Planner] licence. Pour plus d’informations sur les initiatives, voir [Aperçu des initiatives dans la section [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).

* Fonction d&#39;initiative
   * Vous pouvez créer un rapport pour les rôles de tâche associés aux initiatives d’un plan uniquement si votre société a acheté une [!DNL Workfront Scenario Planner] licence. Pour plus d’informations sur la création d’initiatives et leur association à des rôles de tâche, voir [Créez et modifiez des initiatives dans le [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).

* [!UICONTROL Itération]
* [!UICONTROL Rôle de tâche]
* [!UICONTROL Entrée du journal]
   * Vous pouvez créer des rapports sur les mises à jour système suivies dans la variable [!UICONTROL Mises à jour] zone d’objets tels que les tâches, les projets, les problèmes, etc. Pour plus d’informations, voir [Rapport sur les [!UICONTROL Mises à jour] area](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Modèle de mise en page]
* [!UICONTROL Milestone]
* [!UICONTROL Chemin Milestone]
* [!UICONTROL Remarque] ou [!UICONTROL Mises à jour]
   * Vous pouvez créer des rapports sur les commentaires ajoutés par des utilisateurs individuels.

* [!UICONTROL Paramètre] (ou [!UICONTROL Champ personnalisé])
* [!UICONTROL Groupe de paramètres] (ou [!UICONTROL Saut de section])
* [!UICONTROL Portfolio]
* [!UICONTROL Programme]
* [!UICONTROL Projet (données financières)]
   * Les informations financières sont renseignées dans [!UICONTROL Projet (données financières)] ne signale que lorsque les données qui y sont associées ont moins de 5 ans. Par exemple, si un rôle d’emploi a été attribué à une tâche en janvier 2015 et que nous sommes aujourd’hui septembre 2021, un secteur financier comme le [!UICONTROL Date d’affectation] pour le rôle de tâche ne s’affiche pas dans la variable [!UICONTROL Projet (données financières)] rapport.

  >[!CAUTION]
  >
  >L’exécution d’un rapport Projet (données financières) permet de recalculer les données financières, ce qui peut entraîner une surcharge des données financières précédentes et nécessiter un temps important. Pour plus d’informations sur les conséquences du recalcul des données financières, voir [Recalculer les finances du projet](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md).

* [!UICONTROL Approbation d&#39;épreuve]
   * Vous permet de consulter différentes informations sur la validation du BAT, notamment : le BAT qui a été soumis à validation, des informations sur le [!UICONTROL Approbateur], informations sur le demandeur (si le demandeur est titulaire d’une licence [!DNL Workfront] (utilisateur), les informations de version, l’ID de BAT et la date de création du BAT.\
      [!UICONTROL Approbation du BAT] Les rapports incluent uniquement les bons à tirer disponibles dans les zones Mon travail des utilisateurs où des décisions n’ont pas encore été prises.\
   * Les validations de BAT sont affectées dans [!DNL Workfront] comme décrit [Ajout d’utilisateurs à un BAT](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Partage d’un BAT dans [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL File d’attente]
* [!UICONTROL Rubrique de la file d’attente]
* [!UICONTROL Rate] (affiche ainsi le rôle de tâche [!UICONTROL Taux de facturation] information)
* [!UICONTROL Notification de rappel]
* [!UICONTROL Rapport]
* [!UICONTROL Pool de ressources]
* [!UICONTROL Risque]
* [!UICONTROL Type de risque]
* [!UICONTROL Planning]
* [!UICONTROL Fiche d’évaluation]
* [!UICONTROL Équipe]
* [!UICONTROL Modèle]
* [!UICONTROL Tâche du modèle]
* [!UICONTROL Heure de désactivation]
   * Vous pouvez créer des rapports sur le temps de pause d’un utilisateur comme indiqué par celui-ci dans son profil.

* [!UICONTROL Feuille de temps]
* [!UICONTROL Profil de feuille de calcul]
* [!UICONTROL Groupe de rubriques]
* [!UICONTROL Approbation des utilisateurs]
* [!UICONTROL Délégation d’utilisateurs]

   * Vous pouvez créer des rapports sur les utilisateurs qui ont été délégués pour effectuer les tâches et les problèmes d’autres utilisateurs lorsqu’ils sont absents du bureau. Ce rapport présente l’utilisateur absent du bureau ainsi que l’utilisateur qui remplit ses fonctions lorsqu’il est absent.

* [!UICONTROL Décisions des utilisateurs]

   * Vous pouvez créer un rapport sur le nombre de décisions que les utilisateurs ont prises sur les bons à tirer et les documents au cours du mois en cours.

* [!UICONTROL Afficher]
* [!UICONTROL Élément de travail] (produit un rapport pour les tâches et les problèmes)
