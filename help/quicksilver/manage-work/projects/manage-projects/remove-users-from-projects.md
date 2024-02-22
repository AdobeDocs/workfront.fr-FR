---
product-area: projects;user-management
navigation-topic: manage-projects
title: Suppression des utilisateurs des projets
description: Vous pouvez supprimer des utilisateurs d’un projet lorsqu’ils ne sont plus impliqués dans la réalisation du projet.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Suppression des utilisateurs des projets

Vous pouvez supprimer des utilisateurs d’un projet lorsqu’ils ne sont plus impliqués dans la réalisation du projet. La suppression des utilisateurs des projets a des implications sur les affectations de tâche et de problème, ainsi que sur les rôles de projet. Suppression des utilisateurs qui ne reçoivent plus de notifications destinées à l’équipe de projet. Pour plus d’informations sur les notifications destinées aux équipes de projet, voir [Types de notification d’événement](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Les utilisateurs associés à un projet sont répertoriés dans la zone Personnes d’un projet. Ils représentent l’équipe de projet. Pour plus d’informations sur l’équipe de projet, voir [Présentation de l’équipe de projet](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations sur le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Comment la suppression d’un utilisateur affecte les tâches, problèmes et projets existants

Lorsqu’un utilisateur est supprimé d’un projet, toutes les tâches ou tous les problèmes qui lui sont affectés peuvent être affectés, selon que la tâche ou le problème a été terminé lorsque l’utilisateur a été supprimé :

* **Si l’élément n’est pas terminé lorsque l’utilisateur est supprimé :** L’élément est réaffecté à un rôle de tâche si un rôle de tâche a déjà été attribué ou s’il est affecté au rôle de tâche que l’utilisateur remplissait sur l’élément. Si l’élément ou l’utilisateur n’avait pas de rôle de tâche attribué, vous devez le réaffecter manuellement.
* **Si l’élément est terminé lorsque l’utilisateur est supprimé :** Le nom de l’utilisateur supprimé reste sur l’élément .
* **Si l’utilisateur supprimé est également le créateur d’un projet :** Le projet n’est pas supprimé de leur **Projets actifs** dans la zone Projets . Le projet est supprimé des listes de tous les autres utilisateurs qui filtrent pour ce projet par le champ Entré par .
* **Si l’utilisateur est le propriétaire ou le parrain du projet :** L’utilisateur reste dans ses rôles de parrain ou de propriétaire du projet.

## Suppression d’utilisateurs d’un projet et d’une équipe de projet

Vous pouvez supprimer des utilisateurs d’un projet en les supprimant de l’équipe de projet.

Lorsque les utilisateurs remplissent des rôles sur un projet, ils font partie de l’équipe de projet.

Lorsque vous supprimez des utilisateurs de leurs rôles sur le projet, ils restent membres de l’équipe du projet.

Pour plus d’informations sur les rôles des utilisateurs dans un projet, voir [Gérer l’équipe de projet](../planning-a-project/manage-project-team.md).

Pour supprimer des utilisateurs de l’équipe de projet :

1. Accédez au projet dans lequel vous souhaitez supprimer les utilisateurs.

1. Cliquez sur **Personnes** dans le panneau de gauche, sélectionnez les utilisateurs à supprimer. Vous devrez peut-être cliquer sur **Afficher plus**, puis **Personnes**.

1. Cliquez sur le bouton **Supprimer** icon  ![Supprimer un élément](assets/remove-icon---x-in-circle.png) en haut de la liste des utilisateurs.

1. Cliquez sur **Oui, Supprimer les utilisateurs sélectionnés** pour confirmer la suppression.

   Les utilisateurs sont supprimés de l’équipe du projet et de toutes les tâches ou problèmes incomplets auxquels ils peuvent être affectés. Ils ne reçoivent plus de notifications destinées à l’équipe de projet.
