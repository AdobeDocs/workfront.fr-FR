---
product-area: projects;templates
navigation-topic: create-projects
title: Créer un projet à partir d’un modèle
description: Vous pouvez utiliser des modèles en tant que cadre pour créer des projets dans Adobe Workfront. Si des projets se répètent fréquemment, l’utilisation de modèles pour le nouveau projet vous évite d’avoir à créer les mêmes projets à plusieurs reprises.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 99%

---

# Créer un projet à partir d’un modèle

<!-- Audited: 01/2024 -->

Vous pouvez utiliser des modèles en tant que cadre pour créer des projets dans Adobe Workfront. Si des projets se répètent fréquemment, l’utilisation de modèles pour la chronologie générale du nouveau projet vous évite d’avoir à créer les mêmes projets à plusieurs reprises.

Les modèles vous permettent de capturer des processus, des informations et des paramètres répétables associés à vos projets. Les informations associées à un modèle sont transférées vers le projet. Cela inclut les tâches, les affectations, les durées, les documents, les détails financiers, les risques et les formulaires personnalisés.

>[!TIP]
>
>Workfront définit le groupe et le statut du nouveau projet comme suit :
>
>* Le statut par défaut d’un nouveau projet créé à partir d’un modèle correspond au statut défini par votre équipe d’administration Workfront dans la zone Préférences du projet principale ou par un administrateur ou une administratrice de groupes (ou un administrateur ou une administratrice Workfront) dans la zone Préférences du projet d’un groupe. Pour plus d’informations sur la configuration des préférences de projet, voir [Configurer les préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Configurer les préférences du projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* Le groupe du nouveau projet est le groupe du modèle. Si le modèle n’est pas associé à un groupe, le groupe du projet est le groupe principal de l’utilisateur ou de l’utilisatrice qui crée le projet.
>
>* Les statuts disponibles pour un nouveau projet correspondent aux statuts du groupe du projet, qui est soit le groupe du modèle, soit le groupe principal de l’utilisateur ou de l’utilisatrice qui crée le projet.

Vous disposez des options suivantes pour créer un projet à partir d’un modèle :

* Créer un projet à partir d’un modèle dans la zone Projets
* Créer un projet à partir d’un modèle au niveau du modèle
* Joindre un modèle à un projet existant

  Pour plus d’informations, voir [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Créer un projet à partir d’un modèle dans la zone Groupes

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Workfront</td> 
   <td> <p>Nouvelle : standard</p>
        <p>ou</p>
        <p>Actuelle : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès en modification aux projets et aux modèles</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage sur un modèle</p> <p>Lorsque vous créez un projet, vous recevez automatiquement les autorisations de gestion du projet.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un projet à partir d’un modèle dans la zone Projets

Vous pouvez créer un projet à partir de la zone Projets du menu principal, ou à partir de la zone Projets d’un portfolio ou d’un programme.

>[!NOTE]
>
>Votre administrateur ou administratrice système ou administrateur ou administratrice de groupes peut modifier votre interface à l’aide d’un modèle de disposition. Dans ce cas, certains noms de sections et de zones mentionnées dans les étapes suivantes peuvent être différents dans votre instance de Workfront.

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche. Cliquez sur **Projets**, puis développez **Nouveau projet**.
   * Accédez à un portfolio, puis développez **Nouveau projet**.

     >[!TIP]
     >
     >Lorsque vous créez un projet à l’aide d’un modèle d’un portfolio, le champ Portfolio du nouveau projet est mis à jour pour afficher le portfolio à partir duquel vous avez choisi de créer le projet. S’il est spécifié, le champ Portfolio du modèle est remplacé.

   * Accédez à un programme, puis développez **Nouveau projet**.

     >[!TIP]
     >
     >Lorsque vous créez un projet à l’aide d’un modèle d’un programme, le champ Programme des nouveaux projets est mis à jour pour afficher le programme à partir duquel vous avez choisi de créer le projet. Le champ Portfolio du modèle est mis à jour pour afficher le portfolio du programme à partir duquel vous avez choisi de créer le projet. S’ils sont spécifiés, les champs Programme et Portfolio du modèle sont remplacés.

   * Si vous êtes administrateur ou administratrice de groupes, vous pouvez également créer un projet dans la section Projets d’un groupe que vous gérez. Pour plus d’informations, voir [Créer et modifier les projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >Lorsque vous créez un projet à partir d’un modèle d’un groupe, le groupe à partir duquel vous créez le projet s’affiche dans le champ Groupe du nouveau projet uniquement lorsque le champ Groupe du modèle n’est pas spécifié. Si le champ Groupe du modèle est spécifié, le champ Groupe du nouveau projet est celui du modèle.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![Options du nouveau projet](assets/new-project-dropdown.png)

1. Cliquez sur le nom d’un modèle dans la liste **Modèles favoris**.

   ![Sélectionnez un modèle favori](assets/new-project-from-template-dropdown-with-template-favorites.png)

   Ou

   Procédez comme suit :

   1. Sélectionnez **Nouveau projet à partir d’un modèle**.
   1. Dans le champ **Rechercher modèles**, commencez à saisir le nom d’un modèle, puis cliquez dessus lorsqu’il s’affiche dans la liste.
   1. Examinez les détails du modèle sur la droite.

      Les détails du modèle sont les suivants :

      * Durée du modèle
      * Personne propriétaire du modèle
      * Nombre de tâches de niveau supérieur comprenant les noms des trois premières tâches
      * Nombre de toutes les tâches dans le modèle
      * Noms des modèles de formulaires personnalisés

   1. (Facultatif) Pointez sur le nom d’un modèle dans le volet de gauche, puis cliquez sur l’**icône** ![](assets/favorites-icon-small.png) **Favoris** afin de le marquer comme favori pour une utilisation ultérieure.

      Ou

      Développez l’objet **Modèles favoris** et sélectionnez un modèle dans la liste déroulante.

      >[!TIP]
      >
      >Vous pouvez avoir jusqu’à 40 articles marqués comme favoris dans Workfront. Il s’agit notamment de modèles et d’autres éléments.

   1. Cliquez sur **Utiliser le modèle** lorsque vous avez sélectionné un modèle.

      ![Détails du modèle](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >Si la vue Jalon est appliquée à la liste des projets, cliquez sur le nom d’un modèle dans la section **Nouveau à partir du modèle**.
      >
      >
      >![Vue Jalon de la création d’un projet à partir d’un modèle](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   La zone **Nouveau projet** s’ouvre.

   ![Zone Nouveau projet](assets/new-project-from-template-box.png)

1. Si un champ est déjà rempli dans le modèle, il s’affiche dans la zone **Nouveau projet**. Vous pouvez modifier les valeurs pré-remplies pour qu’elles correspondent mieux à votre projet. Pour plus d’informations, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Cliquez sur **Créer un projet**.

   Tous les détails définis dans le modèle sont associés automatiquement au projet nouvellement créé si vous ne les avez pas modifiés à l’étape précédente.

## Créer un projet à partir d’un modèle dans la zone Modèles

Au lieu de commencer dans la zone Projets, vous pouvez créer un projet à partir d’un modèle en commençant par celui-ci.

{{step1-to-templates}}

1. Cliquez sur le nom du modèle à utiliser.
1. Cliquez sur le menu **Plus** ![](assets/more-icon.png), puis sur **Créer le projet**.

   ![Créer un projet à partir d’un modèle](assets/project-sharing-on-template.png)

   La zone **Nouveau projet** s’ouvre.

1. Saisissez un nom pour le projet, puis passez en revue chaque section et apportez les modifications nécessaires.

   ![Zone Nouveau projet](assets/new-project-from-template-box.png)

   Si un champ est déjà rempli dans le modèle, il s’affiche dans la zone **Nouveau projet**. Vous pouvez modifier les valeurs pré-remplies pour qu’elles correspondent mieux à votre projet. Pour plus d’informations, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Cliquez sur **Créer un projet**.

   Tous les détails définis dans le modèle sont associés automatiquement au projet nouvellement créé si vous ne les avez pas modifiés à l’étape précédente.
