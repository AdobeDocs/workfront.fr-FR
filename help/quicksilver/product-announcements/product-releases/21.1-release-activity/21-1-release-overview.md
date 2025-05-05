---
content-type: release-notes
keywords: notes,trimestrielle,mise à jour
navigation-topic: product-releases
title: Vue d’ensemble de la version 21.1
description: La version 21.1 a été mise à disposition dans l’environnement de production pendant la semaine du .
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 3affee76-347e-4610-b255-4b1bb4414c5d
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3659'
ht-degree: 99%

---

# Vue d’ensemble de la version 21.1

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 21.1 release was made available in the Production environment the week of .</p>
-->

Cette page fournit des informations sur les fonctionnalités d’Adobe Workfront Classic et de la nouvelle expérience Adobe Workfront incluse dans la version 21.1.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

Avec cette version, nous proposons de nouvelles fonctionnalités et améliorations qui vous aideront à prendre une longueur d’avance pour le grand retour de 2021 avec des stratégies adaptables, des processus de travail automatisés et une infrastructure numérique connectée pour garantir le succès de l’entreprise.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 21.1 release nears its planned Production release, this page will be updated with all functionality included with 21.1.</p>
-->

Ces améliorations sont actuellement disponibles

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the Preview environment and will be made available
</MadCap:conditionalText>
-->

dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the first quarter of 2021
</MadCap:conditionalText>
-->

Elles ont été publiées la semaine du 15 février 2021.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.workfront.com/" target="_blank">Adobe Workfront Status Site</a>.
</MadCap:conditionalText>
-->

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées à l’administration](#administrator-enhancements)
* [Améliorations de la gestion des ressources](#resource-management-enhancements)
* [Améliorations de la gestion de projets](#project-management-enhancements)
* [Améliorations apportées à Analytique améliorée](#enhanced-analytics-improvements)
* [Améliorations de l’intégration](#integration-enhancements)
* [Améliorations apportées à l’application mobile](#mobile-enhancements)
* [Autres améliorations](#other-enhancements)

### Améliorations apportées aux administrateurs et administratrices {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Ajout d’un nouveau paramètre Niveau d’accès pour la copie de projets</a> </p> <p>Pour vous donner plus de contrôle, en tant qu’administrateur ou administratrice système, sur ce que les planificateurs et planificatrices peuvent faire avec un projet, nous avons rendu plus granulaire l’accès Modifier aux projets du niveau d’accès, en introduisant un nouveau paramètre qui vous permet d’activer ou de désactiver leur capacité à copier des projets. Avant cette modification, lorsque vous avez activé l’accès des utilisateurs et utilisatrices à l’option Modifier des projets, l’accès à la copie était automatique. Grâce à la nouvelle fonctionnalité, vous pouvez donner à une personne l’accès pour modifier des projets sans nécessairement lui accorder l’accès à les copier en désactivant le nouveau paramètre Copier.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#in" class="MCXref xref" xrefformat="{para}">Dans un formulaire personnalisé sur un objet, sélectionnez tous les éléments d’un champ déroulant à sélection multiple.</a> </p> <p>Sur la page Détails d’un objet, lorsque vous remplissez un champ déroulant à sélection multiple sur un formulaire personnalisé, vous pouvez cliquer sur Sélectionner tout si vous devez sélectionner toutes les options disponibles.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Non disponible actuellement lorsque vous soumettez une nouvelle demande.)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#recalcul" class="MCXref xref" xrefformat="{para}">Recalculer tous les champs de formulaire personnalisé d’un objet</a> </p> <p>Il est désormais plus facile de s’assurer que toutes les données des champs personnalisés calculés sont à jour pour un objet. Une nouvelle option de menu Recalculer les expressions permet de recalculer rapidement toutes les données de ces champs.</p> <p>Cela s’avère particulièrement utile lorsqu’une personne modifie des données dans un autre objet référencé par un champ personnalisé calculé de votre objet.</p> <p>Auparavant, les utilisateurs et utilisatrices devaient utiliser des solutions de contournement pour s’assurer que toutes les données des champs personnalisés calculés étaient à jour. Par exemple, il fallait modifié l’objet avec d’autres objets pour utiliser l’option de recalcul disponible pour la modification en masse.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 10 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#unlock" class="MCXref xref" xrefformat="{para}">Déverrouiller les préférences pour les tâches et les problèmes pour les administrateurs et administratrices de groupe</a> </p> <p>Les administrateurs et administratrices Workfront peuvent désormais accorder aux administrateurs et administratrices de groupe une plus grande autonomie en déverrouillant les préférences individuelles en matière de tâches et de problèmes. Lorsqu’une préférence est déverrouillée, les administrateurs et administratrices de groupes peuvent la configurer pour répondre aux besoins uniques et aux processus internes de chaque groupe.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 2 décembre 2020</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Avant le 24 juin 2021, cette option était disponible dans le cadre d’un déploiement échelonné uniquement pour les clientes et clients des clusters 4 et 6 et quelques autres clientes et clients. Elle est maintenant disponible en production pour tous les clientes et clients.)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configurer séparément les paramètres de niveau d’accès pour les portfolios et les programmes</a> </p> <p>Il est désormais plus facile de gérer l’accès des utilisateurs et utilisatrices aux portefeuilles et aux programmes, car vous pouvez configurer leurs paramètres de niveau d’accès séparément.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 2 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">Cocher toutes les cases d’une série lors de la modification d’informations dans un formulaire personnalisé</a> </p> <p>Sur la page Détails d’un objet, lorsque vous renseignez un champ Formulaire personnalisé contenant des cases à cocher, vous pouvez cliquer sur Sélectionner tout si vous devez cocher toutes les cases disponibles.</p> <p>Cette option s’affiche uniquement si le champ contient plus de 2 cases à cocher.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 2 décembre 2020</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Non disponible actuellement lors de l’envoi d’une demande.)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur2" class="MCXref xref" xrefformat="{para}">Configurer votre liste autorisée d’e-mails Workfront</a> </p> <p>Pour mieux sécuriser vos données, vous pouvez désormais utiliser une liste autorisée de domaines d’e-mail pour :</p> 
    <ul> 
     <li> <p>Contrôler la destination des e-mails de Workfront s’ils contiennent des rapports ou des documents stockés dans Workfront</p> </li> 
     <li> <p>Le contrôle des domaines de messagerie peut se faire dans l’adresse e-mail que les utilisateurs et les utilisatrices spécifient dans leurs profils.</p> </li> 
    </ul> <p>Si, par exemple, vous souhaitez protéger des données sensibles, telles qu’un rapport répertoriant votre clientèle à risque, vous pouvez n’inclure que votre ou vos domaines de messagerie interne dans la liste autorisée d’e-mails. De cette manière, les utilisateurs et les utilisatrices ne peuvent pas envoyer ce rapport (ni aucun autre rapport Workfront) à une adresse e-mail externe.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 20 novembre 2020</p> <p>Version de production : avec la version 21.1 </p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">Affecter un administrateur ou une administratrice de groupe à un sous-groupe</a> </p> <p>Pour faciliter le fonctionnement indépendant des niveaux de votre organisation, nous avons ajouté la possibilité d’affecter un administrateur ou une administratrice de groupes à un sous-groupe. Vous pouvez désormais vous assurer que vous déléguez la gestion des sous-groupes aux personnes appropriées.</p> <p>Auparavant, seul un groupe de niveau supérieur pouvait avoir des administrateurs et des administratrices de groupes qui géraient tous les sous-groupes sous le groupe de niveau supérieur.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 20 novembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#work" class="MCXref xref" xrefformat="{para}">Utiliser des projets de groupe et des processus d’approbation dans la zone Groupes</a> </p> <p>En tant qu’administrateur ou administratrice de groupes, il est désormais facile d’afficher et de travailler sur les projets et les processus d’approbation de votre groupe, car ils sont maintenant répertoriés dans la zone des groupes. </p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 20 novembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur3" class="MCXref xref" xrefformat="{para}">Configurer des notifications d’événement pour les groupes</a> <span style="color: #dc143c; font-weight: bold;">Nouveau en prévisualisation</span></p> <p>Désormais, l’équipe d’administration de Workfront peut accorder une plus grande autonomie à celle des groupes en leur permettant de configurer des notifications d’événement pour leurs groupes de niveau supérieur. Les sous-groupes héritent des configurations de notification d’événement de leur groupe parent.</p> <p>Auparavant, les notifications d’événement n’étaient configurables que par un administrateur ou un administratrice Workfront au niveau du système, ce qui signifiait que tous les groupes devaient utiliser le même jeu de notifications d’événement.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 22 janvier 2021</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Disponible initialement en production uniquement pour les clientes et clients sur le cluster 4 dans le cadre d’un déploiement échelonné ; disponible pour d’autres clusters peu de temps après.)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">Afficher le nombre de licences utilisées et attribuées dans un groupe</a> </p> <p>Pour déterminer la pertinence de la distribution de vos licences, vous pouvez désormais afficher le nombre de licences utilisées dans un groupe et dans les sous-groupes qui lui sont subordonnés.</p> <p>Si vous gérez un groupe de niveau supérieur, vous pouvez afficher le nombre de licences utilisées dans un groupe (et ses sous-groupes) et le nombre maximum de licences affectées au groupe.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 20 novembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Amélioration apportées à la gestion des ressources. {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workload" class="MCXref xref" xrefformat="{para}">Équilibreur de charge de travail pour les projets</a> </p> <p>L’équilibreur de charge de travail est désormais disponible dans un projet. Vous avez désormais la possibilité de choisir entre l’utilisation de l’équilibreur de charge de travail ou l’outil de planification pour gérer les ressources de votre projet.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 17 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Équilibreur de charge de travail disponible pour une équipe</a> </p> <p>L’équilibreur de charge de travail est désormais disponible au sein d’une équipe. Vous avez désormais la possibilité de choisir entre l’utilisation de l’équilibreur de charge de travail ou l’outil de planification pour gérer les ressources de votre équipe. </p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 20 novembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Amélioration apportées à la gestion de projets {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de version et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">Export désormais disponible dans la section Mesures d’un projet</a> </p> <p>Pour partager plus facilement le statut et la progression d’un projet, vous pouvez désormais exporter l’ensemble du tableau de bord de la section Mesures d’un projet vers un fichier .png.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 15 janvier 2021</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#update" class="MCXref xref" xrefformat="{para}">Mettre à jour à jour le pourcentage terminé d’un problème lorsque l’objet (projet ou tâche) a été converti à partir de la mise à jour du problème.</a> </p> <p>Nous avons mis à jour la façon dont le pourcentage terminé des problèmes fonctionne pour les problèmes qui ont été convertis en projets ou en tâches. Avec cette nouvelle fonctionnalité, lorsqu’un problème est converti en tâche ou en projet, le pourcentage terminé du problème est mis à jour en synchronisation avec le pourcentage terminé de la tâche ou du projet de résolution lorsque le paramètre « Mettre à jour automatiquement le statut des problèmes pouvant être résolus lorsque le statut de l’objet de résolution change » est activé dans la configuration.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#fields" class="MCXref xref" xrefformat="{para}">Champs supprimés de la page Nouvelle demande</a> </p> <p>Dans le cadre de la refonte de la page Nouvelle demande, nous avons mis à jour les champs Nouveau problème qui sont configurés dans la section Configuration de la file d’attente d’un projet.</p> <p>Les différents champs Nouveau problème ne s’affichent que lors de la création d’un problème à partir de la section Problèmes du projet. Ils ne s’affichent pas lors de la soumission d’un problème à l’aide d’une file d’attente des demandes dans la zone Demandes.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Retiré de la version)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de la soumission de demandes dans la zone Demandes</a> </p> <p>Afin d’assurer la cohérence avec la nouvelle expérience Workfront et d’améliorer l’efficacité de la soumission des demandes, nous avons repensé la zone Nouvelle demande dans la zone Demandes.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Retiré de la version ; restera dans la version préliminaire et passera en production avec la version 21.2.)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Partager un lien vers une file d’attente des demandes lors de la soumission d’une demande</a> </p> <p>Il est désormais possible de partager un lien vers une file d’attente des demandes, un groupe de rubriques ou une rubrique de file d’attente lorsque vous créez une demande.</p> <p>Avant de soumettre une nouvelle demande, vous pouvez copier un lien vers la file d’attente des demandes, le groupe de rubriques ou la rubrique la file d’attente de la demande et le partager avec d’autres utilisateurs et utilisatrices, ou l’incorporer dans un tableau de bord.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Retiré de la version ; restera dans la version préliminaire et passera en production avec la version 21.2.)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Nouvelle liste Demandes soumises</a> </p> <p>Pour vous permettre de gérer vos demandes soumises de manière plus simple et plus cohérente, nous avons supprimé les sections Demandes que j’ai envoyées et Toutes les demandes dans la zone Demandes et les avons remplacées par une nouvelle liste Demandes soumises. La liste a un aspect familier qui correspond à toutes les autres listes du système, ce qui vous permet de filtrer les différentes catégories de demandes soumises et de rechercher rapidement une demande qui pourrait être difficile à trouver.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 2 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#search" class="MCXref xref" xrefformat="{para}">Rechercher un groupe que vous souhaitez affecter à un projet et afficher ses détails</a> </p> <p>Il est désormais plus facile de s’assurer que vous identifiez le bon groupe lorsque vous assignez un groupe à un projet. Pointez sur le nom d’un groupe que vous trouvez dans la case Groupe, puis cliquez sur l’icône d’information qui s’affiche en regard du nom pour afficher l’infobulle Détails du groupe.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 17 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Rapport sur les nouvelles délégations d’utilisateurs et d’utilisatrices</a> </p> <p>Auparavant, les informations relatives aux délégations d’approbation de tâches, de problèmes et de projets ne pouvaient être consultées par la personne déléguée que dans sa zone d’accueil. Pour permettre à d’autres personnes de consulter ces informations, les utilisateurs et utilisatrices du Plan peuvent désormais créer le rapport de délégation d’utilisateurs et d’utilisatrices, qui vous donne les informations suivantes :</p> 
    <ul> 
     <li> <p>La personne qui a délégué ces approbations à une autre personne.</p> </li> 
     <li> <p>La personne qui s’est vue déléguer ces approbations.</p> </li> 
     <li> <p>Les dates de début et de fin de ces délégations.</p> </li> 
    </ul> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 17 décembre 2020</p> <p>Version de production : 21 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations apportées à l’analytique améliorée {#enhanced-analytics-improvements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates des versions et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#people" class="MCXref xref" xrefformat="{para}">La page « Personnes » est désormais disponible pour tous les clusters</a> </p> <p>La page Personnes est désormais disponible sur Workfront Classic pour le Cluster 4. Cette page comprend les graphiques de l’activité par équipe, de la capacité des ressources et de la capacité de l’équipe.</p> <p>Cette page était auparavant disponible avec la version 20.3 de Workfront Classic et de la nouvelle expérience Workfront pour tous les autres clusters.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 28 janvier 2021</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront (disponible précédemment)</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#enhanced" class="MCXref xref" xrefformat="{para}">L’analytique améliorée s’affiche désormais par défaut.</a> </p> <p>Remarque : cette modification ne s’applique qu’aux personnes nouvellement ajoutées aux modèles de mise en page. Les utilisateurs et utilisatrices affectés à un modèle de disposition personnalisé ne sont pas non plus affectés par cette modification.</p> <p>Dans le modèle de mise en page par défaut, la zone d’analytique est désormais activée par défaut, ce qui signifie que les personnes affectées à ce modèle de mise en page voient désormais la zone d’analytique dans la barre de navigation globale de Workfront Classic et dans le menu principal de la nouvelle expérience Workfront.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 6 novembre 2020</p> <p>Version de production : 3 décembre 2020</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#availab" class="MCXref xref" xrefformat="{para}">Analytique améliorée disponibles pour tous les clusters</a> </p> <p>Analytique améliorée est disponible pour tous les clusters Workfront, y compris les clientes et clients du Cluster 6.</p> <p>Auparavant, Analytique améliorée n’était pas disponible avec Google Cloud Platform, ce qui empêchait les clientes et clients du Cluster 6 d’accéder à la zone Analyse. Désormais, les clientes et clients Entreprises et Grands comptes de Cluster 6 peuvent accéder à la zone Analyse.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 20 novembre 2020</p> <p>Version de production : 3 décembre 2020</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations de l’intégration {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Amélioration des notifications Adobe Workfront dans Microsoft Teams</a> </p> <p>Afin de faciliter l’utilisation de Workfront par le biais de Microsoft Teams, nous avons apporté diverses améliorations aux notifications Microsoft Teams envoyées à partir de Workfront.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : S/O</p> <p>Version de production : 12 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations mobiles {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouveaux chemins de navigation dans l’application Adobe Workfront</a> </p> <p>Nous avons ajouté des chemins de navigation à l’application mobile Workfront. Désormais, vous pouvez utiliser cette fonctionnalité pour naviguer vers les éléments de travail parent au sein d’un projet.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : S/O</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#rich" class="MCXref xref" xrefformat="{para}">Prise en charge du texte enrichi dans les formulaires personnalisés de l’application Workfront</a> </p> <p>Vous pouvez désormais utiliser la mise en forme de texte enrichi dans les champs de texte des formulaires personnalisés dans l’application mobile Workfront.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : S/O</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#sso" class="MCXref xref" xrefformat="{para}">Les personnes utilisant l’authentification unique peuvent désormais se reconnecter à l’application Workfront avec la technologie de reconnaissance faciale ou d’empreinte digitale.</a> </p> <p>Si votre organisation utilise l’authentification unique, vous pouvez désormais utiliser la reconnaissance faciale ou votre empreinte digitale pour vous connecter à l’application mobile Workfront après que votre session a expiré. Vous devez cependant vous connecter avec vos identifiants d’authentification unique au départ.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : S/O</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>
--&gt;

### Autres améliorations {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Mises à jour des exigences relatives à l’échec de l’abonnement aux événements</a> </p> <p>Nous mettons à jour les exigences de désactivation progressive des échecs d’abonnement à un événement. Outre les exigences existantes, les abonnements à des événements seront désormais progressivement désactivés s’ils n’atteignent pas une diffusion réussie avant 2 000 tentatives. L’objectif est de renforcer la règle actuelle des 70 % d’échec, qui peut conduire à des quantités excessives d’échecs dans certains cas.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : S/O</p> <p>Version de production : 11 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouveaux champs d’équipe disponibles dans la synthèse quotidienne</a> </p> <p>Nous avons ajouté des champs d’approbation et d’affectation d’équipe à l’e-mail Synthèse quotidienne des actions nécessaires.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 17 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#replacin" class="MCXref xref" xrefformat="{para}">Remplacement de l’option POP dans les files d’attente des demandes</a> </p> <p>Nous remplaçons l’option d’e-mail POP pour les files d’attente des demandes par un nouveau système géré par Workfront. Vous pourrez toujours soumettre des demandes par e-mail, mais vous devrez configurer une nouvelle adresse e-mail gérée par Workfront dans la zone de la file d’attente des demandes. </p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 17 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">Limiter l’édition des heures sur les feuilles de temps</a> </p> <p>Pour mieux contrôler les feuilles de temps et la modification des heures, nous avons ajouté un paramètre qui permet de réserver la modification des heures aux personnes propriétaires de feuilles de temps et aux équipes d’administration système.</p> <p>Auparavant, les personnes dont l’option Feuilles de temps et heures était activée dans leur niveau d’accès pouvaient modifier les heures sur n’importe quelle feuille de temps.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 21 janvier 2021</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Amélioration des filtres et des vues dans la zone des feuilles de temps</a> </p> <p>Nous avons ajouté des filtres pour les projets et les problèmes, ainsi que des options d’affichage et de regroupement à la page de recherche.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 2 décembre 2020</p> <p>Version de production : 21 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#hide" class="MCXref xref" xrefformat="{para}">Masquer la case des heures supplémentaires dans les feuilles de temps</a> </p> <p>Vous pouvez désormais masquer la zone des heures supplémentaires afin d’atténuer la confusion des utilisateurs et utilisatrices si vous n’effectuez pas le suivi des heures supplémentaires dans Workfront. Vous pouvez masquer la case des heures supplémentaires pour une feuille de temps à usage unique ou dans le profil de feuille de temps.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 2 décembre 2020</p> <p>Version de production : 16 décembre 2020</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#expand" class="MCXref xref" xrefformat="{para}">Développer ou réduire les éléments dans la navigation par chemin de navigation</a> </p> <p>Pour faciliter l’affichage du chemin de navigation complet, nous avons ajouté des fonctionnalités de développement et de réduction.</p> <p>Désormais, tous les éléments tronqués sont regroupés avant le projet, avec le mot « autre(s) ». Par exemple, « 3 autres » indique qu’il existe 3 objets qui ne s’affichent pas.</p> <p>Auparavant, vous deviez cliquer sur les trois points pour afficher les objets tronqués dans un menu déroulant.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 7 janvier 2020</p> <p>Version de production : 21 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nouvel aspect de la navigation par chemin de navigation</a> </p> <p>Pour aider les personnes à mieux identifier où elles se trouvent dans Workfront et à naviguer plus facilement entre les objets, nous avons apporté plusieurs améliorations à la navigation par chemin de navigation.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version préliminaire bêta : 10 décembre 2020</p> <p>Version de production : 21 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>La nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

## Améliorations des Objectifs Workfront

La plupart des nouvelles fonctionnalités d’Objectifs Workfront seront disponibles avec la version 21.1. Pour plus d’informations sur ces nouvelles fonctionnalités disponibles en avant-première, voir [Objectifs Adobe Workfront avec la version 21.1](../../../product-announcements/product-releases/goals-release-activity/goals-release-21-1.md).

## Améliorations du planificateur de scénarios Workfront

Les nouvelles fonctionnalités du planificateur de scénarios Workfront seront disponibles avec la version 21.1. Pour plus d’informations sur ces nouvelles fonctionnalités disponibles en avant-première, voir [Planificateur de scénarios Adobe Workfront avec la version 21.1](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-1.md).

## Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent du planning de la version 21.1. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

## Améliorations de l’API

La version 12 de l’API est désormais disponible avec la version 20.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de la version 12 de l’API](https://experienceleague.adobe.com/fr/docs/workfront/using/adobe-workfront-api/api-notes/new-api-version-12).

Pour plus d’informations sur les versions de l’API, voir [Planning du contrôle de version et du support de l’API](../../../wf-api/api/api-version-support-schedule.md).

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

.

## Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la sortie de la version 21.1, voir [Mises à jour de maintenance Workfront](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Annonces

* [Nouvelles adresses IP pour les e-mails Workfront avec la version 21.1](#new-ip-addresses-for-workfront-email-with-the-21-1-release)
* [Liste d’adresses IP supplémentaires autorisées pour les abonnements aux événements](#allowlist-of-additional-ip-addresses-for-event-subscriptions)
* [Liste autorisée des domaines supplémentaires requis pour accéder à Workfront](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Obsolescence de Flash](#flash-deprecation)
* [Webinaire sur la version 21.1](#21-1-release-webinar)
* [Modification de la cadence des versions préliminaires](#change-in-preview-release-cadence)
* [Workfront One](#workfront-one)

### Nouvelles adresses IP pour les e-mails Workfront avec la version 21.1 {#new-ip-addresses-for-workfront-email-with-the-21-1-release}

Afin d’améliorer la distribution des e-mails, nous ajoutons de nouvelles adresses IP avec la version de production 21.1 pour les clusters 1, 2, 3, 4 et 5.

Pour plus de détails sur les adresses IP que vous devez ajouter à votre cluster, voir [Nouvelles adresses IP pour les e-mails Adobe Workfront avec la version 21.1](../../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md).

Pour savoir sur quel cluster se trouve votre instance, allez dans Configuration > Système > Informations sur le client.

### Liste d’adresses IP supplémentaires autorisées pour les abonnements aux événements {#allowlist-of-additional-ip-addresses-for-event-subscriptions}

Afin d’augmenter le taux de réussite des abonnements aux événements, nous ajouterons 4 nouvelles adresses IP lors de la version de production 21.1 au premier trimestre 2021. Vous devez ajouter ces adresses IP à votre liste d’autorisation avant février 2021 pour vous assurer que vos utilisateurs et utilisatrices continuent à recevoir des abonnements aux événements.

Contactez votre service informatique interne et/ou votre service de sécurité pour obtenir de l’aide pour l’ajout des nouvelles adresses IP indiquées dans l’article, [API d’abonnement aux événements](../../../wf-api/general/event-subs-api.md).

### Liste autorisée des domaines supplémentaires requis pour accéder à Workfront {#allowlist-of-additional-domains-required-for-accessing-workfront}

Si votre entreprise utilise un pare-feu, vous devez ajouter les domaines supplémentaires suivants à votre liste autorisée afin de garantir un accès ininterrompu à Workfront :

* event.split.io
* sdk.split.io

Pour plus d’informations, voir [Configurer la liste d’autorisation de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Abandon de Flash {#flash-deprecation}

Tous les outils basés sur Flash ont été supprimés de tous les produits le 19 novembre 2020.

Pour en savoir plus sur les solutions de remplacement pour chaque outil Flash spécifique, consultez l’article suivant : [Remplacement des outils Flash dans Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

### Webinaire sur la version 21.1 {#21-1-release-webinar}

Le webinaire sur la version 21.1 de Workfront sera présenté le 3 février à 11 h 00 EDT / 16 h 00 BST. Inscrivez-vous au webinaire [ici](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&amp;partnerref=ac&amp;eventid=2934272&amp;sessionid=1&amp;key=5C231B3385686D1E224A49EBE0BF0E37&amp;regTag=&amp;V2=false&amp;sourcepage=register).

### Modification de la cadence des versions préliminaires {#change-in-preview-release-cadence}

À partir du 20 mai 2020, Workfront a commencé à mettre à disposition des fonctionnalités dans l’environnement de prévisualisation sur une base hebdomadaire. Avant cette modification, les fonctionnalités étaient généralement mises à disposition dans l’environnement de prévisualisation toutes les deux semaines.

Pour plus d’informations, voir [Questions fréquentes sur la modification du rythme de publication de la version préliminaire de Workfront](https://experienceleague.adobe.com/fr/docs/workfront/using/home).

### Workfront One {#workfront-one}

Avec Workfront One, vous découvrirez le contenu, les ressources et les nouveautés de Workfront les plus importants, le tout au même endroit, avec la même connexion. Nous avons unifié les sites Expérience, Communauté et Formation pour faciliter la recherche.

[En savoir plus sur Workfront One](https://business.adobe.com/products/workfront.html).
