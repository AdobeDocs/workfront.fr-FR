---
title: Accéder à la liste des statuts des problèmes système
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Vous pouvez utiliser l’état d’un problème pour montrer aux utilisateurs du système à quel stade de développement un problème se trouve à un moment donné.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 5%

---

# Accéder à la liste des statuts des problèmes système

Vous pouvez utiliser l’état d’un problème pour montrer aux utilisateurs du système à quel stade de développement un problème se trouve à un moment donné.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Accès aux statuts des problèmes

Vous pouvez accéder aux états des problèmes au niveau du système et les modifier. Vous pouvez modifier des informations sur les états système par défaut ou créer de nouveaux états personnalisés. Pour plus d’informations sur la création d’états personnalisés ou la modification des états du système, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Pour accéder aux états de problème au niveau du système :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Préférences du projet** > **États**.

1. Cliquez sur l’onglet **Problèmes** pour afficher les états des problèmes disponibles dans Workfront.

   ![](assets/issue-status.png)

## Statuts des problèmes système

Workfront est fourni avec 10 statuts de problème originaux. Les 4 premiers du tableau ci-dessous sont obligatoires, ce qui signifie que vous pouvez les déverrouiller, les renommer et les réorganiser, mais vous ne pouvez pas les masquer ni les supprimer.

Vous pouvez ajouter des états de problème personnalisés pour répondre aux besoins de votre entreprise. Pour plus d’informations, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Pour les utilisateurs, la modification de l’état d’un problème est généralement un processus manuel. Cependant, il existe des situations, décrites dans la liste suivante, où l’état d’un problème change automatiquement, en fonction d’autres facteurs qui se produisent dans le système.

Les statuts de problème suivants sont fournis avec votre instance Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Statut du problème système</th> 
   <th>Utilisation de l’état</th> 
   <th>Ce qui se passe dans l’état</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nouveau (état requis)</td> 
   <td>Il s’agit de l’état par défaut de chaque problème nouvellement créé.</td> 
   <td>Si le problème se trouve sur un projet dont l’état est Actuel, il s’affiche dans l’onglet Demandes de travail des utilisateurs affectés au problème. Les utilisateurs peuvent maintenant commencer à travailler sur le problème.</td> 
  </tr> 
  <tr> 
   <td>En cours (statut requis)</td> 
   <td> <p>Vous pouvez placer un problème dans cet état pour indiquer que le travail sur ce problème a commencé.</p> <p>Si la résolution du problème est connectée à un autre objet (une tâche, un projet ou un autre problème), l’état du problème passe automatiquement à En cours lorsque vous définissez l’état de l’objet de résolution sur En cours. </p> <p>Pour plus d’informations sur la résolution d’objets, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Présentation de la résolution et de la résolution d’objets résolvables </a>.</p> </td> 
   <td> <p>Si le problème se trouve sur un projet dont l’état est Actuel, il s’affiche dans l’onglet Travail sur les utilisateurs affectés au problème.</p> <p>Lorsqu’un problème est En cours, il affiche une valeur pour la Date de début réelle.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Fermé (état requis)</td> 
   <td> <p>Vous pouvez marquer manuellement un problème comme Fermé une fois le travail terminé. </p> <p>Si la résolution du problème est connectée à un autre objet (une tâche, un projet ou un autre problème), l’état du problème passe automatiquement à Fermé lorsque vous définissez l’état de l’objet de résolution sur Fermé.</p> <p>Pour plus d’informations sur la résolution d’objets, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Présentation de la résolution et de la résolution d’objets résolvables </a>.</p> </td> 
   <td> <p>Lorsqu’un problème est Fermé, il est supprimé de la liste de travail sur la personne désignée. Dans ce cas, le problème affiche une valeur pour la date de fin réelle. </p> <p>Une fois toutes les tâches terminées et les problèmes terminés sur un projet, le projet peut être terminé.</p> </td> 
  </tr> 
  <tr> 
   <td>En attente (état requis)</td> 
   <td> <p>Vous pouvez marquer manuellement un problème comme En attente pour indiquer qu’il y a eu un retard dans l’exécution du problème. </p> </td> 
   <td> <p>Si le problème se trouve sur un projet dont l’état est Actuel, il s’affiche dans l’onglet Travail sur les utilisateurs affectés au problème. </p> <p>Lorsque toutes les tâches sont terminées sur un projet, mais qu’un problème au moins est en attente, le projet ne peut pas être terminé. </p> </td> 
  </tr> 
  <tr> 
   <td>rouvert (correspond à en cours)</td> 
   <td> <p>Vous pouvez placer un problème dans cet état pour indiquer que les travaux sur ce problème n’étaient pas encore terminés lorsque le problème a été précédemment fermé et qu’il fallait le rouvrir pour terminer le travail.</p> </td> 
   <td> <p>Si le problème se trouve sur un projet dont l’état est Actuel, il s’affiche dans l’onglet Demandes de travail des utilisateurs affectés au problème. Les utilisateurs peuvent maintenant commencer à travailler sur le problème.</p> <p>Ce statut est important dans les rapports. Il permet de différencier les problèmes ouverts pour la première fois (généralement dans le statut Nouveau) des problèmes ouverts après avoir été fermés auparavant (généralement dans le statut Réouverture). </p> </td> 
  </tr> 
  <tr> 
   <td>Commentaires en attente (équivaut à un blocage)</td> 
   <td>Vous pouvez placer un problème dans cet état pour indiquer que vous attendez les commentaires (généralement de la part du contact de Principal) avant de pouvoir continuer à travailler sur le problème. </td> 
   <td> <p>Si le problème se trouve sur un projet dont l’état est Actuel, il s’affiche dans l’onglet Travail sur les utilisateurs affectés au problème.</p> <p>Si un problème est En attente de commentaires, un projet ne peut pas être terminé.</p> <p>Ce statut est important dans les rapports. Il permet de différencier les problèmes actuellement ouverts mais sur lesquels on travaille (généralement dans l’état En cours ) et ceux qui sont actuellement ouverts, mais qui ne l’ont pas fait car il faut plus de commentaires pour les résoudre (généralement dans l’état Commentaires en attente).</p> </td> 
  </tr> 
  <tr> 
   <td>Impossible de dupliquer (correspond à avec Fermé)</td> 
   <td>Vous pouvez placer un problème dans cet état pour indiquer que vous fermez le problème, mais vous n’avez pas pu voir le problème qui a déclenché l’ouverture du problème. Le problème existe peut-être encore, mais il ne peut être répliqué à un moment donné. </td> 
   <td> <p>Ce statut est important dans les rapports, afin de différencier les problèmes terminés et dont le problème a été résolu (généralement avec le statut Fermé) et les problèmes dont le problème n’est pas visible à un moment donné (généralement avec le statut Impossible de dupliquer ).</p> <p>Lorsqu’un problème est marqué comme Impossible de dupliquer, il est supprimé de la liste de travail sur la personne désignée. Dans ce cas, le problème affiche une valeur pour la Date de fin réelle.</p> <p>Si toutes les tâches d’un projet sont terminées et que certains problèmes sont à l’état Impossible de dupliquer , le projet peut être terminé.</p> </td> 
  </tr> 
  <tr> 
   <td>Résolu (correspond à avec Fermé)</td> 
   <td>Vous pouvez placer un problème dans cet état pour indiquer que vous fermez le problème et que le problème qui l’a créé a été résolu.</td> 
   <td> <p>Ce statut est important dans les rapports, afin de différencier les problèmes fermés avec ou sans résolution (généralement dans le statut Fermé ) et les problèmes fermés avec une résolution réelle (généralement dans le statut Résolu ).</p> <p>Lorsqu’un problème est marqué comme résolu, il est supprimé de la liste de travail sur la personne désignée. Dans ce cas, le problème affiche une valeur pour la date de fin réelle.</p> <p>Si toutes les tâches d’un projet sont terminées et qu’au moins un problème est à l’état Résolu, le projet peut être terminé. </p> </td> 
  </tr> 
  <tr> 
   <td>Vérifié terminé (correspond à Fermé)</td> 
   <td>Vous pouvez placer un problème dans cet état pour indiquer que vous fermez le problème et que vous avez vérifié que le problème qui a généré le problème a été résolu.</td> 
   <td> <p>Lorsqu’un problème est marqué comme terminé par la vérification, il est supprimé de la liste de travail sur la personne désignée. Dans ce cas, le problème affiche une valeur pour la date de fin réelle.</p> <p>Si toutes les tâches d’un projet sont terminées et que certains problèmes sont à l’état Terminé vérifié, le projet peut être terminé.</p> </td> 
  </tr> 
  <tr> 
   <td>Ne pas résoudre (correspond à avec Fermé)</td> 
   <td>Vous pouvez placer un problème dans cet état pour indiquer que vous fermez le problème, mais le problème qui l’a généré ne peut pas être résolu.</td> 
   <td> <p>Ce statut est important dans les rapports, afin de différencier les problèmes qui sont fermés avec ou sans résolution (généralement dans le statut Fermé ) et les problèmes qui sont fermés sans résolution réelle (généralement dans le statut Ne pas résoudre).</p> <p>Lorsqu’un problème est signalé comme ne sera pas résolu, le problème est supprimé de la liste de travail sur les personnes désignées. Dans ce cas, le problème affiche une valeur pour la date de fin réelle.</p> <p>Si toutes les tâches d’un projet sont terminées et qu’au moins un problème est à l’état Ne pas résoudre, le projet peut être terminé.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnalisation des statuts des problèmes

Un administrateur Workfront peut ajouter des statuts de problème au niveau du système et du groupe à Workfront et modifier l’ordre dans lequel les utilisateurs les voient. Pour plus d’informations, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Un administrateur de groupe peut ajouter un état personnalisé spécifique à un groupe. Pour plus d’informations, voir [Création ou modification de l’état d’un groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
