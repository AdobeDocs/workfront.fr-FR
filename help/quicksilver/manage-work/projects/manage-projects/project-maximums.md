---
title: Présentation des limites du projet
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront a des limites quant au nombre d’objets pouvant être associés à un projet. Des limites de projet sont en place pour améliorer les performances du produit et améliorer votre expérience avec Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 809f1c3629c343a55305c0c617f4974dc05439bf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Présentation des limites du projet

Adobe Workfront a des limites quant au nombre d’objets pouvant être associés à un projet. Des limites de projet sont en place pour améliorer les performances du produit et améliorer votre expérience avec Workfront.

Les objets associés aux projets suivants ont les limites suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Tâches</p></td> 
   <td>  <p>Le nombre maximal de tâches par projet est de 5 000. Un message d’avertissement s’affiche lorsque le nombre de tâches approche ce maximum. Lorsque le maximum est atteint, un message d’erreur s’affiche et des tâches supplémentaires ne peuvent pas être ajoutées au projet.</p> <p>Pour éviter d’atteindre ce maximum, déplacez les tâches qui sont fermées vers un autre projet désigné pour les tâches fermées. Il se peut que les rapports sur ces projets doivent être ajustés.</p>

<b>IMPORTANT</b>

Pour les projets pour lesquels les tâches comportent de nombreuses dépendances, nous recommandons que le nombre de tâches dans les projets soit beaucoup plus faible que le nombre maximum de 5 000 tâches autorisé.

Voici quelques exemples de dépendances de tâches pouvant influencer ou empêcher de recalculer la chronologie du projet :

<ul><li>Nombre d'enfants</li>
   <li>Mise en retrait de plusieurs niveaux de tâche</li>
   <li>Nombre de prédécesseurs</li>
   <li>Affectations multiples</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Événements</p></td> 
   <td>  <p>Le nombre maximal de problèmes par projet est de 10 000. Un message d’avertissement s’affiche lorsque le nombre de problèmes approche ce nombre maximum. Lorsque le maximum est atteint, un message d’erreur s’affiche et des problèmes supplémentaires ne peuvent pas être ajoutés au projet.</p> <p>Pour éviter d’atteindre ce maximum, déplacez les problèmes qui sont fermés vers un autre projet désigné pour les problèmes fermés. Il se peut que les rapports sur ces projets doivent être ajustés.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Durée</p></td> 
   <td> <p>La durée maximale d’un projet doit être de 15 ans pour que Workfront calcule automatiquement sa chronologie. Un message d’avertissement s’affiche lorsque la durée du projet approche le maximum. Lorsque le maximum est atteint, un message d’avertissement s’affiche et les calculs automatiques de la chronologie ne sont plus effectués.</p> <p>Les calculs automatiques de la chronologie reprendront dès que la durée d’un projet sera réduite à moins de 15 ans en ajustant les dates des tâches du projet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Calculs chronologiques</p></td> 
   <td>Workfront n’effectue pas de calculs de chronologie automatique pour les projets qui n’ont pas été mis à jour dans 6 mois et ne reprendront pas avant qu’une mise à jour ne soit effectuée.<p>Pour les projets qui n’ont pas été mis à jour depuis 3 mois, Workfront effectue des calculs de chronologie chaque semaine plutôt que la nuit.</p><p>Pour plus d’informations sur le calcul de la chronologie du projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculer les calendriers du projet</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->