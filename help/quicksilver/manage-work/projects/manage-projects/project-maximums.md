---
title: Présentation des limites du projet
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront a des limites quant au nombre d’objets pouvant être associés à un projet. Des limites de projet sont en place pour améliorer les performances du produit et améliorer votre expérience avec Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/t6tfn132hAQe--u8g73CAFAfrJTf2qFi7yOhm4flP58
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 458
ht-degree: 89%

---

# Vue d’ensemble des limites du projet

Adobe Workfront a des limites quant au nombre d’objets pouvant être associés à un projet. Des limites de projet sont en place pour améliorer les performances du produit et améliorer votre expérience avec Workfront.

Les objets associés aux projets suivants ont les limites suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Tâches</p></td> 
   <td>  <p>Le nombre maximal de tâches par projet est de 5 000. Un message d’avertissement s’affiche lorsque le nombre de tâches approche ce maximum. Lorsque le maximum est atteint, un message d’erreur s’affiche et des tâches supplémentaires ne peuvent pas être ajoutées au projet.</p> <p>Pour éviter d’atteindre ce maximum, déplacez les tâches fermées vers un autre projet spécialement conçu pour les tâches fermées. Il se peut que les rapports sur ces projets doivent être ajustés.</p>

<b>IMPORTANT</b>

Pour les projets pour lesquels les tâches comportent de nombreuses dépendances, une dégradation des performances peut survenir lors du calcul de la chronologie ou lorsque vous travaillez dans le projet.

C’est pourquoi il est recommandé que le nombre de tâches dans les projets avec des dépendances complexes soit bien inférieur au nombre maximum de 5 000 tâches autorisé.

Voici quelques exemples de dépendances de tâches pouvant influencer ou empêcher de recalculer la chronologie du projet :

<ul><li>Nombre d’enfants</li>
   <li>Mise en retrait de plusieurs niveaux de tâches</li>
   <li>Nombre de tâches antérieures</li>
   <li>Affectations multiples</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Problèmes</p></td> 
   <td>  <p>Le nombre maximal de problèmes par projet est de 10 000. Un message d’avertissement s’affiche lorsque le nombre de problèmes approche ce maximum. Lorsque le maximum est atteint, un message d’erreur s’affiche et acun problème supplémentaire ne peut être ajouté au projet.</p> <p>Pour éviter d’atteindre ce maximum, déplacez les problèmes fermés vers un autre projet spécialement conçu pour les problèmes fermés. Il se peut que les rapports sur ces projets doivent être ajustés.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Durée</p></td> 
   <td> <p>La durée maximale d’un projet doit être de 15 ans pour que Workfront calcule automatiquement sa chronologie. Un message d’avertissement s’affiche lorsque la durée du projet approche le maximum. Lorsque le maximum est atteint, un message d’avertissement s’affiche et les calculs automatiques de la chronologie ne sont plus effectués.</p> <p>Les calculs automatiques de la chronologie reprendront dès que la durée d’un projet sera réduite à moins de 15 ans en ajustant les dates des tâches du projet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Calculs de la chronologie</p></td> 
   <td>Workfront n’effectue pas de calculs automatiques de la chronologie pour les projets qui n’ont pas été mis à jour dans 6 mois et ne reprendront pas avant qu’une mise à jour ne soit effectuée.<p>Pour les projets qui n’ont pas été mis à jour depuis 3 mois, Workfront effectue des calculs de la chronologie chaque semaine plutôt que la nuit.</p><p>Pour plus d’informations sur le calcul de la chronologie d’un projet, voir <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculer les chronologies d’un projet</a>. </p></td> 
  </tr> 
    <tr> 
   <td role="rowheader"><p>Convertir les objets </p></td> 
   <td>Workfront a une limite de traitement de 5 minutes lors de la conversion d’objets. Si l’objet est associé à un grand nombre de documents, il se peut qu’il ne puisse pas être converti dans la limite de 5 minutes. Vous devrez peut-être supprimer certains des documents, puis réessayer.</td> 
  </tr> 
 </tbody> 
</table>

<!--
 Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->
