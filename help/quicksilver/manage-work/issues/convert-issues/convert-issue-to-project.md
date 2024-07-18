---
product-area: projects
navigation-topic: convert-issues
title: Convertir un problème en projet dans Adobe Workfront
description: Convertir un problème en projet dans Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1957'
ht-degree: 9%

---

# Convertir un problème en projet dans Adobe Workfront

<!--Audited: 01/2024-->

Si vous devez travailler davantage pour résoudre un problème une fois le problème envoyé, vous pouvez le convertir en projet.

Vous pouvez convertir un problème en nouveau projet ou en projet à l’aide d’un modèle. Cet article décrit les deux manières de convertir des problèmes en projets.

>[!IMPORTANT]
>
>Pour obtenir des informations générales sur la conversion des problèmes, nous vous recommandons de lire également l’article [Présentation des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Lors de la création d’un projet à partir d’un problème, certains champs du projet sont renseignés à partir d’autres objets. Pour plus d’informations, voir la section &quot;Nouveaux paramètres par défaut du projet&quot; dans l’article [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouvelle : standard </p> 
    <p>Actuelle : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux problèmes, tâches et projets</p> <p>Modifier l’accès aux données financières pour mettre à jour les informations financières pour une conversion anticipée du problème</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations pour le problème</p> <p>Vous obtenez les autorisations de gestion du projet une fois le problème converti.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Convertir un problème en projet

Vous pouvez convertir un problème en projet vierge.

1. Accédez à un projet et cliquez sur **[!UICONTROL Problèmes]** dans le panneau de gauche.
1. Dans la liste des problèmes qui s’affichent, effectuez l’une des opérations suivantes :

   * Pour convertir un problème en projet vierge, cliquez sur le nom du problème, cliquez sur le menu **[!UICONTROL Plus]** ![](assets/more-icon.png) situé à droite du nom du problème, puis cliquez sur **[!UICONTROL Convertir en projet vierge]**.


     Ou

     Sélectionnez le problème dans la liste de problèmes, cliquez sur le menu **[!UICONTROL Plus]** ![](assets/more-icon.png) en haut de la liste, puis cliquez sur **[!UICONTROL Convertir en projet vierge]**.

     >[!IMPORTANT]
     >
     >L’option Convertir en un projet vierge s’affiche uniquement lorsque l’administrateur de votre système ou de votre groupe a activé l’option [!UICONTROL Autoriser les utilisateurs à créer des projets sans utiliser de préférence template] dans la zone [!UICONTROL Setup]. Pour plus d’informations, voir [Configurer les préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     Vous devez ajouter manuellement des tâches au projet ou joindre un modèle au projet après avoir converti le problème.

     >[!TIP]
     >   
     >* Si le problème a été créé à l’aide d’une file d’attente de requêtes, le nouveau projet hérite du groupe de la file d’attente de requêtes.
     >* Si le problème a été créé en l’ajoutant à la section Problèmes du projet, le nouveau projet hérite du groupe du projet du problème.

     >[!TIP]
     >
     >Si le problème est associé à un processus d’approbation ou s’il est déjà associé à un objet de résolution, Workfront affiche un avertissement dans la partie supérieure de la zone Convertir en projet pour vous informer que l’approbation sera supprimée ou que l’objet de résolution sera remplacé pendant la conversion. Pour plus d’informations, voir [Présentation des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Facultatif et conditionnel) Cliquez sur [!UICONTROL **Options**] dans le panneau de gauche, puis sélectionnez l’une des options disponibles :

   * [!UICONTROL **Conserver le problème d’origine et lier sa résolution à ce projet**]

     Si cette option est désélectionnée, le problème d’origine est supprimé.

     >[!NOTE]
     >
     >Les utilisateurs n’ayant pas accès ou les autorisations nécessaires pour supprimer des problèmes ne pourront pas supprimer le problème lorsqu’ils le convertissent, quel que soit l’état de ce paramètre. Pour plus d’informations sur l’accès et les autorisations pour les problèmes, voir :
     >
     >* [Accorder l’accès aux problèmes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Partager un problème](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Autoriser (nom d’utilisateur) à avoir accès à ce projet**]

     Si cette option n’est pas sélectionnée, le [!UICONTROL contact de Principal] du problème n’a pas accès à la nouvelle tâche.

     >[!NOTE]
     >
     >Les options disponibles ici dépendent de la manière dont l’administrateur Workfront les a configurées pour tous les utilisateurs du système ou pour votre groupe. Pour plus d’informations, voir [Configuration de la tâche à l’échelle du système et des préférences de problème](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Ou, si les groupes de niveau supérieur de votre organisation les ont configurés séparément, les options disponibles ici dépendent du groupe que vous avez sélectionné pour le nouveau projet à l’étape 6. Pour plus d’informations, voir [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. Cliquez sur [!UICONTROL **Forms personnalisée**] et effectuez l’une des opérations suivantes :

   * Examinez les formulaires personnalisés associés au problème. Ils seront transférés vers le nouveau projet, s’il s’agit également de formulaires personnalisés de projet.
   * Ajouter d’autres formulaires personnalisés
   * Assurez-vous que tous les champs requis contiennent des informations valides.
   * Réorganisez les formulaires personnalisés en les faisant glisser ![](assets/drag-object-icon.png) là où vous le souhaitez.
   * Cliquez sur l’icône **x** située à droite d’un formulaire que vous ne souhaitez pas transférer vers le projet. Cela supprime le formulaire du projet.
   * Si nécessaire, transférez les informations de formulaire personnalisées du problème vers le projet.

     >[!TIP]
     >
     >* Si un formulaire personnalisé à plusieurs objets associé au problème est configuré pour être utilisé avec les problèmes et les projets, toutes les informations enregistrées dans le formulaire sont conservées lorsque vous effectuez la conversion si les champs existent à la fois sur le problème et sur les formulaires personnalisés du projet.
     >* Si un formulaire personnalisé à plusieurs objets avec un champ calculé est associé au problème ainsi qu’au projet, le problème et le projet doivent être compatibles avec tous les champs référencés dans les champs personnalisés calculés du formulaire. En cas d’incompatibilité, un message vous avertit d’effectuer des ajustements. Pour plus d’informations, reportez-vous à la section &quot;Champs personnalisés calculés dans les formulaires personnalisés à plusieurs objets&quot; dans la section [Ajout de champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

1. Cliquez sur [!UICONTROL **Convertir en projet**].

   >[!TIP]
   >
   >Si vous avez décidé de supprimer le problème d’origine, le problème est maintenant un projet.
   >   
   >Ou
   >  
   >Si vous avez décidé de conserver le problème d’origine, le problème est maintenant lié au nouveau projet et il se terminera une fois le projet terminé.
   >
   >Les informations de certains champs de problème sont transférées vers le projet si vous ne les avez pas modifiées pendant la conversion.

1. (Facultatif) Définissez d’autres &#x200B; de détails du projet (propriétaire du projet, dates du projet) et tâches, le cas échéant.
1. Cliquez sur [!UICONTROL **Convertir en projet**].

   Le problème est désormais converti en projet. La page du projet s’affiche.

## Convertir un problème en projet à l’aide d’un modèle

Vous pouvez convertir un problème en projet à l’aide d’un modèle.

1. Accédez à un projet et cliquez sur **[!UICONTROL Problèmes]** dans le panneau de gauche.
1. Dans la liste des problèmes qui s’affiche, cliquez sur le nom du problème, cliquez sur le menu **[!UICONTROL Plus]** ![](assets/more-icon.png) situé à droite du nom du problème, puis sur **Convertir en projet à partir du modèle** et commencez à saisir le nom d’un modèle dans la zone **Modèle de recherche**, puis cliquez sur le nom du modèle lorsqu’il s’affiche dans la liste. Passez à l’étape 3.

   >[!TIP]
   >
   >Si vous avez ajouté des modèles à votre liste Favoris, vous pouvez placer le pointeur de la souris sur le menu [!UICONTROL **Modèles favoris**] et cliquer sur le modèle à utiliser.

   La zone Nouveau projet à partir d’un modèle s’affiche.

   ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!TIP]
   >
   >* Si le problème est associé à un processus d’approbation ou s’il est déjà associé à un objet de résolution, Workfront affiche un avertissement dans la partie supérieure de la zone Convertir en projet pour vous informer que l’approbation sera supprimée ou que l’objet de résolution sera remplacé pendant la conversion. Pour plus d’informations, voir [Présentation des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).
   >   
   >* Si le problème a été créé à l’aide d’une file d’attente de requêtes, le nouveau projet hérite du groupe de la file d’attente de requêtes.
   >* Si le problème a été créé en l’ajoutant à la section Problèmes du projet, le nouveau projet hérite du groupe du projet du problème.

1. Consultez les détails du modèle à droite.

   Les détails du modèle sont les suivants :

   * Durée du modèle
   * Personne propriétaire du modèle
   * Nombre de tâches de niveau supérieur qui incluent les noms des trois premières tâches
   * Nombre de toutes les tâches dans le modèle
   * Noms des modèles de formulaires personnalisés

1. (Facultatif) Placez le pointeur de la souris sur le nom d’un modèle et cliquez sur l’icône **Favoris** ![](assets/favorites-icon-small.png) pour le marquer comme favori pour une utilisation ultérieure.

   >[!TIP]
   >
   >Vous pouvez avoir jusqu’à 40 articles marqués comme favoris dans Workfront. Il s’agit notamment de modèles et d’autres éléments.

1. Cliquez sur [!UICONTROL **Utiliser le modèle**] pour sélectionner un modèle.

   La zone [!UICONTROL Convertir en projet] s’ouvre.

   ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

1. Si un champ est déjà renseigné dans le modèle, il est prérenseigné dans la zone [!UICONTROL Convertir en projet]. Vous pouvez modifier les valeurs pré-remplies pour qu’elles correspondent mieux à votre projet. Pour plus d’informations, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!TIP]
   >
   >* Votre administrateur système ou groupe peut ajouter ou supprimer des champs dans la [!UICONTROL zone Convertir en projet] en mettant à jour les informations Détails du projet dans votre [!UICONTROL modèle de mise en page].
   >
   >* Pour mettre à jour les champs de la section [!UICONTROL Finance] de la zone [!UICONTROL Convertir en projet], vous devez disposer de l’accès [!UICONTROL Modifier] à [!UICONTROL Données financières] dans votre niveau d’accès. Si vous avez l’accès [!UICONTROL Afficher] à [!UICONTROL Données financières] dans votre niveau d’accès, toutes les informations financières du modèle sont transférées vers le nouveau projet et vous ne pouvez pas les modifier pendant que vous convertissez le problème. Pour plus d’informations, voir [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) et [Partager un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Facultatif et conditionnel) Cliquez sur [!UICONTROL **Options**] dans le panneau de gauche, puis sélectionnez l’une des options disponibles :

   * [!UICONTROL **Conserver le problème d’origine et lier sa résolution à ce projet**]

     Si cette option est désélectionnée, le problème d’origine est supprimé.

     >[!NOTE]
     >
     >Les utilisateurs n’ayant pas accès ou les autorisations nécessaires pour supprimer des problèmes ne pourront pas supprimer le problème lorsqu’ils le convertissent, quel que soit l’état de ce paramètre. Pour plus d’informations sur l’accès et les autorisations pour les problèmes, voir :
     >
     >* [Accorder l’accès aux problèmes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Partager un problème](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Autoriser (nom d’utilisateur) à avoir accès à ce projet**]

     Si cette option n’est pas sélectionnée, le [!UICONTROL contact de Principal] du problème n’a pas accès à la nouvelle tâche.

     >[!NOTE]
     >
     >Les options disponibles ici dépendent de la manière dont l’administrateur Workfront les a configurées pour tous les utilisateurs du système ou pour votre groupe. Pour plus d’informations, voir [Configuration de la tâche à l’échelle du système et des préférences de problème](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Ou, si les groupes de niveau supérieur de votre organisation les ont configurés séparément, les options disponibles ici dépendent du groupe que vous avez sélectionné pour le nouveau projet à l’étape 6. Pour plus d’informations, voir [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Cliquez sur [!UICONTROL **Forms personnalisée**] et effectuez l’une des opérations suivantes :

      * Examinez les formulaires personnalisés associés au modèle. Ils seront transférés vers le nouveau projet.
      * Examinez les formulaires personnalisés associés au problème. Ils seront transférés vers le projet s’ils sont également des formulaires de projet.
      * Assurez-vous que tous les champs requis contiennent des informations valides.
      * Réorganisez les formulaires personnalisés en les faisant glisser ![](assets/drag-object-icon.png) là où vous le souhaitez.
      * Cliquez sur l’icône **x** située à droite d’un formulaire que vous ne souhaitez pas transférer vers le projet.
      * Si nécessaire, transférez les informations de formulaire personnalisées du problème vers le projet.

        >[!TIP]
        >
        >* Si un formulaire personnalisé à plusieurs objets associé au problème est configuré pour être utilisé avec les problèmes et les projets, toutes les informations enregistrées dans le formulaire sont conservées lorsque vous effectuez la conversion si les champs existent à la fois sur le problème et sur les formulaires personnalisés du projet.
        >* Si un formulaire personnalisé à plusieurs objets avec un champ calculé est associé au problème ainsi qu’au projet, le problème et le projet doivent être compatibles avec tous les champs référencés dans les champs personnalisés calculés du formulaire. En cas d’incompatibilité, un message vous avertit d’effectuer des ajustements. Pour plus d’informations, voir [Ajout de champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
        >* Si un formulaire personnalisé associé au modèle contient un champ personnalisé qui se trouve également dans un formulaire personnalisé associé au problème, la valeur de champ du problème est utilisée pour le nouveau projet. Cependant, si le champ personnalisé est vide sur le problème, la valeur du modèle est utilisée.

1. (Facultatif) Définissez d’autres &#x200B; de détails du projet (propriétaire du projet, dates du projet) et tâches, le cas échéant.

   1. Cliquez sur [!UICONTROL **Convertir en projet**].

      >[!TIP]
      >
      >Si vous avez décidé de supprimer le problème d’origine, le problème est maintenant un projet.
      >   
      >Ou
      >  
      >Si vous avez décidé de conserver le problème d’origine, le problème est maintenant lié au nouveau projet et il se terminera une fois le projet terminé.
      >
      >Certains champs de problème sont transférés vers le projet. La plupart des champs définis dans le modèle sont automatiquement transférés vers le projet nouvellement créé si vous ne les avez pas modifiés aux étapes précédentes. Pour plus d’informations, voir [Présentation des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

   Le problème est désormais converti en projet. La page du projet s’affiche.