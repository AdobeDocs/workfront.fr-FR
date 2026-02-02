---
product-area: projects
navigation-topic: manage-tasks
title: Déplacer tâches
description: Vous pouvez déplacer des tâches vers différents projets ou vers différentes tâches parent dans Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 47%

---

# Déplacer les tâches

<!--Audited: 5/2025-->


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Vous pouvez déplacer des tâches dans Adobe Workfront entre les objets suivants :

* Une tâche ad hoc vers un projet.
* Une tâche d’un projet vers un autre projet.
* Une tâche d’un projet sous un autre parent dans un autre projet.
* Une tâche dans le même projet sous un parent différent.

Vous pouvez déplacer une tâche au niveau de la tâche ou déplacer une tâche à partir d’une liste de tâches.

Vous pouvez déplacer une seule tâche ou déplacer plusieurs tâches à la fois à partir d’une liste de tâches.

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
   <td> <p>Standard </p> 
 <p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion pour les tâches</p> <p>Autorisations de contribution ou supérieures au projet avec possibilité d’ajouter des tâches</p>  </td> 
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
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p> 
 <p>or</p>  
<p>Current: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks</p> <p>Contribute or higher permissions to the project with ability to Add Tasks</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Remarques concernant le déplacement des tâches

Tenez compte des points suivants lors du déplacement d’une tâche :

* Votre administrateur système ou de groupe peut vous empêcher de déplacer des tâches comportant des heures consignées en fonction de la manière dont il configure l&#39;option Autoriser les utilisateurs à déplacer les tâches et les événements comportant des heures consignées de préférence dans la zone Configuration. Pour plus d’informations, voir [Configurer les préférences de tâche et de problème à l’échelle du système](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Lorsque vous déplacez une tâche d’un projet à un autre, les dates de la tâche peuvent être recalculées. Le nouveau calcul prendra en compte le planning utilisé par le nouveau projet, ainsi que les informations « Planifier à partir de » du projet.

* Vous pouvez déplacer certains éléments associés à la tâche vers la tâche déplacée au cours du processus de déplacement. Toutefois, par défaut, les objets suivants sont transférés vers la tâche déplacée :

   * Problèmes
   * Heures consignées
   * Commentaires des utilisateurs et des utilisatrices
   * Formulaires personnalisés et informations sur les champs personnalisés
   * Sous-tâches

* Par défaut, les éléments suivants ne se déplacent pas avec la tâche :

   * Jalons

## Déplacer des tâches dans une liste

{{step1-to-projects}}

1. Sur la page **Projets**, sélectionnez le projet contenant la ou les tâches à déplacer.
1. Cliquez sur **Tâche** dans le panneau de gauche pour afficher la liste des tâches.
1. Cliquez sur l’icône **Mode Plan** ![Icône Mode Plan](assets/plan-mode.png) et assurez-vous que le bouton (bascule) **Enregistrement automatique** est activé, puis sélectionnez la ou les tâches à déplacer.

   ![Option d’enregistrement automatique](assets/autosave-icon.png)

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas déplacer des tâches lorsque le bouton (bascule) **Enregistrement automatique** est désactivé.

1. (Facultatif et conditionnel) Si vous souhaitez déplacer les tâches sélectionnées dans le même projet, cliquez sur les tâches sélectionnées, puis faites-les glisser et déposez-les à l’endroit où vous souhaitez les déplacer dans le projet. La hiérarchie de tâches change et est enregistrée immédiatement, et les informations associées à chaque tâche sont déplacées avec les tâches.

1. (Le cas échéant) Sélectionnez la ou les tâches à déplacer, puis effectuez l’une des opérations suivantes :

   * Cliquez sur le menu **Plus** ![icône Plus](assets/main-more-icon.png) en haut de la liste des tâches, puis cliquez sur **Déplacer vers**.
   * Cliquez avec le bouton droit sur les tâches sélectionnées, puis cliquez sur **Déplacer vers**.
   * Lors de la sélection d’une tâche, cliquez sur le menu **Plus** ![icône Plus dans la liste des tâches](assets/more-icon-task-list.png) en regard du nom de la tâche dans la liste, puis cliquez sur **Déplacer vers**.

   La zone **Déplacer la tâche** s’affiche.

1. Continuez à déplacer la tâche comme décrit dans la section [Déplacer une tâche au niveau de la tâche](#move-a-task-at-the-task-level) dans cet article.

   <!--
   is this still accurate?!
   -->

## Déplacer une tâche au niveau de la tâche {#move-a-task-at-the-task-level}

Outre le déplacement de tâches à partir d’une liste de tâches, vous pouvez déplacer une tâche au niveau de la tâche après l’avoir ouverte.

1. Accédez à une tâche dans votre système Workfront en la recherchant.
1. Cliquez sur le nom de la tâche pour l’ouvrir.
1. Cliquez sur le menu déroulant **Plus** ![icône Plus](assets/main-more-icon.png) en regard du nom de la tâche, puis cliquez sur **Déplacer vers**. Le panneau latéral **Déplacer la tâche** s’affiche.

1. (Facultatif) Mettez à jour le **Nom de la tâche**. La tâche est déplacée avec le nouveau nom au nouvel emplacement.

   >[!TIP]
   >
   >Le champ **Nom de la tâche** est grisé et n’est pas modifiable lorsque vous choisissez de déplacer plusieurs tâches dans une liste. Vous pouvez pointer sur le champ **Nom de la tâche** pour afficher la liste de toutes les tâches sélectionnées.
   >
   >
   >![Afficher les noms des tâches](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Dans le champ **Sélectionner le projet de destination**, saisissez le nom du projet vers lequel vous souhaitez déplacer la tâche. Si vous souhaitez déplacer la tâche dans le même projet, saisissez le nom du projet actif.

   >[!TIP]
   >
   >* Le nom du projet respecte la casse.
   >* Vous pouvez rechercher un projet en saisissant son numéro de référence ou son identifiant. Cela peut vous aider à faire la distinction entre les projets portant des noms identiques.
   >* Seuls 100 projets s’affichent dans la liste.

1. (Conditionnel) Si vous n’avez pas accès au projet, cliquez sur **Demander l’accès**.
1. (Conditionnel) Continuez à déplacer la tâche vers le projet de destination sans demander l’accès si vous avez accès à l’ajout de tâches à l’une des tâches du projet de destination.

   ![Déplacer une tâche sans demander l’accès](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Des messages similaires s’affichent si le projet sélectionné est en attente d’approbation, terminé ou immobilisé lorsque l’administrateur Workfront empêche l’ajout de tâches à ces projets. Pour plus d’informations, consultez la section [Configurer des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Facultatif) Dans la section **Options**, désélectionnez l’un des éléments répertoriés dans le tableau ci-dessous pour le supprimer des tâches déplacées. Toutes les options sont sélectionnées par défaut.

   >[!IMPORTANT]
   >
   >La désélection d’éléments dans la liste **Options** entraîne une perte de données. Les informations de la tâche existante seront supprimées et ne pourront pas être récupérées.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sélectionner tout</td> 
      <td>Désélectionnez cette option pour supprimer toutes les informations de la tâche lorsque vous la déplacez vers son nouvel emplacement. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Contrainte</td> 
      <td> <p>La contrainte de tâche est définie sur Aussi Tôt Que Possible ou Aussi Tard Que Possible en fonction du paramètre Mode horaire du projet.</p> <p> Lorsque cette option est sélectionnée, la contrainte actuelle de la tâche est transférée avec la tâche. </p> 
      <p>Note : Lorsque vous déplacez ou copiez une tâche avec des contraintes spécifiques à une date vers un autre projet et que les dates de contrainte de la tâche sont en dehors des nouvelles dates du projet, la contrainte de tâche devient Dès Que Possible ou Le Plus Tard Possible ou les dates de début prévu ou d'achèvement prévu des projets sont ajustées.

   Vous trouverez ci-dessous des exemples de contraintes spécifiques aux dates :
   <ul>
      <li> Démarré le</li>
      <li> Il Faut Finir Le</li>
      <li> Commencer Au Plus Tôt</li>
      <li> Commencer Au Plus Tard</li>
      </ul>

   Pour plus d’informations, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Vue d’ensemble des contraintes de tâche</a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Affectations</td> 
      <td> <p>Toutes les affectations sont supprimées de la tâche. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processus d’approbation</td> 
      <td>Tous les processus de validation sont supprimés de la tâche.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progression</td> 
      <td>Le statut de la tâche est défini sur Nouveau. Sinon, le statut existant de la tâche est conservé. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informations financières</td> 
      <td>Les informations financières de la tâche sont supprimées et Workfront met à jour le Type de coût de la tâche sur Aucun coût et le Type de revenu de la tâche sur Non facturable. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toutes les tâches antérieures</td> 
      <td> <p>Lorsque cette option est sélectionnée, la dépendance devient un projet transversal antérieur lorsque vous déplacez la tâche vers un autre projet. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td> <p>Les documents joints à la tâche ne sont pas transférés vers la tâche déplacée. Il s’agit notamment des versions, des épreuves et des documents associés.</p> <p>Cela n’inclut pas les approbations de documents. Les approbations de document ne peuvent jamais être déplacées lorsqu’une tâche est déplacée.</p> 
      <p>Remarque : si vous choisissez de ne pas déplacer les documents avec la tâche, les documents seront supprimés et placés dans la corbeille pendant 30 jours. Un administrateur ou une administratrice peut les restaurer vers la tâche déplacée. </p>

   <p>Si la tâche est supprimée après son déplacement, les documents restaurés sont placés dans la zone Documents de la page d’utilisation de l’administrateur ou de l’administratrice qui procède à la restauration.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications de rappel</td> 
      <td>Les rappels de tâche ne sont pas transférés vers la tâche déplacée. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td>Les dépenses consignées sur la tâche ne sont pas transférées vers la tâche déplacée. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autorisations</td> 
      <td> <p>Workfront supprime les noms de toutes les entités qui s’affichent dans la liste Partage de la tâche. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (Facultatif) Dans la section **Sélectionner le parent**, sélectionnez la tâche du projet de destination qui deviendra le parent de la tâche déplacée.

   >[!TIP]
   >
   >Lorsque vous choisissez de déplacer plusieurs tâches dans une liste, toutes les tâches sélectionnées deviennent les enfants du parent sélectionné.

   Sélectionnez un parent en effectuant l’une des opérations suivantes :

   * Dans la liste des tâches, sélectionnez l’un des parents du plan de projet.
   * Cliquez sur l’icône de recherche ![Icône de recherche](assets/search-icon.png) et recherchez une tâche parent par nom.

   La tâche s’affiche dans la liste.

   ![Sélection d’une tâche parent lors du déplacement d’une tâche avec la fonctionnalité de recherche](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

   >[!NOTE]
   >
   >Si vous ne sélectionnez pas de tâche parent, les tâches sont déplacées en tant que tâches principales plutôt que sous-tâches, et elles sont placées à la fin de la liste des tâches sur le projet de destination.

1. Cliquez sur **Déplacer la tâche**. Les tâches sont déplacées vers le projet spécifié sous forme de sous-tâches vers une tâche parent ou les dernières tâches du projet.
