---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Création d’une itération dans un flux de travail
description: Une itération est la durée affectée à la réalisation d’un travail. Certaines équipes Agile peuvent faire référence à une itération en tant que sprint.
author: Jenny
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 92%

---

# Créer une itération dans un flux de travail

>[!IMPORTANT]
>
>Les flux de travail ne sont disponibles que pour un groupe spécifique de clientes et de clients.

Une itération est la durée affectée à la réalisation d’un travail. Certaines équipes Agile peuvent faire référence à une itération en tant que sprint.

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
   <td> 
   <p>Contributeur ou version ultérieure</p> 
   <p>Requête ou supérieure</p>
   </td> 
  </tr>  
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une itération dans un flux de travail

{{step1-to-boards}}

1. Ouvrez le flux de travail dans lequel vous souhaitez ajouter l’itération. Pour ouvrir un flux de travail, cliquez sur [!UICONTROL **Afficher le flux de travail**].
1. Créez une itération à l’aide de l’une des méthodes suivantes :

   * Dans l’onglet Liste des cartes, dans la vue de l’itération, cliquez sur [!UICONTROL **Créer une itération**].
   * Dans l’onglet Liste des cartes, en mode Liste, cliquez sur [!UICONTROL **Créer une itération**].
   * Dans l’onglet Panoramas, cliquez sur [!UICONTROL **Ajouter un panorama**] et sélectionnez [!UICONTROL **Processus d’itération**] comme modèle de panorama. Ouvrez ensuite le panneau d’itération, puis cliquez sur [!UICONTROL **Configurer des itérations**].

1. Dans la boîte de dialogue Détails de l’itération, ajoutez les informations suivantes :

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Iteration name]</strong></td> 
      <td>Nom de l’itération, par exemple « Sprint 1 ».</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Iteration length]</strong></td> 
      <td>Durée de l’itération, en jours, semaines ou mois.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Start date]</strong></td> 
      <td>Date de début de l’itération. La date de fin est automatiquement renseignée en fonction de la durée d’itération.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur [!UICONTROL **Enregistrer**].

   L’itération apparaît désormais dans la vue de l’itération de la liste des cartes et dans la zone Mesures du panorama d’itération.

   Pour ajouter des cartes à une itération, consultez la section [Utiliser la liste des cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## Modifier une itération existante

1. Pour ouvrir un flux de travail, cliquez sur [!UICONTROL **Afficher le flux de travail**].
1. Ouvrez l’itération à l’aide de l’une des méthodes suivantes :

   * Dans l’onglet Liste des cartes, dans la vue de l’itération, cliquez sur l’icône [!UICONTROL **Détails de l’itération**] ![Détails de l’itération](assets/iteration-details-button.png).
   * Dans la panorama d’itération, cliquez sur l’icône [!UICONTROL **Détails de l’itération**] ![Détails de l’itération](assets/iteration-details-button.png) dans la zone Mesures en haut à droite.

1. Dans le panneau [!UICONTROL Configuration de l’itération], modifiez l’itération selon vos besoins.
1. Pour modifier le nom de l’itération, développez le menu [!UICONTROL **Détails de l’itération**].

   Une fois qu’une itération a commencé, vous pouvez encore modifier le nom de l’itération, mais plus les dates ou la durée.

<!--   

1. <span class="preview">To add goals to the iteration, expand [!UICONTROL **Goals**].</span>
1. <span class="preview">Click [!UICONTROL **Add goal**], and type the goal name.</span>

   <span class="preview">As goals are completed during the iteration, you can select the check box to mark them complete, or click the **Delete** icon ![Delete icon](assets/delete.png) to delete a goal. The metrics area on the top right of the iteration shows how many goals exist and how many have been completed.</span>

<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## Supprimer une itération

1. Cliquez sur l’onglet [!UICONTROL **Liste des cartes**] dans le flux de travail et ouvrez la vue de l’itération.
1. Cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/delete.png) en regard de l’itération.
1. Cliquez sur [!UICONTROL **Supprimer l’itération**] dans le message de confirmation qui s’affiche.
