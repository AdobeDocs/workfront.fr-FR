---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Création d’une itération dans un workflow
description: Une itération est un temps défini réservé à la réalisation du travail. Certaines équipes agiles peuvent appeler une itération sprint.
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: 563e0f443ecef9ee99e9f9bfb5a0d579aa50cef4
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Création d’une itération dans un workflow

{{highlighted-preview}}

Une itération est un temps défini réservé à la réalisation du travail. Certaines équipes agiles peuvent appeler une itération sprint.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

## Création d’une itération dans un workflow

{{step1-to-boards}}

1. Ouvrez le workflow dans lequel vous souhaitez ajouter l’itération. Pour ouvrir un workflow, cliquez sur [!UICONTROL **Afficher le flux de travail**].
1. Créez une itération à l’aide de l’une des méthodes suivantes :

   * Dans l’onglet Liste des cartes, dans la vue itération, cliquez sur [!UICONTROL **Créer une itération**].
   * Dans l’onglet Liste de cartes, en mode Liste, cliquez sur [!UICONTROL **Créer une itération**].
   * Dans l’onglet Panoramas , cliquez sur [!UICONTROL **Ajouter un panorama**] et sélectionnez [!UICONTROL **Processus d’itération**] comme modèle de panorama. Ouvrez ensuite le panneau d’itération, puis cliquez sur [!UICONTROL **Configurer des itérations**].

1. Dans la boîte de dialogue Détails de l’itération , ajoutez les informations suivantes :

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Nom de l’itération]</strong></td> 
      <td>Nom de l’itération, par exemple "Sprint 1".</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Longueur de l’itération]</strong></td> 
      <td>Durée de l’itération, en jours, semaines ou mois.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Date de début]</strong></td> 
      <td>Date à laquelle l’itération commence. La date de fin est automatiquement renseignée en fonction de la durée d'itération.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur [!UICONTROL **Enregistrer**].

   L’itération apparaît désormais dans la vue itération de la liste des cartes et dans la zone des mesures de la carte.

   Pour ajouter des cartes à une itération, reportez-vous à la section [Utiliser la liste des cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## Modifier une itération existante

1. Pour ouvrir un workflow, cliquez sur [!UICONTROL **Afficher le flux de travail**].
1. Ouvrez l’itération à l’aide de l’une des méthodes suivantes :

   * Dans l’onglet Liste des cartes, dans la vue itération, cliquez sur le bouton [!UICONTROL **Détails de l’itération**] icon ![Détails de l’itération](assets/iteration-details-button.png).
   * Dans la carte d’itération, cliquez sur le bouton [!UICONTROL **Détails de l’itération**] icon ![Détails de l’itération](assets/iteration-details-button.png) dans la zone des mesures en haut à droite.

1. Dans le [!UICONTROL Configuration de l’itération] modifiez l’itération selon vos besoins.
1. Pour modifier le nom de l’itération, développez [!UICONTROL **Détails de l’itération**].

   Une fois qu&#39;une itération a commencé, vous ne pouvez modifier que le nom de l&#39;itération et non les dates ou la durée de l&#39;itération.

1. <span class="preview">Pour ajouter des objectifs à l’itération, développez [!UICONTROL **Objectifs**].</span>
1. <span class="preview">Cliquez sur [!UICONTROL **Ajouter un objectif**], puis saisissez le nom de l’objectif.</span>

   <span class="preview">Lorsque les objectifs sont terminés lors de l’itération, vous pouvez cocher la case pour les marquer comme terminées ou cliquer sur l’icône **Supprimer** icon ![Icône Supprimer](assets/delete.png) pour supprimer un objectif. La zone des mesures située en haut à droite de l’itération indique le nombre d’objectifs existants et le nombre d’objectifs terminés.</span>

<!--
<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## Suppression d’une itération

1. Cliquez sur le bouton [!UICONTROL **Liste de cartes**] dans le workflow et ouvrez la vue itération.
1. Cliquez sur le bouton **Supprimer** icon ![Icône Supprimer](assets/delete.png) en regard de l’itération.
1. Cliquez sur [!UICONTROL **Suppression de l’itération**] sur le message de confirmation.
