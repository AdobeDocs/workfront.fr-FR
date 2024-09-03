---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Présentation des états du projet système
description: Workfront dispose de neuf statuts de projet système intégrés. Les trois premiers du tableau ci-dessous sont obligatoires, ce qui signifie que vous pouvez les déverrouiller, les renommer et les réorganiser, mais vous ne pouvez ni les masquer ni les supprimer. La modification du statut d’un projet se fait généralement manuellement. Cependant, il peut arriver qu’un statut de projet soit modifié automatiquement, en fonction d’autres activités qui se produisent dans le système.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '1607'
ht-degree: 99%

---

# Vue d’ensemble des statuts des projets du système

<!--Audited: 12/2023-->

Workfront dispose de neuf statuts de projet système intégrés.

Les trois premiers du tableau ci-dessous sont obligatoires, ce qui signifie que vous pouvez les déverrouiller, les renommer et les réorganiser, mais vous ne pouvez ni les masquer ni les supprimer.

La modification du statut d’un projet se fait généralement manuellement. Cependant, dans certains scénarios décrits dans la liste suivante, un statut de projet est modifié automatiquement, en fonction d’autres activités qui se produisent dans le système.

Workfront fournit les statuts de projet suivants avec votre instance Adobe Workfront :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>Statut du projet système</th> 
   <th>Ce statut de projet se produit lorsque</th> 
   <th>Ce qui se passe dans ce statut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planification (statut obligatoire)</td> 
   <td> <p>La personne responsable du projet planifie le calendrier du projet, l’affectation des tâches et les approbations. Elle définit manuellement ce statut sur un projet.</p> <p><b>CONSEIL</p> <p> Nous vous recommandons de définir le statut par défaut pour les nouveaux projets dans Workfront sur Planification. En tant qu’administrateur ou administratrice Workfront, vous pouvez modifier le statut par défaut de tous vos nouveaux projets dans la zone Projets des préférences du projet.</p> <p>Pour plus d’informations, voir la section <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Configurer des préférences de projet à l’échelle du système</a>.</p></td> 
   <td> <p>Les personnes membres de l’équipe du projet peuvent voir le projet dans leurs listes de projets par défaut (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet ne figurent pas dans leur liste de travail. Seuls les approbations et les éléments de travail acceptés s’affichent dans la liste de travail de l’accueil.</p> <p>Aucune notification n’est envoyée lorsqu’un projet présente ce statut.</p> <p>Nous vous recommandons d’apporter toutes les modifications qui peuvent déclencher une mise à jour du journal du projet, ou toute modification des tâches et des affectations de problèmes lorsque le projet a le statut de planification. Cela réduit le nombre de notifications que les personnes reçoivent.</p> <p>Le journal du projet n’est pas calculé automatiquement par le système.</p> </td> 
  </tr> 
  <tr> 
   <td>Actuel (statut obligatoire)</td> 
   <td> <p>Les personnes travaillent sur des tâches et des problèmes du projet. La personne responsable du projet doit attribuer le statut Actuel à un projet pour signaler qu’il a commencé.</p> <p>Il s’agit du statut par défaut des nouveaux projets dans Workfront.</p> <p><b>CONSEIL</b></p>

<p> En tant qu’administrateur ou administratrice Workfront, vous pouvez modifier le statut par défaut des nouveaux projets dans la zone Projets des préférences du projet. Pour plus d’informations, voir la section <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurer les préférences des projets à l’échelle du système</a>.</p> </td> 
   <td> <p>Les personnes membres de l’équipe du projet peuvent voir le projet dans leurs listes de projets par défaut (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet sont indiqués sur leur liste de travail. Elles peuvent commencer à accepter du travail relatif aux tâches et aux problèmes et les déplacer vers leur liste Travaille sur.</p> <p>Dans un projet en cours, toutes les notifications relatives aux modifications de journal, aux affectations, aux actions nécessaires et aux approbations sont envoyées aux personnes membres de l’équipe de projet.</p> <p>Le journal du projet est calculé automatiquement par le système, si le type de mise à jour est défini sur Automatique, En cas de modification ou Automatique et En cas de modification.</p> <p><b>CONSEIL</b></p> <p> Il est conseillé de limiter autant que possible les ajustements du plan de projet lorsqu’un projet a ce statut, afin que les personnes ne reçoivent pas trop de notifications.</p> </td> 
  </tr> 
  <tr> 
   <td>Terminée (statut obligatoire)</td> 
   <td> <p> Tous les tâches et problèmes relatifs au projet sont achevés et le projet est terminé.</p> 
     <p>Si le mode d’achèvement du projet est défini sur Manuel, la personne responsable choisit ce statut manuellement pour informer les personnes membres de l’équipe projet qu’elles doivent cesser de travailler sur le projet.</p> 
    <p>Si le mode d’achèvement du projet est défini sur Automatique, Workfront marque automatiquement le projet comme Terminé lorsque toutes les tâches et tous les problèmes du projet sont marqués comme Terminés. 
    <p><b>IMPORTANT</b> </p>
    <p>Vous ne pouvez marquer un projet comme Terminé que lorsque toutes ses tâches, tous ses problèmes et toutes ses approbations sont résolus.</p> </td> 
   <td>
    <p>Les utilisateurs et utilisatrices de l’équipe de projet ne peuvent pas voir le projet dans leurs listes de projets par défaut (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet ne sont pas pris en compte dans leurs demandes de travail ou leurs listes Travaille sur. </p>
    <p>Toutes les notifications relatives au projet, à l’exception d’une notification de changement de statut, cessent d’être envoyées aux utilisateurs et utilisatrices de l’équipe de projet.</p>
    <p>La chronologie du projet n’est plus calculée par le système. </p>
    <p>Le projet ne peut pas être copié.</p>
    <p>Vous pouvez empêcher les utilisateurs et utilisatrices d’effectuer des actions supplémentaires lorsqu’un projet est marqué comme terminé. </p><p>Pour plus d’informations sur la manière de limiter les actions sur les projets marqués comme terminés, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurer les préférences des projets à l’échelle du système</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Immobilisé</td> 
   <td>Le projet n’est pas encore terminé, mais en raison d’obstacles ou d’un changement de portée, il ne peut pas continuer et a été abandonné. La personne gestionnaire de projet fait passer le statut à « Immobilisé » pour avertir les utilisateurs et utilisatrices de l’équipe de projet que ce projet ne sera jamais terminé et qu’ils ne doivent plus travailler dessus.</td> 
   <td> <p>Les utilisateurs et utilisatrices de l’équipe de projet ne peuvent pas voir le projet dans leurs listes de projets par défaut (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont attribués dans le cadre du projet disparaissent de leur liste de travail.</p> <p>Les décisions d’approbation ne peuvent pas être accordées aux tâches ou aux problèmes.</p> <p>Les notifications concernant les changements de chronologie, les affectations, les actions nécessaires et les approbations ne sont pas envoyées aux utilisateurs et utilisatrices de l’équipe de projet.</p> <p>La chronologie du projet n’est pas calculée automatiquement par le système, car le projet est perçu comme étant terminé.</p> <p>Vous pouvez empêcher les utilisateurs et utilisatrices d’effectuer certaines actions lorsqu’un projet est marqué comme immobilisé. Pour plus d’informations sur la manière de limiter les actions sur les projets immobilisés, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurer les préférences des projets à l’échelle du système</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Suspendu</td> 
   <td>Le projet n’est pas encore terminé, mais en raison de certains retards, il doit être temporairement suspendu. La personne gestionnaire de projet choisit d’utiliser ce statut pour avertir les utilisateurs et utilisatrices de l’équipe de projet qu’ils doivent cesser de travailler sur le projet à l’heure actuelle.</td> 
   <td> <p>Les utilisateurs et utilisatrices de l’équipe de projet ne peuvent pas voir le projet dans leurs listes de projets par défaut (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont attribués dans le cadre du projet disparaissent de leur liste de travail. </p> <p>Les décisions d’approbation ne peuvent pas être accordées aux tâches ou aux problèmes.</p> <p>Les notifications concernant les changements de chronologie, les affectations, les actions nécessaires et les approbations ne sont pas envoyées aux utilisateurs et utilisatrices de l’équipe de projet.</p> <p> <p><b>NOTE</b></p>  <p>Lorsque vous marqué un projet comme Suspendu, la chronologie du projet ne s’arrête pas. Le projet peut toujours apparaître comme étant En danger ou En difficulté même si personne ne travaille activement sur le projet. Il peut être nécessaire d’ajuster manuellement les dates des tâches ouvertes restantes lorsque le projet redevient Actuel, afin que le projet puisse afficher un état de progression actualisé.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Demandé</td> 
   <td>Le statut du projet est automatiquement marqué comme Demandé par le système, lorsque le business case d’une demande de projet a été complété et soumis pour approbation. Pour plus d’informations sur la demande d’un projet à l’aide d’un business case, voir <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Réviser les projets demandés</a>.</td> 
   <td> <p>Les utilisateurs et utilisatrices de l’équipe de projet ne peuvent pas voir le projet dans leurs listes de projets par défaut (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes du projet qui leur sont attribués n’apparaissent pas dans leur liste de travail.</p> <p>Les notifications relatives au projet, à l’exception d’une notification de changement de statut, ne sont envoyées à personne.</p> <p>Le journal du projet n’est pas calculé automatiquement par le système.</p> </td> 
  </tr> 
  <tr> 
   <td>Approuvé</td> 
   <td>Le statut du projet est automatiquement marqué comme Approuvé lorsque le business case d’une demande de projet a été approuvé. Pour plus d’informations sur la demande d’un projet à l’aide d’un business case, voir <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Réviser les projets demandés</a>.</td> 
   <td> <p>Les personnes membres de l’équipe du projet peuvent voir le projet dans leurs listes de projets par défaut (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet ne figurent pas dans leur liste de travail.</p> <p>Les notifications relatives au projet, à l’exception d’une notification de changement de statut, ne sont envoyées à personne.</p> <p>Le journal du projet n’est pas calculé automatiquement par le système. </p> </td> 
  </tr> 
  <tr> 
   <td>Rejeté</td> 
   <td>Le statut du projet est automatiquement marqué comme Rejeté lorsque le business case d’une demande de projet a été rejeté. Pour plus d’informations sur la demande d’un projet à l’aide d’un business case, voir <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Réviser les projets demandés</a>.</td> 
   <td> <p>Les utilisateurs et utilisatrices de l’équipe de projet ne peuvent pas voir le projet dans leurs listes de projets par défaut (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet ne figurent pas dans leur liste de travail.</p> <p>Les notifications relatives au projet, à l’exception d’une notification de changement de statut, ne sont envoyées à personne.</p> <p>Le journal du projet n’est pas calculé automatiquement par le système.</p> </td> 
  </tr> 
  <tr> 
   <td>Idée</td> 
   <td>Le statut du projet est automatiquement marqué comme Idée lorsque vous soumettez une demande de projet, avant que vous ne finissiez le business case. Pour plus d’informations sur la demande d’un projet à l’aide d’un business case, voir <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Réviser les projets demandés</a>.</td> 
   <td> <p>Les utilisateurs et utilisatrices de l’équipe de projet ne peuvent pas voir le projet dans leurs listes de projets par défaut (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet ne figurent pas dans leur liste de travail.</p> <p>Les notifications relatives au projet, à l’exception d’une notification de changement de statut, ne sont envoyées à personne.</p> <p>Le journal du projet n’est pas calculé automatiquement par le système.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Les statuts de projet suivants ne peuvent pas être modifiés au statut Immobilisé, Suspendu ou Terminé :
>
>* Demandé
>* Idée
>* Approuvé
>* Rejeté (ou son équivalent)
>
