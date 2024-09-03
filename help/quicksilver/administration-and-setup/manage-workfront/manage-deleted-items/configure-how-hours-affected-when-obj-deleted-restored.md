---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configuration de l’effet sur les heures lorsqu’un objet est supprimé et restauré
description: Vous pouvez configurer ce qui arrive aux heures lorsqu’une personne supprime un projet, une tâche ou un problème sur lequel des heures sont consignées. L’option choisie détermine également le sort des heures si le projet, la tâche ou le problème est restauré(e) ultérieurement. (Pour plus d’informations sur la restauration d’éléments dans Workfront, consultez la section « Restaurer des éléments supprimés ».)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 94%

---

# Configurer l’effet sur les heures lorsqu’un objet est supprimé et restauré

Vous pouvez configurer ce qui arrive aux heures lorsqu’une personne supprime un projet, une tâche ou un problème sur lequel des heures sont consignées. L’option choisie détermine également le sort des heures si le projet, la tâche ou le problème est restauré(e) ultérieurement. (Pour plus d’informations sur la restauration d’éléments dans Workfront, consultez la section [Restaurer des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurer la gestion des heures lorsqu’un élément est supprimé et restauré.

{{step-1-to-setup}}

1. Développez **Feuilles de temps et heures**, puis cliquez sur **Préférences**.

1. Recherchez la section **Préférences de suppression de projet, de tâche ou de problème**.
1. (Le cas échéant) Pour configurer le mode de gestion des heures lors de la suppression d’un projet, sélectionnez l’une des options suivantes dans la section **Lors de la suppression de projets** :

   * Conserver les heures consignées déjà ajoutées aux feuilles de temps comme heures générales (si ce projet est restauré ultérieurement, les heures restent sur la feuille de temps).\
     Cette option est sélectionnée par défaut.
   * Supprimer toutes les heures consignées (si ce projet est restauré ultérieurement, les heures consignées sont restaurées dans le projet).

1. (Le cas échéant) Pour configurer le mode de gestion des heures lors de la suppression d’une tâche ou d’un problème, sélectionnez l’une des options suivantes dans la section **Lors de la suppression de tâches ou de problèmes** :

   * Déplacer les heures consignées vers le projet contenant la tâche ou le problème (en cas de restauration ultérieure de la tâche ou du problème, les heures restent dans le projet).\
     Cette option est sélectionnée par défaut.
   * Supprimer les heures consignées (en cas de restauration ultérieure de la tâche ou du problème, les heures consignées seront restaurées sur la tâche ou le problème).

1. Cliquer sur **Enregistrer**.
