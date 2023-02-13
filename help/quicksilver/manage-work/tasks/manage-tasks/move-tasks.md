---
product-area: projects
navigation-topic: manage-tasks
title: Déplacer les tâches
description: Vous pouvez déplacer des tâches vers différents projets ou vers différentes tâches parentes dans Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 23a08c929b0a227c7a555af70ff731ef2df7a179
workflow-type: tm+mt
source-wordcount: '1360'
ht-degree: 2%

---

# Déplacer les tâches

Vous pouvez déplacer des tâches dans Adobe Workfront entre les objets suivants :

* Tâche ad hoc sur un projet.
* Tâche d’un projet à un autre.
* Tâche d’un projet sous un autre parent dans un autre projet.
* Tâche dans le même projet sous un parent différent.

Vous pouvez déplacer une tâche au niveau de la tâche ou déplacer une tâche à partir d’une liste de tâches.

## Exigences d’accès

Vous devez disposer des droits d’accès suivants pour effectuer les actions décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour les tâches</p> <p>Attribuer ou des autorisations supérieures au projet avec possibilité d’ajouter des tâches</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Déplacer une tâche dans une liste

Pour déplacer une tâche affichée dans une liste de tâches :

1. Accédez au projet qui contient la ou les tâches que vous souhaitez déplacer.
1. Cliquez sur **Tâches** dans le panneau de gauche pour afficher la liste des tâches.
1. Assurez-vous que la variable **Enregistrement automatique** Le bouton bascule est activé, puis sélectionnez la ou les tâches que vous souhaitez déplacer.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas déplacer des tâches lorsque la variable **Enregistrement automatique** La bascule est désactivée.

1. (Facultatif et conditionnel) Si vous souhaitez déplacer les tâches sélectionnées dans le même projet, cliquez sur les tâches que vous avez sélectionnées, faites-les glisser et déposez-les là où vous souhaitez les déplacer dans le projet.

   Une fois que vous avez déposé les tâches au bon endroit sur le projet, les modifications que vous avez apportées à la hiérarchie de la tâche sont immédiatement enregistrées. Toutes les informations associées à chaque tâche sont déplacées avec les tâches.

1. (Conditionnel) Sélectionnez la ou les tâches à déplacer, puis effectuez l’une des opérations suivantes :

   * Cliquez sur le bouton **Plus** menu ![](assets/qs-more-menu.png) en haut de la liste des tâches, puis cliquez sur **Déplacer vers**.
   * Cliquez avec le bouton droit de la souris sur les tâches sélectionnées, puis cliquez sur **Déplacer vers**.
   * Lorsque vous sélectionnez une tâche, cliquez sur le bouton **Plus** menu ![](assets/more-icon-task-list.png) en regard du nom de la tâche dans la liste, puis cliquez sur **Déplacer vers**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   La zone Déplacer la tâche s’affiche.

1. Poursuivez le déplacement de la tâche, comme décrit dans la section . [Déplacer une tâche au niveau de la tâche](#move-a-task-at-the-task-level) dans cet article, en commençant par l’étape 4.

   <!--
   is this still accurate?!
   -->

## Déplacer une tâche au niveau de la tâche {#move-a-task-at-the-task-level}

En plus de déplacer des tâches d’une liste de tâches, vous pouvez également déplacer une tâche au niveau de la tâche, une fois que vous l’avez ouverte. 

1. Recherchez une tâche dans votre système Workfront en la recherchant.
1. Cliquez sur le nom de la tâche pour l’ouvrir.
1. Cliquez sur le bouton **Plus** menu déroulant ![](assets/qs-more-menu.png) en regard du nom de la tâche, puis cliquez sur **Déplacer vers**. La zone Déplacer la tâche s’affiche.

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (Facultatif) Mettez à jour la variable **Nom de la tâche**. La tâche se déplace avec le nouveau nom au nouvel emplacement. Workfront n’enregistre pas le nom d’origine de la tâche.

   >[!TIP]
   >
   >Ce champ est grisé et ne peut pas être modifié lorsque vous sélectionnez de déplacer plusieurs tâches dans une liste. Vous pouvez placer le pointeur de la souris sur le champ Nom de la tâche pour afficher la liste de toutes les tâches sélectionnées.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Saisissez le nom de la variable **Projet de destination** où vous souhaitez que la tâche se déplace dans la **Sélectionner le projet de destination** champ .

   Si vous souhaitez déplacer la tâche dans le même projet, saisissez le nom du projet actif.

   >[!TIP]
   >
   >* Le nom du projet est sensible à la casse.
   >* Vous pouvez également commencer à saisir le numéro de référence ou saisir l’ID du projet. Cela peut vous aider à distinguer les projets portant des noms identiques.
   >* Seuls 100 projets s’affichent dans la liste.


1. (Conditionnel) Cliquez sur **Demande d’accès** pour demander l’accès au projet, si vous n’avez pas accès au projet sélectionné.
1. (Conditionnel) Continuez à déplacer la tâche vers le projet de destination sélectionné sans demander l’accès si vous avez accès à l’une des tâches du projet de destination.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Des messages similaires s’affichent si le projet sélectionné est en attente d’approbation, terminé ou mort, lorsque l’administrateur de Workfront empêche l’ajout de tâches à ces projets. Pour plus d’informations, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Facultatif) Cliquez sur **Options** dans le panneau de gauche

   Ou

   Faites défiler l’écran vers le bas jusqu’à **Options** dans la zone Déplacer la tâche , puis désélectionnez l’un des éléments répertoriés dans le tableau ci-dessous pour les supprimer des tâches déplacées. Toutes les options sont sélectionnées par défaut.

   >[!IMPORTANT]
   La désélection d’éléments dans la liste Options entraîne une perte de données. Les informations de la tâche existante seront supprimées et ne pourront pas être récupérées.

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
      <td> <p>La contrainte de tâche est définie sur Dès que possible ou Aussi tard que possible en fonction du paramètre Mode de planification du projet.</p> <p> Lorsque cette option est sélectionnée, la contrainte actuelle de la tâche est transférée avec la tâche. </p> 
      <p><b>NOTE</b>

   Lorsque vous déplacez ou copiez une tâche avec des contraintes de date spécifiques à un autre projet et que les dates de contrainte de la tâche ne correspondent pas aux dates du nouveau projet, la contrainte de tâche passe à Dès que possible ou Aussi tard que possible ou les dates de début planifié ou de fin planifiée des projets sont ajustées.

   Vous trouverez ci-dessous des exemples de contraintes spécifiques à une date :
   <ul>
      <li> Démarré le</li>
      <li> Il Faut Finir Le</li>
      <li> Commencer Au Plus Tôt</li>
      <li> Commencer Au Plus Tard</li>
      </ul>

   Pour plus d’informations sur les contraintes de tâche et sur la manière dont les contraintes de tâche ou les dates de projet peuvent être affectées, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Présentation de la contrainte de tâche</a> et recherchez une contrainte spécifique.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Affectations</td> 
      <td> <p>Toutes les affectations sont supprimées de la tâche. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processus d'approbation</td> 
      <td>Tous les processus de validation sont supprimés de la tâche.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progression</td> 
      <td>L’état de la tâche est Nouveau. Sinon, l’état de la tâche existante est conservé. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informations financières</td> 
      <td>Les informations financières de la tâche sont supprimées et Workfront met à jour le Type de coût de la tâche sur Aucun coût et le Type de revenu de la tâche sur Non facturable. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tous les prédécesseurs</td> 
      <td> <p>Lorsque cette option est sélectionnée, la dépendance devient un prédécesseur multi-projet lorsque vous déplacez la tâche vers un autre projet. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td> <p>Les documents joints à la tâche ne sont pas transférés vers la tâche déplacée. Cela inclut les versions, les bons à tirer et les documents liés.</p> <p>Cela ne comprend pas les approbations de documents. Les validations de document ne peuvent jamais être déplacées lorsqu’une tâche est déplacée.</p> 
      <b>NOTE</b>

   Si vous choisissez de ne pas déplacer les documents avec la tâche, les documents seront supprimés et placés dans la Corbeille pendant 30 jours. Un administrateur peut les restaurer et ils seront restaurés lors de la tâche déplacée.

   Si la tâche est supprimée après son déplacement, les documents restaurés sont placés dans la zone Documents de la page utilisateur de l’administrateur qui les restaure.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications de rappel</td> 
      <td>Les rappels de tâche ne sont pas transférés vers la tâche déplacée. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td>Les dépenses enregistrées sur la tâche ne sont pas transférées vers la tâche déplacée. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autorisations</td> 
      <td> <p>Workfront supprime les noms de toutes les entités qui s'affichent dans la liste Partage de la tâche. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (Facultatif) Cliquez sur **Sélectionner le parent** dans le panneau de gauche

   Ou

   Faites défiler l’écran jusqu’à **Sélectionner le parent** , puis sélectionnez la tâche dans le projet de destination que vous souhaitez devenir le parent de la tâche déplacée.

   >[!TIP]
   Lorsque vous choisissez de déplacer plusieurs tâches dans une liste, toutes les tâches sélectionnées deviennent les enfants du parent sélectionné.

   Sélectionnez un parent en effectuant l’une des opérations suivantes :

   * Dans la liste des tâches, sélectionnez l’un des parents du plan de projet.
   * Cliquez sur l’icône de recherche ![Icône Rechercher](assets/search-icon.png) et recherchez une tâche parente par nom.

   La tâche doit apparaître dans la liste.

   ![Sélection d’une tâche parente lors du déplacement d’une tâche avec une fonctionnalité de recherche ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Sélectionnez le bouton radio du parent une fois que vous l’avez trouvé.

   Si vous ne sélectionnez pas de tâche parent, les tâches sont déplacées en tant que tâches principales plutôt que sous-tâches et elles seront placées à la fin de la liste des tâches sur le projet de destination.

1. Cliquez sur **Tâche de déplacement**

   Ou

   Cliquez sur **Déplacer les tâches** lorsque vous sélectionnez plusieurs tâches dans une liste.
Les tâches déplacées se trouvent désormais sur le projet spécifié et sont soit des sous-tâches à une tâche parente, soit les dernières tâches du projet.
