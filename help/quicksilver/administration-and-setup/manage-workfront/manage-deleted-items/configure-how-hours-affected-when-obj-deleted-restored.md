---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configurer l’effet sur les heures lorsqu’un objet est supprimé et restauré
description: Vous pouvez configurer ce qui arrive aux heures lorsque quelqu’un supprime un projet, une tâche ou un problème sur lequel les heures sont consignées. L’option choisie détermine également ce qui se passe aux heures si le projet, la tâche ou le problème est restauré ultérieurement. (Pour plus d’informations sur la restauration d’éléments dans Workfront, voir Restaurer des éléments supprimés.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Configurer l’effet sur les heures lorsqu’un objet est supprimé et restauré

Vous pouvez configurer ce qui arrive aux heures lorsque quelqu’un supprime un projet, une tâche ou un problème sur lequel les heures sont consignées. L’option choisie détermine également ce qui se passe aux heures si le projet, la tâche ou le problème est restauré ultérieurement. (Pour plus d’informations sur la restauration d’éléments dans Workfront, voir [Restauration des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configuration de la gestion des heures lorsqu’un élément est supprimé et restauré

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Développer **Fiches horaires et heures**, puis cliquez sur **Préférences**.

1. Recherchez la variable **Préférences de suppression de projet, de tâche ou de problème** .
1. (Conditionnel) Pour configurer le mode de gestion des heures lors de la suppression d’un projet, sélectionnez l’une des options suivantes dans le **Lors de la suppression de projets** section :

   * Conservez les heures journalisées déjà ajoutées aux feuilles de temps en tant qu’heures générales (si ce projet est restauré ultérieurement, les heures restent sur la feuille de temps).\
      Cette option est sélectionnée par défaut.
   * Supprimez toutes les heures consignées (si ce projet est restauré ultérieurement, les heures consignées sont restaurées dans le projet).

1. (Conditionnel) Pour configurer le mode de gestion des heures lorsqu’une tâche ou un problème est supprimé, sélectionnez l’une des options suivantes dans la **Lors de la suppression de tâches ou de problèmes** section :

   * Déplacez les heures consignées vers le projet où réside la tâche ou le problème (si cette tâche ou ce problème est restauré ultérieurement, les heures restent sur le projet).\
      Cette option est sélectionnée par défaut.
   * Supprimez toutes les heures consignées (si cette tâche ou ce problème est restauré ultérieurement, les heures consignées sont restaurées à la tâche ou au problème).

1. Cliquer sur **Enregistrer**.
