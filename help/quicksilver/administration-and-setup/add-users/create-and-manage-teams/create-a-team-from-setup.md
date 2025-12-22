---
title: Création d’une équipe à partir de la zone Configuration
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer une équipe à partir de la zone Configuration.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 90%

---

# Créer une équipe à partir de la zone Configuration

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer une équipe à partir de la zone Configuration.
Pour plus d’informations sur les équipes, voir [Vue d’ensemble des équipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Une personne chargée de l’administration de groupes peut créer une équipe pour un groupe qu’elle administre à partir de la zone Configuration. Pour plus d’informations, voir [Créer et modifier les équipes d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un utilisateur disposant d’une licence Standard ou Plan peut également créer une équipe à partir de la zone Équipes . Pour plus d’informations, consultez [Créer une équipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

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

## Créer une équipe

{{step-1-to-setup}}

1. Cliquez sur **Équipes**, puis sur **Nouvelle équipe**.

1. Dans la zone **Nouvelle équipe** qui s’affiche, indiquez les informations suivantes :

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
      <td> <p>Si vous souhaitez associer l’équipe à un groupe, commencez à saisir son nom, puis sélectionnez-le lorsqu’il s’affiche.</p> <p>Pour vous assurer que vous associez le bon groupe à la bonne équipe, pointez dessus et cliquez sur l’icône d’information <img src="assets/info-icon.png"> qui s’affiche en regard de celle-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus et son équipe d’administration.</p> <p><b>REMARQUE</b> : lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, les administrateurs et administratrices de groupe de ce groupe ou de ce sous-groupe peuvent gérer l’équipe sans en être membre. Les administrateurs et administratrices de groupes peuvent accéder à la zone Équipes dans le menu principal et cliquer sur la flèche Changer d’équipe <img src="assets/switch-team-icon.png" alt="Icône Changer l’équipe"> pour répertorier toutes les équipes affectées aux groupes qu’ils ou elles gèrent.</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">Voici une liste d'attente</td> 
      <td>Sélectionnez cet élément si vous souhaitez configurer cette nouvelle équipe pour qu'elle soit une équipe Agile. Pour plus d’informations sur les équipes Agile, voir <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Créer une équipe Agile</a>.</td> 
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

1. Cliquez sur **Créer une équipe**.

## Personnes propriétaires d’équipe

Lorsque vous créez une équipe, vous en devenez la personne propriétaire par défaut.

Vous pouvez afficher les personnes propriétaires d’équipes pour toutes les équipes lors de la création des rapports d’équipes et y inclure le nom de la personne propriétaire. (Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
