---
product-area: projects
navigation-topic: create-projects
title: Importation d’un projet à partir d’un projet Microsoft
description: Vous pouvez importer des projets de Microsoft Project dans Adobe Workfront et gérer tous vos projets dans une seule application. Chaque fois que vous importez un projet à partir d’un projet Microsoft, un nouveau projet est créé dans Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 2%

---

# Importation d’un projet à partir d’un projet Microsoft

Vous pouvez importer des projets de Microsoft Project dans Adobe Workfront et gérer tous vos projets dans une seule application. Chaque fois que vous importez un projet à partir d’un projet Microsoft, un nouveau projet est créé dans Workfront.

>[!IMPORTANT]
>
>Tous les champs de projet Microsoft ne sont pas transférés vers Workfront.
>
>Pour plus d’informations sur la compatibilité des champs entre Workfront et Microsoft Project, voir [Mappage des champs de projet Microsoft aux projets Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Exigences d’accès

ébauché pour P&amp;P :

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
   <td> <p>Licence actuelle : Standard </p> 
   Ou
   <p>Licence héritée : Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux projets, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Accorder l’accès aux projets</a>. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Lorsque vous créez un projet, vous recevez automatiquement les autorisations de gestion du projet. </p> <p> Pour plus d’informations sur les autorisations de projet, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Partage d’un projet dans Adobe Workfront</a>.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux projets, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Accorder l’accès aux projets</a>. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Lorsque vous créez un projet, vous recevez automatiquement les autorisations de gestion du projet. </p> <p> Pour plus d’informations sur les autorisations de projet, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Partage d’un projet dans Adobe Workfront</a>.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Création d’un projet à partir d’un projet MS

Vous pouvez créer un projet à partir de la zone Projets du menu principal ou de la zone Projets d’un portfolio ou d’un programme.

1. Accédez à Projet Microsoft et ouvrez un projet à partir duquel vous souhaitez importer des données dans Workfront.
1. Cliquez sur **Fichier**, puis **Enregistrer sous** pour enregistrer le projet au format .xml.

1. Connectez-vous à Workfront.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur le bouton **Menu Principal** ![](assets/main-menu-icon.png), cliquez sur **Projets**, puis développez **Nouveau projet**.
   * Accédez à un portfolio, puis développez **Nouveau projet**.
   * Accédez à un programme, puis développez **Nouveau projet**.
   * Si vous êtes administrateur de groupe, vous pouvez également créer un projet dans la section Projets d’un groupe que vous gérez. Pour plus d’informations, voir [Création et modification des projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Choisissez la **Importer un projet MS** .

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Cliquez sur **Sélectionner un fichier**, puis recherchez le fichier .xml sur l’ordinateur que vous avez exporté à partir de Microsoft Project.
1. Importez le fichier sélectionné.

   Workfront lance le processus d’importation et crée un projet basé sur le fichier exporté à partir du projet Microsoft.

   Une fois le processus d’importation terminé, vous êtes dirigé vers la nouvelle page du projet qui affiche la confirmation que l’importation s’est correctement terminée.

   >[!NOTE]
   >
   >Workfront est limité à 15 minutes pour les téléchargements de fichiers. Si le téléchargement de fichier prend plus de temps, nous vous recommandons de diviser votre projet en projets plus petits et de les importer séparément. Une fois qu’ils ont été importés dans Workfront, déplacez les tâches d’un projet vers l’autre projet pour les combiner dans un seul projet. Pour plus d’informations sur le déplacement des tâches, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Facultatif) Continuez à modifier le projet dans Workfront. Pour plus d’informations sur la modification de projets, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

   L’état d’un nouveau projet créé à partir d’un modèle correspond à l’état défini par votre administrateur Workfront dans la zone Préférences du projet ou par un administrateur de groupe dans la zone Préférences du projet de groupe . Pour plus d’informations sur la configuration des préférences du projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
