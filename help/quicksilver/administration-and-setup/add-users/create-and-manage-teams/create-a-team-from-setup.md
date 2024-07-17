---
title: Création d’une équipe à partir de la zone Configuration
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: En tant qu’administrateur Adobe Workfront, vous pouvez créer une équipe à partir de la zone Configuration .
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 23%

---

# Création d’une équipe à partir de la zone Configuration

En tant qu’administrateur Adobe Workfront, vous pouvez créer une équipe à partir de la zone Configuration . Pour plus d’informations sur les équipes, voir [Présentation des équipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Un administrateur de groupe peut créer une équipe pour un groupe qu’il administre à partir de la zone Configuration . Pour plus d’informations, voir [Création et modification des équipes d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Un utilisateur disposant d’une licence Plan peut également créer une équipe à partir de la zone Personnes. Pour plus d’informations, voir [Création d’une équipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
>

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Créer une équipe

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Equipes**, puis sur **Nouvelle équipe**.

1. Dans la zone **New Team** qui s’affiche, spécifiez les informations suivantes :

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
      <td> <p>Si vous souhaitez associer l’équipe à un groupe, commencez à saisir son nom, puis sélectionnez-le lorsqu’il s’affiche.</p> <p>Vous pouvez vous assurer que vous associez le groupe de droite à l’équipe en pointant dessus et en cliquant sur l’icône d’information <img src="assets/info-icon.png"> qui s’affiche à côté. Cette option permet d’afficher une infobulle contenant des informations sur le groupe, telles que la hiérarchie des groupes qui le précèdent et ses administrateurs et administratrices.</p> <p><b>REMARQUE</b> : lorsqu’une équipe est affectée à un groupe ou à un sous-groupe, les administrateurs de groupe de ce groupe ou de ce sous-groupe peuvent gérer l’équipe sans en être membre. Les administrateurs de groupe peuvent accéder à la zone Équipes dans le menu principal et cliquer sur la flèche Changer d’équipe <img src="assets/switch-team-icon.png" alt="Icône Changer l’équipe"> pour répertorier toutes les équipes affectées aux groupes qu’ils gèrent.</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">Voici une liste d'attente</td> 
      <td>Sélectionnez cet élément si vous souhaitez configurer cette nouvelle équipe pour qu’elle soit agile. Pour plus d’informations sur les équipes agiles, voir <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Création d’une équipe agile</a>.</td> 
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

1. Cliquez sur **Créer une équipe**.

## Propriétaires d’équipe

Lorsque vous créez une équipe, vous devenez le propriétaire de l’équipe, par défaut.

Vous pouvez afficher les propriétaires de toutes les équipes lorsque vous créez un rapport pour les équipes et inclure le champ Nom du propriétaire dans votre rapport. (Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
