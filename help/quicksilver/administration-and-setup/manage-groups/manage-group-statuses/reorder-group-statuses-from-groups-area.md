---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Réorganiser les états du groupe
description: En tant qu’administrateur ou administratrice de groupes, vous pouvez modifier l’ordre des statuts des projets, des tâches et des problèmes d’un groupe que vous gérez.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 96%

---

# Réorganiser les statuts des groupes

En tant qu’administrateur ou administratrice de groupes, vous pouvez modifier l’ordre des statuts des projets, des tâches et des problèmes d’un groupe que vous gérez.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

>[!NOTE]
>
>* Un administrateur ou une administratrice Workfront peut réorganiser les statuts au niveau du système. Cela n’a aucune incidence sur l’ordre des statuts au sein des groupes.
>
>  Toutefois, les statuts d’un groupe de niveau supérieur nouvellement créé héritent de l’ordre des statuts à l’échelle du système. (Un nouveau sous-groupe hérite de l’ordre des statuts du groupe d’un niveau supérieur.)
>
>* Vous pouvez réorganiser les statuts verrouillés. Pour plus d’informations sur les statuts verrouillés, voir [Créer ou modifier un statut de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

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
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
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
     <p>Actuel</p> 
     <p>Immobilisé</p> 
     <p> Suspendu </p> 
     <p> Planification </p> 
     <p> Terminé </p> 
     <p> Demandé </p> 
     <p> Approuvé </p> 
     <p> Rejeté </p> 
     <p> Idée </p> 
   </td> 
   <td> 
     <p>Nouveau</p> 
     <p>En cours</p> 
     <p>Terminé</p> 
   </td> 
   <td> 
     <p>Nouveau</p> 
     <p>En cours</p> 
     <p>Rouvert</p> 
     <p>Réaction en attente</p> 
     <p>Suspendu</p> 
     <p>Impossible de reproduire</p> 
     <p>Fermé</p> 
     <p>Résolu</p> 
     <p>Achèvement vérifié</p> 
     <p>Impossible de résoudre</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## Réorganiser les statuts des tâches et des projets d’un groupe que vous gérez.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**, puis cliquez sur le nom du groupe.
1. Dans le panneau de gauche, cliquez sur **Statuts**.
1. Au-dessus de la liste de statuts qui s’affiche, cliquez sur l’onglet **Projets** ou **Tâches**.

1. Faites glisser et déposez les statuts dans l’ordre de votre choix.

   Le nouvel ordre de statuts est enregistré automatiquement.

1. Pour tester le nouvel ordre des statuts, accédez à une tâche associée ou à un projet associé au groupe, cliquez sur le statut dans le coin supérieur droit, puis vérifiez que les statuts s’affichent dans l’ordre que vous avez configuré.

## Réorganiser les statuts pour les problèmes

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**, puis cliquez sur le nom du groupe.
1. Dans le panneau de gauche, cliquez sur **Statuts**.
1. Sélectionnez l’onglet **Problèmes**.
1. (Facultatif) Sélectionnez un type de problème (**Rapport de bogues**, **Ordre de modification**, **Problème**, ou **Demande**).

   >[!NOTE]
   >
   >* Vous ne pouvez pas personnaliser l’ordre des statuts pour la liste principale des statuts.
   >* Nous vous recommandons d’organiser les statuts pour chaque type de problème de la même manière. Pour plus d’informations sur les types de problèmes, voir [Configuration des types de demandes](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Faites glisser et déposez les statuts dans l’ordre de votre choix.

   Le nouvel ordre de statuts est enregistré automatiquement.

1. Pour tester le nouvel ordre des statuts, accédez à un problème associé au groupe, cliquez sur le statut dans le coin supérieur droit, puis assurez-vous que les statuts s’affichent dans l’ordre que vous avez configuré.
