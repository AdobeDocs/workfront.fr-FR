---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Création et modification des équipes d’un groupe
description: Quand vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez voir et modifier les équipes liées au groupe et ses sous-groupes.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 87%

---

# Créer et modifier les équipes d’un groupe

Quand vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez voir et modifier les équipes liées au groupe et ses sous-groupes.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs et administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

Pour plus d’informations sur la façon dont les utilisateurs et utilisatrices disposant d’une licence Plan peuvent créer une équipe, consultez la section [Créer une équipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Pour plus d’informations sur la création d’une équipe par un administrateur ou une administratrice Workfront, consultez la section [Créer une équipe à partir de la zone de configuration](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher, utiliser et créer des équipes pour votre groupe à partir de la zone Groupes

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

1. Cliquez sur le nom du groupe pour lequel vous souhaitez créer ou modifier des équipes.
1. Dans le panneau de gauche, cliquez sur **Équipes** ![Équipes](assets/teams.png) pour répertorier les équipes associées au groupe et aux sous-groupes qu’il peut avoir.

1. Effectuez l’une des opérations suivantes :

   * **Ajouter une équipe** : cliquez sur **Nouvelle équipe**, puis utilisez les options suivantes pour la configurer :

   <!-- WRITER please check table below. I stripped out wonky conditions-->

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Nom de l'équipe</td> 
       <td>Saisissez le nom de l’équipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Groupe</td> 
       <td> <p> Le système renseigne le champ du groupe pour la nouvelle équipe avec le groupe que vous affichez. Si vous souhaitez associer l’équipe à un autre groupe, commencez à saisir son nom, puis sélectionnez-le lorsqu’il s’affiche.</p> <p>Assurez-vous d’associer le bon groupe à l’équipe en pointant dessus et en cliquant sur l’icône d’information <img src="assets/info-icon.png"> qui apparaît à côté. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus et son équipe d’administration.</p> <p><b>REMARQUE</b> : lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, les administrateurs et administratrices de groupe de ce groupe ou de ce sous-groupe peuvent gérer l’équipe sans en être membre. Les administrateurs et administratrices de groupes peuvent accéder à la zone Équipes dans le menu principal et cliquer sur la flèche Changer d’équipe <img src="assets/switch-team-icon.png" alt="Icône Changer l’équipe"> pour répertorier toutes les équipes affectées aux groupes qu’ils ou elles gèrent.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Membres d'équipe</td> 
       <td> <p>Commencez à saisir le nom d’un utilisateur ou d’une utilisatrice qui doit faire partie de l’équipe, puis sélectionnez le nom lorsqu’il apparaît dans la liste déroulante. Répétez cette procédure pour ajouter plusieurs personnes à l’équipe.</p> <p>Le nombre d’utilisateurs et d’utilisatrices que vous pouvez ajouter à une équipe n’est pas limité. Cependant, nous vous recommandons de ne pas ajouter un trop grand nombre de personnes à une seule équipe, au risque de rendre votre gestion de travail trop complexe pour ces équipes.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Description</td> 
       <td>Saisissez une description pour l’équipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Calendrier</td> 
       <td>Choisissez l'onglet de calendrier qui apparaîtra pour cette équipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Travailler sur ce projet</td> 
       <td>Remplacez le bouton Travailler sur ce projet par un bouton Démarrer. Lorsqu’une personne clique sur Démarrer, le statut de l’élément est automatiquement mis à jour.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Bouton Terminé</td> 
       <td>Sélectionnez le statut que vous voulez affecter aux éléments lorsque vous cliquez sur le bouton « Terminé ».</td> 
       </tr> 
      </tbody> 
     </table>

   * **Modifier les équipes** : sélectionnez au moins une équipe, cliquez sur **l&#39;icône** Modifier ![icône Modifier](assets/edit-icon.png), puis utilisez les options suivantes pour la configurer :

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Nom de l'équipe</td> 
       <td>Saisissez le nom de l’équipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Groupe</td> 
       <td> <p>Associez l’équipe à un groupe. Commencez à saisir le nom du groupe, puis sélectionnez-le lorsqu’il s’affiche.</p> <p>Pour vous assurer que vous associez le bon groupe à la bonne équipe, pointez dessus et cliquez sur l’icône d’information <img src="assets/info-icon.png"> qui s’affiche en regard de celle-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus et son équipe d’administration.</p> <p><b>REMARQUE</b> : lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, les administrateurs et administratrices de groupe de ce groupe ou de ce sous-groupe peuvent gérer l’équipe sans en être membre. Les administrateurs et administratrices de groupes peuvent accéder à la zone Équipes dans le menu principal et cliquer sur la flèche Changer d’équipe <img src="assets/switch-team-icon.png" alt="Icône Changer l’équipe"> pour répertorier toutes les équipes affectées aux groupes gérés.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Propriétaire</td> 
       <td>Sélectionnez une personne propriétaire pour l’équipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Membres d'équipe</td> 
       <td> <p>Ajoutez les personnes membres de l’équipe. Commencez à saisir le nom d’une personne, puis sélectionnez-le lorsqu’il s’affiche. Répétez cette procédure pour ajouter plusieurs personnes à l’équipe.</p> <p><b>CONSEIL</b> : le nombre de personnes que vous pouvez ajouter à une équipe n’est pas limité. Cependant, nous vous recommandons de ne pas ajouter un trop grand nombre de personnes à une seule équipe, au risque de rendre votre gestion de travail trop complexe pour ces équipes.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Description</td> 
       <td>Saisissez une description pour l’équipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Modèle de mise en page</td> 
       <td> <p>Commencez à saisir le nom du modèle de mise en page que l’équipe doit utiliser, puis cliquez dessus lorsqu’il apparaît.</p> <p>Lorsque vous désignerez l’équipe avec ce modèle de mise en page comme équipe interne, toutes les personnes de cette équipe verront les personnalisations dans ce modèle de disposition.<br>Leurs paramètres de modèle de mise en page individuels remplacent ceux du modèle de mise en page de l’équipe interne. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Indiquez s'il s'agit d'une équipe Agile. Pour plus d’informations sur les équipes Agile et la gestion de leur travail, voir <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Création d’une équipe Agile</a>.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Travailler sur ce projet</td> 
       <td> <p>Remplacez le bouton Travailler sur ce projet par un bouton Démarrer. Lorsqu’une personne clique sur Démarrer, le statut de l’élément est automatiquement mis à jour.</p> <p>Pour plus d’informations sur la configuration du bouton Démarrer, voir <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Remplacer le bouton Travailler dessus par un bouton Démarrer</a>.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Bouton Terminé</td> 
       <td> <p>Personnalisez le bouton Terminé. Pour plus d’informations, voir :</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Configurer le bouton Terminé pour les tâches</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Configurer le bouton Terminé pour les problèmes</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **Supprimer des équipes** : sélectionnez au moins une équipe, puis cliquez sur l’icône Supprimer ![icône Supprimer](assets/delete.png).
   * **Exporter la liste des équipes** : cliquez sur **Exporter** ![Icône Exporter](assets/export.png), puis sélectionnez le format de fichier souhaité pour la liste exportée.
