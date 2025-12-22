---
title: Modifier les paramètres d'une équipe à partir de la zone Configuration
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez modifier les paramètres d’une équipe dans la zone Configuration. Vous pouvez ajouter des personnes à une équipe, définir le modèle de mise en page d’une équipe et définir comment le statut est enregistré lorsqu’une équipe termine des éléments de travail.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 90%

---

# Modifier les paramètres d’une équipe à partir de la zone Configuration

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez modifier les paramètres d’une équipe dans la zone Configuration. Vous pouvez ajouter des personnes à une équipe, définir le modèle de mise en page d’une équipe et définir comment le statut est enregistré lorsqu’une équipe termine des éléments de travail.

Pour plus d’informations sur les équipes, voir [Vue d’ensemble des équipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Un administrateur ou une administratrice de groupes peut modifier les paramètres d’une équipe pour un groupe qu’il ou elle administre. Pour plus d’informations, voir [Créer et modifier les équipes d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un utilisateur disposant d’une licence Standard ou Plan peut modifier les paramètres d’une équipe à partir de la zone Équipes . Pour plus d’informations, voir [Modifier les paramètres d’une équipe](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier les paramètres d’une équipe

{{step-1-to-setup}}

1. Cliquez sur **Équipes** dans le panneau de gauche.
1. Sélectionnez une équipe, puis cliquez sur **Modifier** ![icône Modifier](assets/edit-icon.png).

1. Effectuez l’une des modifications suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom de l'équipe</td> 
      <td>Saisissez le nom de l’équipe.</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Est active </td> 
       <td>Cette option est activée par défaut pour les nouvelles équipes et les équipes existantes. Désactivez-la pour désactiver l’équipe. Pour plus d’informations, voir <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">Désactiver une équipe</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Groupe</td> 
      <td> <p>Associez l’équipe à un groupe. Commencez à saisir le nom du groupe, puis sélectionnez-le lorsqu’il s’affiche.</p> <p><b>REMARQUE</b> : lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, les administrateurs et administratrices de groupe de ce groupe ou de ce sous-groupe peuvent gérer l’équipe sans en être membre. Les administrateurs et administratrices de groupes peuvent accéder à la zone Équipes dans le menu principal et cliquer sur la flèche Changer d’équipe <img src="assets/switch-team-icon.png" alt="Icône Changer l’équipe"> pour répertorier toutes les équipes affectées aux groupes qu’ils ou elles gèrent.</p> <p>Vous pouvez vous assurer que vous associez le groupe approprié à l’équipe en pointant dessus et en cliquant sur l’icône d’information <img src="assets/info-icon.png"> qui s’affiche en regard de celle-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus et son équipe d’administration.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propriétaire</td> 
      <td>Sélectionnez une personne propriétaire pour l’équipe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membres d'équipe</td> 
      <td> <p>Ajoutez les personnes membres de l’équipe. Commencez à saisir le nom d’une personne, puis sélectionnez-le lorsqu’il s’affiche. Répétez cette procédure pour ajouter plusieurs personnes à l’équipe.</p> 
      <p><b>CONSEIL</b> : vous pouvez ajouter un nombre indéfini de personnes à une équipe. Cependant, nous vous recommandons de ne pas ajouter un nombre trop important dans une seule équipe, car la gestion du travail de l’équipe risque de devenir trop complexe.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Saisissez une description pour l’équipe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modèle de mise en page</td> 
      <td> <p>Commencez à saisir le nom du modèle de mise en page que l’équipe doit utiliser, puis cliquez dessus lorsqu’il apparaît.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agile</td> 
      <td>Indiquez s'il s'agit d'une équipe Agile. Pour plus d’informations sur les équipes Agile et la gestion de leur travail, voir <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Création d’une équipe Agile</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
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

1. Cliquez sur **Enregistrer les modifications**.
