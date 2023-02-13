---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Statuts des tâches du système
description: Les trois états de tâches système intégrés dans Workfront sont obligatoires, ce qui signifie que vous pouvez les déverrouiller, les renommer et les réorganiser, mais vous ne pouvez pas les masquer ni les supprimer. Vous pouvez également ajouter de nouveaux états de tâches système pour répondre aux besoins de votre entreprise. La modification de l’état d’une tâche est généralement un processus manuel, mais parfois l’état d’une tâche est modifié automatiquement, en fonction d’autres facteurs qui se produisent dans le système.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Statuts des tâches du système

Les trois états de tâches système intégrés dans Workfront sont obligatoires, ce qui signifie que vous pouvez les déverrouiller, les renommer et les réorganiser, mais vous ne pouvez pas les masquer ni les supprimer.

Vous pouvez également ajouter de nouveaux états de tâches système pour répondre aux besoins de votre entreprise.

La modification de l’état d’une tâche est généralement un processus manuel. Cependant, certains moments sont décrits dans la liste suivante lorsque l’état d’une tâche est automatiquement modifié, en fonction d’autres facteurs qui se produisent dans le système.

Les états de tâche suivants sont fournis avec votre instance Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>État des tâches système</th> 
   <th>Lorsque cet état se produit</th> 
   <th>Actions qui se produisent lorsqu’une tâche est dans cet état</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nouveau (état requis)</td> 
   <td>Il s’agit de l’état par défaut de chaque tâche nouvellement créée.</td> 
   <td>Si la tâche se trouve sur un projet dont l’état est Actuel, la tâche s’affiche dans l’onglet Requêtes de travail des utilisateurs affectés aux tâches. Les utilisateurs peuvent maintenant commencer à travailler sur la tâche.</td> 
  </tr> 
  <tr> 
   <td>En cours (statut requis)</td> 
   <td>Vous pouvez placer une tâche dans cet état pour indiquer que le travail sur cette tâche a commencé.</td> 
   <td> <p>Lorsque vous marquez une tâche comme En cours, la tâche affiche une valeur pour la Date de début réelle.</p> <p>L’état d’avancement de la tâche n’est pas enregistré tant que vous n’avez pas mis à jour manuellement le pourcentage d’achèvement de la tâche.</p> </td> 
  </tr> 
  <tr> 
   <td>Terminé (état requis)</td> 
   <td> <p>Vous pouvez marquer manuellement la fin d’une tâche lorsque celle-ci est terminée.</p> <p>Lorsque le mode de suivi d’une tâche est défini sur Terminé automatiquement, la tâche est automatiquement marquée Terminée lorsqu’elle atteint la Date d’achèvement planifiée.</p> </td> 
   <td> <p>Lorsqu’une tâche est terminée, le pourcentage d’achèvement de la tâche est marqué comme 100 %. La tâche est supprimée de la liste de travail de la personne désignée dans la zone Accueil une fois qu’elle est terminée.</p> <p>Lorsque vous marquez une tâche comme terminée, la tâche affiche une valeur pour la Date de fin réelle.</p> <p><b>REMARQUE</b>: Si la tâche présente des problèmes incomplets et que vous définissez l’état de la tâche sur Terminé, l’état passe automatiquement à Terminé - Problèmes en attente.</p> </td> 
  </tr> 
 </tbody> 
</table>
