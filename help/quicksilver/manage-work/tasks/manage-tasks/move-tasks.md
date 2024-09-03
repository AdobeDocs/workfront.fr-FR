---
product-area: projects
navigation-topic: manage-tasks
title: Déplacer les tâches
description: Vous pouvez déplacer des tâches vers différents projets ou vers différentes tâches parent dans Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 421fd012c2ce6a4ae0b11fe343c279d1a3fd551c
workflow-type: tm+mt
source-wordcount: '1488'
ht-degree: 100%

---

# Déplacer les tâches

Vous pouvez déplacer des tâches dans Adobe Workfront entre les objets suivants :

* Une tâche ad hoc vers un projet.
* Une tâche d’un projet vers un autre projet.
* Une tâche d’un projet sous un autre parent dans un autre projet.
* Une tâche dans le même projet sous un parent différent.

Vous pouvez déplacer une tâche au niveau de la tâche ou déplacer une tâche à partir d’une liste de tâches.
Vous pouvez déplacer une seule tâche ou plusieurs tâches à la fois depuis une liste de tâches.

## Conditions d’accès

Vous devez disposer des droits d’accès suivants pour effectuer les actions décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Nouveau plan : standard </p> 
 <p>ou</p>  
<p>Plan actuel : travail ou supérieur </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion pour les tâches</p> <p>Autorisations de contribution ou supérieures au projet avec possibilité d’ajouter des tâches</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Remarques concernant le déplacement des tâches

Tenez compte des points suivants lors du déplacement d’une tâche :

* Lorsque vous déplacez une tâche d’un projet à un autre, les dates de la tâche peuvent être recalculées. Le nouveau calcul prendra en compte le planning utilisé par le nouveau projet, ainsi que les informations « Planifier à partir de » du projet.

* Vous pouvez choisir de déplacer certains éléments associés à la tâche vers la tâche déplacée pendant le processus de déplacement. Toutefois, par défaut, les objets suivants sont transférés vers la tâche déplacée :

   * Problèmes
   * Heures consignées
   * Commentaires des utilisateurs et des utilisatrices
   * Formulaires personnalisés et informations sur les champs personnalisés
   * Sous-tâches

Par défaut, les éléments suivants ne se déplacent pas avec la tâche :

* Jalons

## Déplacer des tâches dans une liste

1. Accédez au projet qui contient la ou les tâches que vous souhaitez déplacer.
1. Cliquez sur **Tâche** dans le panneau de gauche pour afficher la liste des tâches.
1. Cliquez sur l’icône **Mode Plan** ![](assets/plan-mode-icon.png) et assurez-vous que le bouton (bascule) **Enregistrement automatique** est activé, puis sélectionnez la ou les tâches que vous souhaitez déplacer.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >Vous ne pouvez pas déplacer des tâches lorsque le bouton (bascule) **Enregistrement automatique** est désactivé.

1. (Facultatif et le cas échéant) Si vous souhaitez déplacer les tâches sélectionnées dans le même projet, cliquez sur les tâches que vous avez sélectionnées, faites-les glisser et déposez-les à l’endroit où vous souhaitez les déplacer dans le projet.

   Une fois que vous avez déposé les tâches au bon endroit sur le projet, les modifications que vous avez apportées à la hiérarchie de la tâche sont immédiatement enregistrées. Toutes les informations associées à chaque tâche sont déplacées avec les tâches.

1. (Le cas échéant) Sélectionnez la ou les tâches à déplacer, puis effectuez l’une des opérations suivantes :

   * Cliquez sur le menu **Plus** ![](assets/qs-more-menu.png) en haut de la liste des tâches, puis sur **Déplacer vers**.
   * Faites un clic droit sur les tâches sélectionnées, puis sélectionnez **Déplacer vers**.
   * Lorsque vous sélectionnez une tâche, cliquez sur le menu **Plus** ![](assets/more-icon-task-list.png) en regard du nom de la tâche dans la liste, puis sur **Déplacer vers**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   La zone Déplacer la tâche s’affiche.

1. Continuez à déplacer la tâche en suivant l’étape 4 de la section [Déplacer une tâche au niveau de la tâche](#move-a-task-at-the-task-level) de cet article.

   <!--
   is this still accurate?!
   -->

## Déplacer une tâche au niveau de la tâche {#move-a-task-at-the-task-level}

En plus de déplacer des tâches d’une liste de tâches, vous pouvez également déplacer une tâche au niveau de la tâche, une fois que vous l’avez ouverte.

1. Accédez à une tâche dans votre système Workfront en la recherchant.
1. Cliquez sur le nom de la tâche pour l’ouvrir.
1. Cliquez sur le menu déroulant **Plus** ![](assets/qs-more-menu.png) en regard du nom de la tâche, puis sur **Déplacer vers**. La zone Déplacer la tâche s’affiche.

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (Facultatif) Mettez à jour le **Nom de la tâche**. La tâche renommée est alors déplacée vers le nouvel emplacement. Workfront n’enregistre pas le nom initial de la tâche.

   >[!TIP]
   >
   >Le champ Nom de la tâche est grisé et ne peut pas être modifié lorsque vous choisissez de déplacer plusieurs tâches dans une liste. Vous pouvez placer le pointeur sur le champ Nom de la tâche pour afficher la liste de toutes les tâches sélectionnées.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Saisissez le nom du **Projet de destination** où vous souhaitez déplacer la tâche dans le champ **Sélectionner le projet de destination**.

   Si vous souhaitez déplacer la tâche dans le même projet, saisissez le nom du projet actif.

   >[!TIP]
   >
   >* Le nom du projet est sensible à la casse.
   >* Vous pouvez également commencer à saisir le numéro de référence ou l’ID du projet. Cela peut vous aider à distinguer les projets portant des noms identiques.
   >* Seuls 100 projets s’affichent dans la liste.

1. (Le cas échéant) Cliquez sur **Demander l’accès** pour demander l’accès au projet, si vous ne pouvez pas y accéder.
1. (Le cas échéant) Continuez à déplacer la tâche vers le projet de destination sélectionné sans demander l’accès si vous avez accès à l’une des tâches du projet de destination.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Des messages similaires s’affichent si le projet sélectionné est en attente d’approbation, terminé ou inactif, lorsque l’administration de Workfront empêche l’ajout de tâches à ces projets. Pour plus d’informations, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Facultatif) Cliquez sur **Options** dans le panneau de gauche.

   Ou

   Faites défiler l’écran vers le bas jusqu’à la section **Options** de la zone Déplacer la tâche, puis désélectionnez l’un des éléments répertoriés dans le tableau ci-dessous pour les supprimer des tâches déplacées. Toutes les options sont sélectionnées par défaut.

   >[!IMPORTANT]
   >
   >La désélection d’éléments dans la liste des options entraîne une perte de données. Les informations de la tâche existante seront supprimées de manière irréversible.

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
      <p><b>NOTE</b>

   Lorsque vous déplacez ou copiez une tâche avec des contraintes de date spécifiques vers un autre projet et que les dates de contrainte de la tâche ne correspondent pas aux dates du nouveau projet, la contrainte de tâche passe à Aussi Tôt Que Possible ou Aussi Tard Que Possible, ou les dates de début ou de fin prévues des projets sont ajustées.

   Vous trouverez ci-dessous des exemples de contraintes spécifiques aux dates :
   <ul>
      <li> Démarré le</li>
      <li> Il Faut Finir Le</li>
      <li> Commencer Au Plus Tôt</li>
      <li> Commencer Au Plus Tard</li>
      </ul>

   Pour plus d’informations sur les contraintes de tâche et sur la manière dont les contraintes de tâche ou les dates de projet peuvent être affectées, voir <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Vue d’ensemble des contraintes de tâches</a> et recherchez une contrainte spécifique.</p> </td>
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
      <td>Le statut de la tâche passe à Nouveau. Sinon, le statut existant de la tâche est conservé. </td> 
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
      <td> <p>Les documents joints à la tâche ne sont pas transférés vers la tâche déplacée. Il s’agit notamment des versions, des épreuves et des documents associés.</p> <p>Les approbations de documents suivent un processus distinct. Les approbations de document ne peuvent jamais être déplacées lorsqu’une tâche est déplacée.</p> 
      <b>NOTE</b>

   Si vous choisissez de ne pas déplacer les documents avec la tâche, ces derniers seront supprimés et placés dans la corbeille pendant 30 jours. Un administrateur ou une administratrice peut les restaurer vers la tâche déplacée.

   Si la tâche est supprimée après son déplacement, les documents restaurés sont placés dans la zone Documents de la page d’utilisation de l’administrateur ou de l’administratrice qui procède à la restauration.

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



1. (Facultatif) Cliquez sur **Sélectionner le parent** dans le panneau de gauche,

   Ou

   faites défiler l’écran jusqu’à la section **Sélectionner le parent**, puis sélectionnez la tâche dans le projet de destination qui doit devenir le parent de la tâche déplacée.

   >[!TIP]
   >
   >Lorsque vous choisissez de déplacer plusieurs tâches dans une liste, toutes les tâches sélectionnées deviennent les enfants du parent sélectionné.

   Sélectionnez un parent en effectuant l’une des opérations suivantes :

   * Dans la liste des tâches, sélectionnez l’un des parents du plan de projet.
   * Cliquez sur l’icône de recherche ![Icône de recherche](assets/search-icon.png) et recherchez une tâche parent par nom.

   La tâche s’affiche dans la liste.

   ![Sélection d’une tâche parent lors du déplacement d’une tâche avec la fonctionnalité de recherche](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Sélectionnez la case d’option du parent une fois que vous l’avez trouvée.

   Si vous ne sélectionnez pas de tâche parent, les tâches sont déplacées en tant que tâches principales plutôt que sous-tâches et elles sont placées à la fin de la liste des tâches sur le projet de destination.

1. Cliquez sur **Déplacer la tâche**.

   Ou

   Cliquez sur **Déplacer les tâches** lorsque vous sélectionnez plusieurs tâches dans une liste.

   Les tâches déplacées se trouvent désormais sur le projet spécifié et sont soit des sous-tâches d’une tâche parent, soit les dernières tâches du projet.
