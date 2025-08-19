---
title: Présentation de l’intégrité du projet
content-type: reference
description: La fonctionnalité d’intégrité du projet utilise la puissance de l’assistant d’IA pour vous donner instantanément une évaluation des performances de vos projets.
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
hide: true
hidefromtoc: true
source-git-commit: 420ddfa1f12f21332f460f9dc5fd1393cfc6e435
workflow-type: tm+mt
source-wordcount: '1822'
ht-degree: 2%

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

+++ Développez pour afficher les exigences d’accès. 
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront</p></td> 
   <td> 
<p>Select, Prime ou Ultimate </p> 
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
   <td><p>L’administrateur doit gérer les configurations d’intégrité du projet </p>
   <p>Modifier pour appliquer les configurations d’intégrité du projet </p>
     <p>Afficher pour afficher les configurations d’intégrité du projet </p>
  </td> 
  </tr>  
    </tr>  
</tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## S’inscrire à la version bêta de l’intégrité du projet

Pour utiliser l’intégrité du projet, l’assistant AI doit être activé pour votre organisation.

Pour activer l’assistant AI pour votre organisation, toutes les conditions suivantes doivent être remplies :

* Votre organisation doit avoir migré vers Adobe IMS (système Identity Management).
* L’expérience unifiée Adobe doit être activée.
* Adobe doit disposer d’un contrat Adobe Gen AI signé dans ce fichier.
* L’administrateur Workfront doit activer l’assistant AI pour les utilisateurs de votre entreprise. L’assistant AI est activé par le biais des niveaux d’accès.

Pour plus d’informations, voir [ Présentation de l’assistant AI ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

## Liste des invites de l&#39;assistant AI

Vous trouverez ci-dessous une liste d’invites que vous pouvez utiliser pour demander à AI Assessment de générer une évaluation de l’intégrité d’un projet, d’un programme ou de tous les projets de votre compte.

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


## Liste des conditions du projet et du programme

Vous trouverez ci-dessous les conditions disponibles que l’assistant AI attribuera à votre projet ou programme lors de la génération d’une évaluation de l’intégrité du projet.

<table>
    <tr>
        <td><b>Statut du projet</b></td>
        <td><b>Statut de la progression du projet</b></td>
    </tr>
    <tr>
        <td>Dans les temps</td>
        <td>Lorsque le statut d'avancement du projet est Dans les délais, le statut du projet est Dans les délais.</td>
    </tr>
    <tr>
        <td>En danger</td>
        <td>Lorsque le statut d'avancement du projet est En retard ou À risque, le statut du projet est À risque.</td>
    </tr>
    <tr>
        <td>En difficulté</td>
        <td>Lorsque le statut d'avancement du projet est En retard, le statut du projet est En danger.</td>
    </tr>
    </tr>
   </table>

## Gérer les configurations d’intégrité du projet

Une configuration d’intégrité du projet contient des critères spécifiques qui déterminent la manière dont l’intégrité de votre projet est calculée. Une fois la configuration créée, vous pouvez l’appliquer à un projet.

>[!NOTE]
>
>Vous devez être administrateur système pour gérer les configurations d’intégrité du projet.

{{step-1-to-setup}}

1. Cliquez sur **Préférences du projet** dans le panneau de gauche, puis sélectionnez **Intégrité du projet** dans la liste déroulante qui s’affiche.

1. Dans le coin supérieur droit de la page, sélectionnez **Nouvelle configuration**.

1. (Facultatif) Sur la page des détails des configurations, remplacez *Configuration sans titre* par une nouvelle configuration **Nom**.

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

1. Dans la zone **Quels champs voulez-vous vérifier l&#39;exhaustivité ?** section, sélectionnez un ou plusieurs champs qui seront vérifiés pour déterminer l’exhaustivité du projet.

   ![Champs d&#39;exhaustivité du projet](assets/project-completeness-fields.png)


1. Cliquez sur **Enregistrer** dans le coin supérieur droit.

## Application des configurations d’intégrité du projet

Une fois qu’un administrateur a créé une configuration d’intégrité de projet, les utilisateurs disposant d’un accès en modification peuvent l’appliquer à un projet.


{{step1-to-projects}}

1. Sélectionnez un projet sur la page **Projets**.

1. Cliquez sur l’icône **Plus** ![Plus](assets/more-icon.png) à droite du nom du projet, puis sélectionnez **Modifier**. Le panneau latéral **Modifier le projet** s’ouvre.

1. Dans le panneau de gauche, sélectionnez **Paramètres du projet**.

1. Dans le champ **Configuration de l’intégrité du projet**, sélectionnez la configuration à appliquer à ce projet.

   ![Champ de configuration de l’intégrité du projet](assets/project-health-configurations.png)

1. Cliquez sur **Enregistrer** dans le coin inférieur gauche du panneau.

## Générer une évaluation de l’intégrité d’un projet ou programme

Si vous disposez d’un accès en lecture seule à un projet ou programme, vous pouvez générer son évaluation de l’intégrité du projet à l’aide de l’assistant IA.

Si vous générez une évaluation pour un projet, vous pouvez le faire à partir de la page du projet ou en référençant le nom du projet lorsque vous demandez à l&#39;assistant quelles sont les performances du projet.

Si vous générez une évaluation pour un programme, vous pouvez le faire à partir de la page des détails du programme.

>[!NOTE]
>
>Une évaluation de l&#39;intégrité d&#39;un projet ne peut pas être générée tant que le projet n&#39;a pas démarré. Vous pouvez configurer l’événement qui déclenche un projet à démarrer dans les paramètres du projet.

Pour plus d’informations, consultez la section suivante de cet article : [Gérer les configurations d’intégrité du projet](#manage-project-health-configurations).

1. Accédez au projet ou programme pour lequel vous souhaitez générer une évaluation de l’intégrité du projet.

1. Sur la page de détails du projet/programme, cliquez sur l’icône **Assistant AI** icône ![Assistant AI](assets/ai-assistant-icon.png) dans le coin supérieur droit de l’écran. L’assistant d’IA s’ouvre.

1. Saisissez ce qui suit dans le champ **Me demander à propos de Workfront** : *Quel est l’état de ce projet ?*

   Ou

   Saisissez ce qui suit dans le champ **Me demander à propos de Workfront** : *Quel est l’état de ce programme ?*

   >[!NOTE]
   >
   >Si vous accédez à l’assistant AI à partir d’une autre page de Workfront, vous pouvez saisir *Quel est l’intégrité du projet [NOM DU PROJET] ?* ou *Quel est l&#39;état du programme [NOM DU PROGRAMME] ?* <br>
   >Pour obtenir la liste complète des invites actuelles que vous pouvez saisir, reportez-vous à la section suivante de cet article : [Liste des invites de l&#39;assistant AI](#ai-assistant-prompts-list).

1. Appuyez sur l’icône **Envoyer** ![Icône Envoyer](assets/send-icon.png). L’évaluation de l’intégrité du projet génère et s’affiche dans le panneau. Un badge s’affiche en haut de chaque évaluation de l’intégrité du projet, qui reflète l’état actuel du projet.

   ![Évaluation de l’intégrité du projet](assets/health-assessment.png)

   Si vous générez une évaluation pour un portefeuille, plusieurs badges seront répertoriés indiquant l&#39;état de chaque projet dans le programme. Pour plus d’informations sur les libellés des badges, consultez la section suivante de cet article : [Liste des conditions du projet et du programme](#project-and-program-conditions-list).

1. (Facultatif) Cliquez sur l’un des points d’évaluation pour en développer les détails.

1. (Facultatif) En mode Détails développés, cliquez sur le lien de la tâche pour ouvrir les détails de la tâche.

   ![Détails développés](assets/expanded-details.png)

1. Après avoir consulté les détails d’intégrité du projet, cliquez sur l’icône **Fermer** ![Icône Fermer](assets/close-icon.png) dans le coin supérieur droit de l’assistant AI.

## Générer une évaluation de l’intégrité du projet pour plusieurs projets

Vous pouvez générer une évaluation de l’intégrité combinée du projet pour tous les projets pour lesquels vous disposez actuellement d’un accès en lecture seule (ou supérieur).

Un projet ne sera inclus dans l&#39;évaluation combinée de l&#39;état de santé du projet que s&#39;il a commencé. Vous pouvez configurer l’événement qui déclenche un projet à démarrer dans les paramètres du projet. Pour plus d’informations, consultez la section suivante de cet article : [Gérer les configurations d’intégrité du projet](#manage-project-health-configurations).

1. Cliquez sur l’icône **Assistant AI** ![icône de l’assistant AI](assets/ai-assistant-icon.png) dans le coin supérieur droit de l’écran. L’assistant d’IA s’ouvre.

1. Saisissez ce qui suit dans le champ **Me poser des questions sur Workfront** : *Quel est l’intégrité de mes projets ?*

   Pour obtenir la liste complète des invites actuelles que vous pouvez saisir, reportez-vous à la section suivante de cet article : [Liste des invites de l&#39;assistant AI](#ai-assistant-prompts-list).

1. Appuyez sur l’icône **Envoyer** ![Icône Envoyer](assets/send-icon.png). L’évaluation de l’intégrité du projet génère et s’affiche dans le panneau.

   ![Évaluation de projets multiples](assets/multiple-projects-assessment.png)

   Lors de la génération d’une évaluation pour plusieurs projets, l’assistant AI regroupe les résultats en fonction des performances actuelles des projets.

1. (Facultatif) Cliquez sur l’un des badges de statut d’intégrité du projet pour développer la liste des projets, puis sélectionnez un lien pour un projet spécifique afin d’accéder à la page de détails de ce projet.

1. Après avoir consulté les détails d’intégrité du projet, cliquez sur l’icône **Fermer** ![Icône Fermer](assets/close-icon.png) dans le coin supérieur droit de l’assistant AI pour la fermer.


## Créer un rapport Tableau d’intégrité du projet dans un tableau de bord Zone de travail

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Pour plus d’informations, voir [Informations bêta sur les tableaux de bord de la zone de travail](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Vous pouvez ajouter un rapport tabulaire à un tableau de bord Zone de travail afin de visualiser facilement les données d’intégrité de votre projet au format tableau.

### Conditions préalables

Vous devez créer un tableau de bord avant de pouvoir créer un rapport tabulaire.

Pour plus d’informations, consultez la section [Créer un tableau de bord de zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

### Créer un rapport Tableau d’intégrité du projet

De nombreuses options de configuration sont disponibles pour créer un rapport Tableau d’intégrité du projet. Dans cette section, nous vous guiderons tout au long du processus de création d’un rapport qui affiche les colonnes suivantes :

* **Nom** : contient le nom du projet.
* **Analyse de l’intégrité du projet** : contient un résumé de l’évaluation de l’intégrité du projet.
* **Intégrité du projet créée à** : contient la date/l’heure de la dernière génération de l’évaluation de l’intégrité du projet.
* **Étiquette d&#39;intégrité du projet** : contient l&#39;étiquette du projet (par exemple, Ciblés, à risque ou en difficulté).

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.
1. Dans le coin supérieur droit, cliquez sur **Nouveau tableau de bord**.
1. Dans la zone **Créer un tableau de bord**, saisissez les **Nom** et **Description** du tableau de bord.
1. Cliquez sur **Créer**.
1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.
1. Sur le côté gauche, sélectionnez **Tableau**.
1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.
1. (Facultatif) Suivez les étapes ci-dessous pour configurer la section **Détails** ![Icône Détails](assets/details-icon.png) :
   1. Saisissez un rapport **Nom**.
   1. Saisissez un état **Description**.
1. Pour configurer la section **Créer le tableau** ![Icône Créer le tableau](assets/drilldown-column.png), procédez comme suit :
   1. Dans le panneau de gauche, cliquez sur l’icône **Colonnes du tableau**.
   1. Cliquez sur **Ajouter une colonne**, puis sélectionnez **Projet** > **Nom**.
   1. Cliquez sur **Ajouter une colonne**, puis sélectionnez **Projet** > **Intégrité du projet** > **Analyse de l’intégrité**.
   1. Cliquez sur **Ajouter une colonne**, puis sélectionnez **Projet** > **Intégrité du projet** > **Créé à**.
   1. Cliquez sur **Ajouter une colonne**, puis sélectionnez **Projet** > **Intégrité du projet** > **Étiquette d’intégrité**.

1. Pour configurer la section **Filtre** ![Icône Filtre](assets/filter-icon.png), procédez comme suit :
   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer**.
   1. Sélectionnez **Modifier le filtre**.
   1. Cliquez sur **Ajouter une condition** puis spécifiez le champ à utiliser comme filtre et le modificateur qui définit le type de condition auquel le champ doit répondre. La colonne s’affiche dans la section de prévisualisation à droite.
   1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OU.

1. Suivez les étapes ci-dessous pour configurer la section **Paramètres du groupe d’analyse** ![Paramètres du groupe](assets/drilldown-group-icon.png) :
   1. Dans le panneau de gauche, cliquez sur l’icône **Paramètres du groupe**.
   1. Cliquez sur le bouton **Ajouter un regroupement** puis sélectionnez le champ à créer en tant que regroupement. La colonne de regroupement s’affiche dans la section de prévisualisation à droite.

1. Cliquez sur **Enregistrer** pour créer le rapport.
