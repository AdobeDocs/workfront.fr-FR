---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Attribuer des tâches en bloc à l’aide de l’équilibreur de charge de travail
description: Vous pouvez affecter des ressources à plusieurs tâches et événements en bloc à l’aide de l’équilibreur de charge de travail d’Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 88%

---

# Attribuer du travail en bloc à l’aide de l’équilibreur de charge de travail

<!--Audited: 07/2024-->

Vous pouvez affecter des ressources à plusieurs tâches et événements en bloc à l’aide de l’équilibreur de charge de travail d’Adobe Workfront.

Pour des informations générales sur l’attribution de travail aux utilisateurs et utilisatrices à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’attribution de travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td>
  </tr>
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan, lors de l’utilisation de l’équilibreur de charge de travail dans la zone Ressource ; Travail, lors de l’utilisation de l’équilibreur de charge de travail d’une équipe ou d’un projet</p></td>
  </tr>
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Modifiez l’accès aux éléments suivants :</p> 
    <ul> 
     <li>Gestion des ressources</li> 
     <li>Projets</li> 
     <li>Tâches</li> 
     <li>Problèmes</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Autorisations Contribuer ou supérieures aux projets, tâches et problèmes qui incluent la création d’affectations.</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques sur les affectations en masse dans l’équilibreur de charge de travail

* Vous pouvez rapidement gérer les affectations d’utilisateurs et d’utilisatrices pour plusieurs tâches et problèmes sur un ou plusieurs projets. Les modifications d’affectations sont immédiatement visibles dans l’équilibreur de charge de travail.
* Vous ne pouvez pas affecter de ressources aux éléments de travail terminés ou aux éléments qui se trouvent dans un projet terminé.
* Vous pouvez effectuer les opérations suivantes lorsque vous affectez des utilisateurs et utilisatrices en masse :

   * Affecter un utilisateur ou une utilisatrice à tous les éléments de travail actuellement affectés à une fonction.
   * Remplacer les affectations entre les utilisateurs et utilisatrices.
   * Annuler l’affectation d’un utilisateur ou d’une utilisiatrice à tous ses éléments de travail.

**EXEMPLES**

* Vous devez effectuer des affectations d’utilisateurs et utilisatrices sur plusieurs nouveaux projets. Les projets ont été créés à partir de modèles et les fonctions sont déjà affectées aux différentes tâches des projets. Vous souhaitez affecter une utilisatrice spécifique, Jackie Simms, à toutes les tâches actuellement affectées à une fonction. Vous pouvez utiliser la fonction Affecter pour affecter ces tâches à Jackie Simms.
* 45 tâches sur 3 projets différents sont affectées à Jackie Simms. Jackie quitte l’entreprise et vous devez maintenant réaffecter ses tâches à une autre personne. Vous pouvez utiliser la fonction Remplacer pour affecter ces tâches à la nouvelle personne.
* 10 tâches sur 2 projets différents sont affectées à un autre utilisateur, Rick Kuvec. Vous réalisez que Rick a été affecté à ces tâches par erreur, mais vous ne savez pas à qui elles doivent être affectées à ce moment. Vous devez annuler l’affectation de Rick à toutes les tâches en même temps. Vous pouvez utiliser la fonction Annuler l’affectation pour retirer Rick de ces tâches.

## Attribuer du travail en masse dans l’équilibreur de charge de travail

1. Accédez à l’équilibreur de charge de travail auquel vous souhaitez attribuer du travail.

   Vous pouvez attribuer du travail aux utilisateurs et utilisatrices à l’aide de l’équilibreur de charge de travail dans la zone Ressources, au niveau du projet ou de l’équipe. Pour plus d’informations sur l’emplacement de l’équilibreur de charge de travail dans Workfront, voir [Localiser l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).


1. Cliquez sur **Affectations en bloc** ![Affectations en bloc](assets/bulk-assignments-wb.png) en haut de l’équilibreur de charge de travail.

   Le panneau Affectations groupées s’ouvre à droite de l’équilibreur de charge de travail.

1. (Le cas échéant) Si vous accédez à l’équilibreur de charge de travail à partir de la zone Ressources ou pour une équipe, développez le menu déroulant **Projet : nom** et utilisez les modificateurs de filtre pour sélectionner le ou les projets pour lesquels vous souhaitez effectuer des affectations. Vous pouvez sélectionner les projets par nom (option par défaut) ou par statut.

   Pour plus d’informations sur les modificateurs de filtre Workfront, voir [Modificateurs de filtre et de condition](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Le nom du projet est sélectionné par défaut lorsque vous accédez à l’équilibreur de charge de travail pour un projet.

   ![Nom du projet dans les affectations en bloc](assets/project-name-status-dropdown-bulk-assignments-wb-nwe-350x133.png)

1. (Facultatif) Cliquez sur **Sélectionner les tâches de projet** pour sélectionner la ou les tâches pour lesquelles vous souhaitez effectuer des affectations, puis dans le menu déroulant **Tâche : nom**, sélectionnez les tâches par nom (option par défaut) ou par statut et utilisez les modificateurs de filtre pour rechercher des tâches spécifiques.

   Pour plus d’informations sur les modificateurs de filtre Workfront, voir [Modificateurs de filtre et de condition](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Vous ne pouvez pas sélectionner de tâches dont le statut est Terminé.

   ![Statut de la tâche dans les affectations en bloc](assets/task-name-status-dropdown-bulk-assignments-wb-nwe-350x102.png)

   >[!TIP]
   >
   >Laissez cette sélection vide si vous souhaitez effectuer des affectations groupées pour les problèmes ainsi que pour les tâches.

1. (Facultatif) Cliquez sur l’icône **Supprimer** ![Supprimer](assets/delete.png) en regard de l’un des critères sélectionnés

   Ou

   Cliquez sur **Effacer tout** dans le coin supérieur droit du panneau Affectations groupées pour supprimer toutes les sélections.

1. Sélectionnez l’une des options suivantes et procédez comme suit :

   * [Affecter un utilisateur ou une utilisatrice](#assign-user)
   * [Remplacer un utilisateur ou une utilisatrice](#replace-user)
   * [Annuler l’affectation de l’utilisateur](#unassign-user)

   >[!TIP]
   >
   >Si aucun élément ne correspond aux filtres sélectionnés, ces options sont grisées.

### Affecter un utilisateur {#assign-user}

Lorsque vous affectez un utilisateur ou une utilisatrice à l’aide d’affectations groupées dans l’équilibreur de charge de travail, les événements suivants se produisent :

* Tous les éléments de travail actuellement affectés à un rôle spécifié dans les projets sélectionnés sont affectés à un utilisateur ou une utilisatrice.
* Les types d’éléments de travail suivants ne sont pas affectés à l’utilisateur ou à l’utilisatrice :

   * Éléments déjà affectés à un utilisateur ou une utilisatrice.
   * Éléments terminés.

* Si la personne que vous avez sélectionnée n’est pas associée au rôle spécifié, le rôle est remplacé par la personne dans son rôle principal.

Pour affecter un utilisateur ou une utilisatrice aux éléments de travail précédemment affectés à des fonctions, procédez comme suit :

1. Commencez à affecter des éléments de travail à l’aide des affectations groupées dans l’équilibreur de charge de travail tel que décrit ci-dessus, puis sélectionnez **Affecter**.

1. Dans le champ **Affectation des rôles**, cliquez sur la flèche déroulante pour effectuer un choix dans une liste de rôles. Seuls les rôles affectés actuellement dans les projets spécifiés s’affichent. Champ obligatoire.

   ![Affectation de rôle](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. Dans le champ **Utilisateur ou utilisatrice à affecter**, cliquez sur la flèche déroulante pour choisir parmi les personnes suggérées ou pour saisir le nom d’un autre utilisateur ou d’une autre utilisatrice.

   Sélectionnez des utilisateurs et utilisatrices dans les zones suivantes :

   * **Affectations suggérées** : utilisateurs et utilisatrices pouvant remplir le rôle sélectionné et correspondant aux critères des affectations intelligentes. Pour plus d’informations, voir [Vue d’ensemble des affectations intelligentes](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **Autres affectations** : tous les utilisateurs et toutes les utilisatrices du système pouvant remplir le rôle sélectionné.

     >[!TIP]
     >
     >Seules les 50 premières personnes sont répertoriées dans la zone Autres affectations.


   Après avoir sélectionné un utilisateur ou une utilisatrice, Workfront affiche une note indiquant le nombre d’éléments auxquels la personne que vous avez spécifiée sera affectée et la fonction qu’elle remplacera.

   >[!TIP]
   >
   >Tous les rôles de l’utilisateur ou de l’utilisatrice s’affichent dans la liste, sous son nom.


1. Cliquez sur **Affecter**.

   Les rôles spécifiés sont remplacés par les utilisateurs que vous avez sélectionnés.

   Vous recevez une confirmation indiquant le nombre d’éléments de travail pour lesquels le rôle sélectionné a été remplacé par la personne sélectionnée.

   ![Confirmation d’affectation en bloc](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

### Remplacer l’utilisateur {#replace-user}

Vous pouvez remplacer une personne déjà affectée à des éléments de travail par un autre utilisateur ou une autre utilisatrice dans les projets sélectionnés.

Lorsque vous remplacez une personne par une autre en utilisant les affectations groupées dans l’équilibreur de charge de travail, les événements suivants se produisent :

* La personne de remplacement est affectée à tous les éléments de travail actuellement affectés à un utilisateur ou une utilisatrice d’origine dans les projets sélectionnés.

* Aucun élément de travail déjà marqué comme terminé n’est affecté au nouvel utilisateur ou à la nouvelle utilisatrice.
* Si le rôle associé au premier utilisateur ou à la première utilisatrice ne correspond à aucun des rôles de la deuxième personne, la troisième personne est affectée à son rôle principal.

Pour remplacer un utilisateur ou une utilisatrice par une autre personne, procédez comme suit :

1. Commencez à affecter des éléments de travail dans l’équilibreur de charge de travail tel que décrit ci-dessus et sélectionnez **Remplacer**.
1. Dans le champ **Personne affectée actuellement**, cliquez sur la flèche déroulante pour effectuer un choix dans la liste des utilisateurs et utilisatrices. Seules les personnes affectées actuellement à des éléments de travail incomplets dans les projets spécifiés s’affichent. Champ obligatoire.

   ![Remplacer un utilisateur ou une utilisatrice](assets/bulk-assignments-workload-balancer-replace-selected-350x345.png)

1. Dans le champ **Personne à affecter**, cliquez sur la flèche déroulante pour choisir parmi la liste des personnes suggérées ou pour saisir un autre nom d’utilisateur ou d’utilisatrice. Les utilisateurs répertoriés dans la liste correspondent par défaut aux critères des affectations intelligentes. Pour en savoir plus, consultez la section [Vue d’ensemble des affectations intelligentes](../../manage-work/tasks/assign-tasks/smart-assignments.md).

   Workfront affiche une note relative au nombre d’éléments pour lesquels la personne affectée remplacera la deuxième personne et les rôles qu’elle remplacera.

   ![Confirmation d’utilisation du remplacement en bloc](assets/bulk-replace-user-confirmation-before-replacing-nwe-350x49.png)

1. Cliquez sur **Remplacer**.

   La première personne sélectionnée est remplacée par la deuxième personne dans tous les éléments de travail du projet sélectionné.

   Vous recevez une confirmation par rapport au nombre d’éléments de travail pour lesquelles l’affectation d’origine de l’utilisateur ou de l’utilisatrice a été remplacée par la deuxième personne sélectionnée.

### Annuler l’affectation de l’utilisateur {#unassign-user}

Vous pouvez annuler l’affectation d’une personne à toutes les tâches dont elle a reçu l’affectation dans les projets sélectionnés.

Lorsque vous annulez l’affectation d’un utilisateur ou d’une utilisatrice de toutes ses affectations à l’aide des affectations groupées dans l’équilibreur de charge de travail, les événements suivants se produisent :

* L’utilisateur spécifié est supprimé de toutes les tâches qui lui sont affectées.
* Si la personne non affectée est associée à des fonctions, les fonctions demeurent affectées aux éléments de travail lors de la suppression de la personne.

* Si la personne spécifiée est affectée aux éléments de travail terminés, la personne demeure affectée à ces éléments de travail.

Pour plus d’informations sur les affectations d’utilisateurs et d’utilisatrices et de fonctions, voir [Vue d’ensemble de l’affectation de travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Pour annuler l’affectation d’un utilisateur ou d’une utilisatrice à des éléments de travail dans les projets sélectionnés ou pour les tâches ou problèmes sélectionnés auxquels la personne est affectée, procédez comme suit :

1. Commencez à attribuer des éléments de travail dans l’équilibreur de charge de travail comme décrit ci-dessus et sélectionnez **Annuler l’affectation**.

1. Dans le champ **Personne à affecter**, cliquez sur la flèche déroulante et choisissez dans la liste d’utilisateurs et d’utilisatrices. Seuls les utilisateurs et utilisatrices affectés actuellement à des tâches incomplètes dans les projets spécifiés s’affichent. Champ obligatoire.

   ![Annuler l’affectation d’un utilisateur](assets/bulk-assignments-workload-balancer-unassign-selected-350x318.png)

   Workfront affiche une note par rapport au nombre d’éléments dont la personne affectée actuellement se verra annuler l’affectation.

   ![Confirmation d’annulation de l’affectation en bloc](assets/bulk-unassign-user-confirmation-before-assigning-nwe-350x45.png)

1. Cliquez sur **Annuler l’affectation**.\
   Vous recevez une confirmation par rapport au nombre d’éléments de travail dont la personne spécifiée a été supprimée.


