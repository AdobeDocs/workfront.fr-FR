---
title: Vue d’ensemble de la version 22.3
description: Vue d’ensemble de la version 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bfc7ce9e-b715-47b7-bab7-2e3540d0da3e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3221'
ht-degree: 99%

---

# Vue d’ensemble de la version 22.3

Cette page fournit des informations sur les fonctionnalités incluses dans la version 22.3. Toutes les fonctionnalités répertoriées sont disponibles dans la nouvelle expérience Adobe Workfront. Certaines fonctionnalités sont également disponibles dans Adobe Workfront Classic. Toutefois, [Workfront Classic sera abandonné en mars 2022](https://experienceleague.adobe.com/fr/docs/workfront/using/home) et atteindra sa date de fin de vie en juillet 2022.

Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 juillet 2022.

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations apportées aux projets](#project-enhancements)
* [Amélioration apportées à la gestion des ressources.](#resource-management-enhancements)
* [Amélioration des rapports](#reporting-enhancements)
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Intégrer Adobe Workfront avec JumpSeat
</a></p></p> <p>Vous pouvez désormais intégrer JumpSeat à Workfront afin de créer des conseils personnalisés et intégrés au produit à l’intention de vos utilisateurs et de vos utilisatrices. Pour activer l’intégration, vous devez disposer d’une licence d’entreprise Adobe Workfront et d’un abonnement JumpSeat actif.</p>  
    </td>
    <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Utiliser des statuts Déverrouillé dans des processus d’approbation
</a></p></p> <p>Cette fonctionnalité a été supprimée de la version de production 22.3. Cette fonctionnalité devrait être mise en production ultérieurement.</p> 
<p>Pour vous permettre de mieux contrôler les processus et les statuts d’approbation dans votre système, nous avons autorisé la création d’un processus d’approbation basé sur un statut de système déverrouillé. De plus, vous pouvez désormais déverrouiller tout statut déjà utilisé dans un processus d’approbation. Auparavant, un statut système utilisé dans un processus d’approbation devait être verrouillé. Cela le rendait disponible pour tous les groupes, sans possibilité de le supprimer ou de le renommer. Les équipes d’administration de groupe ne pouvaient donc pas rationaliser la liste des statuts de leur groupe en fonction de leurs besoins spécifiques.</p>   
   </td> 
    <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : 15 septembre 2022</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Paramètres par défaut de l’épreuve déplacés vers Workfront
</a></p></p> <p>Vous pouvez désormais modifier les paramètres suivants de l’épreuve dans la zone de configuration de Workfront :</p> 
<ul>
   <li><p>Paramètres par défaut de l’épreuve</p></li>
   <li><p>Paramètres du statut de décision de l’épreuve</p></li>
   </ul> 
   </td> 
    <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 1er juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter un fichier PDF à un formulaire personnalisé
</a></p></p> <p>Nous vous aidons à rendre les formulaires personnalisés plus visuels et informatifs grâce aux nouveaux widgets de ressources que vous pouvez ajouter, tels que des images et des vidéos. Vous pouvez maintenant ajouter dans un formulaire personnalisé un lien vers un fichier PDF. Lorsque le formulaire est joint à un objet, les personnes qui l’utilisent peuvent afficher le PDF et interagir avec lui depuis le formulaire.</p>
   </td> 
    <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">L’éditeur de calcul de champ de formulaire personnalisé affiche les informations d’erreur</a><span style="color: #ff0000; font-weight: bold;"> (temporairement indisponible)</span></p></p> <p>La modification des calculs pour les champs personnalisés est désormais plus facile avec des informations d’erreur utiles indiquées directement dans le calcul. Lorsque vous créez un champ calculé dans un formulaire personnalisé, les erreurs sont surlignées en rose. Lorsque vous pointez sur la partie mise en surbrillance, une info-bulle s’affiche pour décrire le problème.</p>
    </td> 
    <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 9 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Personnalisation de l’en-tête du projet
</a></p></p> <p>En tant qu’administrateur ou administratrice Workfront ou de groupes, vous pouvez désormais personnaliser les champs qui s’affichent dans l’en-tête d’un projet lorsque vous utilisez un modèle de mise en page.</p>
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
    <td>
    <ul> 
     <li> <p>Version préliminaire : 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
   </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Contrôler la création d’un projet vierge</a></p></p> <p>En tant qu’administrateur ou administratrice système ou de groupes, vous pouvez désormais contrôler le fait que les personnes puissent ou non créer des projets vierges sans utiliser de modèle. Nous avons ajouté un nouveau paramètre dans la zone Préférences du projet de la configuration. Il permet de désactiver la création de projets vierges dans les zones suivantes :</p> 
   <ul>
   <li><p>À partir de l’option Nouveau projet dans une liste de projets</p></li>
   <li><p>Lors de la conversion d’un problème en projet à partir de la page des problèmes</p></li>
   </ul>
   <p>Le nouveau paramètre est « Autoriser les personnes à créer des projets sans utiliser de modèle » et est activé par défaut.</p> </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 19 mai 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Désactiver un groupe à partir de la page Groupes</a> </p> <p>Récemment, nous avons ajouté la possibilité de désactiver et de réactiver les groupes. Pour rendre cette action plus rapide et plus facile, nous l’avons ajoutée à la page des groupes. Désormais, après avoir cliqué sur le nom d’un groupe pour accéder à sa page, vous pouvez sélectionner le menu Plus <img src="assets/more-icon.png"> en regard du nom du groupe, puis sélectionner Désactiver ou Réactiver.</p> <p>Auparavant, vous ne pouviez désactiver ou réactiver un groupe qu’à l’aide de la case à cocher Est actif sur sa page Détails. </p> </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 14 avril 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter des vidéos aux formulaires personnalisés</a> </p> <p>Vous pouvez désormais ajouter un nouvel outil proposant des informations, un intérêt visuel et de la créativité à un formulaire personnalisé à l’aide d’une vidéo. Lorsque le formulaire est joint à un objet, les personnes travaillant avec l’objet peuvent lire la vidéo à tout moment.</p> <p>Auparavant, vous ne pouviez ajouter que des champs textuels et des images à un formulaire personnalisé.</p> </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 14 avril 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations apportées aux projets {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Délégation du travail lors d’absences du bureau</a></p> <p>Vous pouvez déléguer les tâches et les problèmes qui vous sont affectés à d’autres personnes lorsque vous prévoyez de vous absenter du bureau pour une brève période. Cela permet de s’assurer que votre absence ne constitue pas un obstacle à la réalisation du travail.</p> 
   <p>Avant cette amélioration, vous ne pouviez que déléguer des approbations.</p></td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 9 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de la conversion d’un problème en tâche</a></p> <p>Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface de conversion d’un problème en tâche.</p> 
   </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 9 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de la conversion d’un problème en projet sans modèle</a></p> <p>Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface permettant de convertir un problème en projet sans utiliser de modèle.</p> 
   <p>En plus d’une interface utilisateur mise à jour qui correspond au reste de la nouvelle expérience Workfront, nous avons également ajouté la possibilité de convertir un problème en projets vierges à partir d’une liste ou d’un rapport.</p></td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Tags intelligents dans le flux de mises à jour</a></p> <p>Nous avons amélioré la façon de taguer des personnes dans le flux de mises à jour lorsque vous créez une mise à jour ou répondez à une mise à jour existante. Désormais, lorsque vous taguez une personne pour l’inclure dans une mise à jour, en plus de son nom et de son avatar, nous affichons également son rôle principal et son e-mail. Cela permet de distinguer plusieurs utilisateurs portant des noms similaires ou identiques.</p> </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 19 mai 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle syntaxe pour les calculs dans les champs personnalisés</a> </p> <p>Pour préparer les futures améliorations qui vous permettront d’ajouter des calculs aux formulaires personnalisés, nous avons normalisé la syntaxe des champs référencés que vous ajoutez à un calcul. Il est facile d’utiliser cette nouvelle syntaxe, car le système la saisit pour vous lorsque vous commencez à taper le nom d’un champ et que vous le sélectionnez.</p> </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 5 mai 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Conserver des informations précises lorsque deux personnes ayant un rôle commun sont impliquées dans un processus d’approbation</a>. </p> <p>Afin de garantir l’exactitude des données relatives à l’approbation du travail, nous avons modifié la manière dont les informations d’approbation sont enregistrées sur un élément lorsqu’un processus d’approbation nécessitant plusieurs rôles est associé à cet élément.</p> <p>Certains processus d’approbation requièrent l’approbation de deux rôles différents, et deux personnes différentes chargées de l’approbation peuvent avoir l’un de ces rôles en commun. Lorsque cela se produit, après que les décisions d’approbation ont été prises, Workfront enregistre chaque personne chargée de l’approbation et son rôle respectif associé au processus d’approbation.</p> <p>Avant cette modification, les deux approbations étaient enregistrées pour la deuxième personne parce qu’elle partageait l’un des rôles d’approbation avec la première. Dans ce cas, la deuxième personne approbatrice écrasait les informations de la première.</p> </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 21 avril 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://experienceleague.adobe.com/fr/docs/workfront/using/home" target="_blank">Workfront Classic a été arrêté en mars 2022</a>, suivi de peu par sa date de fin de vie en juillet 2022).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de la conversion d’un problème en projet à l’aide d’un modèle au niveau du problème</a> </p> <p>Afin d’harmoniser votre utilisation de Workfront avec la nouvelle expérience Workfront, nous avons repensé l’interface de conversion d’un problème en projet lorsque vous utilisez un modèle et que vous le convertissez à partir de la page du problème.</p> <p>Vous pouvez désormais accéder plus facilement à votre liste de favoris immédiatement après avoir choisi de convertir le problème.</p> <p>L’interface reconçue correspond à l’expérience de création d’un projet à partir d’un modèle que nous avons mis à jour récemment.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> 
    <ul> 
     <li> <p>Version préliminaire : 8 décembre 2021<br></p> </li> 
     <li> <p>Version de production : déploiement par phases à partir du 28 avril 2022 <span style="color: #ff0000; font-weight: bold;">Cette fonctionnalité a été temporairement supprimée de l’environnement de production le 4 mars 2022. Elle a ensuite été déployée de manière progressive à partir du 28 avril 2022. Le déploiement s’est achevé le 5 mai 2022. Cette option est désormais disponible en prévisualisation et en production pour toute la clientèle.</span></p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">Convertir les problèmes en projets à l’aide d’un modèle à partir de listes, de rapports et de tableaux de bord</a> </p> <p>Pour améliorer l’efficacité de votre travail et faciliter la conversion des problèmes dans un environnement en constante évolution, nous avons ajouté la possibilité de convertir un problème en projet à partir d’un modèle d’une liste, d’un rapport ou d’un tableau de bord.</p> <p>Avant cette amélioration, cette fonctionnalité n’existait que lorsque vous convertissiez le problème à partir de la page des problèmes.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> 
    <ul> 
     <li> <p>Version préliminaire : 8 décembre 2021<br></p> </li> 
     <li> <p>Version de production : déploiement par phases à partir du 28 avril 2022 <span style="color: #ff0000; font-weight: bold;">Cette fonctionnalité a été temporairement supprimée de l’environnement de production le 4 mars 2022. Elle a ensuite été déployée de manière progressive à partir du 28 avril 2022. Le déploiement s’est achevé le 5 mai 2022. Cette option est désormais disponible en prévisualisation et en production pour toute la clientèle.</span></p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#allocati" class="MCXref xref" xrefformat="{para}">Les heures d’affectation ne seront plus supprimées lors de la modification des affectations.</a> </p> <p>Pour garantir l’exactitude de vos données, nous avons apporté une modification afin de préserver les heures d’attribution et de maintenir inchangé le nombre d’heures prévues pour la tâche lorsque des changements sont apportés aux affectations de la tâche.</p> <p>Les changements suivants ont été apportés aux tâches avec un type de durée simple :</p> 
    <ul> 
     <li> <p>Les attributions d’affectations individuelles sont conservées lors du remplacement des utilisateurs et utilisatrices et des rôles.</p> </li> 
     <li> <p>Les attributions d’affectations individuelles sont conservées sur le rôle lors de la suppression de l’utilisateur ou de l’utilisatrice.</p> </li> 
    </ul> </td> 
   <td><strong>Disponible à ces dates :</strong> 
    <ul> 
     <li> <p>Version préliminaire : 10 février 2022<br></p> </li> 
     <li> <p>Version de production : 21 avril 2022 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://experienceleague.adobe.com/fr/docs/workfront/using/home" target="_blank">Workfront Classic a été arrêté en mars 2022</a>, suivi de peu par sa date de fin de vie en juillet 2022).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Partager des dossiers uniquement aux cinq premiers niveaux d’une hiérarchie de dossiers</a> (Ce lien renvoie aux notes de mise à jour de la version 20.2, date à laquelle cette fonctionnalité a été introduite dans l’environnement de prévisualisation.)</p> <p>Pour garantir les meilleures performances aux utilisateurs et utilisatrices qui partagent des dossiers, nous limitons actuellement le partage aux cinq premiers niveaux d’une hiérarchie de dossiers sur un objet.</p> <p>Chaque dossier du sixième niveau ou d’un niveau inférieur hérite ses configurations de partage du dossier qui lui est directement supérieur.</p> </td> 
   <td><strong>Disponible à ces dates :</strong> 
    <ul> 
     <li> <p>Version préliminaire : 10 février 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 <span style="color: #ff0000; font-weight: bold;">Cette fonctionnalité est temporairement indisponible. Cette page sera mise à jour lorsque la fonctionnalité sera disponible dans l’environnement de production.</span></p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://experienceleague.adobe.com/fr/docs/workfront/using/home" target="_blank">Workfront Classic sera arrêté en mars 2022</a>, suivi de peu par sa date de fin de vie en juillet 2022).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Campagnes Workfront (version bêta)</a> </p>
                        <p>Nous introduisons un nouvel objet dans Adobe Workfront qui a le potentiel de modifier la façon dont vous gérez le travail. </p>
                        <p>Les campagnes Workfront vous permettent d’organiser des projets provenant de différents portfolios et programmes dans un nouveau conteneur de travail.
Les campagnes ont été publiées en juillet 2022 dans la version préliminaire bêta 22.3. Pour plus d’informations, consultez la section <a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations apportées au projet dans la version 22.3 </a> </p>
<p>Ce nouveau conteneur évoluera dans les prochaines versions pour relier des objets de travail qui sont actuellement gérés dans des silos séparés.</p>

</td>
                    <td><span class="bold">Disponible à ces dates :</span>
                        <ul>
                            <li>
                                <p>Version préliminaire : pendant toute la période de la version 22.4<br /><span style="color: #ff0000; font-weight: bold;">Cette fonctionnalité devrait être supprimée de la prévisualisation le 9 janvier 2023. Pour plus d’informations, consultez la page <a href="../23.1-release-activity/23-1-release-overview.md">Vue d’ensemble de la version 23.1.</a> </span></p>
                            </li>
                            <li>
                                <p>Version de production : à déterminer</p>
                            </li>
                        </ul>
                    </td>
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-resource-management-enhancements.md" class="MCXref xref" xrefformat="{para}">Préférences de tri et améliorations de la convivialité dans l’équilibreur de charge de travail</a> </p> <p>Afin d’améliorer votre expérience lors de l’utilisation de l’équilibreur de charge de travail, nous avons introduit les améliorations suivantes : un meilleur tri dans les sections « Non affecté » et « Affecté », une nouvelle présentation des barres de projet, un design actualisé et plus facile à lire pour les dates prévisionnelles, et bien plus encore.</p> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Amélioration des rapports {#reporting-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">Suppression et ajout de champs de budgétisation des ressources dans les listes et les rapports
</a> </p> <p>Afin de refléter les informations sur la budgétisation des ressources provenant du planificateur de ressources, nous avons ajouté un nouveau champ « Heures budgétées du planificateur de ressources » dans les listes et les rapports. Divers champs ont été supprimés des listes et des rapports, car ils font référence à des outils obsolètes qui ont été supprimés de Workfront dans les versions précédentes.</p> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version de prévisualisation : 23 juin 2022<br></p> </li> 
     <li> <p>Version de production : 23 juin 2022</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Intégration d’Adobe Workfront pour Experience Manager Assets</a> </p> <p>Nous sommes heureux d’annoncer que l’intégration d’Adobe Workfront pour Experience Manager Assets est désormais disponible pour Cloud Service.</p>
   <p>Nous avons également introduit de nouvelles fonctionnalités pour Cloud Service et Assets Essentials.</p> </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : S/O<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Combiner plusieurs fichiers en une seule épreuve dans le module externe Creative Cloud</a> </p> <p>Vous pouvez désormais charger des fichiers externes avec le contenu que vous avez créé dans le module externe Adobe Workfront pour Creative Cloud afin de créer des épreuves à plusieurs fichiers dans Workfront. Les fichiers externes apparaissent en tant que pages de l’épreuve supplémentaires dans Workfront. Grâce à cette amélioration, nous avons également mis à jour l’aspect de l’expérience de création d’épreuve.</p> </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : S/O<br></p> </li> 
     <li> <p>Version de production : à déterminer</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
   <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle intégration de SharePoint (API Graph) maintenant disponible</a> </p> <p>Nous avons créé une nouvelle intégration SharePoint plus simple. Désormais, vous n’avez pas besoin de configurer l’intégration de SharePoint. La nouvelle intégration de SharePoint est simplement une option que vous pouvez choisir, comme pour d’autres intégrations de documents.</p>
   <p>L’accès aux documents actuellement liés via l’ancienne intégration SharePoint ne sera pas perdu. Cependant, vous ne pourrez pas lier de nouveaux documents par le biais de l’intégration héritée.</p>
   <p>Les administrateurs et les administratrices de Workfront peuvent activer et désactiver séparément les intégrations SharePoint et SharePoint héritées, en fonction des besoins de leur entreprise.</p> </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations de l’application mobile de relecture</a> </p> <p>L’application mobile Adobe Workfront vous permet désormais d’afficher les pièces jointes aux commentaires des épreuves et d’ajouter de nouvelles pièces jointes. Vous pouvez joindre des fichiers de type image, document ou vidéo.</p> </td>
   <td> <p><b>Disponible à ces dates :</b> </p> 
   <p>Vous pouvez également taguer d’autres utilisateurs et d’autres utilisatrices de l’épreuve dans les commentaires et les réponses. Toute personne que vous taguez reçoit une notification par e-mail.</p>
    <ul> 
     <li> <p>Version préliminaire : S/O<br></p> </li> 
     <li> <p>Version de production : disponible dans Apple App Store et Google Play Store de mi-juillet à fin juillet 2022.</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Mise à jour des feuilles de temps</a> </p> <p>Nous continuons à améliorer et à mettre à jour votre expérience lorsque vous utilisez des feuilles de temps. </p> </td>
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Mises à jour de l’aspect pendant la période de la version 22.3</a> </p> <p>Des mises à jour mineures de l’aspect des différentes zones de l’application sont effectuées pendant la période de la version 22.3. Ces améliorations seront disponibles dans l’environnement de production au moins deux semaines après le lancement de la version préliminaire.</p> </td>
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version de prévisualisation : pendant toute la période de la version 22.3<br></p> </li> 
     <li> <p>Version de production : au moins 2 semaines après la publication dans l’environnement de prévisualisation (sauf indication contraire)</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Activer la rotation automatique des jetons d’actualisation dans vos applications OAuth2 personnalisées</a></p> <p>Pour vous permettre de mieux contrôler la sécurité de vos applications OAuth2 personnalisées, nous avons ajouté une option permettant d’activer la rotation du jeton d’actualisation. Lorsque cette option est activée, chaque fois qu’un jeton d’actualisation est utilisé, votre application crée et envoie automatiquement un nouveau jeton d’actualisation, puis désactive l’ancien.</p> <p>Votre application doit stocker le nouveau jeton d’actualisation après chaque actualisation. Workfront ne stocke pas ce jeton d’actualisation.</p> <p>Auparavant, les jetons d’actualisation expiraient après un délai défini configuré dans les paramètres personnalisés de l’application OAuth2.</p> </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 5 mai 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Utiliser PKCE dans vos intégrations OAuth2 personnalisées pour les applications web d’une seule page</a></p> <p>Vous pouvez désormais créer des applications web d’une seule page dans vos intégrations personnalisées à l’aide de PKCE. PKCE est un flux d’autorisation sécurisé qui fonctionne bien avec les applications à actualisation dynamique, telles que les applications mobiles, mais qui est utile pour tous les clients OAuth2. Au lieu d’utiliser un secret client statique, PKCE emploie une chaîne générée dynamiquement, éliminant ainsi le risque de fuite d’un secret client.</p> <p>Auparavant, les options disponibles pour les applications OAuth2 personnalisées utilisaient le nom et le mot de passe d’un utilisateur ou d’une utilisatrice ou un secret client.</p> </td> 
   <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 5 mai 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>La nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent du calendrier de la version 22.3. Pour plus d’informations sur les dernières fonctionnalités, consultez la section [Activité Version d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

## Améliorations du planificateur de scénarios Workfront

Il n’y a pas de mise à jour du planificateur de scénarios à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Améliorations de Workfront Proof

Il n’y a pas de mise à jour de Workfront Proof à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of November 29, 2021</a>.</p>
-->

## Améliorations des Objectifs Workfront

Il n’y a pas de mise à jour des Objectifs Workfront à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## Version 14 de l’API

Pour la version 14 de l’API, nous avons modifié certaines ressources et certains points d’entrée. Certains des changements prennent en charge de nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de la version 14 de l’API](../../../wf-api/api/new-api-version-14.md).

Pour plus d’informations sur les versions de l’API, voir [Calendrier des versions et de la prise en charge de l’API](../../../wf-api/api/api-version-support-schedule.md).

## Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version 22.3, consultez la section [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/fr/docs/workfront-known-issues/releases/current-updates).

## Webinaire sur la version 22.3

Le webinaire de la version 22.3 a été présenté le 23 juin 2022. Vous pouvez visionner son enregistrement [ici](https://webinars.on24.com/adobe_workfront/whatsnew223?partnerref=WF1).
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Workfront 22.2 Release Webinar will be presented on March 24, 2022 at 8:00 a.m. MST. You can register for the event on the <a href="https://webinars.on24.com/adobe_workfront/WF22point2?partnerref=WFOne" target="_blank">Events page on Workfront One</a>.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This area will be updated as more information becomes available.
</MadCap:conditionalText>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
was presented on January 12, 2022. You can view the webinar recording on the
<a href="https://one.workfront.com/s/event">Events page on Workfront One</a>.
</MadCap:conditionalText>
</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, voir la [page Mise à jour des versions de formation](https://experienceleague.adobe.com/fr/docs/workfront-learn/tutorials-workfront/home).

## Fonctionnalités n’étant plus prises en charge

### Internet Explorer 11

Avec la suppression de la prise en charge d’Internet Explorer, Workfront prend désormais officiellement en charge Microsoft Edge.

Pour plus d’informations sur les navigateurs pris en charge, voir [Configuration requise pour le navigateur Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).
