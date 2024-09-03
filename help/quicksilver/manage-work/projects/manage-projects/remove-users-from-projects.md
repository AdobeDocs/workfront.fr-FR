---
product-area: projects;user-management
navigation-topic: manage-projects
title: Supprimer des utilisateurs et utilisatrices d’un projet
description: Vous pouvez supprimer des personnes d’un projet lorsqu’elles ne sont plus impliquées dans la réalisation du projet.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 100%

---

# Supprimer des utilisateurs et utilisatrices d’un projet

Vous pouvez supprimer des personnes d’un projet lorsqu’elles ne sont plus impliquées dans la réalisation du projet. La suppression de personnes des projets a des implications sur les affectations de tâche et de problème, ainsi que sur les rôles de projet. Les personnes supprimées ne reçoivent plus de notifications destinées à l’équipe du projet. Pour plus d’informations sur les notifications destinées aux équipes du prrojet, voir [Types de notification d’événement](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Les personnes associées à un projet sont répertoriées dans la zone Personnes d’un projet. Elles représentent l’équipe du projet. Pour plus d’informations sur les équipes du projet, voir [Vue d’ensemble des équipes du projet](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en modification aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Supprimer une personne affecte les tâches, problèmes et projets existants

Lorsqu’une personne est supprimée d’un projet, toutes les tâches ou tous les problèmes qui lui sont affectés peuvent en souffrir, selon que la tâche ou le problème a été terminé lorsque la personne été supprimée :

* **Si l’élément n’est pas terminé lorsque la personne est supprimée :** l’élément est réaffecté à une fonction si une fonction a déjà été affectée ou si elle est affectée à la fonction que la personne remplissait sur l’élément. Si l’élément ou la personne n’avait pas de fonction affectée, vous devez le ou la réaffecter manuellement.
* **Si l’élément est terminé lorsque la personne est supprimée :** le nom de la personne supprimée reste sur l’élément.
* **Si la personne supprimée est également la personne créatrice d’un projet :** le projet n’est pas supprimé de sa liste **Projets auxquels je participe** dans la zone Projets. Le projet est supprimé des listes de toutes les autres personnes qui filtrent pour ce projet par le champ Saisi par.
* **Si la personne est propriétaire ou sponsor du projet :** la personne reste dans ses rôles de sponsor ou de propriétaire du projet.

## Supprimer des personnes d’un projet et d’une équipe de projet

Vous pouvez supprimer des personnes d’un projet en les supprimant de l’équipe de projet.

Lorsque les personnes remplissent des rôles sur un projet, elles font partie de l’équipe de projet.

Lorsque vous supprimez le rôle d’une personne dans le projet, celle-ci continue à faire partie de l’équipe du projet.

Pour plus d’informations sur les rôles des personnes dans un projet, voir [Gérer l’équipe de projet](../planning-a-project/manage-project-team.md).

Pour supprimer des personnes de l’équipe de projet :

1. Accédez au projet dans lequel vous souhaitez supprimer les personnes.

1. Cliquez sur **Personnes** dans le panneau de gauche, sélectionnez les personnes à supprimer. Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Personnes**.

1. Cliquez sur l’icône **Supprimer** ![Supprimer un élément](assets/remove-icon---x-in-circle.png) en haut de la liste des personnes.

1. Cliquez sur **Oui, supprimer les personnes sélectionnées** pour confirmer la suppression.

   Les personnes sont supprimées de l’équipe du projet et de toutes les tâches ou problèmes incomplets auxquels elles peuvent être affectées. Elles ne reçoivent plus de notifications destinées à l’équipe de projet.
