---
product-area: projects;templates
navigation-topic: create-projects
title: Créer un projet à partir d’un modèle
description: Vous pouvez utiliser des modèles en tant que cadre pour créer des projets dans Adobe Workfront. Si des projets se répètent fréquemment, l’utilisation de modèles pour le nouveau projet vous évite d’avoir à créer les mêmes projets à plusieurs reprises.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '1159'
ht-degree: 92%

---

# Créer un projet à partir d’un modèle

<!-- Audited: 01/2024 -->

Vous pouvez utiliser des modèles comme cadre pour créer des projets dans Adobe Workfront. Si certains de vos projets se répètent fréquemment, vous pouvez utiliser des modèles pour la chronologie générale du nouveau projet pour éviter de créer le même projet à nouveau.

Les modèles vous permettent de capturer des processus, des informations et des paramètres reproductibles associés à vos projets. Les informations associées à un modèle sont transférées vers le projet. Cela inclut les tâches, les affectations, les durées, les documents, les détails financiers, les risques et les formulaires personnalisés.

>[!TIP]
>
>Workfront définit le groupe et le statut du nouveau projet comme suit :
>
>* Le statut par défaut d’un projet créé à partir d’un modèle correspond au statut défini par votre administrateur ou une administratrice Workfront dans la zone principale Préférences du projet, ou par un administrateur ou une administratrice de groupe (ou un administrateur ou une administratrice Workfront) dans la zone Préférences du projet pour un groupe. Pour plus d’informations sur la configuration des préférences du projet, consultez [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Configurer les préférences de projet de groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* Le groupe du nouveau projet est le groupe du modèle. Si le modèle n’est pas associé à un groupe, le groupe du projet est le groupe principal de l’utilisateur ou de l’utilisatrice qui crée le projet.
>
>* Les statuts disponibles pour un nouveau projet correspondent aux statuts du groupe du projet (qui peut être le groupe du modèle ou le groupe principal de l’utilisateur ou de l’utilisatrice qui a créé le projet).

Vous disposez des options suivantes pour créer un projet à partir d’un modèle :

* Créer un projet à partir d’un modèle dans la zone Projets
* Créer un projet à partir d’un modèle au niveau du modèle
* Joindre un modèle à un projet existant

  Pour plus d’informations, consultez [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Créer un projet à partir d’un modèle dans la zone des groupes

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Workfront</td> 
   <td> <p>Standard</p>
        <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux projets et aux modèles</p>
   <p>Modifiez l’accès aux Portfolios et Programmes si le modèle que vous utilisez contient un Portfolio et un Programme</p>  
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage pour un modèle</p> 
  <p>Si le modèle que vous utilisez contient un Portfolio et un programme, vous devez disposer des autorisations de niveau Gérer sur le portfolio et le programme pour créer le projet </p> 
   <p>Lorsque vous créez un projet, vous recevez automatiquement les autorisations de gestion du projet.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and to Templates</p>
   
   <p>edit access to Portfolios and Programs, if the template you use contains a Portfolio and a Program</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> 
  <p>If the template you use contains a Portfolio and a Program, you must have Manage permissions to the portfolio and program to create the project </p> 
   <p>When you create a project, you automatically receive Manage permissions to the project.</p></td> 
  </tr> 
 </tbody> 
</table>-->

## Créer un projet à partir d’un modèle dans la zone Projets

Vous pouvez créer un projet à partir de la zone Projets du menu principal, ou à partir de la zone Projets d’un portfolio ou d’un programme.

>[!NOTE]
>
>Votre administrateur ou administratrice système ou administrateur ou administratrice de groupes peut modifier votre interface à l’aide d’un modèle de mise en page. Dans ce cas, certains noms de sections et de zones mentionnées dans les étapes suivantes peuvent être différents dans votre instance de Workfront.

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche. Cliquez sur **Projets**, puis développez **Nouveau projet**.
   * Accédez à un portfolio, puis développez **Nouveau projet**.

     >[!TIP]
     >
     >Lorsque vous créez un projet à l’aide d’un modèle de portfolio, le champ Portfolio du nouveau projet se met à jour pour afficher le portfolio à partir duquel vous avez créé le projet. Le champ Portfolio du modèle est alors remplacé, s’il est spécifié.

   * Accédez à un programme, puis développez **Nouveau projet**.

     >[!TIP]
     >
     >Lorsque vous créez un projet à l’aide d’un modèle issu d’un programme, le champ Programme des nouveaux projets est mis à jour afin d’afficher le programme à partir duquel vous avez créé le projet. Le champ Portfolio du modèle se met à jour pour afficher le portfolio du programme à partir duquel vous avez créé le projet. Cela remplace les champs Programme et Portfolio du modèle, s’ils sont spécifiés.

   * Si vous êtes administrateur ou administratrice de groupes, vous pouvez également créer un projet dans la section Projets d’un groupe que vous gérez. Pour plus d’informations, voir [Créer et modifier les projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >Lorsque vous créez un projet à partir d’un groupe, le groupe à partir duquel vous créez le projet s’affiche dans le champ Groupe du nouveau projet uniquement lorsque le champ Groupe du modèle n’est pas spécifié. Si le champ Groupe du modèle est spécifié, le champ Groupe du nouveau projet correspond à celui du modèle.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![Nouvelles options du projet](assets/new-project-dropdown.png)

1. Cliquez sur le nom d’un modèle dans la liste **Modèles favoris**.

   ![Sélection d’un modèle favori](assets/new-project-from-template-dropdown-with-template-favorites.png)

   Ou

   Procédez comme suit :

   1. Sélectionnez **Nouveau projet à partir d’un modèle**.
   1. Dans le champ **Modèles de recherche**, commencez à saisir le nom d’un modèle et cliquez dessus lorsqu’il s’affiche dans la liste.
   1. Examinez les détails du modèle sur la droite.

      Les détails du modèle sont les suivants :

      * Durée du modèle
      * Propriétaire du modèle
      * Nombre de tâches de niveau supérieur comprenant les noms des trois premières tâches
      * Nombre de toutes les tâches dans le modèle
      * Noms des modèles de formulaires personnalisés

   1. (Facultatif) Passez la souris sur le nom d’un nom de modèle dans le volet de gauche et cliquez sur l’**icône Favoris** **icône** ![icône Favoris](assets/favorites-icon-small.png) pour le marquer comme favori en vue d’une utilisation ultérieure.

      Ou

      Développez la liste **Modèles favoris** et sélectionnez un modèle dans la liste déroulante.

      >[!TIP]
      >
      >Vous pouvez avoir jusqu’à 40 articles marqués comme favoris dans Workfront. Il s’agit notamment de modèles et d’autres éléments.

   1. Cliquez sur **Utiliser un modèle** lorsque vous avez sélectionné un modèle.

      ![Détails du modèle](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >Si la vue Jalon est appliquée à la liste des projets, cliquez sur le nom d’un modèle dans la section **Créer à partir d’un modèle**.
      >
      >
      >![Vue Jalon de la création d’un projet à partir d’un modèle](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   La boîte de dialogue **Nouveau projet** s’ouvre.

   ![Boîte de dialogue Nouveau projet](assets/new-project-from-template-box.png)

1. Si un champ est déjà rempli dans le modèle, il sera pré-rempli dans la boîte de dialogue **Nouveau projet**. Vous pouvez modifier les valeurs pré-remplies pour qu’elles correspondent mieux à votre projet. Pour plus d’informations, consultez [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Cliquez sur **Créer un projet**.

   Tous les détails définis dans le modèle sont associés automatiquement au nouveau projet si vous ne les avez pas modifiés à l’étape précédente.

## Créer un projet à partir d’un modèle dans la zone Modèles

Au lieu de commencer dans la zone Projets, vous pouvez créer un projet à partir d’un modèle.

{{step1-to-templates}}

1. Cliquez sur le nom du modèle à utiliser.
1. Cliquez sur le menu **Plus** ![icône Plus](assets/more-icon.png), puis sur **Créer un projet**.

   ![Créer un projet à partir d’un modèle](assets/project-sharing-on-template.png)

   La boîte de dialogue **Nouveau projet** s’ouvre.

1. Saisissez un nom pour le projet, puis passez en revue chaque section et apportez les modifications nécessaires.

   ![Boîte de dialogue Nouveau projet](assets/new-project-from-template-box.png)

   Si un champ est déjà rempli dans le modèle, il sera pré-rempli dans la boîte de dialogue **Nouveau projet**. Vous pouvez modifier les valeurs pré-remplies pour qu’elles correspondent mieux à votre projet. Pour plus d’informations, consultez [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Cliquez sur **Créer un projet**.

   Tous les détails définis dans le modèle sont associés automatiquement au nouveau projet si vous ne les avez pas modifiés à l’étape précédente.
