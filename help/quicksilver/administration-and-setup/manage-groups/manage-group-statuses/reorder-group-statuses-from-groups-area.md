---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Réorganiser les statuts des groupes
description: En tant qu’administrateur de groupe, vous pouvez modifier l’ordre du projet, des tâches et des états des problèmes pour un groupe que vous gérez.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 6%

---

# Réorganiser les statuts des groupes

En tant qu’administrateur de groupe, vous pouvez modifier l’ordre du projet, des tâches et des états des problèmes pour un groupe que vous gérez.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

>[!NOTE]
>
>* Un administrateur Workfront peut réorganiser les états au niveau du système. Cela n’a aucune incidence sur l’ordre des états au sein des groupes.
>
>  Toutefois, les états d’un groupe de niveau supérieur nouvellement créé héritent de l’ordre des états au niveau du système. (Un nouveau sous-groupe hérite de l’ordre des états du groupe d’un niveau vers le haut.)
>
>* Vous pouvez réorganiser les états verrouillés. Pour plus d’informations sur les états verrouillés, voir [Création ou modification d’un état de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>


## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront* </td> 
   <td>Tous</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur de groupe du groupe ou un administrateur Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Ordre par défaut des états

Par défaut, les états s’affichent dans l’ordre suivant :

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

## Réorganiser les états des tâches et des projets dans un groupe que vous gérez

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes**, puis cliquez sur le nom du groupe.
1. Dans le panneau de gauche, cliquez sur **Statuts**.
1. Au-dessus de la liste États qui s’affiche, cliquez sur le bouton **Projets** ou **Tâches** .

1. Faites glisser les états dans l’ordre de votre choix.

   Le nouvel ordre d’état est enregistré automatiquement.

1. Pour tester le nouvel ordre de statut, accédez à une tâche ou un projet associé au groupe, cliquez sur l’état dans le coin supérieur droit, puis vérifiez que les états qui s’affichent sont dans l’ordre que vous avez configuré.

## Réorganiser les états pour les problèmes

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes**, puis cliquez sur le nom du groupe.
1. Dans le panneau de gauche, cliquez sur **Statuts**.
1. Cliquez sur le bouton **Problèmes** .
1. (Facultatif) Sélectionnez un type de problème (**Rapport de bogues**, **Modifier l’ordre**, **Problème** ou **Requête**).

   >[!NOTE]
   >
   >* Vous ne pouvez pas personnaliser l’ordre des états pour la liste des Principal.
   >* Nous vous recommandons d’organiser les états pour chaque type de problème de la même manière. Pour plus d’informations sur les types de problèmes, voir [Configuration des types de requête](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. Faites glisser les états dans l’ordre de votre choix.

   Le nouvel ordre d’état est enregistré automatiquement.

1. Pour tester le nouvel ordre de statut, accédez à un problème associé au groupe, cliquez sur l’état dans le coin supérieur droit, puis assurez-vous que les états qui s’affichent sont dans l’ordre que vous avez configuré.
