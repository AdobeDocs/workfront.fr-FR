---
title: Accéder à la liste des statuts des problèmes système
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Vous pouvez utiliser le statut d’un problème pour montrer à quel stade de développement il se trouve à un moment donné.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 99%

---

# Accéder à la liste des statuts des problèmes du système

Vous pouvez utiliser le statut d’un problème pour montrer à quel stade de développement il se trouve à un moment donné.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Administrateur ou administratrice système</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Accéder aux statuts des problèmes

Vous pouvez accéder aux statuts des problèmes au niveau du système et les modifier. Vous pouvez modifier certaines informations sur les statuts système par défaut ou créer de nouveaux statuts personnalisés. Pour plus d’informations sur la création de statuts personnalisés ou la modification de statuts système, voir la section [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Pour accéder aux statuts des problèmes au niveau du système :

{{step-1-to-setup}}

1. Cliquez sur **Préférences du projet** > **Statuts**.

1. Cliquez sur l’onglet **Problèmes** pour voir les statuts des problèmes disponibles dans Workfront.

   ![Statut des événements](assets/issue-status.png)

## Statuts des problèmes du système

Workfront est livré avec 10 statuts de problèmes initiaux. Les quatre premiers du tableau ci-dessous sont obligatoires, ce qui signifie que vous pouvez les déverrouiller, les renommer et les réorganiser, mais ni les masquer ni les supprimer.

Vous pouvez ajouter des statuts de problème personnalisés pour répondre aux besoins de votre organisation. Pour plus d’informations, voir la section [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Pour les utilisateurs ou utilisatrices, la modification du statut d’un problème se fait généralement manuellement. Cependant, il existe des situations, décrites ci-dessous, dans lesquelles le statut d’un problème change automatiquement, en fonction d’autres facteurs qui se produisent dans le système.

Les statuts de problèmes suivants sont fournis avec votre instance Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Statut de problème du système</th> 
   <th>Comment utiliser le statut</th> 
   <th>Ce qui se passe dans le statut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nouveau (statut obligatoire)</td> 
   <td>Il s’agit du statut par défaut pour tout problème nouvellement créé.</td> 
   <td>Si le problème se trouve sur un projet dont le statut est En cours, il s’affiche dans l’onglet Demandes de travail des personnes affectées au problème. Les personnes peuvent maintenant commencer à travailler sur le problème.</td> 
  </tr> 
  <tr> 
   <td>En cours (statut obligatoire)</td> 
   <td> <p>Vous pouvez placer un problème dans ce statut pour indiquer que le travail sur ce problème a commencé.</p> <p>Si la résolution du problème est liée à un autre objet (une tâche, un projet ou un autre problème), le statut du problème passe automatiquement à En cours lorsque vous modifiez le statut de l’objet de résolution à En cours. </p> <p>Pour plus d’informations sur les objets de résolution, voir la section <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Vue d’ensemble des objets de résolution et des objets résolvables</a>.</p> </td> 
   <td> <p>Si le problème se trouve sur un projet dont le statut est Actuel, le problème s’affiche dans l’onglet En train de travailler sur des personnes qui sont assignées au problème.</p> <p>Lorsqu’un problème est En cours, il affiche une valeur pour la date de début effective.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Fermé (statut obligatoire)</td> 
   <td> <p>Vous pouvez marquer manuellement un problème comme Fermé lorsque le travail sur ce problème est terminé. </p> <p>Si la résolution du problème est liée à un autre objet (une tâche, un projet ou un autre problème), le statut du problème passe automatiquement à Fermé lorsque vous modifiez le statut de l’objet de résolution en Fermé.</p> <p>Pour plus d’informations sur les objets de résolution, voir la section <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Vue d’ensemble des objets de résolution et des objets résolvables</a>.</p> </td> 
   <td> <p>Lorsqu’un problème est Fermé, il est supprimé de la liste En train de travailler sur de la personne assignée. Dans ce cas, le problème indique une valeur pour la date d’achèvement effective. </p> <p>Lorsque toutes les tâches sont terminées et que les problèmes sont résolus dans un projet, le projet peut être achevé.</p> </td> 
  </tr> 
  <tr> 
   <td>En suspens (statut obligatoire)</td> 
   <td> <p>Vous pouvez marquer manuellement un problème comme étant En supens, pour indiquer qu’il y a eu un retard dans la résolution du problème. </p> </td> 
   <td> <p>Si le problème se trouve sur un projet dont le statut est Actuel, le problème s’affiche dans l’onglet En train de travailler sur des personnes qui sont assignées au problème. </p> <p>Lorsque toutes les tâches d’un projet sont terminées, mais qu’il reste au moins un problème En suspens, le projet ne peut pas être achevé. </p> </td> 
  </tr> 
  <tr> 
   <td>Rouvert (équivaut à En cours)</td> 
   <td> <p>Vous pouvez placer un problème dans ce statut pour indiquer que le travail sur ce problème n’était pas tout à fait terminé lorsque le problème a été précédemment fermé, et qu’il a dû être rouvert pour terminer le travail.</p> </td> 
   <td> <p>Si le problème se trouve sur un projet dont le statut est En cours, il s’affiche dans l’onglet Demandes de travail des personnes affectées au problème. Les personnes peuvent maintenant commencer à travailler sur le problème.</p> <p>Ce statut est important dans les rapports, pour différencier les problèmes ouverts pour la première fois (généralement dans le statut Nouveau), et les problèmes ouverts après avoir été fermés auparavant (généralement dans le statut Rouvert). </p> </td> 
  </tr> 
  <tr> 
   <td>En attente de commentaires (équivaut à En suspens)</td> 
   <td>Vous pouvez placer un problème dans ce statut pour indiquer que vous attendez du feedback (généralement de la part du contact principal) avant de pouvoir continuer à travailler sur le problème. </td> 
   <td> <p>Si le problème se trouve sur un projet dont le statut est Actuel, le problème s’affiche dans l’onglet En train de travailler sur des personnes qui sont assignées au problème.</p> <p>Si un problème est en attente de feedback, un projet ne peut pas être achevé.</p> <p>Ce statut est important dans les rapports, pour faire la différence entre les problèmes qui sont actuellement ouverts mais sur lesquels quelqu’un travaille (généralement dans le statut En cours) et les problèmes qui sont actuellement ouverts, mais sur lesquels personne ne travaille parce que du feedback supplémentaire est nécessaire pour les achever (généralement dans le statut En attente de feedback).</p> </td> 
  </tr> 
  <tr> 
   <td>Impossible à dupliquer (équivaut à Fermé)</td> 
   <td>Vous pouvez placer un problème dans ce statut pour indiquer que vous le fermez, mais que vous n’avez pas pu voir la raison qui a déclenché l’ouverture du problème. La raison peut toujours exister, mais elle ne peut pas être reproduite à un moment donné. </td> 
   <td> <p>Ce statut est important dans les rapports, pour différencier les problèmes qui sont terminés et dont la raison a été traitée (généralement dans le statut Fermé) des problèmes dont la raison n’est pas visible à un moment donné (généralement dans le statut Impossible à dupliquer).</p> <p>Lorsqu’un problème est marqué comme ne pouvant pas être dupliqué, il est supprimé de la liste En train de travailler sur de la personne cessionnaire. Dans ce cas, le problème indique une valeur pour la date d’achèvement réelle.</p> <p>Si toutes les tâches d’un projet sont achevées et que certains problèmes sont dans un statut Impossible de reproduire, le projet peut être achevé.</p> </td> 
  </tr> 
  <tr> 
   <td>Résolu (équivalent à Fermé)</td> 
   <td>Vous pouvez placer un problème dans ce statut pour indiquer que vous le clôturez et que la raison qui l’a créé a été résolue.</td> 
   <td> <p>Ce statut est important dans les rapports, pour différencier les problèmes qui sont clôturés avec ou sans résolution (généralement dans le statut Fermé) et les problèmes qui sont clôturés avec une résolution réelle (généralement dans le statut Résolu).</p> <p>Lorsqu’un problème est marqué comme Résolu, il est supprimé de la liste En train de travailler sur de la personne cessionnaire. Dans ce cas, le problème indique une valeur pour la date d’achèvement effective.</p> <p>Si toutes les tâches d’un projet sont terminées et qu’au moins un problème a le statut Résolu, le projet peut être achevé. </p> </td> 
  </tr> 
  <tr> 
   <td>Achèvement vérifié (équivalent à Fermé)</td> 
   <td>Vous pouvez placer un problème dans ce statut pour indiquer que vous clôturez le problème et que vous avez vérifié que la raison qui l’a généré a été résolue.</td> 
   <td> <p>Lorsqu’un problème est marqué comme Achèvement vérifié, il est supprimé de la liste En train de travailler sur de la personne cessionnaire. Dans ce cas, le problème indique une valeur pour la date d’achèvement effective.</p> <p>Si toutes les tâches d’un projet sont achevées et que certains problèmes sont dans un statut Achèvement vérifié, le projet peut être achevé.</p> </td> 
  </tr> 
  <tr> 
   <td>Impossible de résoudre (équivalent à Fermé)</td> 
   <td>Vous pouvez placer un problème dans ce statut pour indiquer que vous le clôturez, mais que la raison qui l’a généré ne peut pas être résolue.</td> 
   <td> <p>Ce statut est important dans les rapports, car il permet de différencier les problèmes qui sont clôturés avec ou sans résolution (généralement dans le statut Fermé) des problèmes qui sont clôturés sans résolution réelle (généralement dans le statut Impossible de résoudre).</p> <p>Lorsqu’un problème est marqué comme Impossible de résoudre, il est supprimé de la liste En train de travailler sur de la personne cessionnaire. Dans ce cas, le problème indique une valeur pour la date d’achèvement effective.</p> <p>Si toutes les tâches d’un projet sont achevées et qu’au moins un problème est dans le statut Impossible de résoudre, le projet peut être achevé.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnaliser les statuts du problème

Un administrateur ou une administratrice Workfront peut ajouter des statuts de problèmes au niveau du système et du groupe dans Workfront et modifier l’ordre dans lequel les personness les voient. Pour plus d’informations, voir [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Un administrateur ou une administratrice de groupes peut ajouter un statut personnalisé spécifique à un groupe. Pour plus d’informations, voir [Créer ou modifier un statut de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
