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
ht-degree: 98%

---

# Convertir un problème en projet dans Adobe Workfront

<!--Audited: 01/2024-->

Si un travail supplémentaire doit être effectué pour compléter un problème après sa soumission, vous pouvez convertir le problème en projet.

Vous pouvez convertir un problème en nouveau projet ou en projet à partir d’un modèle. Cet article décrit les deux façons de convertir les problèmes en projets.

>[!IMPORTANT]
>
>Pour avoir plus d’informations générales sur la conversion de problèmes, nous vous recommandons de lire également l’article [Vue d’ensemble de la conversion des problèmes dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Lors de la création d’un projet à partir d’un problème, certains champs du projet sont alimentés à partir d’autres objets. Pour plus d’informations, consultez la section « Paramètres par défaut du nouveau projet » dans l’article [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).

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
    <p>Actuelle : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux problèmes, aux tâches et aux projets</p> <p>Accès en modification aux données financières pour mettre à jour les informations financières pour un projet converti à partir du problème</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage pour le problème</p> <p>Vous obtenez les autorisations de gestion du projet une fois le problème converti.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Convertir un problème en projet

Vous pouvez convertir un problème en un projet vide.

1. Accédez au projet et cliquez sur **[!UICONTROL Problèmes]** dans le panneau de gauche.
1. Dans la liste des problèmes qui s’affiche, effectuez l’une des opérations suivantes :

   * Pour convertir un problème en un projet vide, cliquez sur le nom du problème, puis sur le menu **[!UICONTROL Plus]** ![](assets/more-icon.png) à droite du nom du problème, et enfin sur **[!UICONTROL Convertir en projet vide]**.


     Ou

     Sélectionnez le problème dans la liste des problèmes, cliquez sur le menu **[!UICONTROL Plus]** ![](assets/more-icon.png) en haut de la liste, puis cliquez sur **[!UICONTROL Convertir en projet vide]**.

     >[!IMPORTANT]
     >
     >L’option Convertir en projet vide s’affiche uniquement si l’administrateur ou l’administratrice du système ou du groupe a activé la préférence Autoriser les utilisateurs et les utilisatrices à créer des projets sans utiliser de modèle dans la zone Configuration.  Pour plus d’informations, voir [Configurer les préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     Vous devez ajouter manuellement des tâches au projet ou lier un modèle au projet après avoir converti le problème.

     >[!TIP]
     >   
     >* Si le problème a été créé à l’aide d’une file d’attente des demandes, le nouveau projet hérite du groupe de la file d’attente.
     >* Si le problème a été créé en l’ajoutant à la section Problèmes du projet, le nouveau projet hérite du groupe du projet du problème.

     >[!TIP]
     >
     >Si le problème est associé à un processus d’approbation ou s’il est déjà associé à un objet de résolution, Workfront affiche un avertissement en haut de la zone Convertir en projet pour vous avertir que l’approbation sera supprimée ou que l’objet de résolution sera écrasé au cours de la conversion. Pour plus d’informations, voir [Vue d’ensemble de la conversion des problèmes dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Facultatif et le cas échéant) Cliquez sur [!UICONTROL **Options**] dans le panneau de gauche, puis sélectionnez l’une des options disponibles :

   * [!UICONTROL **Conserver le problème d’origine et lier sa résolution à ce projet**]

     Si cette option est désactivée, le problème d’origine est supprimé.

     >[!NOTE]
     >
     >Les utilisateurs et les utilisatrices qui n’ont pas l’accès ou les autorisations nécessaires pour supprimer des problèmes ne pourront pas supprimer le problème pendant la conversion, quel que soit le statut de ce paramètre. Pour plus d’informations sur l’accès et les autorisations relatives aux problèmes, consultez ce qui suit :
     >
     >* [Accorder l’accès aux problèmes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Partager un problème](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Autoriser (nom de l’utilisateur ou de l’utilisatrice) à accéder à ce projet**]

     Si cette option n’est pas sélectionnée, le [!UICONTROL contact principal] du problème n’a pas accès à la nouvelle tâche.

     >[!NOTE]
     >
     >Les options disponibles ici dépendent de la manière dont l’administrateur ou l’administratrice de Workfront les a configurées pour l’ensemble des utilisateurs et des utilisatrices du système ou pour votre groupe. Pour plus d’informations, consultez [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Ou, si les groupes de niveau supérieur de votre organisation les ont configurées séparément, les options disponibles ici dépendent du groupe que vous avez sélectionné pour le nouveau projet à l’étape 6. Pour plus d’informations, voir [Configurer les préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. Cliquez sur [!UICONTROL **Formulaires personnalisés**] et effectuez l’une des opérations suivantes :

   * Examinez les formulaires personnalisés joints au problème. Ils seront transférés dans le nouveau projet s’il s’agit de formulaires personnalisés.
   * Ajouter davantage de formulaires personnalisés
   * Assurez-vous que tous les champs obligatoires contiennent des informations valides.
   * Réorganisez les formulaires personnalisés en les faisant glisser ![](assets/drag-object-icon.png) à l’endroit souhaité.
   * Cliquez sur l’icône x à droite de tout formulaire à ne pas transférer au projet. **** Cette opération supprime le formulaire du projet.
   * Si nécessaire, transférez les informations du formulaire personnalisé du problème au projet.

     >[!TIP]
     >
     >* Si un formulaire personnalisé contenant plusieurs objets associés au problème est configuré pour être utilisé avec les problèmes et les projets, toutes les informations enregistrées dans le formulaire sont conservées lorsque vous effectuez la conversion, si les champs existent à la fois sur le problème et sur les formulaires personnalisés du projet.
     >* Si un formulaire personnalisé à plusieurs objets avec un champ calculé est joint au problème et au projet, l’un comme l’autre doivent être compatibles avec tous les champs référencés dans les champs personnalisés calculés du formulaire. En cas d’incompatibilité, un message vous invite à effectuer des ajustements. Pour plus d’informations, reportez-vous à la section &quot;Champs personnalisés calculés dans les formulaires personnalisés à plusieurs objets&quot; dans la section [Ajout de champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

1. Cliquez sur [!UICONTROL **Convertir en projet**].

   >[!TIP]
   >
   >Si vous avez décidé de supprimer le problème original, celui-ci devient un projet.
   >   
   >Ou
   >  
   >Si vous avez décidé de conserver le problème original, celui-ci est désormais lié au nouveau projet et se terminera lorsque le projet se terminera.
   >
   >Les informations contenues dans certains champs du problème sont transférées dans le projet si vous ne les avez pas modifiées lors de la conversion.

1. (Facultatif) Définissez d’autres détails du projet (personne propriétaire du projet, dates du projet) et des tâches si nécessaire.
1. Cliquez sur [!UICONTROL **Convertir en projet**].

   Le problème est maintenant converti en projet. La page du projet s’affiche.

## Convertir un problème en projet à l’aide d’un modèle

Vous pouvez convertir un problème en projet à l’aide d’un modèle.

1. Accédez au projet et cliquez sur **[!UICONTROL Problèmes]** dans le panneau de gauche.
1. Dans la liste des problèmes qui s’affiche, cliquez sur le nom du problème, cliquez sur le menu Plus  à droite du nom du problème, puis cliquez sur Convertir en projet à partir du modèle. Commencez à saisir le nom d’un modèle dans la zone Rechercher un modèle, puis cliquez sur le nom du modèle lorsqu’il s’affiche dans la liste. ****![](assets/more-icon.png)******** Passez à l’étape 3.

   >[!TIP]
   >
   >Si vous avez ajouté des modèles à votre liste de favoris, vous pouvez passer la souris sur le menu [!UICONTROL **Modèles favoris**] et cliquer sur le modèle à utiliser.

   La boîte de dialogue Nouveau projet à partir d’un modèle s’affiche.

   ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!TIP]
   >
   >* Si le problème est associé à un processus d’approbation ou s’il est déjà associé à un objet de résolution, Workfront affiche un avertissement en haut de la zone Convertir en projet pour vous avertir que l’approbation sera supprimée ou que l’objet de résolution sera écrasé au cours de la conversion. Pour plus d’informations, voir [Vue d’ensemble de la conversion des problèmes dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).
   >   
   >* Si le problème a été créé à l’aide d’une file d’attente des demandes, le nouveau projet hérite du groupe de la file d’attente.
   >* Si le problème a été créé en l’ajoutant à la section Problèmes du projet, le nouveau projet hérite du groupe du projet du problème.

1. Examinez les détails du modèle sur la droite.

   Les détails du modèle sont les suivants :

   * Durée du modèle
   * Personne propriétaire du modèle
   * Nombre de tâches de niveau supérieur comprenant les noms des trois premières tâches
   * Nombre de toutes les tâches dans le modèle
   * Noms des modèles de formulaires personnalisés

1. (Facultatif) Passez la souris sur le nom d’un modèle et cliquez sur l’icône **Favoris** ![](assets/favorites-icon-small.png) pour le marquer comme favori en vue d’une utilisation ultérieure.

   >[!TIP]
   >
   >Vous pouvez avoir jusqu’à 40 articles marqués comme favoris dans Workfront. Il s’agit notamment de modèles et d’autres éléments.

1. Cliquez sur [!UICONTROL **Utiliser le modèle**] pour sélectionner un modèle.

   La zone [!UICONTROL Convertir en projet] s’ouvre.

   ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

1. Si un champ est déjà rempli dans le modèle, il est pré-rempli dans la zone Convertir en projet.  Vous pouvez modifier les valeurs pré-remplies pour qu’elles correspondent mieux à votre projet. Pour plus d’informations, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!TIP]
   >
   >* L’administrateur ou l’administratrice système ou de groupes peut ajouter ou supprimer des champs dans la zone [!UICONTROL Convertir en projet] en mettant à jour les informations sur les détails du projet dans votre [!UICONTROL Modèle de mise en page].
   >
   >* Pour mettre à jour les champs de la section [!UICONTROL Finance] dans la zone [!UICONTROL Convertir en projet], vous devez disposer d’un niveau d’accès en [!UICONTROL modification] aux [!UICONTROL données financières]. Si vous disposez d’un niveau d’accès en affichage aux données financières, toutes les informations financières du modèle sont transférées vers le nouveau projet et vous ne pouvez pas les modifier pendant la conversion du problème.  Pour plus d’informations, voir [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) et [Partager un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Facultatif et le cas échéant) Cliquez sur [!UICONTROL **Options**] dans le panneau de gauche, puis sélectionnez l’une des options disponibles :

   * [!UICONTROL **Conserver le problème d’origine et lier sa résolution à ce projet**]

     Si cette option est désactivée, le problème d’origine est supprimé.

     >[!NOTE]
     >
     >Les utilisateurs et les utilisatrices qui n’ont pas l’accès ou les autorisations nécessaires pour supprimer des problèmes ne pourront pas supprimer le problème pendant la conversion, quel que soit le statut de ce paramètre. Pour plus d’informations sur l’accès et les autorisations relatives aux problèmes, consultez ce qui suit :
     >
     >* [Accorder l’accès aux problèmes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Partager un problème](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Autoriser (nom de l’utilisateur ou de l’utilisatrice) à accéder à ce projet**]

     Si cette option n’est pas sélectionnée, le [!UICONTROL contact principal] du problème n’a pas accès à la nouvelle tâche.

     >[!NOTE]
     >
     >Les options disponibles ici dépendent de la manière dont l’administrateur ou l’administratrice de Workfront les a configurées pour l’ensemble des utilisateurs et des utilisatrices du système ou pour votre groupe. Pour plus d’informations, consultez [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Ou, si les groupes de niveau supérieur de votre organisation les ont configurées séparément, les options disponibles ici dépendent du groupe que vous avez sélectionné pour le nouveau projet à l’étape 6. Pour plus d’informations, voir [Configurer les préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Cliquez sur [!UICONTROL **Formulaires personnalisés**] et effectuez l’une des opérations suivantes :

      * Vérifiez les formulaires personnalisés joints au modèle. Ils seront transférés vers le nouveau projet.
      * Examinez les formulaires personnalisés joints au problème. Ils seront transférés vers le projet s’il s’agit également de formulaires de projet.
      * Assurez-vous que tous les champs obligatoires contiennent des informations valides.
      * Réorganisez les formulaires personnalisés en les faisant glisser ![](assets/drag-object-icon.png) à l’endroit souhaité.
      * Cliquez sur l’icône **x** à droite de tout formulaire à ne pas transférer au projet.
      * Si nécessaire, transférez les informations du formulaire personnalisé du problème au projet.

        >[!TIP]
        >
        >* Si un formulaire personnalisé contenant plusieurs objets associés au problème est configuré pour être utilisé avec les problèmes et les projets, toutes les informations enregistrées dans le formulaire sont conservées lorsque vous effectuez la conversion, si les champs existent à la fois sur le problème et sur les formulaires personnalisés du projet.
        >* Si un formulaire personnalisé à plusieurs objets avec un champ calculé est joint au problème et au projet, l’un comme l’autre doivent être compatibles avec tous les champs référencés dans les champs personnalisés calculés du formulaire. En cas d’incompatibilité, un message vous invite à effectuer des ajustements. Pour plus d’informations, voir [Ajout de champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
        >* Si un formulaire personnalisé joint au modèle contient un champ personnalisé qui se trouve également dans un formulaire personnalisé joint au problème, la valeur du champ du problème est utilisée pour le nouveau projet. Cependant, si le champ personnalisé est vide dans le problème, la valeur du modèle est utilisée.

1. (Facultatif) Définissez d’autres détails du projet (personne propriétaire du projet, dates du projet) et des tâches si nécessaire.

   1. Cliquez sur [!UICONTROL **Convertir en projet**].

      >[!TIP]
      >
      >Si vous avez décidé de supprimer le problème original, celui-ci devient un projet.
      >   
      >Ou
      >  
      >Si vous avez décidé de conserver le problème original, celui-ci est désormais lié au nouveau projet et se terminera lorsque le projet se terminera.
      >
      >Certains champs de problème sont transférés vers le projet. La plupart des champs définis dans le modèle sont automatiquement transférés vers le nouveau projet créé si vous ne les avez pas modifiés lors des étapes précédentes. Pour plus d’informations, voir [Vue d’ensemble de la conversion des problèmes dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

   Le problème est maintenant converti en projet. La page du projet s’affiche.