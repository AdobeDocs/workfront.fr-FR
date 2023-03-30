---
product-area: projects
navigation-topic: convert-issues
title: Convertir un problème en projet dans Adobe Workfront
description: Convertir un problème en projet dans Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: e38411056b3f9be6d0241ee18e71984ef2a678a0
workflow-type: tm+mt
source-wordcount: '1373'
ht-degree: 0%

---

# Convertir un problème en projet dans Adobe Workfront

Si vous devez travailler davantage pour résoudre un problème une fois le problème envoyé, vous pouvez le convertir en projet.

Vous pouvez convertir un problème en nouveau projet ou en projet à l’aide d’un modèle. Cet article décrit les deux manières de convertir des problèmes en projets.

Pour obtenir des informations générales sur la conversion de problèmes, voir [Présentation des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Lors de la création d’un projet à partir d’un problème, certains champs du projet sont renseignés à partir d’autres objets. Pour plus d’informations, voir la section &quot;Paramètres par défaut du nouveau projet&quot; dans l’article . [Création d’un projet](../../../manage-work/projects/create-projects/create-project.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux problèmes, tâches et projets</p> <p>Modifier l’accès aux données financières pour mettre à jour les informations financières pour une conversion anticipée du problème</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations pour le problème</p> <p>Vous obtenez les autorisations de gestion du projet une fois le problème converti.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Convertir un problème en projet

Vous pouvez convertir un problème en projet vierge ou le convertir en projet à l’aide d’un modèle.

1. Accédez à un projet et cliquez sur **[!UICONTROL Problèmes]** dans le panneau de gauche.
1. Dans la liste des problèmes qui s’affichent, effectuez l’une des opérations suivantes :

   * Pour convertir une publication en projet vierge, cliquez sur le nom de la publication, puis sur le bouton **[!UICONTROL Plus]** menu ![](assets/more-icon.png) à droite du nom du problème, puis cliquez sur **[!UICONTROL Convertir en projet vierge]**.


      Ou

      Sélectionnez le problème dans la liste des problèmes, puis cliquez sur le bouton **[!UICONTROL Plus]** menu ![](assets/more-icon.png) en haut de la liste, puis cliquez sur **[!UICONTROL Convertir en projet vierge]**.

      >[!IMPORTANT]
      >
      >L’option Convertir en projet vierge s’affiche uniquement lorsque l’administrateur de votre système ou groupe a activé la fonction [!UICONTROL Autoriser les utilisateurs à créer des projets sans utiliser de modèle] dans la [!UICONTROL Configuration] zone. Pour plus d’informations, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


      Vous devez ajouter manuellement des tâches au projet ou joindre un modèle au projet après avoir converti le problème.

      Passez à l’étape 3e ci-dessous.

      <!--
     Is this accurate?
     -->

      >[!TIP]
      >   
      >* Si le problème a été créé à l’aide d’une file d’attente de requêtes, le nouveau projet hérite du groupe de la file d’attente de requêtes.
      >* Si le problème a été créé en l’ajoutant à la section Problèmes du projet, le nouveau projet hérite du groupe du projet du problème.


   * Pour convertir un problème en projet à l’aide d’un modèle, effectuez l’une des opérations suivantes :

      * Cliquez sur le nom d’un problème, puis sur le [!UICONTROL **Plus**] menu ![](assets/more-icon.png) à droite du nom du problème

         ![](assets/issue-more-menu-expanded-with-convert-to-project-options-nwe-350x213.png)

         Ou

      * Sélectionnez le problème dans la liste des problèmes, dans un rapport ou dans un tableau de bord, cliquez sur le bouton **Plus** menu ![](assets/more-icon.png) en haut de la liste, puis cliquez sur **Convertir en projet à partir d’un modèle** et commencez à saisir le nom d’un modèle dans le champ **Modèle de recherche** puis cliquez sur le nom du modèle lorsqu’il s’affiche dans la liste. Passez à l’étape 3.

         <!--      
        (is this accurate?)      
        -->
      >[!TIP]
      >
      >Si vous avez ajouté des modèles à votre liste Favoris, vous pouvez placer le pointeur de la souris sur la [!UICONTROL **Modèles favoris**] et cliquez sur le modèle à utiliser.

      La zone Nouveau projet à partir d’un modèle s’affiche.

      ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

      >[!TIP]
      >
      >Si le problème est associé à un processus d’approbation ou s’il est déjà associé à un objet de résolution, Workfront affiche un avertissement dans la partie supérieure de la zone Convertir en projet pour vous informer que l’approbation sera supprimée ou que l’objet de résolution sera remplacé pendant la conversion. Pour plus d’informations, voir [Présentation des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).


1. (Conditionnel) Si vous avez choisi de convertir le problème en projet à l’aide d’un modèle, procédez comme suit :

   1. Consultez les détails du modèle à droite.

      Les détails du modèle sont les suivants :

      * Durée du modèle
      * Propriétaire du modèle
      * Nombre de tâches de niveau supérieur qui incluent les noms des trois premières tâches
      * Nombre de tâches dans le modèle
      * Les noms des modèles de formulaires personnalisés
   1. (Facultatif) Placez le pointeur de la souris sur le nom d’un modèle, puis cliquez sur l’icône Favoris . ![](assets/favorites-icon-small.png) pour le marquer comme favori pour une utilisation ultérieure.

      >[!TIP]
      >
      >Vous pouvez marquer jusqu’à 40 éléments Workfront comme favoris. Cela inclut les modèles et d’autres éléments.

   1. Cliquez sur [!UICONTROL **Utiliser un modèle**] pour sélectionner un modèle.

      Le [!UICONTROL Convertir en projet] s’ouvre.

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. Si un champ est déjà renseigné dans le modèle, il est prérenseigné dans la variable [!UICONTROL Convertir en projet] de la boîte. Vous pouvez modifier les valeurs prérenseignées afin de mieux correspondre à votre projet. Pour plus d’informations, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* Votre administrateur système ou groupe peut ajouter ou supprimer des champs dans la variable [!UICONTROL Zone Convertir en projet] en mettant à jour les informations Détails du projet dans votre [!UICONTROL Modèle de mise en page].
      >
      >* Pour mettre à jour les champs dans la variable [!UICONTROL Finance] dans la section [!UICONTROL Convertir en projet] que vous devez avoir [!UICONTROL Modifier] accès à [!UICONTROL Données financières] dans votre niveau d’accès. Si vous avez [!UICONTROL Affichage] accès à [!UICONTROL Données financières] dans votre niveau d’accès, toutes les informations financières du modèle sont transférées vers le nouveau projet et vous ne pouvez pas les modifier pendant que vous convertissez le problème. Pour plus d’informations, voir [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) et [Partage d’un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).


   1. (Facultatif et conditionnel) Cliquez sur [!UICONTROL **Options**] dans le panneau de gauche, puis sélectionnez l’une des options disponibles :

      * [!UICONTROL **Conserver le problème d’origine et lier sa résolution à ce projet**]

         Si cette option est désélectionnée, le problème d’origine est supprimé.

         >[!NOTE]
         >
         >Les utilisateurs n’ayant pas accès ou les autorisations nécessaires pour supprimer des problèmes ne pourront pas supprimer le problème lorsqu’ils le convertissent, quel que soit l’état de ce paramètre. Pour plus d’informations sur l’accès et les autorisations pour les problèmes, voir :
         >
         >* [Accorder l’accès aux problèmes](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
         > 
         >* [Partage d’un problème](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


      * [!UICONTROL **Autoriser (nom d’utilisateur) à accéder à ce projet**]

         Si cette option n’est pas sélectionnée, le problème est [!UICONTROL Contact Principal] n’a aucun accès à la nouvelle tâche.

         >[!NOTE]
         >
         >Les options disponibles ici dépendent de la manière dont l’administrateur Workfront les a configurées pour tous les utilisateurs du système ou pour votre groupe. Pour plus d’informations, voir [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
         >
         >
         >Ou, si les groupes de niveau supérieur de votre organisation les ont configurés séparément, les options disponibles ici dépendent du groupe que vous avez sélectionné pour le nouveau projet à l’étape 6. Pour plus d’informations, voir [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).
   1. Cliquez sur [!UICONTROL **Forms personnalisée**] et effectuez l’une des opérations suivantes :

      * Examinez les formulaires personnalisés associés au modèle. Ils seront transférés vers le nouveau projet.
      * Assurez-vous que tous les champs requis contiennent des informations valides.
      * Réorganiser les formulaires personnalisés en les faisant glisser ![](assets/drag-object-icon.png) où vous les voulez.
      * Cliquez sur le bouton **x** à droite d’un formulaire que vous ne souhaitez pas transférer vers le projet.
      * Si nécessaire, transférez les informations de formulaire personnalisées du problème vers le projet.

         >[!TIP]
         >
         >* Si un formulaire personnalisé à plusieurs objets associé au problème est configuré pour être utilisé avec les problèmes et les projets, toutes les informations enregistrées dans le formulaire sont conservées lorsque vous effectuez la conversion.
         >
         >* Si vous utilisez un modèle pour la conversion et qu’un formulaire personnalisé associé au modèle contient un champ personnalisé qui se trouve également dans un formulaire personnalisé associé au problème, la valeur de champ du problème est utilisée pour le nouveau projet. Cependant, si le champ personnalisé est vide sur le problème, la valeur du modèle est utilisée.

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




1. (Facultatif) Définissez d’autres &#x200B; de détails du projet (propriétaire du projet, dates du projet) et tâches, le cas échéant.
1. Cliquez sur [!UICONTROL **Convertir en projet**].

   Le problème est désormais converti en projet.

1. Cliquez sur [!UICONTROL **Aller au projet**] à l’intérieur de [!UICONTROL Succès] dans le coin supérieur droit de la page. La page du projet s’ouvre alors.
