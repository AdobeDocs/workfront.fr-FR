---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Création et modification des équipes d’un groupe
description: Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et travailler avec les équipes associées au groupe et à l’un de ses sous-groupes.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 6f9eddd46430990e11d5d661ea09f0595a9acebc
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 3%

---

# Création et modification des équipes d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et travailler avec les équipes associées au groupe et à l’un de ses sous-groupes.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

Pour plus d’informations sur la façon dont les utilisateurs disposant d’une licence Plan peuvent créer une équipe, voir [Création d’une équipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Pour plus d’informations sur la création d’une équipe par un administrateur Workfront, voir [Création d’une équipe à partir de la zone Configuration](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur de groupe du groupe ou un administrateur Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Administrateurs de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Affichage, utilisation et création d’équipes pour votre groupe à partir de la zone Groupes

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Cliquez sur le nom du groupe pour lequel vous souhaitez créer ou modifier des équipes.
1. Dans le panneau de gauche, cliquez sur **Équipes** ![](assets/teams.png) pour répertorier les équipes associées au groupe et aux sous-groupes qu’il peut avoir.

1. Effectuez l’une des opérations suivantes :

   * **Ajout d’une équipe**: cliquez sur **Nouvelle équipe**, puis utilisez les options suivantes pour la configurer :

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
       <td> <p> Le système renseigne le champ Groupe pour la nouvelle équipe avec le groupe que vous affichez. Si vous souhaitez associer l’équipe à un autre groupe, commencez à saisir son nom, puis sélectionnez-le lorsqu’il s’affiche.</p> <p>Vous pouvez vous assurer que vous associez le groupe approprié à l’équipe en pointant dessus et en cliquant sur l’icône d’information. <img src="assets/info-icon.png"> qui s’affiche en regard de celle-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus de celui-ci et ses administrateurs.</p> <p><b>REMARQUE</b>: lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, les administrateurs de groupe de ce groupe ou de ce sous-groupe peuvent gérer l’équipe sans en être membre. Les administrateurs de groupe peuvent accéder à la zone Équipes dans le menu principal et cliquer sur la flèche Changer d’équipe . <img src="assets/switch-team-icon.png" alt="Icône Changer l’équipe"> pour répertorier toutes les équipes affectées aux groupes qu’elles gèrent.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Membres d'équipe</td> 
       <td> <p>Commencez à saisir le nom d’un utilisateur qui doit faire partie de l’équipe, puis sélectionnez le nom lorsqu’il apparaît dans la liste déroulante. Répétez cette procédure pour ajouter plusieurs utilisateurs à l’équipe.</p> <p>Le nombre d’utilisateurs que vous pouvez ajouter à une équipe n’est pas limité. Cependant, nous vous recommandons de ne pas avoir un trop grand nombre d’utilisateurs dans une seule équipe, car la gestion du travail de l’équipe peut devenir trop complexe.</p> </td> 
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
       <td>Définissez le bouton Travailler dessus sur un bouton Démarrer . Lorsqu’un utilisateur clique sur Démarrer, l’état de l’élément est automatiquement mis à jour.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Bouton Terminé</td> 
       <td>Sélectionnez l’état que vous souhaitez définir pour les éléments lorsque vous cliquez sur le bouton Terminé .</td> 
       </tr> 
      </tbody> 
     </table>

   * **Modifier les équipes**: sélectionnez au moins une équipe, puis cliquez sur **la valeur** Icône Modifier ![](assets/edit-icon.png), puis utilisez les options suivantes pour la configurer :

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
       <td> <p>Associez l’équipe à un groupe. Commencez à saisir le nom du groupe, puis sélectionnez-le lorsqu’il s’affiche.</p> <p>Vous pouvez vous assurer que vous associez le groupe approprié à l’équipe en pointant dessus et en cliquant sur l’icône d’information. <img src="assets/info-icon.png"> qui s’affiche en regard de celle-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus de celui-ci et ses administrateurs.</p> <p><b>REMARQUE</b>: lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, les administrateurs de groupe de ce groupe ou de ce sous-groupe peuvent gérer l’équipe sans en être membre. Les administrateurs de groupe peuvent accéder à la zone Équipes dans le menu principal et cliquer sur la flèche Changer d’équipe . <img src="assets/switch-team-icon.png" alt="Icône Changer l’équipe"> pour répertorier toutes les équipes affectées aux groupes qu’elles gèrent.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Propriétaire</td> 
       <td>Sélectionnez un propriétaire pour l’équipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Membres d'équipe</td> 
       <td> <p>Ajoutez des membres de l’équipe et . Commencez à saisir le nom d’un utilisateur, puis sélectionnez-le lorsqu’il s’affiche. Répétez cette procédure pour ajouter plusieurs utilisateurs à l’équipe.</p> <p><b>CONSEIL</b>: le nombre d’utilisateurs que vous pouvez ajouter à une équipe n’est pas limité. Cependant, nous vous recommandons de ne pas avoir un trop grand nombre d’utilisateurs dans une seule équipe, car la gestion du travail de l’équipe peut devenir trop complexe.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Description</td> 
       <td>Saisissez une description pour l’équipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Modèles de mise en page</td> 
       <td> <p>Commencez à saisir le nom du modèle de mise en page que vous souhaitez que l’équipe utilise, puis cliquez dessus lorsqu’il apparaît.</p> <p>Lorsque vous désignerez l’équipe avec ce modèle de mise en page comme l’équipe d’accueil des utilisateurs, tous les utilisateurs de cette équipe verront les personnalisations dans ce modèle de mise en page.<br>Leurs paramètres de modèle de mise en page individuels remplacent ceux du modèle de mise en page de l’équipe d’accueil. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Indiquez s’il s’agit d’une équipe agile. Pour plus d’informations sur les équipes agiles et la gestion de leur travail, voir <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Créer une équipe agile</a>.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Travailler sur ce projet</td> 
       <td> <p>Définissez le bouton Travailler dessus sur un bouton Démarrer . Lorsqu’un utilisateur clique sur Démarrer, l’état de l’élément est automatiquement mis à jour.</p> <p>Pour plus d’informations sur la configuration du bouton Démarrer , voir <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Remplacez le bouton Travailler dessus par un bouton Démarrer</a>.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Bouton Terminé</td> 
       <td> <p>Personnalisez le bouton Terminé . Pour plus d’informations, voir :</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Configuration du bouton Terminé pour les tâches</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Configuration du bouton Terminé pour les problèmes</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **Suppression d’équipes**: sélectionnez au moins une équipe, puis cliquez sur l’icône Supprimer ![](assets/delete.png).
   * **Exporter la liste des équipes**: cliquez sur **Exporter** ![](assets/export.png), puis sélectionnez le format de fichier souhaité pour la liste exportée.
