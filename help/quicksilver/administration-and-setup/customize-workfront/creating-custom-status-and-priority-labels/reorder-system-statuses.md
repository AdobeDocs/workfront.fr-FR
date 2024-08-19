---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Réorganiser les états au niveau du système et du groupe
description: En tant qu’administrateur Workfront, vous pouvez modifier l’ordre du projet, de la tâche et des états des problèmes pour tous les membres du système ou pour un seul groupe.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 16%

---

# Réorganiser les états au niveau du système et du groupe

En tant qu’administrateur Workfront, vous pouvez modifier l’ordre du projet, de la tâche et des états des problèmes pour tous les membres du système ou pour un seul groupe.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![](assets/statuses.png)

>[!NOTE]
>
>* La réorganisation des états au niveau du système n’a aucune incidence sur l’ordre des états au sein des groupes.
>
>  Toutefois, les états d’un groupe de niveau supérieur nouvellement créé héritent de l’ordre des états au niveau du système. (Un nouveau sous-groupe hérite de l’ordre des états du groupe d’un niveau vers le haut.)
>
>* Vous pouvez réorganiser les états verrouillés. Pour plus d’informations sur les états verrouillés, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Les administrateurs de groupe peuvent également réorganiser les états utilisés dans leurs groupes. Pour plus d’informations, voir [Réorganiser les états d’un groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
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
  <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur Workfront. Pour plus d’informations sur les administrateurs de Workfront, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès d’administration complet à un utilisateur</a>.</p> </td> 
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

## Réorganiser les états pour les tâches et les projets à l’échelle du système ou pour un groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Préférences du projet > Statuts**.
1. (Conditionnel) Si vous réorganisez les états d’un groupe, commencez à saisir le nom du groupe dans la zone située dans le coin supérieur droit, puis cliquez sur le nom lorsqu’il s’affiche.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Au-dessus de la liste États qui s’affiche, cliquez sur l’onglet **Projets** ou **Tâches** .

1. Faites glisser les états dans l’ordre de votre choix.

   Le nouvel ordre d’état est enregistré automatiquement.

1. Pour tester le nouvel ordre de statut, accédez à une tâche ou un projet, cliquez sur l’état dans le coin supérieur droit, puis assurez-vous que les états qui s’affichent sont dans l’ordre que vous avez configuré.

## Réorganiser les états pour les problèmes

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Préférences du projet > États.**
1. (Conditionnel) Si vous réorganisez les états d’un groupe, commencez à saisir le nom du groupe dans la zone située dans le coin supérieur droit, puis cliquez sur le nom lorsqu’il s’affiche.

   ![](assets/issue-statuses-group-name.png)

1. Cliquez sur l’onglet **Problèmes** .
1. (Facultatif) Sélectionnez un type de problème (**Rapport de bogues**, **Modifier l’ordre**, **Problème** ou **Requête**).

   >[!NOTE]
   >
   >* Vous ne pouvez pas personnaliser l’ordre des états pour la liste des Principal.
   >* Nous vous recommandons d’organiser les états pour chaque type de problème de la même manière. Pour plus d’informations sur les types de problèmes, voir [Configuration des types de requêtes](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Faites glisser les états dans l’ordre de votre choix.

   Le nouvel ordre d’état est enregistré automatiquement.

1. Pour tester le nouvel ordre de statut, accédez à un problème, cliquez sur l’état dans le coin supérieur droit, puis assurez-vous que les états qui s’affichent sont dans l’ordre que vous avez configuré.
