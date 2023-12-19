---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Aperçu des états du projet système
description: Workfront dispose de 9 statuts de projet système intégrés. Les 3 premiers du tableau ci-dessous sont obligatoires, ce qui signifie que vous pouvez les déverrouiller, les renommer et les réorganiser, mais vous ne pouvez pas les masquer ni les supprimer. La modification de l’état d’un projet est généralement un processus manuel. Cependant, il arrive parfois qu’un état de projet soit modifié automatiquement, en fonction d’autres activités qui se produisent dans le système.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '1607'
ht-degree: 0%

---

# Aperçu des états du projet système

Workfront dispose de 9 statuts de projet système intégrés.

Les 3 premiers du tableau ci-dessous sont obligatoires, ce qui signifie que vous pouvez les déverrouiller, les renommer et les réorganiser, mais vous ne pouvez pas les masquer ni les supprimer.

La modification de l’état d’un projet est généralement un processus manuel. Cependant, certains scénarios sont décrits dans la liste suivante lorsqu’un état de projet est modifié automatiquement, selon d’autres activités qui se produisent dans le système.

Workfront fournit les états de projet suivants avec votre instance Adobe Workfront :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>État du projet système</th> 
   <th>Cet état de projet se produit lorsque</th> 
   <th>Que se passe-t-il dans cet état ?</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planification (état requis)</td> 
   <td> <p>Le chef de projet planifie le calendrier du projet, l’attribution des tâches et les validations. Le chef de projet définit manuellement cet état sur un projet.</p> <p><b>CONSEIL</p> <p> Nous vous recommandons de définir l’état par défaut pour les nouveaux projets dans Workfront sur Planification. En tant qu’administrateur Workfront, vous pouvez modifier l’état par défaut de tous vos nouveaux projets dans la zone Projets des préférences du projet.</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Configuration des préférences de projet à l’échelle du système</a>.</p></td> 
   <td> <p>Par défaut, les utilisateurs de l’équipe de projet peuvent voir le projet dans la liste Projets (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet ne figurent pas dans leur liste de tâches. Seules les validations et les tâches acceptées s’affichent dans la liste de tâches à domicile.</p> <p>Aucune notification n’est envoyée lorsqu’un projet a cet état.</p> <p>Nous vous recommandons d’effectuer toutes les modifications qui peuvent déclencher une mise à jour de la chronologie du projet, ou toute modification des tâches et des affectations de problèmes lorsque le projet est en état Planification . Cela réduit le nombre de notifications que les utilisateurs reçoivent.</p> <p>La chronologie du projet n’est pas calculée automatiquement par le système.</p> </td> 
  </tr> 
  <tr> 
   <td>Actuel (état requis)</td> 
   <td> <p>Les utilisateurs travaillent sur les tâches et les problèmes du projet. Le chef de projet doit changer un projet en actuel pour signaler qu’il a commencé.</p> <p>Il s’agit de l’état par défaut des nouveaux projets dans Workfront.</p> <p><b>CONSEIL</b></p>

<p> En tant qu’administrateur Workfront, vous pouvez modifier l’état par défaut des nouveaux projets dans la zone Projets des préférences du projet. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p> </td> 
   <td> <p>Par défaut, les utilisateurs de l’équipe de projet peuvent voir le projet dans la liste Projets (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont assignés sur le projet renseignent leur liste de tâches. Ils peuvent commencer à accepter les tâches et les problèmes et les déplacer vers leur liste de tâches.</p> <p>Dans un projet en cours, toutes les notifications relatives aux modifications de la chronologie, aux affectations, aux actions nécessaires et aux approbations sont envoyées aux utilisateurs de l’équipe du projet.</p> <p>La chronologie du projet est calculée automatiquement par le système, si le type de mise à jour du projet est défini sur Automatique, Sur changement ou Automatique et Sur changement.</p> <p><b>CONSEIL</b></p> <p> Il est conseillé de ne pas alourdir au minimum les ajustements des plans de projet lorsqu’un projet est dans cet état afin que les utilisateurs ne reçoivent pas trop de notifications.</p> </td> 
  </tr> 
  <tr> 
   <td>Terminé (état requis)</td> 
   <td> <p> Toutes les tâches et tous les problèmes du projet sont terminés et le projet est terminé.</p> 
     <p>Si le mode d’achèvement du projet est défini sur Manuel, le chef de projet choisit ce statut manuellement pour informer les utilisateurs de l’équipe du projet de cesser de travailler sur le projet.</p> 
    <p>Si le mode d’achèvement du projet est défini sur Automatique, Workfront marque automatiquement un projet comme terminé lorsque toutes les tâches et tous les problèmes du projet sont marqués comme Terminé. 
    <p><b>IMPORTANT</b> </p>
    <p>Vous pouvez marquer un projet comme terminé uniquement lorsque toutes les tâches, problèmes et approbations du projet sont résolus.</p> </td> 
   <td>
    <p>Par défaut, les utilisateurs de l’équipe de projet ne peuvent pas voir le projet dans la liste Projets (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet ne sont pas renseignés dans les listes Requêtes de travail ou Travail sur . </p>
    <p>Toutes les notifications liées au projet, à l’exception d’une notification de changement d’état, cessent d’être envoyées aux utilisateurs de l’équipe du projet.</p>
    <p>La chronologie du projet n’est plus calculée par le système. </p>
    <p>Le projet ne peut pas être copié.</p>
    <p>Vous pouvez empêcher les utilisateurs d’effectuer d’autres actions lorsqu’un projet est marqué comme terminé. </p><p>Pour plus d’informations sur la manière de restreindre les actions sur les projets marqués comme terminés, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Immobilisé</td> 
   <td>Le projet n'est pas encore terminé, mais en raison de barrages routiers ou de changements de portée, le projet ne peut pas continuer à être traité et a été abandonné. Le chef de projet passe alors à l’état Mort pour informer les utilisateurs de l’équipe de projet que ce projet ne se terminera jamais et qu’ils ne devraient plus y travailler.</td> 
   <td> <p>Par défaut, les utilisateurs de l’équipe de projet ne peuvent pas voir le projet dans la liste Projets (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet disparaissent de leur liste de tâches.</p> <p>Les décisions de validation ne peuvent pas être accordées à des tâches ou des problèmes.</p> <p>Les notifications relatives aux modifications de la chronologie, aux affectations, aux actions nécessaires et aux approbations ne sont pas envoyées aux utilisateurs de l’équipe de projet.</p> <p>La chronologie du projet n’est pas calculée automatiquement par le système, car le projet est perçu comme étant terminé.</p> <p>Vous pouvez empêcher les utilisateurs d’effectuer certaines actions lorsqu’un projet est marqué comme mort. Pour plus d’informations sur la manière de restreindre les actions sur les projets inactifs, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configuration des préférences de projet à l’échelle du système</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Suspendu</td> 
   <td>Le projet n'est pas encore terminé, mais en raison de certains délais, le projet doit être temporairement suspendu. Le chef de projet choisit d’utiliser cet état pour avertir les utilisateurs de l’équipe de projet de ne plus travailler sur le projet, à l’heure actuelle.</td> 
   <td> <p>Par défaut, les utilisateurs de l’équipe de projet ne peuvent pas voir le projet dans la liste Projets (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet disparaissent de leur liste de tâches. </p> <p>Les décisions de validation ne peuvent pas être accordées à des tâches ou des problèmes.</p> <p>Les notifications relatives aux modifications de la chronologie, aux affectations, aux actions nécessaires et aux approbations ne sont pas envoyées aux utilisateurs de l’équipe de projet.</p> <p> <p><b>NOTE</b></p>  <p>Lorsque vous placez un projet En attente, la chronologie du projet ne s’arrête pas. Le projet peut toujours être présenté comme En danger ou En danger même si personne ne travaille activement sur le projet. Certains réglages manuels des dates des tâches restantes en cours peuvent être nécessaires lors de la réactivation du projet sur Actuel, de sorte que le projet puisse afficher la progression mise à jour.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Demandé</td> 
   <td>Le statut du projet est automatiquement marqué comme Demandé par le système, lorsque l’analyse de cas d’une demande de projet est terminée et soumise à approbation. Pour plus d’informations sur la demande d’un projet à l’aide d’une analyse de cas, voir <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Révision des projets demandés</a>.</td> 
   <td> <p>Par défaut, les utilisateurs de l’équipe de projet ne peuvent pas voir le projet dans la liste Projets (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes du projet qui leur sont assignés ne sont pas renseignés dans leur liste de tâches.</p> <p>Toutes les notifications liées au projet, à l’exception d’une notification de changement d’état, ne sont envoyées à aucun utilisateur.</p> <p>La chronologie du projet n’est pas calculée automatiquement par le système.</p> </td> 
  </tr> 
  <tr> 
   <td>Approuvé</td> 
   <td>Le statut du projet est automatiquement marqué comme Approuvé lorsque le dossier commercial d’une demande de projet a été approuvé. Pour plus d’informations sur la demande d’un projet à l’aide d’une analyse de cas, voir <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Révision des projets demandés</a>.</td> 
   <td> <p>Par défaut, les utilisateurs de l’équipe de projet peuvent voir le projet dans la liste Projets (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet ne figurent pas dans leur liste de tâches.</p> <p>Toutes les notifications liées au projet, à l’exception d’une notification de changement d’état, ne sont envoyées à aucun utilisateur.</p> <p>La chronologie du projet n’est pas calculée automatiquement par le système. </p> </td> 
  </tr> 
  <tr> 
   <td>Rejeté</td> 
   <td>Le statut du projet est automatiquement marqué comme Refusé lorsque l’analyse de cas sur une demande de projet a été rejetée. Pour plus d’informations sur la demande d’un projet à l’aide d’une analyse de cas, voir <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Révision des projets demandés</a>.</td> 
   <td> <p>Par défaut, les utilisateurs de l’équipe de projet ne peuvent pas voir le projet dans la liste Projets (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet ne figurent pas dans leur liste de tâches.</p> <p>Toutes les notifications liées au projet, à l’exception d’une notification de changement d’état, ne sont envoyées à aucun utilisateur.</p> <p>La chronologie du projet n’est pas calculée automatiquement par le système.</p> </td> 
  </tr> 
  <tr> 
   <td>Idée</td> 
   <td>Le statut du projet est automatiquement marqué comme Idée lorsque vous soumettez une demande de projet, avant de terminer l’analyse de cas. Pour plus d’informations sur la demande d’un projet à l’aide d’une analyse de cas, voir <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Révision des projets demandés</a>.</td> 
   <td> <p>Par défaut, les utilisateurs de l’équipe de projet ne peuvent pas voir le projet dans la liste Projets (sans filtre personnalisé), dans la zone Projets de Workfront. Les tâches et les problèmes qui leur sont affectés sur le projet ne figurent pas dans leur liste de tâches.</p> <p>Toutes les notifications liées au projet, à l’exception d’une notification de changement d’état, ne sont envoyées à aucun utilisateur.</p> <p>La chronologie du projet n’est pas calculée automatiquement par le système.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Les états de projet suivants ne peuvent pas être modifiés en état Mort, En attente ou Terminé :
>
>* Demandé
>* Idée
>* Approuvé
>* Refusé (ou son équivalent)
>
