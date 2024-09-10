---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Réorganiser les états au niveau du système et du groupe
description: En tant qu’administrateur ou administratrice Workfront, vous pouvez modifier l’ordre des statuts des projets, des tâches et des problèmes pour toutes les personnes membres du système ou pour un seul groupe.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 99%

---

# Réorganiser les statuts à l’échelle du système et du groupe

En tant qu’administrateur ou administratrice Workfront, vous pouvez modifier l’ordre des statuts des projets, des tâches et des problèmes pour toutes les personnes membres du système ou pour un seul groupe.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![](assets/statuses.png)

>[!NOTE]
>
>* La réorganisation des statuts à l’échelle du système n’a aucune incidence sur l’ordre des statuts au sein des groupes.
>
>  Toutefois, les statuts d’un groupe de niveau supérieur nouvellement créé héritent de l’ordre des statuts à l’échelle du système. (Un nouveau sous-groupe hérite de l’ordre des statuts du groupe d’un niveau supérieur.)
>
>* Vous pouvez réorganiser les statuts verrouillés. Pour plus d’informations sur les statuts verrouillés, voir [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Les administrateurs et administratrices de groupe peuvent également réorganiser les statuts utilisés dans leurs groupes. Pour plus d’informations, voir [Réorganiser les statuts des groupes](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
>

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
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
     <p>Nouveau : Standard</p>
     <p>ou</p>
     <p>Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ordre par défaut des statuts

Par défaut, les statuts s’affichent dans l’ordre suivant :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">Projet</th> 
   <th width="33.33%">Tâche</th> 
   <th width="33.33%">Problème</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Actuel</li> 
     <li>Immobilisé</li> 
     <li> Suspendu </li> 
     <li> Planification </li> 
     <li> Terminé </li> 
     <li> Demandé </li> 
     <li> Approuvé </li> 
     <li> Rejeté </li> 
     <li> Idée </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nouveau</li> 
     <li>En cours</li> 
     <li>Terminé</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Nouveau</li> 
     <li>En cours</li> 
     <li>Rouvert</li> 
     <li>Réaction en attente</li> 
     <li>Suspendu</li> 
     <li>Impossible de reproduire</li> 
     <li>Fermé</li> 
     <li>Résolu</li> 
     <li>Achèvement vérifié</li> 
     <li>Impossible de résoudre</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Réorganiser les statuts pour les tâches et les projets à l’échelle du système ou pour un groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Préférences du projet > Statuts**.
1. (Le cas échéant) Si vous réorganisez les statuts d’un groupe, commencez à saisir le nom du groupe dans la zone située dans le coin supérieur droit, puis cliquez sur le nom lorsqu’il s’affiche.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Au-dessus de la liste Statuts qui s’affiche, cliquez sur l’onglet **Projets** ou **Tâches**.

1. Faites glisser et déposez les statuts dans l’ordre de votre choix.

   Le nouvel ordre de statuts est enregistré automatiquement.

1. Pour tester le nouvel ordre de statuts, accédez à une tâche ou un projet, cliquez sur le statut dans le coin supérieur droit, puis assurez-vous que les statuts qui s’affichent sont dans l’ordre que vous avez configuré.

## Réorganiser les statuts pour les problèmes

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Préférences du projet > Statuts.**
1. (Le cas échéant) Si vous réorganisez les statuts d’un groupe, commencez à saisir le nom du groupe dans la zone située dans le coin supérieur droit, puis cliquez sur le nom lorsqu’il s’affiche.

   ![](assets/issue-statuses-group-name.png)

1. Cliquez sur l’onglet **Problèmes**.
1. (Facultatif) Sélectionnez un type de problème (**Rapport de bogues**, **Ordre de modification**, **Problème**, ou **Demande**).

   >[!NOTE]
   >
   >* Vous ne pouvez pas personnaliser l’ordre des statuts pour la liste principale des statuts.
   >* Nous vous recommandons d’organiser les statuts pour chaque type de problème de la même manière. Pour plus d’informations sur les types de problèmes, voir [Configuration des types de demandes](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Faites glisser et déposez les statuts dans l’ordre de votre choix.

   Le nouvel ordre de statuts est enregistré automatiquement.

1. Pour tester le nouvel ordre de statuts, accédez à un problème, cliquez sur le statut dans le coin supérieur droit, puis assurez-vous que les statuts qui s’affichent sont dans l’ordre que vous avez configuré.
