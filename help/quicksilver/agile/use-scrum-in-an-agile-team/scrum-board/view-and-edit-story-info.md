---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Afficher et modifier les informations sur l'histoire sur le scrum board
description: Quand une mosaïque d’histoire est affichée sur le tableau Kanban, certaines données peuvent être modifiées en ligne, directement à partir de cette mosaïque.
author: Jenny
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 77%

---

# Afficher et modifier les informations d’une histoire dans un panorama [!UICONTROL Scrum]

## Comprendre quelles informations peuvent être affichées et modifiées.

Lors de l’affichage d’une mosaïque d’histoire sur le storyboard, les informations du tableau suivant sont disponibles. Vous pouvez modifier la plupart des informations en ligne, directement à partir de la mosaïque de l’histoire.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Informations</strong> </th> 
   <th><strong>Visibles</strong> </th> 
   <th><strong>Modifiables en ligne</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nom de l’histoire avec un lien direct vers la tâche ou le problème</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Nom du projet avec un lien direct vers le projet<br>Ce lien s’affiche uniquement sur les articles (tâches parents, et non les sous-tâches) lors de l’utilisation de la vue Agile sur une itération ; il ne s’affiche pas lors de l’utilisation d’une vue Agile sur un projet.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Nombre de points ou d’heures terminés sur cette histoire et nombre de points ou d’heures affectés à cette histoire<br> Ces nombres sont utilisés pour calculer et afficher le [!UICONTROL Percent Complete] pour chaque histoire.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Percent Complete] pour chaque histoire et problème.<br>Le [!UICONTROL Percent Complete] pour l’itération est calculé d’après le [!UICONTROL Percent Complete] pour chaque histoire.</p> <p>Lors de la mise à jour du [!UICONTROL Percent Complete] pour une histoire ou un problème, vous pouvez choisir un nombre compris entre 0 et 100.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>À qui l’histoire est affectée.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Couleur ou catégorie de la mosaïque</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Tous les champs supplémentaires (y compris les champs personnalisés) qui ont pu être ajoutés à la vue Agile en modifiant la vue Agile, comme décrit dans la section « Création et personnalisation d’une vue [!UICONTROL Agile] » dans <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Présentation des vues dans [!UICONTROL Adobe Workfront]</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p> 
   ou
   <p>Actuelle : [!UICONTROL Work] ou niveau supérieur</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Accès de [!UICONTROL Contribute] ou de [!UICONTROL Manage] à la tâche ou à l'événement</td> 
  </tr>
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher et modifier les informations sur une mosaïque d’histoire

{{step1-to-team}}

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Itérations]** pour sélectionner une itération spécifique, ou choisissez **[!UICONTROL Itération actuelle]**.

1. Accédez au storyboard [!UICONTROL Scrum] Agile.
1. Développez la tuile de l’[!UICONTROL histoire] pour afficher tous les champs associés à l’histoire.

   ![carte d’histoire](assets/agile-storycard-scrum-2021-350x333.png)

1. (Facultatif) Pour modifier un champ, cliquez dessus, puis effectuez les modifications nécessaires.

   Vous devez disposer des droits [!UICONTROL Modifier] de la tâche ou du problème pour modifier la tuile de l’histoire.

>[!NOTE]
>
>Pour modifier le [!UICONTROL pourcentage d’achèvement], vous devez saisir un nombre compris entre 0 et 100. Le champ n’est pas un curseur que vous pouvez déplacer.
