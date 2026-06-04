---
product-area: projects
navigation-topic: create-projects
title: Importer un projet à partir de Microsoft Project
description: Vous pouvez importer des projets de Microsoft Project dans Adobe Workfront et gérer tous vos projets dans une seule application. Chaque fois que vous importez un projet depuis Microsoft Project, un nouveau projet est créé dans Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/drxvgi-xQLjEt5JOL6-MxLdkmVcXxkcXMN14nwmNZvs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 604
ht-degree: 58%

---

# Importer un projet à partir de Microsoft Project

<!-- Audited: 10/2025 -->

Vous pouvez importer des projets de Microsoft Project dans Adobe Workfront et gérer tous vos projets dans une seule application. Chaque fois que vous importez un projet depuis Microsoft Project, un nouveau projet est créé dans Workfront.

>[!IMPORTANT]
>
>Tous les champs de Microsoft Project ne sont pas transférés dans Workfront.
>
>Pour plus d’informations sur la compatibilité des champs entre Workfront et Microsoft Project, voir [Mapper des champs Microsoft Project à des projets Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

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
    <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Accès en modification aux projets</p> 
   <p>Si vous ajoutez un projet à un portefeuille ou à un programme, vous devez disposer d'un accès en modification aux portefeuilles et programmes.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Lorsque vous créez un projet, vous recevez automatiquement les droits de gestion du projet.</p>
   <p>Si vous ajoutez un projet à un portfolio ou à un programme, vous devez disposer des autorisations de gestion pour le portfolio et le programme.</p>
   </td> 
    </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
old permissions model: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Créer un projet à partir d’un projet MS

Vous pouvez créer un projet à partir de la zone **Projets** du **Menu principal** ou à partir de la zone **Projets** d’un portefeuille ou d’un programme.

1. Connectez-vous au projet Microsoft et ouvrez un projet à partir duquel vous souhaitez effectuer un import dans Workfront.
1. Cliquez sur **Fichier**, puis sur **Enregistrer sous** pour enregistrer le projet en tant que fichier .xml.

1. Connectez-vous à Workfront.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Projets** et développez **Nouveau projet**.
   * Accédez à un portfolio, puis développez **Nouveau projet**.
   * Accédez à un programme, puis développez **Nouveau projet**.
   * Si vous êtes un administrateur de groupes, vous pouvez créer un projet dans la section **Projets** d’un groupe que vous gérez. Pour plus d’informations, voir [Créer et modifier les projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Cliquez sur **Importer MS Project**.

   ![Liste déroulante du nouveau projet](assets/import-ms-project-option.png)

   La boîte de dialogue **Importer un fichier MS** s’ouvre.

1. Cliquez sur **Sélectionner un fichier**, puis recherchez le fichier .xml sur votre ordinateur que vous avez exporté à partir du projet Microsoft.
1. Importer le fichier sélectionné. Workfront commence le processus d’import et crée un nouveau projet basé sur le fichier exporté de Microsoft Project.

   >[!NOTE]
   >
   >Workfront a une limite de temps de 15 minutes pour les chargements de fichiers. Si le chargement du fichier prend plus de temps, nous vous recommandons de diviser votre projet en plusieurs projets plus petits et de les importer séparément. Une fois qu’elles ont été importées dans Workfront, déplacez les tâches d’un projet à l’autre pour les combiner en un seul projet. Pour plus d’informations sur le déplacement des tâches, voir [Déplacer des tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

   Une fois le processus d’import terminé, vous faites l’objet d’une redirection vers la page du nouveau projet qui affiche une confirmation que l’import s’est déroulé avec succès.

   >[!CAUTION]
   >
   >Si votre instance Workfront a accès à la fois au stockage cloud Workfront et Adobe pour les documents, l’importation d’un projet à partir de MS Project crée un projet de stockage Workfront hérité, même si votre administrateur Workfront a défini le stockage cloud Adobe par défaut pour votre système.
   >
   >Pour plus d’informations, voir [Présentation de la gestion des documents pour les projets et les objets associés](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).


1. (Facultatif) Continuez à modifier le projet dans Workfront. Pour plus d’informations sur la modification des projets, voir [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).


   >[!NOTE]
   >
   >Le statut d’un nouveau projet créé à partir d’un modèle correspond au statut défini par l’administrateur de Workfront dans la zone **Préférences du projet** ou par un administrateur de groupes dans la zone **Préférences du projet du groupe**. Pour plus d’informations sur la configuration des préférences de projet, voir [Configurer les préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
