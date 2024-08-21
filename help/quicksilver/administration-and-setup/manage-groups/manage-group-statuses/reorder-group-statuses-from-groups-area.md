---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Réorganiser les états du groupe
description: En tant qu’administrateur de groupe, vous pouvez modifier l’ordre du projet, des tâches et des états des problèmes pour un groupe que vous gérez.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 29%

---

# Réorganiser les statuts de groupe

En tant qu’administrateur de groupe, vous pouvez modifier l’ordre du projet, des tâches et des états des problèmes pour un groupe que vous gérez.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

S’il existe des groupes au-dessus du groupe que vous gérez, leur équipe d’administration peut également le faire pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

>[!NOTE]
>
>* Un administrateur Workfront peut réorganiser les états au niveau du système. Cela n’a aucune incidence sur l’ordre des états au sein des groupes.
>
>  Toutefois, les états d’un groupe de niveau supérieur nouvellement créé héritent de l’ordre des états au niveau du système. (Un nouveau sous-groupe hérite de l’ordre des états du groupe d’un niveau vers le haut.)
>
>* Vous pouvez réorganiser les états verrouillés. Pour plus d’informations sur les états verrouillés, voir [Création ou modification de l’état d’un groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront* </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur ou une administratrice de groupe pour le groupe ou un administrateur ou une administratrice de Workfront. Pour plus d’informations, consultez les sections <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à une personne</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir votre plan ou type de licence, contactez l’administration de Workfront.

+++

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

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**, puis sur le nom du groupe.
1. Dans le panneau de gauche, cliquez sur **Statuts**.
1. Au-dessus de la liste États qui s’affiche, cliquez sur l’onglet **Projets** ou **Tâches** .

1. Faites glisser les états dans l’ordre de votre choix.

   Le nouvel ordre d’état est enregistré automatiquement.

1. Pour tester le nouvel ordre de statut, accédez à une tâche ou à un projet associé au groupe, cliquez sur l’état dans le coin supérieur droit, puis vérifiez que les états qui s’affichent sont dans l’ordre que vous avez configuré.

## Réorganiser les états pour les problèmes

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**, puis sur le nom du groupe.
1. Dans le panneau de gauche, cliquez sur **Statuts**.
1. Cliquez sur l’onglet **Problèmes** .
1. (Facultatif) Sélectionnez un type de problème (**Rapport de bogues**, **Modifier l’ordre**, **Problème** ou **Requête**).

   >[!NOTE]
   >
   >* Vous ne pouvez pas personnaliser l’ordre des états pour la liste des Principal.
   >* Nous vous recommandons d’organiser les états pour chaque type de problème de la même manière. Pour plus d’informations sur les types de problèmes, voir [Configuration des types de requêtes](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Faites glisser les états dans l’ordre de votre choix.

   Le nouvel ordre d’état est enregistré automatiquement.

1. Pour tester le nouvel ordre de statut, accédez à un problème associé au groupe, cliquez sur l’état dans le coin supérieur droit, puis assurez-vous que les états qui s’affichent sont dans l’ordre que vous avez configuré.
