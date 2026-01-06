---
product-area: projects
navigation-topic: convert-issues
title: Convertir un événement en tâche
description: Si davantage de travail doit être effectué pour résoudre un problème après l’envoi du problème, vous pouvez convertir le problème en tâche dans Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 87%

---

# Convertir un problème en une tâche

<!--Audited: 08/2025-->

Si davantage de travail doit être effectué pour résoudre un problème après l’envoi du problème, vous pouvez convertir le problème en tâche dans Adobe Workfront.

Pour obtenir des informations générales sur la conversion de problèmes, voir [Vue d’ensemble de la conversion de problèmes dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Travail ou supérieur</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes, aux tâches et aux projets</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations relatives au problème</p> <p>Autorisations de contribution au projet</p> <p>Vous obtenez des autorisations de niveau Gérer pour la tâche une fois l’événement converti</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p>Contribute permissions to the project</p> <p>You obtain Manage permissions to the task after the issue is converted</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table> -->

## Considérations

* Le temps de traitement est limité à 5 minutes lors de la conversion d’un événement en tâche. Si le problème est associé à un grand nombre de documents et qu’il ne parvient pas à être converti, vous devrez peut-être supprimer certains des documents et réessayer.

## Convertir un problème en une tâche

1. Accédez à un projet et cliquez sur [!UICONTROL **Problèmes**] dans le panneau de gauche.
1. Cliquez sur le problème que vous souhaitez convertir pour accéder à la page de destination du problème.
1. Cliquez sur le menu [!UICONTROL **Plus**] sur le problème, puis [!UICONTROL **Convertir en une tâche**].

   ![Menu Autres événements](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >Si le problème est associé à un processus d’approbation ou s’il est déjà associé à un objet de résolution, Workfront affiche un avertissement en haut de la zone [!UICONTROL Convertir en un projet] pour vous informer que l’approbation est supprimée ou que l’objet de résolution est remplacé pendant la conversion. Pour plus d’informations, voir [Vue d’ensemble de la conversion de problèmes dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Mettez à jour le nom de la tâche dans la section [!UICONTROL Nom de la tâche]. Par défaut, le nom de la tâche sera le même que celui du problème d’origine.

   ![Convertir en zone de tâche](assets/convert-to-task-box-nwe.png)

1. Cliquez sur [!UICONTROL **Projet de destination**], puis commencez à saisir le nom du projet dans lequel vous souhaitez placer la nouvelle tâche dans le champ [!UICONTROL **Projet de destination**] et sélectionnez-le lorsqu’il s’affiche dans la liste. Le projet du problème est sélectionné par défaut.

1. Cliquez sur [!UICONTROL **Vue d’ensemble**], puis saisissez une [!UICONTROL **Description**] pour la tâche.

   >[!TIP]
   >
   >   Un administrateur ou une administratrice système ou de groupes peut modifier l’ordre des sections dans le panneau de gauche de la zone de conversion en modifiant votre modèle de mise en page.

1. (Facultatif et le cas échéant) Cliquez sur [!UICONTROL **Options**] et sélectionnez l’une des options ci-dessous.

   L’administrateur ou aministratrice Workfront ou de groupes doit activer ces préférences avant qu’elles ne soient visibles lors de la conversion des problèmes :

   * [!UICONTROL **Conserver le problème d’origine et lier sa résolution à ce projet**]

     Si cette option n’est pas sélectionnée, le problème d’origine est supprimé.

     >[!NOTE]
     >
     >Les utilisateurs et les utilisatrices qui n’ont pas l’accès ou les autorisations nécessaires pour supprimer des problèmes ne pourront pas supprimer le problème pendant la conversion, quel que soit le statut de ce paramètre. Pour plus d’informations sur l’accès et les autorisations relatives aux problèmes, consultez :
     >   
     >   * [Accorder l’accès aux problèmes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     >   * [Partager un problème](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)
     >   
     >

   * [!UICONTROL **Autoriser (nom de l’utilisateur ou de l’utilisatrice) à accéder à cette tâche**]

     Si cette option n’est pas sélectionnée, le contact principal du problème n’a pas accès à la nouvelle tâche.

   * [!UICONTROL **Conserver la date d’achèvement prévue pour le problème**]

     Si cette option n’est pas sélectionnée, la [!UICONTROL Date d’achèvement prévue] de la nouvelle tâche est calculée à partir de la [!UICONTROL Date de début prévue] de la tâche. La [!UICONTROL Date de début prévue] de la nouvelle tâche est définie en fonction des préférences du système pour les nouvelles tâches.

     >[!NOTE]
     >
     >
     >Les options qui s’affichent ici dépendent de la manière dont l’administrateur ou administratrice Workfront les a configurées pour tous les utilisateurs et utilisatrices du système. Pour plus d’informations, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >Ou, si les groupes de niveau supérieur de votre organisation les ont configurées séparément, les options qui s’affichent ici dépendent du groupe associé au projet que vous avez sélectionné à l’étape 6. Pour plus d’informations, voir [Configurer les préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (Facultatif) Cliquez sur [!UICONTROL **Formulaires personnalisés**] et joignez un formulaire personnalisé pour la nouvelle tâche.

   >[!TIP]
   >
   >* Si un formulaire personnalisé contenant plusieurs objets associés au problème est configuré pour être utilisé avec les problèmes et les tâches, toutes les informations enregistrées dans le formulaire sont conservées lorsque vous effectuez la conversion, si les champs existent à la fois sur le problème et sur les formulaires personnalisés de la tâche.
   >* Si un formulaire personnalisé à plusieurs objets avec un champ calculé est joint au problème et à la tâche, l’un comme l’autre doivent être compatibles avec tous les champs référencés dans les champs personnalisés calculés du formulaire. En cas d’incompatibilité, un message vous invite à effectuer des ajustements. Pour plus d’informations, voir [&#x200B; Ajouter des champs calculés à un formulaire &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
   >* Si le projet de destination comporte des formulaires par défaut définis dans le champ Formulaires personnalisés par défaut de la tâche lors de la modification du projet, ces formulaires de tâche sont également ajoutés à la nouvelle tâche. Tous les champs personnalisés communs au problème d’origine et les champs des formulaires de tâches par défaut sont préremplis avec les informations des champs de problème.


1. Cliquez sur [!UICONTROL **Convertir en une tâche**].

   Le problème est maintenant une tâche sur le projet désigné, si vous avez décidé de supprimer le problème d’origine.

   Ou

   Le problème est maintenant lié à la nouvelle tâche sur le projet que vous avez choisi et il se terminera une fois la tâche terminée, si vous avez décidé de conserver le problème d’origine.

   Certains champs du problème sont transférés à la tâche. Pour plus d’informations, voir la section [Consulter les informations du problème d’origine sur les projets et les tâches](#view-original-issue-information-on-projects-and-tasks) de cet article.

1. (Facultatif) Continuez à modifier la tâche si nécessaire.

## Consulter les informations du problème d’origine sur les projets et les tâches {#view-original-issue-information-on-projects-and-tasks}

Vous pouvez consulter les informations du problème d’origine dans les listes et les rapports de projets et de tâches ou dans la zone Détails du projet. Pour plus d’informations sur la création de rapports, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Le tableau suivant illustre les champs du problème visibles à partir des projets et des tâches convertis.

| Champs du problème | Champ du projet ou de la tâche | Liste ou rapport de projet | Zone Détails du projet | Liste ou rapport de tâche | Zone Détails de la tâche |
|---|---|---|---|---|---|
| [!UICONTROL Nom du problème] | [!UICONTROL Nom du problème converti] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL Contact principal] | [!UICONTROL Nom du créateur ou de la créatrice du problème converti] | ✔ | ✔ | ✔ |  |
| [!UICONTROL Date d’entrée] | [!UICONTROL Date d&#39;entrée de l&#39;événement converti] | ✔ |  | ✔ |  |


>[!CAUTION]
>
>Si le [!UICONTROL Contact principal] d’un problème change ou si le problème est dissocié du projet ou de la tâche après avoir été converti, le [!UICONTROL Nom du créateur ou de la créatrice du problème converti] n’est pas mis à jour et affiche le [!UICONTROL Contact principal] d’origine du problème au moment de sa conversion.
