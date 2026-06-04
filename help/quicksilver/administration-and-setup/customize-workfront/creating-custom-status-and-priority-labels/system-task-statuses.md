---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Statuts des tâches système
description: Les trois statuts de tâches du système intégrés dans Workfront sont obligatoires, ce qui signifie que vous pouvez les déverrouiller, les renommer et les réorganiser, mais vous ne pouvez pas les masquer ou les supprimer. Vous pouvez également ajouter de nouveaux statuts de tâches du système pour répondre aux besoins de votre organisation. La modification du statut d’une tâche est généralement un processus manuel, mais il arrive que le statut d’une tâche soit modifié automatiquement, en fonction d’autres facteurs intervenant dans le système.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
TQID: https://experienceleague.adobe.com/FACmZvT5v00-FS0lOBCMh347ZqM6c-Upfq4ITymVpV0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 409
ht-degree: 94%

---

# Statuts de tâches du système

Les trois statuts de tâches du système intégrés dans Workfront sont obligatoires, ce qui signifie que vous pouvez les déverrouiller, les renommer et les réorganiser, mais vous ne pouvez pas les masquer ou les supprimer.

Vous pouvez également ajouter de nouveaux statuts de tâches du système pour répondre aux besoins de votre organisation.

La modification du statut d’une tâche est généralement un processus manuel. Toutefois, dans certains cas décrits dans la liste suivante, le statut d’une tâche est modifié automatiquement, en fonction d’autres facteurs intervenant dans le système.

Les statuts de tâches suivants sont fournis avec votre instance Workfront :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Statut de tâche du système</th> 
   <th>Lorsque ce statut se produit :</th> 
   <th>Actions qui se produisent lorsqu’une tâche a ce statut :</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nouveau (statut obligatoire)</td> 
   <td>Il s’agit du statut par défaut de toute tâche qui vient d’être créée.</td> 
   <td>Si la tâche se trouve dans un projet dont le statut est Actuel, la tâche s’affiche dans l’onglet Demandes de travail des utilisateurs et utilisatrices affectés aux tâches. Les utilisateurs et utilisatrices peuvent maintenant commencer à travailler sur la tâche.</td> 
  </tr> 
  <tr> 
   <td>En cours (statut obligatoire)</td> 
   <td>Vous pouvez donner ce statut à une tâche pour indiquer que le travail sur cette tâche a commencé.</td> 
   <td> <p>Lorsque vous marquez une tâche comme En cours, la tâche affiche une valeur pour la date de début effective.</p> <p>La progression de la tâche n’est pas enregistrée tant que vous n’avez pas mis à jour manuellement le pourcentage terminé de la tâche.</p> </td> 
  </tr> 
  <tr> 
   <td>Terminée (statut obligatoire)</td> 
   <td> <p>Vous pouvez marquer manuellement une tâche comme terminée lorsque le travail est achevé.</p> <p>Lorsque le mode de suivi d’une tâche est défini sur Achèvement automatique, la tâche est automatiquement marquée comme terminée lorsqu’elle atteint la date d’achèvement prévue.</p> </td> 
   <td> <p>Lorsqu’une tâche est achevée, le pourcentage terminé de la tâche apparaît sur 100 %. Une fois terminée, la tâche est supprimée de la liste Mes tâches de la personne désignée dans la zone d’Accueil.</p> <p>Lorsque vous marquez une tâche comme Terminée, la tâche affiche une valeur pour la date d’achèvement effective.</p> <p><b>NOTE</b> : si la tâche a des problèmes incomplets et que vous changez le statut de la tâche sur Terminée, le statut devient automatiquement Terminée - Problèmes en attente.</p> </td> 
  </tr> 
 </tbody> 
</table>
