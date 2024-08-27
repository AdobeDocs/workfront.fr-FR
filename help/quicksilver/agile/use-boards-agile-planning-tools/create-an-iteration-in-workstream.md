---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Création d’une itération dans un flux de travail
description: Une itération est un temps défini réservé à la réalisation du travail. Certaines équipes agiles peuvent appeler une itération sprint.
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 20%

---

# Créer une itération dans un flux de travail

>[!IMPORTANT]
>
>Les flux de travail ne sont disponibles que pour un groupe spécifique de clientes et de clients.

Une itération est un temps défini réservé à la réalisation du travail. Certaines équipes agiles peuvent appeler une itération sprint.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> 
   <p>Nouvelle : [!UICONTROL Contributor] ou niveau supérieur</p> 
   <p>ou</p>
   <p>Actuel : [!UICONTROL Request] ou supérieure</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une itération dans un flux de travail

{{step1-to-boards}}

1. Ouvrez le workflow dans lequel vous souhaitez ajouter l’itération. Pour ouvrir un workflow, cliquez sur [!UICONTROL **Afficher le workflow**].
1. Créez une itération à l’aide de l’une des méthodes suivantes :

   * Dans l’onglet Liste des cartes, dans la vue itération, cliquez sur [!UICONTROL **Créer une itération**].
   * Dans l’onglet Liste des cartes, en mode Liste, cliquez sur [!UICONTROL **Créer une itération**].
   * Dans l’onglet Panoramas, cliquez sur [!UICONTROL **Ajouter un panorama**] et sélectionnez [!UICONTROL **Processus d’itération**] comme modèle de panorama. Ouvrez ensuite le tableau d’itération et cliquez sur [!UICONTROL **Configurer les itérations**].

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
      <td><strong>[!UICONTROL Start date]</strong></td> 
      <td>Date à laquelle l’itération commence. La date de fin est automatiquement renseignée en fonction de la durée d'itération.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur [!UICONTROL **Enregistrer**].

   L’itération apparaît désormais dans la vue itération de la liste des cartes et dans la zone des mesures de la carte.

   Pour ajouter des cartes à une itération, reportez-vous à la section [Utilisation de la liste de cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## Modifier une itération existante

1. Pour ouvrir un workflow, cliquez sur [!UICONTROL **Afficher le workflow**].
1. Ouvrez l’itération à l’aide de l’une des méthodes suivantes :

   * Dans l’onglet Liste des cartes, dans la vue itération, cliquez sur l’icône [!UICONTROL **Détails de l’itération**] ![Détails de l’itération](assets/iteration-details-button.png).
   * Sur le panneau d’itération, cliquez sur l’icône [!UICONTROL **Détails de l’itération**] ![Détails de l’itération](assets/iteration-details-button.png) dans la zone des mesures en haut à droite.

1. Dans le panneau [!UICONTROL  Iteration Configuration] , modifiez l’itération selon vos besoins.
1. Pour modifier le nom de l’itération, développez [!UICONTROL **Iteration details**].

   Une fois qu&#39;une itération a commencé, vous ne pouvez modifier que le nom de l&#39;itération et non les dates ou la durée de l&#39;itération.

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

1. Cliquez sur l’onglet [!UICONTROL **Liste de cartes**] du workflow et ouvrez la vue itération.
1. Cliquez sur l&#39;icône **Supprimer** ![Icône Supprimer](assets/delete.png) en regard de l&#39;itération.
1. Cliquez sur [!UICONTROL **Supprimer l&#39;itération**] dans le message de confirmation.
