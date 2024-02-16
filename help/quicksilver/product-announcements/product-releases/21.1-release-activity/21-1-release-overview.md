---
content-type: release-notes
keywords: notes,trimestriel,mise à jour
navigation-topic: product-releases
title: Présentation de la version 21.1
description: La version 21.1 a été mise à disposition dans l’environnement de production pendant la semaine de .
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 3affee76-347e-4610-b255-4b1bb4414c5d
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '3658'
ht-degree: 0%

---

# Présentation de la version 21.1

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 21.1 release was made available in the Production environment the week of .</p>
-->

Cette page fournit des informations sur les fonctionnalités d’Adobe Workfront Classic et de la nouvelle expérience Adobe Workfront incluse dans la version 21.1.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

Avec cette version, nous proposons de nouvelles fonctionnalités et améliorations qui vous aideront à prendre la tête du retour en 2021 avec des stratégies adaptables, des processus de travail automatisés et une infrastructure numérique connectée pour garantir le succès de l’entreprise.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 21.1 release nears its planned Production release, this page will be updated with all functionality included with 21.1.</p>
-->

Ces améliorations sont actuellement disponibles.

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

Ils ont été relâchés la semaine du 15 février 2021.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.workfront.com/" target="_blank">Adobe Workfront Status Site</a>.
</MadCap:conditionalText>
-->

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs](#administrator-enhancements)
* [Améliorations de la gestion des ressources](#resource-management-enhancements)
* [Améliorations de la gestion de projet](#project-management-enhancements)
* [Améliorations des analyses](#enhanced-analytics-improvements)
* [Améliorations de l’intégration](#integration-enhancements)
* [Améliorations apportées aux mobiles](#mobile-enhancements)
* [Autres améliorations](#other-enhancements)

### Améliorations apportées aux administrateurs {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Ajout d’un nouveau paramètre Niveau d’accès pour la copie de projets</a> </p> <p>Pour vous donner plus de contrôle, en tant qu’administrateur système, sur ce que les planificateurs peuvent faire d’un projet, nous avons rendu l’accès Modifier aux projets du niveau d’accès plus granulaire, en introduisant un nouveau paramètre qui vous permet d’activer ou de désactiver leur capacité à copier des projets. Avant cette modification, lorsque vous avez activé l’accès des utilisateurs à l’option Modifier des projets, ils avaient automatiquement accès à la copie. Grâce à la nouvelle fonctionnalité, vous pouvez donner à une personne l’accès pour modifier des projets sans nécessairement avoir accès à les copier en désactivant le nouveau paramètre Copier.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#in" class="MCXref xref" xrefformat="{para}">Dans un formulaire personnalisé sur un objet, sélectionnez tous les éléments d’un champ déroulant à sélection multiple.</a> </p> <p>Sur la page Détails d’un objet, lorsque vous remplissez un champ déroulant à sélection multiple sur un formulaire personnalisé, vous pouvez cliquer sur Sélectionner tout si vous devez sélectionner toutes les options disponibles.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Non disponible actuellement lorsque vous envoyez une nouvelle requête.)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#recalcul" class="MCXref xref" xrefformat="{para}">Recalculer tous les champs de formulaire personnalisés d’un objet</a> </p> <p>Il est désormais plus facile de s’assurer que toutes les données des champs personnalisés calculés sont à jour pour un objet. Une nouvelle option de menu Recalculer les expressions permet de recalculer rapidement toutes les données de ces champs.</p> <p>Cela s’avère particulièrement utile lorsqu’une personne modifie des données dans un autre objet référencé par un champ personnalisé calculé de votre objet.</p> <p>Auparavant, les utilisateurs devaient utiliser des solutions pour s’assurer que toutes les données des champs personnalisés calculés étaient à jour. Par exemple, ils ont modifié l’objet avec d’autres objets pour utiliser l’option de recalcul disponible pour la modification en masse.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 10 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#unlock" class="MCXref xref" xrefformat="{para}">Déverrouiller les préférences de tâche et de problème pour les administrateurs de groupe</a> </p> <p>Les administrateurs Workfront peuvent désormais accorder aux administrateurs de groupe une plus grande autonomie en déverrouillant les tâches individuelles et les préférences de problème. Lorsqu’une préférence est déverrouillée, les administrateurs de groupe peuvent la configurer pour que leurs groupes répondent aux besoins uniques et aux processus internes de chaque groupe.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version bêta de l’aperçu : 2 décembre 2020</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Avant le 24 juin 2021, cette option était disponible dans le cadre d’un déploiement échelonné uniquement pour les clients des groupes 4 et 6 et quelques autres clients. Elle est maintenant disponible en production pour tous les clients.)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configurer séparément les paramètres de niveau d’accès pour les portefeuilles et les programmes</a> </p> <p>Il est désormais plus facile de gérer l’accès des utilisateurs aux portefeuilles et aux programmes, car vous pouvez configurer leurs paramètres de niveau d’accès séparément.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version bêta de l’aperçu : 2 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">Cochez toutes les cases d’une série lors de la modification d’informations dans un formulaire personnalisé.</a> </p> <p>Sur la page Détails d’un objet, lorsque vous renseignez un champ Formulaire personnalisé contenant des cases à cocher, vous pouvez cliquer sur Sélectionner tout si vous devez cocher toutes les cases disponibles.</p> <p>Cette option s’affiche uniquement si le champ contient plus de 2 cases à cocher.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version bêta de l’aperçu : 2 décembre 2020</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Non disponible actuellement lors de l’envoi d’une demande.)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur2" class="MCXref xref" xrefformat="{para}">Configuration de votre liste autorisée de messagerie Workfront</a> </p> <p>Pour mieux sécuriser vos données, vous pouvez désormais utiliser une liste autorisée de domaine de courriel pour :</p> 
    <ul> 
     <li> <p>Contrôle de l’emplacement où se rendent les emails Workfront s’ils contiennent des rapports ou des documents stockés dans Workfront</p> </li> 
     <li> <p>Les domaines de contrôle des courriers électroniques peuvent se trouver dans l’adresse électronique que les utilisateurs peuvent spécifier dans leur profil utilisateur.</p> </li> 
    </ul> <p>Par exemple, si vous souhaitez protéger des données sensibles, telles qu’un rapport répertoriant vos clients à risque, vous pouvez inclure uniquement votre domaine de courriel interne ou vos domaines dans la liste autorisée de courriel. De cette manière, les utilisateurs ne peuvent pas envoyer ce rapport (ni aucun autre rapport Workfront) à une adresse électronique externe.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 20 novembre 2020</p> <p>Version de production : avec la version 21.1 </p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">Affecter un administrateur de groupe à un sous-groupe</a> </p> <p>Pour faciliter le fonctionnement indépendant des niveaux de votre organisation, nous avons ajouté la possibilité d’affecter un administrateur de groupe à un sous-groupe. Vous pouvez désormais vous assurer que vous déléguez la gestion des sous-groupes aux personnes appropriées.</p> <p>Auparavant, seul un groupe de niveau supérieur pouvait avoir des administrateurs de groupe, et ces administrateurs géraient tous les sous-groupes sous le groupe de niveau supérieur.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 20 novembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#work" class="MCXref xref" xrefformat="{para}">Utilisation des projets de groupe et des processus de validation dans la zone Groupes</a> </p> <p>Si vous êtes administrateur de groupe, il est facile d’afficher et de travailler avec les projets de votre groupe et les processus d’approbation maintenant qu’ils sont répertoriés dans la zone Groupes . </p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 20 novembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur3" class="MCXref xref" xrefformat="{para}">Configuration des notifications d’événement pour les groupes</a> <span style="color: #dc143c; font-weight: bold;">Nouveau dans Aperçu .</span></p> <p>Les administrateurs de Workfront peuvent désormais accorder aux administrateurs de groupe une plus grande autonomie en leur permettant de configurer des notifications d’événement pour leurs groupes de niveau supérieur. Les sous-groupes héritent des configurations de notification d’événement de leur groupe parent supérieur.</p> <p>Auparavant, les notifications d’événement n’étaient configurables que par un administrateur Workfront au niveau du système, ce qui signifie que tous les groupes devaient utiliser le même ensemble de notifications d’événement.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 22 janvier 2021</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Disponible initialement en production uniquement pour les clients sur la grappe 4 dans le cadre d’un déploiement échelonné ; disponible pour d’autres grappes peu de temps après)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">Afficher le nombre de licences utilisées et allouées dans un groupe</a> </p> <p>Pour déterminer la distribution de vos licences, vous pouvez désormais afficher le nombre de licences utilisées dans un groupe et les sous-groupes situés en dessous.</p> <p>Si vous gérez un groupe de niveau supérieur, vous pouvez afficher à la fois le nombre de licences utilisées dans un groupe (et ses sous-groupes) et le nombre maximal de licences attribuées au groupe.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 20 novembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations de la gestion des ressources {#resource-management-enhancements}

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
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 17 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Équilibreur Workfront disponible pour l’équipe</a> </p> <p>L’équilibreur de charge de travail est désormais disponible au sein d’une équipe. Vous avez désormais la possibilité de choisir entre l’utilisation de l’équilibreur de charge de travail ou l’outil de planification pour gérer les ressources de votre équipe. </p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 20 novembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations de la gestion de projet {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">Exportation désormais disponible dans la section Mesures d’un projet</a> </p> <p>Pour partager plus facilement l’état et la progression d’un projet, vous pouvez désormais exporter l’intégralité du tableau de bord dans la section Mesures d’un projet vers un fichier .png .</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 15 janvier 2021</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#update" class="MCXref xref" xrefformat="{para}">Mettre à jour le pourcentage de problème terminé lorsque le projet ou la tâche a été converti à partir de la mise à jour du problème</a> </p> <p>Nous avons mis à jour la façon dont le pourcentage de problèmes terminés fonctionne pour les problèmes qui ont été convertis en projets ou en tâches. Avec la nouvelle fonctionnalité, lorsqu’un problème est converti en tâche ou projet, le pourcentage de fin du problème est mis à jour en synchronisation avec le pourcentage de fin de la tâche ou du projet de résolution lorsque l’état "Mettre à jour automatiquement le problème résolvable lorsque l’état du paramètre Résoudre l’objet change" est activé à partir de la configuration.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#fields" class="MCXref xref" xrefformat="{para}">Champs supprimés de la page Nouvelle requête</a> </p> <p>Dans le cadre de la reconception de la page Nouvelle requête, nous avons mis à jour les nouveaux champs de problème configurés dans la section Configuration de la file d’attente d’un projet.</p> <p>Divers nouveaux champs de problème s’affichent uniquement lors de la création d’un problème à partir de la section Problèmes du projet. Elles ne s’affichent pas lors de l’envoi d’un problème à l’aide d’une file d’attente de demandes dans la zone Demandes .</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Retiré de la version)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de l’envoi de requêtes dans la zone Demandes</a> </p> <p>Afin d’assurer la cohérence avec la nouvelle expérience Workfront et d’améliorer l’efficacité de votre action lors de l’envoi de requêtes, nous avons repensé la zone Nouvelle requête dans la zone Demandes .</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Suppression de la version ; elle reste dans Aperçu et version en production avec la version 21.2)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Partage d’un lien vers une file d’attente de demandes lors de l’envoi d’une demande</a> </p> <p>Nous avons maintenant rendu possible le partage d’un lien vers une file d’attente de requêtes, un groupe de rubriques ou une rubrique de file d’attente.</p> <p>Avant d’envoyer une nouvelle requête, vous pouvez copier un lien vers la file d’attente des requêtes, le groupe de rubriques ou la rubrique de la file d’attente de la requête et le partager avec d’autres utilisateurs, ou l’incorporer dans un tableau de bord.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 13 janvier 2021</p> <p>Version de production : avec la version 21.1 <span style="color: #dc143c; font-weight: bold;">(Suppression de la version ; elle reste dans Aperçu et version en production avec la version 21.2)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Nouvelle liste des requêtes envoyées</a> </p> <p>Pour vous permettre de gérer vos requêtes envoyées de manière plus simple et cohérente, nous avons supprimé les sections Demandes que j’ai envoyées et Toutes les requêtes de la zone Demandes et les avons remplacées par une nouvelle liste Envoyées. L’aspect familier de la liste correspond à toutes les autres listes du système, ce qui vous permet de filtrer différentes catégories de demandes envoyées et de rechercher rapidement une demande qui peut être difficile à trouver.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version bêta de l’aperçu : 2 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#search" class="MCXref xref" xrefformat="{para}">Recherchez un groupe à affecter à un projet et affichez ses détails.</a> </p> <p>Il est désormais plus facile de vous assurer d’identifier le bon groupe lorsque vous affectez un groupe à un projet. Pointez sur le nom d’un groupe que vous trouvez dans la zone Groupe, puis cliquez sur l’icône d’information qui s’affiche en regard du nom pour afficher l’info-bulle Détails du groupe.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 17 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nouveau rapport Délégation d’utilisateurs</a> </p> <p>Auparavant, les informations relatives aux délégations de tâche, de problème et d’approbation de projet ne pouvaient être visualisées que par le délégué dans sa zone d’accueil. Pour permettre à d’autres utilisateurs de voir ces informations, Planifier les utilisateurs peut maintenant créer le rapport Délégation d’utilisateurs , qui vous indique :</p> 
    <ul> 
     <li> <p>Qui a délégué ces approbations à un autre utilisateur</p> </li> 
     <li> <p>Quel utilisateur a reçu ces validations ?</p> </li> 
     <li> <p>Les dates de début et de fin de ces délégations</p> </li> 
    </ul> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 17 décembre 2020</p> <p>Version de production : 21 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations des analyses {#enhanced-analytics-improvements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#people" class="MCXref xref" xrefformat="{para}">La page Personnes est désormais disponible pour toutes les grappes.</a> </p> <p>La page Personnes est désormais disponible sur Workfront Classic pour la grappe 4. Cette page comprend les graphiques de l’activité par équipe, capacité des ressources et capacité de l’équipe.</p> <p>Cette page était auparavant disponible avec la version 20.3 de Workfront Classic et la nouvelle expérience Workfront pour toutes les autres grappes.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 28 janvier 2021</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront (précédemment disponible)</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#enhanced" class="MCXref xref" xrefformat="{para}">Les analyses améliorées s’affichent désormais par défaut.</a> </p> <p>Remarque : cette modification s’applique uniquement aux utilisateurs qui viennent d’être ajoutés aux modèles de mise en page. Les utilisateurs affectés à un modèle de mise en page personnalisé ne sont pas non plus affectés par cette modification.</p> <p>Dans le modèle de mise en page par défaut, la zone Analytics est désormais activée par défaut, ce qui signifie que les utilisateurs affectés à ce modèle de mise en page voient désormais la zone Analytics dans la barre de navigation globale de Workfront Classic et le menu principal dans la nouvelle expérience Workfront.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 6 novembre 2020</p> <p>Version de production : 3 décembre 2020</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#availab" class="MCXref xref" xrefformat="{para}">Analyse améliorée disponible pour toutes les grappes</a> </p> <p>Les analyses améliorées sont disponibles pour toutes les grappes Workfront, y compris les clients sur la grappe 6.</p> <p>Auparavant, les analyses améliorées n’étaient pas disponibles avec Google Cloud Platform, ce qui empêchait les clients du cluster 6 d’accéder à la zone Analytics. Désormais, les clients professionnels et d’entreprise du cluster 6 peuvent accéder à la zone Analytics.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 20 novembre 2020</p> <p>Version de production : 3 décembre 2020</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Améliorations des notifications Adobe Workfront dans Microsoft Teams</a> </p> <p>Afin que vous puissiez plus facilement utiliser Workfront par le biais de Microsofts Teams, nous avons ajouté diverses améliorations aux notifications de Microsofts Teams envoyées depuis Workfront.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : S.O.</p> <p>Version de production : 12 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations apportées aux mobiles {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouveaux chemins de navigation dans l’application Adobe Workfront</a> </p> <p>Nous avons ajouté une navigation par chemin de navigation à l’application mobile Workfront. Vous pouvez désormais utiliser cette fonction pour accéder aux tâches parentes au sein d’un projet.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : S.O.</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#rich" class="MCXref xref" xrefformat="{para}">Texte enrichi pris en charge dans les formulaires personnalisés sur l’application Workfront</a> </p> <p>Vous pouvez désormais utiliser la mise en forme de texte enrichi dans les champs de texte de formulaire personnalisés dans l’application mobile Workfront.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : S.O.</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#sso" class="MCXref xref" xrefformat="{para}">Les utilisateurs SSO peuvent désormais se reconnecter à l’application Workfront à l’aide de la technologie d’identification de visage ou d’empreinte digitale.</a> </p> <p>Si votre entreprise utilise la fonction SSO, vous pouvez désormais utiliser votre ID de visage ou votre empreinte digitale pour vous connecter à l’application mobile Workfront une fois la session expirée. Toutefois, vous devez vous connecter avec vos informations d’identification SSO au départ.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : S.O.</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Mises à jour des exigences en matière d’échec d’abonnement à un événement</a> </p> <p>Nous mettons à jour les exigences de désactivation progressive des échecs d’abonnement à un événement. Outre les exigences existantes, les abonnements à des événements seront désormais désactivés en douceur s’ils ne parviennent pas à obtenir une diffusion réussie dans les 2000 tentatives. Il s’agit de renforcer la règle actuelle de 70 % d’échec, qui peut conduire à des quantités excessives de défaillances, sous certaines conditions.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : S.O.</p> <p>Version de production : 11 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouveaux champs d’équipe disponibles pour le Daily Digest</a> </p> <p>Nous avons ajouté les champs d’approbation et d’affectation de l’équipe au courrier électronique Action Needed Daily Digest.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 17 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#replacin" class="MCXref xref" xrefformat="{para}">Remplacement de l’option de courrier électronique POP dans les files d’attente de requête</a> </p> <p>Nous remplaçons l’option de messagerie POP pour les files d’attente de demandes par un nouveau système géré par Workfront. Vous pourrez toujours envoyer des demandes par courrier électronique, mais vous devrez plutôt configurer une nouvelle adresse électronique gérée par Workfront dans la zone File d’attente des demandes . </p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 17 décembre 2020</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">Limitation de la modification des heures sur les feuilles de temps</a> </p> <p>Pour mieux contrôler les feuilles de temps et la modification des heures, nous avons ajouté un paramètre qui vous permet de limiter la modification des heures aux propriétaires de feuilles de temps et aux administrateurs système.</p> <p>Auparavant, les utilisateurs dont l’option Fiches horaires et heures était activée dans leur niveau d’accès pouvaient modifier les heures sur n’importe quelle feuille de temps.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 21 janvier 2021</p> <p>Version de production : avec la version 21.1</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Amélioration des filtres et des vues dans la zone Fiches horaires</a> </p> <p>Nous avons ajouté des filtres pour les projets et les problèmes, ainsi que des options d’affichage et de regroupement à la page de recherche.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version bêta de l’aperçu : 2 décembre 2020</p> <p>Version de production : 21 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#hide" class="MCXref xref" xrefformat="{para}">Masquer la zone des heures supplémentaires dans les feuilles de calcul</a> </p> <p>Vous pouvez désormais masquer la zone des heures supplémentaires afin de faciliter la confusion des utilisateurs si vous ne effectuez pas le suivi des heures supplémentaires dans Workfront. Vous pouvez masquer la zone des heures supplémentaires pour une feuille de temps à usage unique ou dans le profil de la feuille de temps.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version bêta de l’aperçu : 2 décembre 2020</p> <p>Version de production : 16 décembre 2020</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#expand" class="MCXref xref" xrefformat="{para}">Développer ou réduire les éléments dans la navigation du chemin de navigation</a> </p> <p>Pour faciliter l’affichage du chemin de navigation complet, nous avons ajouté des fonctionnalités de développement et de réduction.</p> <p>Désormais, tous les éléments tronqués sont regroupés avant le projet avec le texte "plus". Par exemple, "3 autres" indique qu’il existe 3 objets qui ne s’affichent pas.</p> <p>Auparavant, vous deviez cliquer sur les points de suspension pour afficher les objets tronqués dans un menu déroulant.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 7 janvier 2020</p> <p>Version de production : 21 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nouvelle apparence de la navigation dans le chemin de navigation</a> </p> <p>Pour aider les utilisateurs à mieux identifier leur emplacement dans Workfront et à naviguer plus facilement entre les objets, nous avons apporté plusieurs améliorations à la navigation dans le chemin de navigation.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> <p>Version d’aperçu bêta : 10 décembre 2020</p> <p>Version de production : 21 janvier 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

## Améliorations des objectifs de Workfront

La plupart des nouvelles fonctionnalités de la version 21.1 des objectifs de Workfront. Pour plus d’informations sur ces nouvelles fonctionnalités désormais disponibles dans l’aperçu, voir [Objectifs Adobe Workfront avec la version 21.1](../../../product-announcements/product-releases/goals-release-activity/goals-release-21-1.md).

## Améliorations du planificateur de scénario Workfront

Nouvelles fonctionnalités de la version 21.1 de Workfront Scenario Planner. Pour plus d’informations sur ces nouvelles fonctionnalités désormais disponibles dans l’aperçu, voir [Planificateur de scénario Adobe Workfront avec la version 21.1](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-1.md).

## Améliorations apportées à Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent du calendrier de version 21.1. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Publication de fusion Adobe Workfront](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)

## Améliorations des API

L’API version 12 est désormais disponible avec la version 20.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de l’API version 12](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWF_API%2FAPI%2Fnew-api-version-12.htm).

Pour plus d’informations sur les versions d’API, voir [Contrôle de version des API et planification de la prise en charge](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

.

## Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version 21.1, voir [Mises à jour de maintenance Workfront](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Annonces

* [Nouvelles adresses IP pour les emails Workfront avec la version 21.1](#new-ip-addresses-for-workfront-email-with-the-21-1-release)
* [Liste autorisée d’adresses IP supplémentaires pour les abonnements à des événements](#allowlist-of-additional-ip-addresses-for-event-subscriptions)
* [Liste autorisée des domaines supplémentaires requis pour accéder à Workfront](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [obsolescence des Flashs](#flash-deprecation)
* [Webinaire sur la version 21.1](#21-1-release-webinar)
* [Modification de la cadence de publication de l’aperçu](#change-in-preview-release-cadence)
* [Workfront One](#workfront-one)

### Nouvelles adresses IP pour les emails Workfront avec la version 21.1 {#new-ip-addresses-for-workfront-email-with-the-21-1-release}

Afin d’améliorer la diffusion des emails, nous ajoutons de nouvelles adresses IP avec la version de production 21.1 pour les grappes 1, 2, 3, 4 et 5.

Pour plus d’informations sur les adresses IP que vous devez ajouter à votre grappe, voir [Nouvelles adresses IP pour les emails Adobe Workfront avec la version 21.1](../../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md).

Pour savoir sur quelle grappe se trouve l’instance, accédez à Configuration > Système > Informations client.

### Liste autorisée d’adresses IP supplémentaires pour les abonnements à des événements {#allowlist-of-additional-ip-addresses-for-event-subscriptions}

Afin d’améliorer la diffusion réussie de l’abonnement à un événement, nous ajoutons 4 nouvelles adresses IP avec la version de production 21.1 au premier trimestre 2021. Vous devez ajouter ces adresses IP à votre liste autorisée avant février 2021 pour vous assurer que vos utilisateurs continuent à recevoir des abonnements à un événement.

Contactez votre service informatique et/ou de sécurité interne pour obtenir de l’aide sur l’ajout des nouvelles adresses IP trouvées dans l’article, [API d’abonnement à un événement](../../../wf-api/general/event-subs-api.md).

### Liste autorisée des domaines supplémentaires requis pour accéder à Workfront {#allowlist-of-additional-domains-required-for-accessing-workfront}

Si votre entreprise utilise un pare-feu, vous devez ajouter les domaines supplémentaires suivants à votre liste autorisée pour garantir un accès ininterrompu à Workfront :

* event.split.io
* sdk.split.io

Pour plus d’informations, voir [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### obsolescence des Flashs {#flash-deprecation}

Le 19 novembre 2020, tous les outils basés sur le Flash ont été supprimés de tous les produits.

Pour en savoir plus sur les solutions de remplacement pour chaque outil spécifique basé sur les Flashs, consultez l’article suivant : [Remplacement des outils par Flash dans Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

### Webinaire sur la version 21.1 {#21-1-release-webinar}

Le webinaire sur la version 21.1 de Workfront sera présenté le 3 février à 11h00 (heure d’été)/16h00 (heure d’été). Inscrivez-vous au webinaire [here](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&amp;partnerref=ac&amp;eventid=2934272&amp;sessionid=1&amp;key=5C231B3385686D1E224A49EBE0BF0E37&amp;regTag=&amp;V2=false&amp;sourcepage=register).

### Modification de la cadence de publication de l’aperçu {#change-in-preview-release-cadence}

À compter du 20 mai 2020, Workfront a commencé à rendre les fonctionnalités disponibles chaque semaine dans l’environnement Aperçu. Avant cette modification, la fonctionnalité était généralement publiée dans l’environnement Aperçu toutes les deux semaines.

Pour plus d’informations, voir [FAQ sur le changement de la cadence de prévisualisation de Workfront](https://one.workfront.com/s/article/Change-in-Workfront-Preview-release-cadence)

### Workfront One {#workfront-one}

Avec Workfront One, vous découvrirez le contenu, les ressources et les informations les plus importants de Workfront, le tout à un seul emplacement, avec une seule connexion. Nous avons unifié les sites Expérience, Communauté et Formation pour faciliter la recherche de ce que vous recherchez.

[En savoir plus sur Workfront One](https://www.workfront.com/campaigns/workfront-one).
