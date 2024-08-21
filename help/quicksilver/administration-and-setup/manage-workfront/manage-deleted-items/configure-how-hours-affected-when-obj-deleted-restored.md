---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configuration de l’effet sur les heures lorsqu’un objet est supprimé et restauré
description: Vous pouvez configurer ce qui arrive aux heures lorsque quelqu’un supprime un projet, une tâche ou un problème sur lequel les heures sont consignées. L’option choisie détermine également ce qui se passe aux heures si le projet, la tâche ou le problème est restauré ultérieurement. (Pour plus d’informations sur la restauration d’éléments dans Workfront, voir Restaurer des éléments supprimés.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 17%

---

# Configurer l’effet sur les heures lorsqu’un objet est supprimé et restauré

Vous pouvez configurer ce qui arrive aux heures lorsque quelqu’un supprime un projet, une tâche ou un problème sur lequel les heures sont consignées. L’option choisie détermine également ce qui se passe aux heures si le projet, la tâche ou le problème est restauré ultérieurement. (Pour plus d’informations sur la restauration d’éléments dans Workfront, voir [Restauration des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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

+++

## Configuration de la gestion des heures lorsqu’un élément est supprimé et restauré

{{step-1-to-setup}}

1. Développez **Fiches horaires et heures**, puis cliquez sur **Préférences**.

1. Recherchez la section **Préférences de suppression de projet, de tâche ou de problème** .
1. (Conditionnel) Pour configurer le mode de gestion des heures lors de la suppression d’un projet, sélectionnez l’une des options suivantes dans la section **Lors de la suppression de projets** :

   * Conserver les heures journalisées déjà ajoutées aux feuilles de temps en tant qu’heures générales (si ce projet est restauré ultérieurement, les heures restent sur la feuille de temps)\
     Cette option est sélectionnée par défaut.
   * Supprimer toutes les heures consignées (si ce projet est restauré ultérieurement, les heures consignées sont restaurées dans le projet)

1. (Conditionnel) Pour configurer la façon dont les heures sont gérées lorsqu’une tâche ou un problème est supprimé, sélectionnez l’une des options suivantes dans la section **Lors de la suppression de tâches ou de problèmes** :

   * Déplacez les heures consignées vers le projet où réside la tâche ou le problème (si cette tâche ou ce problème est restauré ultérieurement, les heures restent sur le projet).\
     Cette option est sélectionnée par défaut.
   * Supprimer toutes les heures consignées (si cette tâche ou ce problème est restauré ultérieurement, les heures consignées sont restaurées à la tâche ou au problème)

1. Cliquer sur **Enregistrer**.
