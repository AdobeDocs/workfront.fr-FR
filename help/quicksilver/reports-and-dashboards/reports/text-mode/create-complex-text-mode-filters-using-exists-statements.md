---
product-area: reporting
navigation-topic: text-mode-reporting
title: Création de filtres de mode de texte complexes à l’aide d’instructions EXISTS
description: Vous pouvez créer des filtres de mode Texte complexes à l’aide d’instructions EXISTS. Cet article nécessite une compréhension approfondie de l’API Adobe Workfront et de l’interface de création de rapports en mode texte.
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 09492b2657aaf599bb31a19329d5de23791b66ec
workflow-type: tm+mt
source-wordcount: '2649'
ht-degree: 0%

---

# Création de filtres de mode de texte complexes à l’aide d’instructions EXISTS

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>Cet article nécessite une compréhension approfondie de l’API Adobe Workfront et de l’interface de création de rapports en mode texte. Pour plus d’informations sur l’API Workfront, voir [Principes de base des API](../../../wf-api/general/api-basics.md).\
>Pour plus d’informations sur l’utilisation du mode texte, voir [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Présentation des relations d’objet dans Workfront

Tous les objets sont liés à d’autres objets de la base de données Workfront.

La compréhension de la hiérarchie et de l’interdépendance des objets permet de déterminer les objets qui peuvent être référencés dans les rapports.

Pour plus d’informations sur les objets de Workfront et sur leur hiérarchie et leur interdépendance, voir [Présentation des objets Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Lors de la création de filtres, vous pouvez référencer d’autres objets connectés à l’objet du filtre dans un rapport allant jusqu’à 2 niveaux à l’aide de l’interface de création de rapports standard.

Par exemple, vous pouvez référencer l’ID de Portfolio dans un filtre de problèmes pour afficher uniquement les problèmes sur les projets associés à un certain portfolio à l’aide de l’interface standard. Dans ce cas, le portefeuille est à 2 niveaux des problèmes.

Cependant, vous ne pouvez pas référencer le propriétaire du Portfolio dans un filtre de problèmes à l’aide de l’interface standard pour afficher uniquement les problèmes provenant de projets associés à des portefeuilles dont le propriétaire est un utilisateur spécifique. Vous devez utiliser le mode texte pour accéder au champ Nom du propriétaire du Portfolio, qui se trouve à trois niveaux des problèmes.

![Problème lié aux icônes des propriétaires de portefeuille](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

Pour obtenir la liste complète des objets dans Workfront, reportez-vous à la section [Explorateur d’API](../../../wf-api/general/api-explorer.md).

Pour plus d’informations sur la navigation dans l’explorateur d’API et la recherche d’objets, voir [Utilisation de l’explorateur d’API](../../../wf-api/general/using-api-explorer.md).

Lors de la création de filtres, vous devez créer des instructions complexes dans l’interface du mode texte pour référencer ces types d’objets.

Pour plus d’informations sur la création de filtres complexes, voir [Présentation des filtres de mode texte complexes qui utilisent des instructions EXISTS](#overview-of-complex-text-mode-filters-that-use-exists-statements) de cet article.

## Présentation des filtres de mode de texte complexes qui utilisent des instructions EXISTS {#overview-of-complex-text-mode-filters-that-use-exists-statements}

Tenez compte des points suivants lors de la création de filtres qui s’étendent sur plusieurs niveaux dans la hiérarchie d’objets ou qui filtrent les objets manquants :

* Vous devez créer des filtres complexes lorsque vous souhaitez référencer des objets qui ne sont pas directement connectés à l’objet de filtre.
* Vous devez utiliser une instruction EXISTS pour effectuer les opérations suivantes :

   * Créez des filtres qui s’étendent sur plusieurs niveaux.
   * Créez des filtres qui recherchent les objets manquants.\
     Par exemple, lors de la création d’un rapport d’utilisateur, vous pouvez filtrer les utilisateurs qui n’ont pas effectué de journalisation pendant une certaine période.

Tenez compte des règles suivantes lors de l’utilisation d’instructions EXISTS dans un filtre :

* Vous pouvez référencer trois objets dans un filtre EXISTS :

   * Objet du filtre (objet original).
   * Objet dont vous souhaitez référencer le champ (objet cible).
   * Objet qui connecte les objets d’origine et de cible s’ils ne sont pas directement connectés les uns aux autres (objet de liaison).

* Les filtres qui utilisent EXISTS contiennent deux instructions distinctes liées par un signe égal :

   * L’instruction précédant le signe égal fait référence à l’objet auquel vous faites référence (la liaison ou l’objet cible).
   * L’instruction située après le signe égal fait référence à l’objet à partir duquel vous faites référence (l’objet d’origine).

* Vous devez utiliser le code d’objet de l’objet de liaison pour connecter vos instructions.\
  Vous trouverez le code d’objet de tous les objets dans l’explorateur d’API.\
  Pour plus d’informations sur l’explorateur d’API, voir [Explorateur d’API](../../../wf-api/general/api-explorer.md).

* Lorsqu’un objet de liaison est manquant car les objets d’origine et de cible sont directement connectés les uns aux autres, vous pouvez utiliser le code d’objet de l’objet cible au lieu de l’objet de lien.
* Vous pouvez faire référence à plusieurs champs (champs cibles) sur le même objet (objet cible), auquel cas vous devez connecter les lignes faisant référence aux champs par AND.\
  Pour un exemple de filtrage de plusieurs champs appartenant à l’objet cible, reportez-vous à la section [Exemple 4 : filtrer par plusieurs champs : tâches par nom de propriétaire du Portfolio et identifiant de la Fiche d’évaluation d’alignement des Portfolios](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) dans cet article.

* Le seul modificateur pris en charge pour une instruction EXISTS est NOTEXISTS.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification des filtres dans un rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport pour modifier des filtres dans un rapport</p> <p>Gérer les autorisations d’un filtre pour le modifier</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Créez des filtres de mode de texte complexe qui s’étendent sur plusieurs niveaux dans la hiérarchie d’objets.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

Vous pouvez créer un filtre qui référence des objets à plusieurs niveaux de la hiérarchie d’objets dans laquelle l’objet de filtre existe. Par exemple, vous pouvez créer un filtre de problèmes pour les problèmes qui se trouvent sur des projets qui ne sont pas associés à un certain propriétaire de Portfolio.

Vous devez toujours utiliser une instruction EXISTS et l’interface du mode texte pour créer ce filtre.

Pour obtenir des exemples de filtres, reportez-vous à la section [Exemple 1 : filtre pour les problèmes par nom de propriétaire de Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) dans cet article.

Pour créer un filtre couvrant plusieurs niveaux dans la hiérarchie d’objets :

1. Identifiez l’objet de votre filtre. Nous appelons cet objet l’objet d’origine.\
   Par exemple, Problème.

1. Identifiez le champ en fonction duquel vous souhaitez filtrer les données. Nous appelons cet objet le champ cible qui appartient à un objet cible.\
   Par exemple, le champ propriétaireID (champ cible), qui appartient à Portfolio (objet cible).

1. (Conditionnel) Si l’objet d’origine (problème) et le champ cible (propriétaireID) ne sont pas directement connectés l’un à l’autre, vous devez trouver un troisième objet, un objet de liaison (projet) qui les connecte. L’objet de liaison doit comporter au moins un champ qui est référencé à partir des onglets Champs ou Références de l’objet d’origine (Champ de liaison affiché sur l’objet d’origine). Il doit également comporter un champ de liaison vers l’objet cible affiché dans les onglets Champs ou Références de l’objet de liaison. Le champ Liaison vers l’objet cible qui s’affiche sur l’objet de liaison (ou le champ de liaison affiché sur l’objet de liaison) doit correspondre au champ cible.

   Par exemple, l’ID (projet) (champ de liaison affiché sur l’objet d’origine) est référencé à partir de Problèmes (objet d’origine). (Portfolio) ownerID (Association du champ à l’objet cible) s’affiche dans l’onglet Champs du projet (association de l’objet). PropriétaireID du Portfolio est également un champ de l’objet cible (Portfolio). Le champ Liaison de l’objet de liaison correspond au champ cible.\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. À l’aide de l’explorateur d’API, identifiez la variable **Code objet** de l’objet de liaison (projet).\
   Par exemple, le code d’objet du projet est PROJ.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. Créez un filtre pour l’objet original.\
   Par exemple, créez un filtre Problème .\
   Pour plus d’informations sur la création de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Cliquez sur **Passer en mode Texte**.
1. Collez l’exemple de formule suivant dans l’interface du mode texte du nouveau filtre et remplacez l’exemple de texte par les objets et les champs appropriés :

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>`

   `EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>`

   Pour un exemple utilisant les champs que nous avons identifiés ci-dessus, reportez-vous à la section [Exemple 1 : filtre pour les problèmes par nom de propriétaire de Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) dans cet article.

1. Cliquez sur **Enregistrer le filtre**.

## Création de filtres de mode texte complexes pour les objets manquants

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

Vous pouvez créer un filtre qui référence les objets manquants. Par exemple, vous pouvez créer un filtre utilisateur qui indique les utilisateurs qui n’ont pas effectué d’heures de connexion dans Workfront.

Vous devez toujours utiliser un *EXISTE* et l’interface du mode texte pour créer ce filtre.

Pour des exemples de filtres pour les objets manquants, reportez-vous aux sections suivantes de cet article :

* [Exemple 2 : filtrer les objets manquants : champs personnalisés qui n’apparaissent dans aucun formulaire personnalisé](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Exemple 3 : filtre pour les objets manquants : utilisateurs qui n’ont pas consigné de temps pendant une certaine période](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

Pour créer un filtre qui référence les objets manquants :

1. Identifiez l’objet de votre filtre. Nous appelons cet objet l’objet d’origine.\
   Par exemple, Paramètre ou Champ personnalisé.

1. Identifiez le champ en fonction duquel vous souhaitez filtrer les données. Nous appelons cet objet le champ cible qui appartient à un objet cible.\
   Par exemple, le champ categoryID (champ cible), qui appartient à la catégorie (objet cible).

1. Puisque l’objet d’origine (paramètre) et le champ cible (ID de catégorie) ne sont pas directement connectés l’un à l’autre, vous devez trouver un troisième objet, un objet de liaison (un paramètre de catégorie), qui les connecte. L’objet de liaison doit comporter au moins un champ qui est référencé à partir des onglets Champs ou Références de l’objet d’origine (Champ de liaison affiché sur l’objet d’origine). Il doit également comporter un champ de liaison vers l’objet cible affiché dans les onglets Champs ou Références de l’objet de liaison. Le champ Liaison vers l’objet cible qui s’affiche sur l’objet de liaison (ou le champ de liaison affiché sur l’objet de liaison) doit correspondre au champ cible.

   Par exemple, l’identifiant du paramètre de catégorie (champ de liaison affiché sur l’objet d’origine) est référencé à partir du paramètre (objet d’origine). parameterID (liaison de champ à l’objet cible) s’affiche dans l’onglet Champs du paramètre de catégorie (liaison d’objet). Le champ Liaison à l’objet cible qui s’affiche sur l’objet de liaison correspond au champ cible.

1. À l’aide de l’explorateur d’API, identifiez la variable **Code objet** de l’objet de liaison (paramètre de catégorie).\
   Par exemple, le code d’objet pour le paramètre de catégorie est CTGYPA.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. Créez un filtre pour l’objet original.\
   Par exemple, créez un filtre Paramètre .\
   Pour plus d’informations sur la création de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Cliquez sur **Passer en mode Texte**.
1. (Conditionnel) Si vous filtrez les objets manquants, collez l’exemple de formule suivant dans l’interface du mode texte du nouveau filtre et remplacez le texte d’exemple par les objets et les champs appropriés :

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

   Pour un exemple de création de rapports sur les champs personnalisés qui ne sont pas associés à Forms personnalisé, reportez-vous à la section [Exemple 2 : filtrer les objets manquants : champs personnalisés qui n’apparaissent dans aucun formulaire personnalisé](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) dans cet article.

1. Cliquez sur **Enregistrer le filtre**.

## Exemples de filtres de mode texte s’étendant sur plusieurs niveaux dans la hiérarchie d’objets

Utilisez ces exemples pour créer des filtres de mode texte avec des instructions EXISTS.

### Exemple 1 : filtre pour les problèmes par nom de propriétaire de Portfolio {#example-1-filter-for-issues-by-portfolio-owner-name}

À l’aide de l’interface du mode texte, vous pouvez créer un filtre pour une liste de problèmes afin d’afficher uniquement les problèmes qui concernent des projets associés à un portfolio dont le propriétaire est un utilisateur spécifique.

Pour filtrer les problèmes selon le nom du propriétaire du Portfolio :

1. Créez un filtre Problème .\
   Pour plus d’informations sur la création de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Cliquez sur **Passer en mode Texte**.
1. Reportez-vous au code générique suivant :

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>`

1. Collez le code suivant dans le **Définition de règles de filtrage pour votre rapport** zone pour remplacer le code générique ci-dessus :

   `EXISTS:A:$$OBJCODE=PROJ`

   `EXISTS:A:ID=FIELD:projectID`

   `EXISTS:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221`

   >[!NOTE]
   >
   >* L’objet original est l’objet du rapport : Problème
   >* L’objet cible est Portfolio.
   >* L’objet de liaison est Projet.
   >* Le champ cible et le champ de liaison à l’objet cible référencé à partir de l’objet de liaison sont ownerID.
   >* Le code objet de l’objet de liaison ici est PROJ.
   >* Le champ de liaison affiché sur l’objet d’origine est projectID et le champ de liaison est ID.

1. Remplacez la valeur du champ cible (propriétaireID) dans la dernière instruction par un ID utilisateur de votre environnement.
1. Cliquez sur **Enregistrer le filtre**.

### Exemple 2 : filtrer les objets manquants : champs personnalisés qui n’apparaissent dans aucun formulaire personnalisé {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

À l’aide de l’interface du mode texte, vous pouvez créer un filtre afin d’afficher les champs personnalisés (paramètres) qui ne sont pas associés à la Forms personnalisée (catégories). Ce filtre lie les paramètres aux catégories, qui sont connectées via un autre objet, le paramètre de catégorie. Comme les deux champs ne sont pas directement connectés les uns aux autres et que vous filtrez les informations manquantes, vous devez utiliser une instruction EXISTS.

>[!IMPORTANT]
>
>Un paramètre est un champ tel qu’il existe dans la bibliothèque de champs référencée dans un formulaire personnalisé. Un paramètre de catégorie est la version d’un champ qui apparaît sur un formulaire spécifique. Par exemple, si le même champ apparaît sur 5 formulaires, il y aura 1 paramètre et 5 paramètres de catégorie dans la base de données Workfront.

Pour filtrer les champs personnalisés qui ne sont pas associés à un formulaire personnalisé :

1. Créez un filtre Paramètre ou Champ personnalisé .\
   Pour plus d’informations sur la création de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Cliquez sur **Passer en mode Texte**.
1. Reportez-vous au code générique suivant :

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

1. Collez le code suivant dans le **Définition de règles de filtrage pour votre rapport** zone pour remplacer le code générique ci-dessus :

   `EXISTS:A:$$OBJCODE=CTGYPA`

   `EXISTS:A:parameterID=FIELD:ID`

   `EXISTS:A:$$EXISTSMOD=NOTEXISTS`

   >[!NOTE]
   >
   >* L’objet d’origine est l’objet du rapport : Paramètre.
   >* L’objet cible est Catégorie.
   >* L’objet de liaison est un paramètre de catégorie.
   >* Le code objet de l’objet de liaison est CTGYPA.
   >* Le champ Lier à l’objet cible est parameterID, car parameterID existe à la fois dans le tableau Objet de liaison et dans le tableau Objet cible.
   >* Le champ de liaison affiché sur l’objet d’origine est l’identifiant (du paramètre de catégorie).

1. Cliquez sur **Enregistrer le filtre**.

### Exemple 3 : filtre pour les objets manquants : utilisateurs qui n’ont pas consigné de temps pendant une certaine période {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

À l’aide de l’interface du mode texte, vous pouvez créer un filtre afin d’afficher les utilisateurs qui n’ont pas consigné de temps pendant une certaine période. Ce filtre lie les utilisateurs aux heures, qui sont directement connectés les uns aux autres. Cependant, vous devez utiliser une instruction EXISTS et l’interface du mode texte pour pouvoir filtrer les informations manquantes.

Pour filtrer les utilisateurs qui n’ont pas effectué de journalisation au cours de la semaine précédente :

1. Créez un filtre Utilisateur .\
   Pour plus d’informations sur la création de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Cliquez sur **Passer en mode Texte**.
1. Reportez-vous au code générique suivant :

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

1. Collez le code suivant dans le **Définition de règles de filtrage pour votre rapport** zone pour remplacer le code générique ci-dessus :

   `EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

   >[!NOTE]
   >
   >* L’objet d’origine est l’objet du rapport : Utilisateur.
   >* L’objet cible est Heure.
   >* Dans cet exemple, vous n’avez pas besoin d’objet de liaison, car les utilisateurs et les heures sont directement connectés dans la base de données Workfront.
   >* Puisqu’il n’existe aucun objet de liaison, vous devez utiliser le code d’objet de l’objet cible : HEURE.
   >* Le champ Liaison à l’objet cible est ownerID (qui s’affiche sur l’objet d’origine ; l’objet de liaison est manquant).
   >* Le champ de liaison affiché sur l’objet d’origine est l’identifiant (de l’heure) (qui s’affiche sur l’objet cible ; l’objet de liaison est manquant).
   >* LES EXISTANTS:A:L’instruction entryDate fait référence aux champs qui définissent l’objet cible (heure) et qui utilisent la même syntaxe que dans une instruction de filtre ordinaire. Vous affichez ainsi uniquement les utilisateurs qui n’ont pas consigné de temps pendant une période spécifique, dans ce cas la semaine précédente.
   >* Le modificateur NOTEXISTS indique que nous recherchons des éléments (heures) qui n’existent pas pour l’objet du rapport (Utilisateurs).

1. Cliquez sur **Enregistrer le filtre**.

### Exemple 4 : filtrer par plusieurs champs : tâches par nom de propriétaire du Portfolio et identifiant de la Fiche d’évaluation d’alignement des Portfolios {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

À l’aide de l’interface du mode texte, vous pouvez créer un filtre qui fait référence à plusieurs champs de l’objet cible. Dans ce cas, les instructions de filtre qui font référence aux champs cibles doivent être connectées par AND.

Par exemple, vous pouvez filtrer une liste de tâches afin de n’afficher que les tâches qui répondent aux critères suivants :

* Ils se trouvent sur un projet associé à un portefeuille dont le propriétaire est un utilisateur spécifique.
* Ils se trouvent sur un projet associé à un portefeuille dont les projets ne sont pas associés à une fiche d’évaluation d’alignement spécifique.

Pour filtrer les tâches selon le nom du propriétaire du Portfolio et l’identifiant de la Fiche d’évaluation de l’alignement des Portfolios :

1. Créez un filtre Tâche .\
   Pour plus d’informations sur la création de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Cliquez sur **Passer en mode Texte**.
1. Collez le code suivant dans le **Définition de règles de filtrage pour votre rapport** area :

   `EXISTS:A:$$OBJCODE=PROJ`
   `EXISTS:A:ID=FIELD:projectID`
   `EXISTS:A:portfolio:ownerID=4d80ce5200000528787d57807732a33f`
   `AND:A:EXISTS:A:$$EXISTSMOD=NOTEXISTS`
   `AND:A:EXISTS:A:$$OBJCODE=PROJ`
   `AND:A:EXISTS:A:ID=FIELD:projectID`
   `AND:A:EXISTS:A:portfolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad`

   >[!NOTE]
   >
   >* L’objet d’origine est l’objet du filtre : Tâche.
   >* L’objet cible est Portfolio.
   >* Le premier champ cible est ownerID.
   >* Le deuxième champ cible est l’identifiant de la Fiche d’évaluation d’alignement.
   >* L’objet de liaison est Projet.
   >* Le code objet de l’objet de liaison est PROJ.
   >* Le champ Liaison à l’objet cible est l’identifiant (du Portfolio).
   >* Le champ de liaison affiché sur l’objet d’origine est projectID.
   >* Remplacez le propriétaireID par un ID utilisateur issu de votre environnement.

1. Cliquez sur **Enregistrer le filtre**.
