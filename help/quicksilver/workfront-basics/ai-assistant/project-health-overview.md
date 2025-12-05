---
title: Présentation de l’intégrité du projet
content-type: reference
description: La fonctionnalité d’intégrité du projet utilise la puissance de l’assistant d’IA pour vous donner instantanément une évaluation des performances de vos projets.
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
source-git-commit: b95be2e0917b53195ac327880a2ea7399c1485de
workflow-type: tm+mt
source-wordcount: '2060'
ht-degree: 4%

---

# Présentation de l’intégrité du projet

>[!IMPORTANT]
>
>La fonctionnalité d’intégrité du projet est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta.

La fonctionnalité d’intégrité des projets d’Adobe Workfront utilise la puissance de l’assistant d’IA pour vous donner instantanément une évaluation des performances de vos projets, des domaines nécessitant votre attention et de la manière d’éviter les problèmes qui peuvent vous coûter du temps et de l’argent.

L’assistant AI peut générer une évaluation de l’intégrité du projet pour les objets suivants :

* Un seul projet
* Un seul programme
* Projets multiples

Pour plus d’informations sur l’assistant AI, voir [Présentation de l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Sélectionner ou supérieur </p> 
<p>Workflow Select ou version ultérieure</p>
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td> 
<p>Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurations des niveaux d’accès</p></td> 
   <td><p>Vous devez être administrateur système pour gérer les configurations d’intégrité du projet </p>
   <p>Modifier l’accès aux projets pour appliquer les configurations d’intégrité des projets </p>
     <p>Afficher l’accès aux projets pour afficher les configurations d’intégrité du projet </p>
     <p>Afficher l’accès aux programmes pour utiliser Afficher l’intégrité du projet pour tous les projets d’un programme</p>
  </td> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td><p>Gérer les autorisations des projets pour appliquer les configurations d’intégrité du projet </p>
     <p>Afficher les autorisations des projets pour afficher les configurations d’intégrité du projet </p>
  </td> 
  </tr> 
  </tr>  
    </tr>  
</tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## S’inscrire à la version bêta de l’intégrité du projet

L’assistant AI doit être activé pour que votre entreprise puisse utiliser l’intégrité du projet.

Pour activer l’assistant AI et l’intégrité du projet pour votre organisation, toutes les conditions suivantes doivent s’appliquer :

* Votre organisation doit avoir migré vers le système Adobe Identity Management (IMS).
* Votre organisation doit disposer d’un package Workfront ou Workflow Select, Prime ou Ultimate.
* L’expérience unifiée Adobe doit être activée.
* Adobe doit disposer d’un contrat Adobe Gen AI signé dans ce fichier.
* L’administrateur Workfront doit activer l’assistant d’IA pour les utilisateurs de votre entreprise. L’assistant AI est activé par le biais des niveaux d’accès.
* Les options Activer l’IA et Intégrité du projet doivent être sélectionnées dans la section Préférences de l’IA de la zone Préférences système de la Configuration.

  ![section Préférences IA](assets/ai-preferences.png)

Pour plus d’informations, consultez [Présentation de l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md) et [Configuration des préférences système](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Méthode de calcul de l’intégrité du projet

L’assistant AI vous donne une évaluation rapide de l’état global d’un projet en lui affectant l’un des états d’intégrité de projet disponibles :

* Dans les temps
* En danger
* En difficulté

Cet état est calculé à l’aide des composants du projet, tels que l’avancement du projet, le travail sous-estimé, etc. Pour obtenir la liste complète des composants utilisés pour mesurer l’intégrité du projet, reportez-vous à la section [Liste des états du projet et du programme](#project-and-program-states-list).

Chaque composant de projet se voit attribuer une note de risque numérique comprise entre (0 et 100), qui est ensuite moyennée pour créer l’état d’intégrité global du projet :

* Respect de l’objectif (75 ans ou plus) : les performances du projet se situent dans les seuils prévus.
* En danger (50-74) : des problèmes émergents sont détectés qui peuvent avoir une incidence sur la performance du projet.
* En difficulté (49 ans ou moins) : les performances du projet sont inférieures aux seuils acceptables et nécessitent une attention immédiate.

>[!NOTE]
>
>* Actuellement, l’assistant AI évalue uniquement les données du projet sélectionné.
>* L’analyse transversale ou historique n’est pas encore incluse dans le calcul de l’intégrité du projet.

### Exemples de calcul de l’intégrité d’un projet

Dans le premier exemple, quatre composantes du projet sont évaluées et leurs scores de risque individuels sont calculés comme suit :

* 2 Dans les temps (score de risque de 90)
* 1 À Risque (45 score de risque)
* 1 En difficulté (20 score de risque)

Si vous faites la moyenne de ces scores, le résultat est de 61. En utilisant les critères d’intégrité du projet répertoriés ci-dessus, ce projet est à l’état En danger.

Dans l’exemple suivant, une modification de planification d’un jour s’est produite au début de la chronologie du projet. Dans ce scénario, l’assistant AI évalue à la fois le calendrier et l’impact de la modification par rapport à la durée globale du projet :

* Un changement de planning d’un jour au début d’un calendrier de projet de 60 jours est mineur et généralement noté comme Atteint la cible.
* Un changement de calendrier d’un jour proche de la date d’achèvement d’un projet est plus perturbateur et peut être noté En danger ou En difficulté.

Étant donné que la modification était mineure et s’est produite au début de la chronologie du projet, le projet est ainsi à l’état Ciblé.

Si plusieurs modifications de planification se produisent dans la chronologie d’un projet, elles sont notées puis moyennées avant d’être appliquées au calcul de l’intégrité du projet.

## Comprendre la différence entre les conditions du projet et l&#39;intégrité du projet

Les conditions du projet et l&#39;intégrité du projet sont des concepts similaires dans Workfront et portent les mêmes noms par défaut pour décrire la condition ou l&#39;état du projet (Ciblé, À risque et À problème), mais ils ont des objectifs différents.

Les conditions d’un projet donnent un aperçu de base des performances actuelles d’un projet, en fonction uniquement des dates prévues, prévues et estimées. Il peut être défini manuellement par le propriétaire du projet ou automatiquement par Workfront en fonction des tâches du projet. L’intégrité du projet est également plus complète et évalue des facteurs supplémentaires, ce qui vous permet de mieux comprendre ses performances.

Pour plus d’informations sur les conditions du projet, consultez les articles suivants :

* [Mettre à jour la condition d’un projet](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-condition-on-project.md)
* [&#x200B; Conditions personnalisées &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

## Liste des états d’intégrité des projets et programmes

Le tableau ci-dessous contient une répartition des états disponibles que l’assistant AI attribuera à votre projet ou programme lors de la génération d’une évaluation de l’intégrité du projet.

<table>
    <tr>
        <td><b>Statut du projet</b></td>
        <td><b>Définition</b></td>
        <td><b>Facteurs</b></td>
    </tr>
    <tr>
        <td>Dans les temps</td>
        <td>Ce niveau de risque est attribué lorsque le niveau de risque moyen pour les facteurs suivants se situe à l’intérieur du seuil sain.
        </td>
        <td> 
        <ul><li>Dérive des objectifs</li>
        <li>Champs manquants</li>
        <li>Modifications de planning</li>
        <li>Travail sous-estimé</li>
        <li>Progression du projet</li>
        <li>Tâches en retard</li>
        <li>Budget</li>
        </ul></td>
    </tr>
    <tr>
        <td>En danger</td>
        <td>Ce niveau de risque est attribué lorsque le niveau de risque moyen pour les facteurs suivants tombe juste en dessous du seuil sain.</td>
        <td>
        <ul><li>Dérive des objectifs</li>
        <li>Champs manquants</li>
        <li>Modifications de planning</li>
        <li>Travail sous-estimé</li>
        <li>Progression du projet</li>
        <li>Tâches en retard</li>
        <li>Budget</li>
        </ul></td>
    </tr>
    <tr>
        <td>En difficulté</td>
        <td>Ce niveau de risque est attribué lorsque le niveau de risque moyen pour les facteurs suivants est inférieur au seuil sain.</td>
        <td>
        <ul><li>Dérive des objectifs</li>
        <li>Champs manquants</li>
        <li>Modifications de planning</li>
        <li>Travail sous-estimé</li>
        <li>Progression du projet</li>
        <li>Tâches en retard</li>
        <li>Budget</li>
        </ul></td>
    </tr>
    </tr>
   </table>

## Liste des invites de l&#39;assistant AI

Vous trouverez ci-dessous une liste d’invites que vous pouvez utiliser pour demander à l’assistant d’IA de générer une évaluation de l’intégrité d’un projet, d’un programme ou de tous les projets que vous êtes autorisé à consulter.

<table>
    <tr>
        <td><b>Emplacement</b></td>
        <td><b>Invite</b></td>
    </tr>
    <tr>
        <td>Page de détails d’un projet spécifique</td>
        <td><em>Quel est l'état de santé de ce projet ?</em></td>
    </tr>
    <tr>
        <td>N’importe quelle page dans Workfront </td>
        <td><em>Quel est l'état de santé du projet [NOM DU PROJET] ?</em></td>
    </tr>
    <tr>
        <td>N’importe quelle page dans Workfront </td>
        <td><em>Quel est l'état de mes projets ?</em></td>
    </tr>
       <tr>
        <td>Page de détails d’un programme spécifique</td>
        <td><em>Quel est l'état de ce programme ?</em></td>
    </tr>
       <tr>
        <td>N’importe quelle page dans Workfront </td>
        <td><em>Quelle est la santé du programme [NOM DU PROGRAMME] ?</em></td>
    </tr>
   </table>

## Gérer les configurations d’intégrité du projet

Vous devez être administrateur système pour gérer les configurations d’intégrité du projet.

Une configuration d’intégrité du projet contient des critères spécifiques qui déterminent la manière dont l’intégrité de votre projet est calculée. Une fois la configuration créée par l’administrateur Workfront, vous pouvez l’appliquer à un projet.

Vous pouvez avoir plusieurs configurations d’intégrité de projet dans votre système.

{{step-1-to-setup}}

1. Cliquez sur **Préférences du projet** dans le panneau de gauche, puis sélectionnez **Intégrité du projet**.

1. Dans l’angle supérieur droit de la page, cliquez sur **Nouvelle configuration**.

   La page **Paramètres d’IA** s’ouvre.

1. (Facultatif) Cliquez dans le titre **Configuration sans titre** pour renommer la configuration.

1. Dans la section **Quels facteurs souhaitez-vous inclure dans l’intégrité du projet**, désélectionnez tout facteur que vous ne souhaitez pas inclure lors de la détermination des critères d’intégrité de votre projet :
   * **Fluctuation de l’étendue** : pourcentage d’extension de l’étendue du projet depuis son lancement.

   * **Champs obligatoires** : si des champs obligatoires sont manquants (par exemple, description du projet). Ces champs obligatoires déterminent l’exhaustivité du projet et sont spécifiés dans le **Quels champs voulez-vous vérifier l’exhaustivité ?** la section Configuration ci-dessous.


   * **Modifications de planification** : nombre de modifications de planification qui se sont produites depuis le début du projet.

   * **Estimation de la tâche** : Précision du travail estimé pour la tâche (par exemple, aucune tâche en retard n&#39;est actuellement dans le projet).

   * **Avancement de la tâche** : progression du projet par rapport à la chronologie du projet.

   * **Tâches en retard** : nombre de tâches dont la date d&#39;échéance est actuellement dépassée.

   * **Coût** : si le projet dépasse actuellement le budget.

1. Dans la **Quand votre projet commence-t-il officiellement ?** section, sélectionnez l’événement qui signale le début de votre projet dans la liste déroulante.

1. Dans le **Comment estimez-vous l&#39;étendue du travail sur un projet ?** section, sélectionnez le facteur de projet qui augmentera à mesure que la portée du projet augmente.

1. Dans la **Quel(le) champ(s) voulez-vous vérifier ?** section, sélectionnez un ou plusieurs champs qui doivent contenir une valeur pour le projet.

   ![Champs obligatoires du projet pour l’intégrité du projet](assets/project-completeness-fields.png)

1. Cliquez sur **Ajouter** pour ajouter d’autres champs de projet ou de tâche natifs ou personnalisés.

1. Cliquez sur **Enregistrer** dans le coin supérieur droit.

## Application des configurations d’intégrité du projet

Une fois que l’administrateur Workfront a créé une configuration d’intégrité du projet, vous pouvez l’appliquer à un projet, si vous disposez des autorisations de gestion pour un projet.

{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.

1. Cliquez sur l’icône **Plus** ![Plus](assets/more-icon.png) à droite du nom du projet, puis sélectionnez **Modifier**. La zone **Modifier le projet** s’ouvre.

1. Dans le panneau de gauche, cliquez sur **Paramètres du projet**.

1. Dans le champ **Configuration de l’intégrité du projet**, sélectionnez la configuration à appliquer à ce projet.

   ![Champ de configuration de l’intégrité du projet](assets/project-health-configurations.png)

1. Cliquez sur **Enregistrer** dans le coin inférieur gauche de la page.

## Générer une évaluation de l’intégrité d’un projet ou programme

Vous pouvez générer une évaluation de l’intégrité du projet à partir de l’assistant d’IA dans les domaines suivants :

* Pour un projet, vous pouvez générer l&#39;évaluation à partir de la page du projet ou en référençant le nom du projet lorsque vous demandez à l&#39;assistant quelles sont les performances d&#39;un projet spécifique.

* Pour un programme, vous pouvez générer l’évaluation à partir de la page Détails du programme.

>[!NOTE]
>
>* Vous avez besoin d’autorisations d’affichage pour le projet ou le programme afin de générer une évaluation.
>* Une évaluation de l&#39;intégrité d&#39;un projet ne peut pas être générée tant que le projet n&#39;a pas démarré. Vous pouvez configurer l’événement qui déclenche un projet à démarrer dans les Préférences du projet

Pour plus d’informations, consultez la section [Gérer les configurations d’intégrité du projet](#manage-project-health-configurations) de cet article.

Pour générer une évaluation de l&#39;intégrité d&#39;un projet ou d&#39;un programme :

1. Accédez au projet ou programme pour lequel vous souhaitez générer une évaluation de l’intégrité du projet.

1. Sur la page de détails du projet/programme, cliquez sur l’icône **Assistant AI** icône ![Assistant AI](assets/ai-assistant-icon.png) dans le coin supérieur droit de l’écran. L’assistant d’IA s’ouvre.

1. Saisissez ce qui suit dans le champ **Me demander à propos de Workfront** : *Quel est l’état de ce projet ?*

   Ou

   Saisissez ce qui suit dans le champ **Me demander à propos de Workfront** : *Quel est l’état de ce programme ?*

   >[!NOTE]
   >
   >Si vous accédez à l’assistant AI à partir d’une autre page de Workfront, vous pouvez saisir *Quel est l’intégrité du projet [NOM DU PROJET] ?* ou *Quel est l&#39;état du programme [NOM DU PROGRAMME] ?* <br>
   >Pour obtenir la liste complète des invites actuelles que vous pouvez saisir, reportez-vous à la section [Liste des invites de l&#39;assistant AI](#ai-assistant-prompts-list) de cet article.

1. Cliquez sur l’icône **Envoyer** ![Icône Envoyer](assets/send-icon.png). L’évaluation de l’intégrité du projet génère et s’affiche dans le panneau. Un badge s’affiche en haut de chaque évaluation de l’intégrité du projet, qui reflète l’état actuel du projet.

   ![Évaluation de l’intégrité du projet](assets/health-assessment.png)

   Si vous générez une évaluation pour un programme, plusieurs badges seront répertoriés indiquant l&#39;état de chaque projet dans le programme. Pour plus d’informations sur les libellés des badges, consultez la section [Liste des états des projets et des programmes](#project-and-program-states-list) dans cet article.

1. (Facultatif) Cliquez sur l’un des points d’évaluation pour en développer les détails.

1. (Facultatif) En mode Détails développé, cliquez sur le lien du projet pour ouvrir les détails du projet.

   ![Détails développés](assets/expanded-details.png)

1. Après avoir consulté les détails d’intégrité du projet, cliquez sur l’icône **Fermer** ![Icône Fermer](assets/close-icon.png) dans le coin supérieur droit de l’assistant AI.

## Générer une évaluation de l’intégrité du projet pour plusieurs projets

Vous pouvez générer une évaluation de l’intégrité combinée du projet pour tous les projets pour lesquels vous disposez actuellement d’autorisations d’affichage ou supérieures.

Un projet ne sera inclus dans l&#39;évaluation combinée de l&#39;état de santé du projet que s&#39;il a commencé. Vous pouvez configurer l’événement qui déclenche un projet à démarrer dans les paramètres du projet. Pour plus d’informations, consultez la section [Gérer les configurations d’intégrité du projet](#manage-project-health-configurations) dans cet article.

1. Cliquez sur l’icône **Assistant AI** ![icône de l’assistant AI](assets/ai-assistant-icon.png) dans le coin supérieur droit de l’écran. L’assistant d’IA s’ouvre.

1. Saisissez ce qui suit dans le champ **Me poser des questions sur Workfront** : *Quel est l’intégrité de mes projets ?*

   Pour obtenir la liste complète des invites actuelles que vous pouvez saisir, reportez-vous à la section suivante de cet article : [Liste des invites de l&#39;assistant AI](#ai-assistant-prompts-list).

1. Cliquez sur l’icône **Envoyer** ![Icône Envoyer](assets/send-icon.png). L’évaluation de l’intégrité du projet génère et s’affiche dans le panneau.

   ![Évaluation de projets multiples](assets/multiple-projects-assessment.png)

   Lors de la génération d’une évaluation pour plusieurs projets, l’assistant AI regroupe les résultats en fonction des performances actuelles des projets.

1. (Facultatif) Cliquez sur l’un des badges de statut d’intégrité du projet pour développer la liste des projets, puis sélectionnez un lien pour un projet spécifique afin d’accéder à la page de détails de ce projet.

1. Après avoir consulté les détails d’intégrité du projet, cliquez sur l’icône **Fermer** ![Icône Fermer](assets/close-icon.png) dans le coin supérieur droit de l’assistant AI pour la fermer.

<!--

## Build a Project Health table report in a Canvas Dashboard

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. For more information, see [Canvas Dashboards beta information](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md). 

You can add a table report to a Canvas Dashboard in order to easily visualize your Project Health data in a table format.  

### Prerequisites 

You must create a dashboard before you can build a table report. 

For more, see [Create a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

### Build a Project Health table report 

There are many configuration options available for building a Project Health table report. In this section, we'll walk you through the process of creating one that displays the following columns: 

* **Name**: Contains the project name. 
* **Project Health Analysis**: Contains a summary of the Project Health assessment. 
* **Project Health Created At**: Contains the date/time when the Project Health assessment was last generated. 
* **Project Health Label**: Contains the project's label (e.g. On Target, At Risk, or In Trouble).

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**. 
1. In the upper-right corner, click **New Dashboard**. 
1. In the **Create dashboard** box, enter the dashboard's **Name** and **Description**. 
1. Click **Create**. 
1. In the **Add report** box, select **Create report**. 
1. On the left side, select **Table**. 
1. In the upper-right corner, click **Create report**. 
1. (Optional) Follow the steps below to configure the **Details** ![Details icon](assets/details-icon.png) section: 
    1. Enter a report **Name**. 
    1. Enter a report **Description**. 
1. Follow the steps below to configure the **Build table** ![Build table icon](assets/drilldown-column.png) section: 
    1. In the left panel, click the **Table columns** icon. 
    1. Click **Add column**, then select **Project** > **Name**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Analysis**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Created At**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Label**. 

1. Follow the steps below to configure the **Filter** ![Filter icon](assets/filter-icon.png) section: 
    1. In the left panel, click the **Filter** icon. 
    1. Select **Edit filter**. 
    1. Click **Add condition** and then specify the field you want to filter by and the modifier that defines what kind of condition the field must meet. The column appears in the preview section on the right.
    1. (Optional) Click **Add filter group** to add another set of filtering criteria. The default operator between the sets is AND. Click the operator to change it to OR. 

1. Follow the steps below to configure the **Drilldown Group Settings** ![Group settings](assets/drilldown-group-icon.png) section: 
    1. In the left panel, click the **Group Settings** icon. 
    1. Click the **Add grouping** button and then select the field you want to create as a grouping. The grouping column appears in the preview section on the right. 

1. Click **Save** to create the report.

-->
