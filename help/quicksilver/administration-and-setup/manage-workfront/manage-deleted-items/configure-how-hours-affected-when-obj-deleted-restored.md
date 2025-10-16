---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configurer l’effet sur les heures de suppression et de restauration d’un objet
description: Vous pouvez configurer ce qui arrive aux heures lorsqu’une personne supprime un projet, une tâche ou un problème sur lequel des heures sont consignées. L’option choisie détermine également le sort des heures si le projet, la tâche ou le problème est restauré(e) ultérieurement. (Pour plus d’informations sur la restauration d’éléments dans Workfront, consultez la section « Restaurer des éléments supprimés ».)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 93%

---

# Configurer l’effet sur les heures de suppression et de restauration d’un objet

Vous pouvez configurer ce qui arrive aux heures lorsqu’une personne supprime un projet, une tâche ou un problème sur lequel des heures sont consignées. L’option choisie détermine également le sort des heures si le projet, la tâche ou le problème est restauré(e) ultérieurement. (Pour plus d’informations sur la restauration d’éléments dans Workfront, consultez la section [Restaurer des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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
