---
title: Modification des paramètres d’une équipe à partir de la zone Configuration
description: En tant qu’administrateur Adobe Workfront, vous pouvez modifier les paramètres d’une équipe dans la zone Configuration . Vous pouvez ajouter des utilisateurs à une équipe, définir le modèle de mise en page d’une équipe et définir comment l’état est enregistré lorsque les tâches sont terminées par une équipe.
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 3%

---

# Modification des paramètres d’une équipe à partir de la zone Configuration

En tant qu’administrateur Adobe Workfront, vous pouvez modifier les paramètres d’une équipe dans la zone Configuration . Vous pouvez ajouter des utilisateurs à une équipe, définir le modèle de mise en page d’une équipe et définir comment l’état est enregistré lorsque les tâches sont terminées par une équipe.

Pour plus d’informations sur les équipes, voir [Présentation des équipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Un administrateur de groupe peut modifier les paramètres d’une équipe pour un groupe qu’il administre. Pour plus d’informations, voir [Création et modification des équipes d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un utilisateur disposant d’une licence Plan peut modifier les paramètres d’une équipe dans la zone Personnes. Pour plus d’informations, voir [Modification des paramètres de l’équipe](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
>


## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modification des paramètres d’une équipe

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Équipes** dans le panneau de gauche.
1. Sélectionnez une équipe, puis cliquez sur **Modifier** ![](assets/edit-icon.png).

1. Apportez l’une des modifications suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom de l'équipe</td> 
      <td>Saisissez le nom de l’équipe.</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Est actif </td> 
       <td>Cette option est activée par défaut pour les nouvelles équipes et les équipes existantes. Désactivez-la pour désactiver l’équipe. Pour plus d’informations, voir <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">Désactivation d’une équipe</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Groupe</td> 
      <td> <p>Associez l’équipe à un groupe. Commencez à saisir le nom du groupe, puis sélectionnez-le lorsqu’il s’affiche.</p> <p><b>REMARQUE</b>: Lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, les administrateurs de groupe de ce groupe ou de ce sous-groupe peuvent gérer l’équipe sans en être membre. Les administrateurs de groupe peuvent accéder à la zone Équipes dans le menu principal et cliquer sur la flèche Changer d’équipe . <img src="assets/switch-team-icon.png" alt="Icône Changer l’équipe"> pour répertorier toutes les équipes affectées aux groupes qu’elles gèrent.</p> <p>Vous pouvez vous assurer que vous associez le groupe approprié à l’équipe en pointant dessus et en cliquant sur l’icône d’information. <img src="assets/info-icon.png"> qui s’affiche en regard de celle-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus de celui-ci et ses administrateurs.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propriétaire</td> 
      <td>Sélectionnez un propriétaire pour l’équipe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membres d'équipe</td> 
      <td> <p>Ajoutez des membres de l’équipe et . Commencez à saisir le nom d’un utilisateur, puis sélectionnez-le lorsqu’il s’affiche. Répétez cette procédure pour ajouter plusieurs utilisateurs à l’équipe.</p> 
      <p><b>CONSEIL</b>: Vous pouvez ajouter n’importe quel nombre d’utilisateurs à une équipe. Cependant, nous vous recommandons de ne pas ajouter un nombre trop important dans une seule équipe, car la gestion du travail de l'équipe risque de devenir trop complexe.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Saisissez une description pour l’équipe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modèles de mise en page</td> 
      <td> <p>Commencez à saisir le nom du modèle de mise en page que vous souhaitez que l’équipe utilise, puis cliquez dessus lorsqu’il apparaît.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agile</td> 
      <td>Indiquez s’il s’agit d’une équipe agile. Pour plus d’informations sur les équipes agiles et la gestion de leur travail, voir <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Création d’une équipe agile</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
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

1. Cliquez sur **Enregistrer les modifications**.
