---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Modifier les informations sur l'histoire
description: Quand une mosaïque d’histoire est affichée sur le tableau Kanban, certaines données peuvent être modifiées en ligne, directement à partir de cette mosaïque.
author: Jenny
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 83%

---

# Modifier les informations d’une histoire

## Comprendre quelles informations peuvent être affichées et modifiées. {#understand-what-information-can-be-viewed-and-edited}

Lors de l’affichage d’une tuile d’histoire sur le tableau [!UICONTROL Kanban], les informations du tableau suivant sont disponibles. Vous pouvez modifier la plupart des informations en ligne, directement à partir de la mosaïque de l’histoire.

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
   <td> <p>Nom du projet avec un lien direct vers le projet</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Le nombre de points ou d’heures réalisés sur l’histoire et le nombre de points ou d’heures affectés à l’histoire<br>Ces nombres sont utilisés pour calculer et afficher le pourcentage d’achèvement pour chaque histoire.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Percent Complete] pour chaque histoire et problème.<br>[!UICONTROL The Percent Complete] de l’itération est calculé sur la base du [!UICONTROL Percent Complete] de chaque histoire.<br></p> <p>Lors de la mise à jour du [!UICONTROL Percent Complete] pour une histoire ou un problème, vous pouvez choisir un nombre compris entre 0 et 100.</p> </td> 
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
   <td> <p>Tous les champs supplémentaires (y compris les champs personnalisés) qui ont pu être ajoutés à la vue Agile en modifiant la vue Agile, comme décrit dans « Création et personnalisation d’une vue Agile » dans <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Présentation des vues dans [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Travail ou supérieur</p> </td> 
  </tr>
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher et modifier les informations sur une mosaïque d’histoire

{{step1-to-team}}

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Kanban dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Accédez au tableau [!UICONTROL Kanban].
1. Développez la tuile de l’histoire pour afficher tous les champs qui lui sont associés.

   ![Carte d’histoire](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Facultatif) Pour modifier un champ, cliquez sur le champ, puis apportez les modifications nécessaires.
Vous devez disposer des droits [!UICONTROL Modifier] sur la tâche ou l’événement pour modifier la mosaïque de l’histoire.
Pour plus d’informations sur chaque champ et savoir s’il peut être modifié, voir la section [Comprendre les informations qui peuvent être visualisées et modifiées](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Pour modifier le [!UICONTROL Pourcentage d’achèvement], vous devez saisir un nombre compris entre 0 et 100. Le champ n’est pas un curseur que vous pouvez déplacer.
