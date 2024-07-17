---
product-area: projects
navigation-topic: convert-issues
title: Convertir un problème en tâche dans Adobe Workfront
description: Si vous devez travailler davantage pour résoudre un problème une fois le problème envoyé, vous pouvez le convertir en tâche.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: 44f01128ef4e6581dc8eaca318a999f2e7274f2a
workflow-type: tm+mt
source-wordcount: '1058'
ht-degree: 12%

---

# Convertir un problème en tâche dans Adobe Workfront

Si vous devez travailler davantage pour résoudre un problème une fois le problème envoyé, vous pouvez le convertir en tâche.

Pour obtenir des informations générales sur la conversion des problèmes, consultez la [Présentation des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux problèmes, tâches et projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations pour le problème</p> <p>Autorisations Contribute pour le projet</p> <p>Vous obtenez les autorisations Gérer pour la tâche une fois le problème converti.</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire, consultez <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Convertir un problème en tâche

1. Accédez à un projet et cliquez sur [!UICONTROL **Problèmes**] dans le panneau de gauche.
1. Cliquez sur le problème que vous souhaitez convertir pour accéder à la page d’entrée du problème.
1. Cliquez sur le menu [!UICONTROL **Plus**] sur le problème, puis [!UICONTROL **Convertir en tâche**].

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >Si le problème est associé à un processus d’approbation ou s’il est déjà associé à un objet de résolution, Workfront affiche un avertissement en haut de la zone [!UICONTROL Convertir en projet] pour vous informer que l’approbation est supprimée ou que l’objet de résolution est remplacé pendant la conversion. Pour plus d’informations, voir [Présentation des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Mettez à jour le nom de la tâche dans la section [!UICONTROL Nom de la tâche]. Par défaut, le nom de la tâche sera le même que celui de la tâche initiale.

   ![](assets/convert-to-task-box-nwe.png)

1. Cliquez sur [!UICONTROL **Projet de destination**], puis commencez à saisir le nom du projet dans lequel vous souhaitez placer la nouvelle tâche dans le champ [!UICONTROL **Projet de destination**] et sélectionnez-la lorsqu’elle s’affiche dans la liste. Le projet du problème est sélectionné par défaut.

1. Cliquez sur [!UICONTROL **Overview**], puis saisissez une [!UICONTROL **description**] pour la tâche.

   >[!TIP]
   >
   >   Un administrateur système ou de groupe peut modifier l’ordre des sections dans le panneau de gauche de la zone de conversion en modifiant votre modèle de mise en page.

1. (Facultatif et conditionnel) Cliquez sur [!UICONTROL **Options**], sélectionnez l’une des options ci-dessous.

   L’administrateur Workfront ou l’administrateur de groupe doit activer ces préférences avant qu’elles ne soient visibles lors de la conversion des problèmes :

   * [!UICONTROL **Conserver le problème d&#39;origine et lier sa résolution à cette tâche**]

     Si cette option n’est pas sélectionnée, le problème d’origine est supprimé.

     >[!NOTE]
     >
     >Les utilisateurs n’ayant pas accès ou les autorisations nécessaires pour supprimer des problèmes ne pourront pas supprimer le problème lorsqu’ils le convertissent, quel que soit l’état de ce paramètre. Pour plus d’informations sur l’accès et les autorisations pour les problèmes, voir :
     >   
     >   * [Accorder l’accès aux problèmes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     >   * [Partager un problème](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)
     >   
     >

   * [!UICONTROL **Autoriser (nom d’utilisateur) à avoir accès à cette tâche**]

     Si cette option n’est pas sélectionnée, le contact Principal du problème n’a pas accès à la nouvelle tâche.

   * [!UICONTROL **Conserver la date d’achèvement prévue du problème**]

     Si cette option n’est pas sélectionnée, la [!UICONTROL Date d’achèvement planifiée] de la nouvelle tâche est calculée à partir de la [!UICONTROL  Date de début planifiée] de la tâche. La [!UICONTROL Date de début planifiée] de la nouvelle tâche est définie en fonction des préférences du système pour les nouvelles tâches.

     >[!NOTE]
     >
     >
     >Les options qui s’affichent ici dépendent de la manière dont l’administrateur Workfront les a configurées pour tous les utilisateurs du système. Pour plus d’informations, voir [Configuration de la tâche à l’échelle du système et des préférences de problème](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >Ou, si les groupes de niveau supérieur de votre organisation les ont configurés séparément, les options qui s’affichent ici dépendent du groupe associé au projet que vous avez sélectionné à l’étape 6. Pour plus d’informations, voir [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (Facultatif) Cliquez sur [!UICONTROL **Forms personnalisé**] et joignez un formulaire personnalisé pour la nouvelle tâche.

   >[!TIP]
   >
   >* Si un formulaire personnalisé contenant plusieurs objets associés au problème est configuré pour être utilisé avec les problèmes et les tâches, toutes les informations enregistrées dans le formulaire sont conservées lorsque vous effectuez la conversion si les champs existent à la fois sur le problème et sur les formulaires personnalisés de la tâche.
   >* Si un formulaire personnalisé à plusieurs objets avec un champ calculé est associé au problème ainsi qu’à la tâche, le problème et la tâche doivent être compatibles avec tous les champs référencés dans les champs personnalisés calculés du formulaire. En cas d’incompatibilité, un message vous avertit d’effectuer des ajustements. Pour plus d’informations, reportez-vous à la section &quot;Champs personnalisés calculés dans les formulaires personnalisés à plusieurs objets&quot; dans la section [Ajout de données calculées à un formulaire personnalisé avec l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
   >* Si le projet de destination comporte des formulaires par défaut définis dans le champ Task Default Custom Forms lors de la modification du projet, ces formulaires de tâche sont également ajoutés à la nouvelle tâche. Tous les champs personnalisés communs au problème d’origine et les champs des formulaires de tâches par défaut sont préremplis avec les informations des champs de problème.


1. Cliquez sur [!UICONTROL **Convertir en tâche**].

   Le problème est maintenant une tâche sur le projet désigné, si vous avez décidé de supprimer le problème d’origine.

   Ou

   Le problème est maintenant lié à la nouvelle tâche sur le projet que vous avez choisi et il se terminera une fois la tâche terminée, si vous avez décidé de conserver le problème d’origine.

   Certains champs d’émission sont transférés vers la tâche. Pour plus d’informations, reportez-vous à la section [Affichage des informations de problème d’origine sur les projets et les tâches](#view-original-issue-information-on-projects-and-tasks) de cet article.

1. (Facultatif) Poursuivez la modification de la tâche si nécessaire.

## Affichage des informations de problème d’origine sur les projets et les tâches {#view-original-issue-information-on-projects-and-tasks}

Vous pouvez afficher les informations sur le problème d’origine dans les listes et rapports de projet et de tâche ou dans la zone Détails du projet . Pour plus d’informations sur la création de rapports, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Le tableau suivant illustre les champs de problème visibles à partir des projets et tâches convertis.

| Champs de problème | Champ de projet ou de tâche | Liste ou rapport de projets | Zone Détails du projet | Liste ou rapport de tâches | Zone Détails de la tâche |
|---|---|---|---|---|---|
| [!UICONTROL Nom du problème] | [!UICONTROL Nom du problème converti] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL Contact Principal] | [!UICONTROL Nom de l’auteur de problèmes convertis] | ✔ | ✔ | ✔ |
| [!UICONTROL Date d’entrée] | [!UICONTROL Date d&#39;entrée de l&#39;événement converti] | ✔ |  | ✔ |


>[!CAUTION]
>
>Si le [!UICONTROL contact par Principal] d’un problème change ou si le problème n’est plus lié au projet ou à la tâche une fois le problème converti, le [!UICONTROL nom de l’auteur du problème converti] ne se met pas à jour et affiche le [!UICONTROL contact du Principal] d’origine du problème au moment de la conversion du problème.
