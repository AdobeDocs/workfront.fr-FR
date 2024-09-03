---
title: Comment les modifications du processus d’approbation et de groupe affectent-elles les processus d’approbation attribués
user-type: administrator
content-type: reference
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Cet article explique ce qui se passe lorsqu’un processus d’approbation est déjà utilisé lorsqu’un administrateur ou une administratrice Workfront (ou un utilisateur ou une utilisatrice ayant un accès administratif aux processus d’approbation) modifie son association avec un groupe.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 77b2dce2-1523-4262-a659-0d301059a54c
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 99%

---

# Comment les modifications du processus d’approbation et de groupe affectent les processus d’approbation affectés

Cet article explique ce qui se passe lorsqu’un processus d’approbation est déjà associé à des tâches, des problèmes, des projets, des modèles ou des tâches de modèle, et qu’un administrateur ou une administratrice Workfront (ou un utilisateur ou une utilisatrice ayant un accès administratif aux processus d’approbation) effectue l’une des opérations suivantes :

* Changer le processus d’approbation (au niveau du groupe) d’un groupe à un autre
* Modifier le groupe associé au projet
* Modifie le processus d’approbation du niveau du groupe au niveau du système.
* Modifie le processus d’approbation du niveau du système au niveau du groupe.

L’article décrit également ce qui se passe lors du déplacement ou de la copie de tâches ou de problèmes associés à un processus d’approbation au niveau du groupe entre deux projets de différents groupes.

Pour plus d’informations sur les trois types de processus d’approbation que vous pouvez utiliser dans Workfront, voir [Vue d’ensemble du processus d’approbation](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

>[!NOTE]
>
>Si le projet, ses tâches ou ses problèmes sont déjà associés à un processus d’approbation au niveau du groupe à l’aide de statuts personnalisés au niveau du groupe, la modification du groupe peut créer un conflit entre les statuts d’approbation du groupe précédent et ceux existant au niveau du système.
>
>Par exemple, si un processus d’approbation contient deux chemins, l’un pour un statut au niveau du système et l’autre pour un statut au niveau du groupe qui équivaut au même statut au niveau du système et que vous modifiez le groupe du projet d’origine, Workfront aura du mal à comprendre le statut spécifique du groupe qui peut ne pas exister sur le second groupe. Dans ce cas, une erreur se produira.
>
>Envisagez de supprimer les processus d’approbation au niveau du groupe sur le projet, ou ses tâches ou problèmes avant de mettre à jour le groupe du projet.
>
>Pour plus d’informations sur la création de processus d’approbation au niveau du groupe, voir [Processus d’approbation au niveau du groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).
>
>Pour plus d’informations sur la création d’un statut personnalisé au niveau du groupe, voir [Créer ou modifier un statut de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)

## Modifier le processus d’approbation d’un groupe à un autre

Les scénarios suivants se produisent lorsqu’un processus d’approbation spécifique à un groupe est déjà utilisé sur un objet et qu’une personne le réaffecte à un autre groupe :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zone ou objet à laquelle ou auquel le processus d’approbation a été associé.</th> 
   <th>Objet d’approbation</th> 
   <th>Modifier le processus d’approbation de l’objet ou de la zone</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Approbation du projet ou du modèle </td> 
   <td>Projet</td> 
   <td>Devient un processus d’approbation à usage unique.</td> 
  </tr> 
  <tr> 
   <td>Approbation de tâche ou de tâche de modèle </td> 
   <td>Tâche</td> 
   <td>Devient un processus d’approbation à usage unique. </td> 
  </tr> 
  <tr> 
   <td>Approbation de problème</td> 
   <td>Problème</td> 
   <td>Devient un processus d’approbation à usage unique.</td> 
  </tr> 
  <tr> 
   <td>Zone Tâches de la zone Modifier le projet ou Modifier le modèle</td> 
   <td>Tâche</td> 
   <td> <p>Le champ Processus d’approbation par défaut de la tâche est réinitialisé sur S/O.</p> <p>Par défaut, aucun processus d’approbation n’est associé à de nouvelles tâches sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Section Détails de la file d’attente d’un projet ou d’un modèle</td> 
   <td>Problème</td> 
   <td> <p>Le champ Approbation par défaut est réinitialisé sur S/O.</p> <p>Par défaut, aucun processus d’approbation n’est associé à de nouveaux problèmes ou requêtes sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Section Rubrique de file d’attente d’un projet ou d’un modèle</td> 
   <td>Problème</td> 
   <td> <p>Le champ Approbation par défaut est réinitialisé sur S/O.</p> <p>Aucun processus d’approbation n’est associé par défaut à de nouveaux problèmes ou demandes sur le projet.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modifier le groupe associé à un projet

Lorsqu’une personne change le groupe associé à un projet pour un autre groupe, les événements suivants se produisent :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zone ou objet dont le processus d’approbation est déjà associé.</th> 
   <th>Objet d’approbation</th> 
   <th>Modifier le processus d’approbation de l’objet ou de la zone</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Approbation du projet ou du modèle </td> 
   <td>Projet</td> 
   <td>Devient un processus d’approbation à usage unique et le statut qui lui est associé se met à jour pour correspondre à un statut similaire pour le nouveau groupe.</td> 
  </tr> 
  <tr> 
   <td>Approbation de tâche ou de tâche de modèle </td> 
   <td>Tâche</td> 
   <td>Devient un processus d’approbation à usage unique et le statut qui lui est associé se met à jour pour correspondre à un statut similaire pour le nouveau groupe.</td> 
  </tr> 
  <tr> 
   <td>Approbation de problème</td> 
   <td>Problème</td> 
   <td>Devient un processus d’approbation à usage unique et le statut qui lui est associé se met à jour pour correspondre à un statut similaire pour le nouveau groupe.</td> 
  </tr> 
  <tr> 
   <td>Zone Tâches de la zone Modifier le projet ou Modifier le modèle</td> 
   <td>Tâche</td> 
   <td> <p>Le champ Processus d’approbation par défaut de la tâche est réinitialisé sur S/O.</p> <p>Par défaut, aucun processus d’approbation n’est associé aux nouvelles tâches du projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Section Détails de la file d’attente d’un projet ou d’un modèle</td> 
   <td>Problème</td> 
   <td> <p>Le champ Processus d’approbation par défaut est réinitialisé sur S/O.</p> <p>Par défaut, aucun processus d’approbation n’est associé à de nouveaux problèmes ou demandes sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Section Rubrique de file d’attente d’un projet ou d’un modèle</td> 
   <td>Problème</td> 
   <td> <p>Le champ Processus d’approbation par défaut est réinitialisé sur S/O.</p> <p>Par défaut, aucun processus d’approbation n’est associé à de nouveaux problèmes ou demandes sur le projet.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modifier un processus d’approbation du niveau du groupe au niveau du système

Lorsqu’une personne définit l’option Groupe d’un processus d’approbation spécifique à un groupe sur « Tous les groupes », le processus d’approbation s’étend à l’ensemble du système et les événements suivants se produisent :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zone ou objet à laquelle ou auquel le processus d’approbation a été associé.</th> 
   <th>Objet d’approbation</th> 
   <th>Modifier le processus d’approbation de l’objet ou de la zone</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Approbation du projet ou du modèle </td> 
   <td>Projet</td> 
   <td>Aucune modification</td> 
  </tr> 
  <tr> 
   <td>Approbation de tâche ou de tâche de modèle </td> 
   <td>Tâche</td> 
   <td>Aucune modification</td> 
  </tr> 
  <tr> 
   <td>Approbation de problème</td> 
   <td>Problème</td> 
   <td>Aucune modification</td> 
  </tr> 
  <tr> 
   <td>Zone Tâches de la zone Modifier le projet ou Modifier le modèle</td> 
   <td>Tâche</td> 
   <td> <p>Aucun changement dans le processus d’approbation, mais il est associé par défaut à de nouvelles tâches sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Section Détails de la file d’attente d’un projet ou d’un modèle</td> 
   <td>Problème</td> 
   <td> <p>Aucune modification du processus d’approbation, mais, par défaut, il est associé à de nouveaux problèmes ou requêtes sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Section Rubrique de file d’attente d’un projet ou d’un modèle</td> 
   <td>Problème</td> 
   <td> <p>Aucune modification du processus d’approbation, mais, par défaut, il est associé à de nouveaux problèmes ou requêtes sur le projet.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modifier un processus d’approbation du niveau du système au niveau du groupe

Lorsqu’une personne modifie la disponibilité d’un processus d’approbation à l’échelle du système de « Tous les groupes » à un groupe spécifique, le processus d’approbation devient spécifique au groupe et les événements suivants se produisent :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zone ou objet à laquelle ou auquel le processus d’approbation a été associé.</th> 
   <th>Objet d’approbation</th> 
   <th>Modifier le processus d’approbation de l’objet ou de la zone</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projet, tâche, problème, modèle ou tâche de modèle appartenant au groupe du processus d’approbation</td> 
   <td> <p>Projet, tâche ou problème</p> </td> 
   <td>Aucune modification</td> 
  </tr> 
  <tr> 
   <td>Zone Tâches de la zone Modifier le projet ou Modifier le modèle pour un projet ou un modèle appartenant au groupe du processus d’approbation</td> 
   <td>Tâche</td> 
   <td> <p>Aucun changement dans le processus d’approbation, mais il est associé par défaut à de nouvelles tâches sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Section « Détails de la file d’attente » pour un projet ou un modèle appartenant au groupe du processus d’approbation</td> 
   <td>Problème</td> 
   <td> <p>Aucune modification du processus d’approbation, mais, par défaut, il est associé à de nouveaux problèmes ou requêtes sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Section « Rubrique de file d’attente » pour un projet ou un modèle appartenant au groupe du processus d’approbation</td> 
   <td>Problème</td> 
   <td> <p>Aucune modification du processus d’approbation, mais, par défaut, il est associé à de nouveaux problèmes ou requêtes sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Tâche, projet, problème, modèle ou tâche de modèle appartenant à un groupe autre que le groupe du processus d’approbation</td> 
   <td> <p>Projets</p> <p>Tâches</p> <p>Problèmes</p> </td> 
   <td>Devient un processus d’approbation à usage unique.</td> 
  </tr> 
  <tr> 
   <td>Zone « Tâches » de la zone « Modifier le projet » ou « Modifier le modèle » pour un projet ou un modèle appartenant à un groupe autre que le groupe du processus d’approbation</td> 
   <td>Tâches</td> 
   <td> <p>Le champ Processus d’approbation par défaut de la tâche est réinitialisé sur S/O.</p> <p>Par défaut, aucun processus d’approbation n’est associé à de nouvelles tâches sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Section « Détails de la file d’attente » pour un projet ou un modèle appartenant à un groupe autre que le groupe du processus d’approbation</td> 
   <td>Problèmes</td> 
   <td> <p>LLe champ Approbation par défaut est réinitialisé sur S/O.</p> <p>Par défaut, aucun processus d’approbation n’est associé à de nouveaux problèmes ou requêtes sur le projet.</p> </td> 
  </tr> 
  <tr> 
   <td>Section « Rubrique de file d’attente » pour un projet ou un modèle appartenant à un groupe autre que le groupe du processus d’approbation</td> 
   <td>Problèmes</td> 
   <td> <p>LLe champ Approbation par défaut est réinitialisé sur S/O.</p> <p>Par défaut, aucun processus d’approbation n’est associé à de nouveaux problèmes ou requêtes sur le projet.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Déplacer ou copier une tâche ou un problème vers un projet avec un groupe différent de celui du processus d’approbation

Le déplacement ou la copie d’une tâche ou d’un problème d’un projet à un autre peut modifier les processus d’approbation existants sur la tâche ou le problème en fonction des groupes des deux projets. Le tableau suivant illustre les scénarios qui peuvent exister :

| Processus d’approbation de la tâche ou du problème d’origine | Groupes des deux projets | Modifications du processus d’approbation après le déplacement de la tâche ou du problème vers un autre projet |
|---|---|---|
| Processus d’approbation à usage unique associé à un statut à l’échelle du système | Les projets se trouvent dans le même groupe ou dans des groupes différents. | Aucune modification |
| Processus d’approbation à usage unique associé à un statut spécifique à un groupe | Les projets se trouvent dans différents groupes. | L’approbation reste un processus d’approbation à usage unique et le statut associé aux mises à jour de l’approbation correspond à un statut similaire pour le nouveau groupe. |
| Processus d’approbation à l’échelle du système | Les projets se trouvent dans le même groupe ou dans des groupes différents. | Aucune modification |
| Processus d’approbation à l’échelle du groupe | Les projets se trouvent dans le même groupe. | Aucune modification |
| Processus d’approbation à l’échelle du groupe | Les projets se trouvent dans différents groupes et chaque groupe a un statut différent spécifique au groupe. | L’approbation devient un processus d’approbation à usage unique et le statut associé aux mises à jour de l’approbation correspond à un statut similaire pour le nouveau groupe. |
| Processus d’approbation à l’échelle du groupe | Les projets se trouvent dans des groupes différents et il existe un statut avec la même clé dans le nouveau groupe que le statut associé au processus d’approbation du premier groupe. | Aucune modification |
