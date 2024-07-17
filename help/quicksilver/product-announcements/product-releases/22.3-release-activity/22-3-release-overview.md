---
title: Vue d’ensemble de la version 22.3
description: Vue d’ensemble de la version 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bfc7ce9e-b715-47b7-bab7-2e3540d0da3e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '3220'
ht-degree: 9%

---

# Vue d’ensemble de la version 22.3

Cette page fournit des informations sur les fonctionnalités incluses dans la version 22.3. Toutes les fonctionnalités répertoriées sont disponibles dans la nouvelle expérience Adobe Workfront. Certaines fonctionnalités sont également disponibles dans Adobe Workfront Classic. Toutefois, [Workfront Classic sera interrompu en mars 2022](https://one.workfront.com/s/new-workfront-experience), suivi de la date de fin de vie de Workfront Classic en juillet 2022.

Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 juillet 2022.

## Améliorations Adobe Workfront

* [Améliorations de l’administrateur](#administrator-enhancements)
* [Améliorations apportées au projet](#project-enhancements)
* [Améliorations de la gestion des ressources](#resource-management-enhancements)
* [Améliorations des rapports](#reporting-enhancements)
* [Améliorations de l’intégration](#integration-enhancements)
* [ Améliorations mobiles ](#mobile-enhancements)
* [Autres améliorations](#other-enhancements)

### Améliorations d’administration {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Intégration d’Adobe Workfront à JumpSeat
</a></p></p> <p>Vous pouvez désormais intégrer JumpSeat à Workfront afin de créer des conseils personnalisés et intégrés au produit à l’intention de vos utilisateurs. Pour activer l’intégration, vous devez disposer d’une licence d’entreprise Adobe Workfront et d’un abonnement JumpSeat actif.</p>  
    </td>
    <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Utiliser des états déverrouillés dans un processus de validation
</a></p></p> <p>Cette fonctionnalité a été supprimée de la version de production 22.3. Cette fonctionnalité devrait être mise en production ultérieurement.</p> 
<p>Pour vous permettre de mieux contrôler les processus et les états de validation dans votre système, nous avons rendu possible la création d'un processus de validation basé sur un état système déverrouillé. De plus, vous pouvez désormais déverrouiller tout statut déjà utilisé dans un processus de validation. Auparavant, un état système utilisé dans un processus de validation devait être verrouillé. Cela l’a rendu disponible pour tous les groupes, sans possibilité de le supprimer ou de le renommer, de sorte que les administrateurs de groupes ne puissent pas rationaliser la liste des états de leur groupe en fonction de leurs besoins spécifiques.</p>   
   </td> 
    <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : vendredi 15 septembre 2022</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Paramètres par défaut du BAT déplacés vers Workfront
</a></p></p> <p>Vous pouvez désormais modifier les paramètres de BAT suivants dans la zone de configuration de Workfront :</p> 
<ul>
   <li><p>Paramètres par défaut du BAT</p></li>
   <li><p>Paramètres de décision de BAT</p></li>
   </ul> 
   </td> 
    <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : jeudi 1 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajout d’un fichier PDF à un formulaire personnalisé
</a></p></p> <p>Nous vous aidons à rendre les formulaires personnalisés plus visuels et informatifs grâce aux nouveaux widgets de ressources que vous pouvez ajouter, tels que les images et les vidéos. Vous pouvez maintenant ajouter un lien vers un fichier de PDF à un formulaire personnalisé. Lorsque le formulaire est joint à un objet, les utilisateurs qui l’utilisent peuvent afficher et interagir avec le PDF depuis le formulaire.</p>
   </td> 
    <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}"> L’éditeur de calcul de champ de formulaire personnalisé affiche des informations d’erreur
</a><span style="color: #ff0000; font-weight: bold;"> (Temporairement indisponible)</span></p></p> <p>La modification des calculs pour les champs personnalisés est désormais plus facile avec des informations d’erreur utiles indiquées directement dans le calcul. Lorsque vous créez un champ calculé dans un formulaire personnalisé, les erreurs sont surlignées en rose. Lorsque vous passez le curseur sur la partie mise en surbrillance, une info-bulle s’affiche pour décrire le problème.</p>
    </td> 
    <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 9 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Personnalisation de l’en-tête du projet
</a></p></p> <p>En tant qu’administrateur Workfront ou de groupe, vous pouvez désormais personnaliser les champs qui s’affichent dans l’en-tête d’un projet lorsque vous utilisez un modèle de mise en page.</p>
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
    <td>
    <ul> 
     <li> <p>Version d’aperçu : vendredi 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
   </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Contrôle de la création d’un projet vierge</a></p></p> <p>En tant qu’administrateur système ou de groupe, vous pouvez désormais contrôler si les utilisateurs peuvent créer des projets vierges sans utiliser de modèle. Nous avons ajouté un nouveau paramètre dans la zone Préférences du projet de la configuration, qui vous permet de désactiver la création de projets vierges dans les zones suivantes :</p> 
   <ul>
   <li><p>À partir de l’option Nouveau projet dans une liste de projets</p></li>
   <li><p>Lors de la conversion d’une publication en projet à partir de la page de problèmes</p></li>
   </ul>
   <p>Le nouveau paramètre est "Autoriser les utilisateurs à créer des projets sans utiliser de modèle" et est activé par défaut.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 19 mai 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Désactivation d’un groupe à partir de la page Groupes</a> </p> <p>Récemment, nous avons ajouté la possibilité de désactiver et de réactiver les groupes. Pour rendre cette action plus rapide et plus facile, nous l’avons ajoutée à la page d’un groupe. Maintenant, après avoir cliqué sur le nom d’un groupe pour accéder à sa page, vous pouvez sélectionner le menu Plus <img src="assets/more-icon.png"> en regard du nom du groupe, puis sélectionner Désactiver ou Réactiver.</p> <p>Auparavant, vous pouviez désactiver ou réactiver un groupe uniquement à l’aide de la case à cocher Est actif sur sa page Détails . </p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 14 avril 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajout de vidéos aux formulaires personnalisés</a> </p> <p>Vous pouvez désormais offrir un nouveau mode d’information, d’intérêt visuel et de créativité à un formulaire personnalisé en ajoutant une vidéo. Lorsque le formulaire est joint à un objet, les utilisateurs qui travaillent avec l’objet peuvent lire la vidéo à tout moment.</p> <p>Auparavant, vous pouviez uniquement ajouter des champs textuels et des images à un formulaire personnalisé.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 14 avril 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations des projets {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Délégation de travail en absence du bureau</a></p> <p>Désormais, vous pouvez temporairement déléguer les tâches et les problèmes qui vous sont assignés à d’autres utilisateurs lorsque vous envisagez de quitter le bureau pendant une courte période. Ainsi, votre absence ne devient pas un obstacle à la réalisation de vos travaux.</p> 
   <p>Avant cette amélioration, vous ne pouviez déléguer que les approbations.</p></td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 9 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de la conversion d’un problème en tâche</a></p> <p>Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface pour convertir un problème en tâche.</p> 
   </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 9 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de la conversion d’un problème en projet sans modèle</a></p> <p>Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface pour convertir un problème en projet sans utiliser de modèle.</p> 
   <p>Outre une interface utilisateur mise à jour qui correspond au reste de la nouvelle expérience Workfront, nous avons également ajouté la possibilité de convertir un problème en projets vierges à partir d’une liste ou d’un rapport.</p></td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Balisage intelligent dans le flux de mise à jour</a></p> <p>Nous avons amélioré le balisage des utilisateurs dans le flux de mise à jour lorsque vous créez une mise à jour ou que vous répondez à une mise à jour existante. Désormais, lorsque vous marquez un utilisateur pour l’inclure dans une mise à jour, en plus de son nom et de son avatar, nous affichons également son rôle de Principal et son email. Cela permet de distinguer plusieurs utilisateurs portant des noms similaires ou identiques.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 19 mai 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle syntaxe pour les calculs dans les champs personnalisés</a> </p> <p>Pour vous préparer aux améliorations à venir qui vous aideront à ajouter des calculs aux formulaires personnalisés, nous avons normalisé la syntaxe des champs référencés que vous ajoutez à un calcul. Il est facile d’utiliser cette nouvelle syntaxe car le système la saisit pour vous lorsque vous commencez à saisir le nom d’un champ, puis vous la sélectionnez.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 5 mai 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Conserver des informations précises lorsque deux utilisateurs avec un rôle commun sont impliqués dans un processus d’approbation</a> </p> <p>Afin d’assurer l’exactitude de vos données pour la validation du travail, nous avons apporté une modification à l’enregistrement des informations d’approbation sur un élément lorsqu’un processus d’approbation multirôle est associé à l’élément.</p> <p>Certains processus d’approbation nécessitent l’approbation de deux rôles différents, et deux approbateurs différents peuvent avoir l’un de ces rôles en commun. Maintenant, lorsque cela se produit, une fois les décisions d’approbation prises, Workfront enregistre chaque approbateur et leur rôle respectif associé au processus d’approbation.</p> <p>Avant cette modification, les deux approbations étaient enregistrées pour le deuxième utilisateur, car il partageait l’un des rôles d’approbation avec le premier approbateur. Dans ce cas, le second approbateur remplaçait les informations du premier approbateur.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 21 avril 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic a été abandonné en mars 2022 </a>, suivi de la date de fin de vie de Workfront Classic en juillet 2022).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de la conversion d’un problème en projet à l’aide d’un modèle au niveau du problème</a> </p> <p>Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface permettant de convertir un problème en projet lors de l’utilisation d’un modèle lorsque vous le convertissez à partir de la page de problèmes.</p> <p>Vous pouvez désormais accéder plus facilement à votre liste de favoris immédiatement après avoir sélectionné pour convertir le problème.</p> <p>L’interface repensée correspond à l’expérience lors de la création d’un projet à partir d’un modèle que nous avons également mis à jour récemment.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : 8 décembre 2021<br></p> </li> 
     <li> <p>Version de production : déploiement par phases à partir du 28 avril 2022 <span style="color: #ff0000; font-weight: bold;">Cette fonctionnalité a été temporairement supprimée de l’environnement de production le 4 mars 2022. Il a ensuite été lancé dans un déploiement progressif à partir du 28 avril 2022. Le déploiement a été achevé le 5 mai 2022. Cette option est désormais disponible dans Aperçu et Production pour tous les clients.</span></p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">Convertir des problèmes en projets à l’aide d’un modèle à partir de listes, de rapports et de tableaux de bord</a> </p> <p>Pour accroître l’efficacité de votre travail et faciliter la conversion des problèmes dans un environnement à rythme rapide, nous avons ajouté la possibilité de convertir un problème en projet à l’aide d’un modèle à partir d’une liste, d’un rapport ou d’un tableau de bord.</p> <p>Avant cette amélioration, cette fonctionnalité existait uniquement lorsque vous convertiez le problème à partir de la page de problèmes.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : 8 décembre 2021<br></p> </li> 
     <li> <p>Version de production : déploiement par phases à partir du 28 avril 2022 <span style="color: #ff0000; font-weight: bold;">Cette fonctionnalité a été temporairement supprimée de l’environnement de production le 4 mars 2022. Il a ensuite été lancé dans un déploiement progressif à partir du 28 avril 2022. Le déploiement a été achevé le 5 mai 2022. Cette option est désormais disponible dans Aperçu et Production pour tous les clients.</span></p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#allocati" class="MCXref xref" xrefformat="{para}">Les heures d’affectation ne seront plus supprimées lors de la modification des affectations</a> </p> <p>Pour garantir l’exactitude de vos données, nous avons apporté une modification afin de conserver les heures d’affectation et de conserver les heures planifiées de la tâche inchangées lors de la modification des affectations sur la tâche.</p> <p>Les modifications suivantes ont été apportées aux tâches avec un type de durée simple :</p> 
    <ul> 
     <li> <p>Les affectations d’affectation individuelles sont conservées lors du remplacement des utilisateurs et des rôles.</p> </li> 
     <li> <p>Les affectations d’affectation individuelles sont conservées sur le rôle lors de la suppression de l’utilisateur.</p> </li> 
    </ul> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 février 2022<br></p> </li> 
     <li> <p>Version de production : 21 avril 2022 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic a été abandonné en mars 2022 </a>, suivi de la date de fin de vie de Workfront Classic en juillet 2022).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Partager des dossiers uniquement aux cinq premiers niveaux d’une hiérarchie de dossiers</a> (ce lien renvoie aux notes de mise à jour de la version 20.2, date à laquelle cette fonctionnalité a été introduite pour la première fois dans l’aperçu.)</p> <p>Afin d’optimiser les performances pour les utilisateurs partageant des dossiers, nous limitons actuellement le partage aux cinq premiers niveaux d’une hiérarchie de dossiers sur un objet.</p> <p>Chaque dossier au sixième niveau ou au-dessous hérite de ses configurations de partage à partir du dossier situé directement au-dessus.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 février 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 <span style="color: #ff0000; font-weight: bold;">Cette fonctionnalité est temporairement hors service. Cette page sera mise à jour lorsque la fonctionnalité sera disponible en production.</span></p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic sera interrompu en mars 2022 </a>, suivi de la date de fin de vie de Workfront Classic en juillet 2022).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Campagnes Workfront (Beta)</a> </p>
                        <p>Nous introduisons un nouvel objet dans Adobe Workfront qui a le potentiel de modifier la façon dont vous gérez le travail. </p>
                        <p>Les campagnes Workfront permettent d’organiser dans un nouveau conteneur de travail des projets issus de différents portefeuilles et programmes.
Les campagnes ont été publiées en juillet 2022 dans la version bêta de l’aperçu avec la version 22.3. Pour plus d’informations, voir <a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">22.3 Améliorations du projet</a> </p>
<p>Ce nouveau conteneur va évoluer dans les prochaines versions pour connecter les objets de travail actuellement gérés dans des silos distincts.</p>

</td>
                    <td><span class="bold">Disponible sur ces dates :</span>
                        <ul>
                            <li>
                                <p>Version d’aperçu : durant toute la période de la version 22.4 <br /><span style="color: #ff0000; font-weight: bold;">Cette fonctionnalité devrait être supprimée de la version d’aperçu le 9 janvier 2023. Pour plus d'informations, consultez la <a href="../23.1-release-activity/23-1-release-overview.md">page de présentation des versions 23.1.</a> </span></p>
                            </li>
                            <li>
                                <p>Version de production : à déterminer</p>
                            </li>
                        </ul>
                    </td>
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-resource-management-enhancements.md" class="MCXref xref" xrefformat="{para}">Amélioration des préférences de tri et de la convivialité dans l’équilibreur de charge de travail</a> </p> <p>Afin d’améliorer votre expérience lors de l’utilisation de l’équilibreur de charge de travail, nous avons apporté les améliorations suivantes, notamment un meilleur tri dans les sections Non affecté et Affecté, un nouvel aspect pour les barres de projet, une conception mise à jour et plus facile à lire pour les dates prévues, etc.</p> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations des rapports {#reporting-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}"> Suppression et ajout de champs de budget des ressources dans les listes et les rapports
</a> </p> <p>Pour refléter les informations de budget des ressources du planificateur de ressources, nous avons ajouté un nouveau champ Heures planifiées des planificateurs de ressources aux listes et aux rapports. Divers champs ont été supprimés des listes et des rapports car ils font référence à des outils obsolètes qui ont été supprimés de Workfront dans les versions précédentes.</p> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 23 juin 2022<br></p> </li> 
     <li> <p>Version de production : 23 juin 2022</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Intégration d’Adobe Workfront for Experience Manager Assets</a> </p> <p>Nous sommes heureux d’annoncer que l’intégration d’Adobe Workfront Experience Manager Assets est désormais disponible pour Cloud Service.</p>
   <p>Nous avons également introduit de nouvelles fonctionnalités pour les Cloud Service et les Assets Essentials.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Aperçu de la version : S.O.<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Combiner plusieurs fichiers dans un seul BAT dans le module externe de Creative Cloud</a> </p> <p>Vous pouvez désormais charger des fichiers externes avec le contenu que vous avez créé dans le module externe Adobe Workfront for Creative Cloud afin de créer des bons à tirer à plusieurs fichiers dans Workfront. Les fichiers externes apparaissent en tant que pages de BAT supplémentaires dans Workfront. Grâce à cette amélioration, nous avons également mis à jour l’aspect de l’expérience de création de BAT.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Aperçu de la version : S.O.<br></p> </li> 
     <li> <p>Version de production : à déterminer</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
   <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle intégration SharePoint (API Graph) désormais disponible</a> </p> <p>Nous avons créé une nouvelle intégration SharePoint plus simple. Désormais, vous n’avez pas besoin de configurer l’intégration de SharePoint. La nouvelle intégration de SharePoint est simplement une option que vous pouvez choisir, comme pour d’autres intégrations de documents.</p>
   <p>Vous ne perdrez pas l’accès aux documents actuellement liés par l’intégration SharePoint héritée. Cependant, vous ne pourrez pas lier de nouveaux documents par le biais de l’intégration héritée.</p>
   <p>Les administrateurs de Workfront peuvent activer et désactiver séparément les intégrations SharePoint et SharePoint héritées, en fonction des besoins de leur entreprise.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}"> Améliorations de la vérification dans l’application mobile</a> </p> <p>L’application mobile Adobe Workfront vous permet désormais d’afficher les pièces jointes aux commentaires de BAT et d’ajouter de nouvelles pièces jointes. Les types de fichiers pris en charge pour les pièces jointes sont les images, les documents et les vidéos.</p> </td>
   <td> <p><b>Disponible sur ces dates :</b> </p> 
   <p>Vous pouvez également marquer d’autres utilisateurs de BAT dans les commentaires et les réponses. Toute personne que vous marquez reçoit une notification par courrier électronique.</p>
    <ul> 
     <li> <p>Aperçu de la version : S.O.<br></p> </li> 
     <li> <p>Version de production : disponible dans Apple App Store et Google Play Store de mi-juillet à fin juillet 2022.</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Fiches horaires mises à jour</a> </p> <p>Nous continuons à améliorer et à mettre à jour votre expérience lorsque vous utilisez des feuilles de temps. </p> </td>
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Mises à jour de l’apparence pendant la période de publication de la version 22.3</a> </p> <p>Des mises à jour mineures de l’aspect des différentes zones de l’application sont effectuées dans le délai de publication de la version 22.3. Ces améliorations seront rendues disponibles dans l’environnement de production au moins 2 semaines après la publication de la version de prévisualisation.</p> </td>
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Aperçu de la version : pendant toute la période de la version 22.3<br></p> </li> 
     <li> <p>Version de production : au moins 2 semaines après la publication dans Aperçu (sauf indication contraire)</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Activation de la rotation automatique des jetons d’actualisation dans vos applications OAuth2 personnalisées</a></p> <p>Pour vous permettre de mieux contrôler la sécurité de vos applications OAuth2 personnalisées, nous avons ajouté à l’option permettant d’activer la rotation du jeton d’actualisation. Lorsque cette option est activée, chaque fois qu’un jeton d’actualisation est utilisé, votre application crée et envoie automatiquement un nouveau jeton d’actualisation, puis désactive l’ancien.</p> <p>Votre application doit stocker le nouveau jeton d’actualisation après chaque actualisation. Workfront ne stocke pas ce jeton d’actualisation.</p> <p>Auparavant, les jetons d’actualisation expiraient après un délai défini configuré dans les paramètres personnalisés de l’application OAuth2.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 5 mai 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Utilisation de PKCE dans vos intégrations OAuth2 personnalisées pour les applications web d’une seule page</a></p> <p>Vous pouvez désormais créer des applications web d’une seule page dans vos intégrations personnalisées à l’aide de PKCE. PKCE est un flux d’autorisation sécurisé qui fonctionne bien avec les applications d’actualisation dynamique telles que les applications mobiles, mais qui est utile pour tous les clients OAuth2. Au lieu d’un secret client statique, PKCE utilise une chaîne générée dynamiquement, éliminant ainsi le risque de fuite d’un secret client.</p> <p>Auparavant, les options disponibles pour les applications OAuth2 personnalisées utilisaient le nom et le mot de passe d’un utilisateur ou un secret client.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 5 mai 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.3</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent du calendrier de version 22.3. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Améliorations apportées au planificateur de scénario de travail

Aucune mise à jour du planificateur de scénario n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Améliorations de l’épreuve Workfront

Aucune mise à jour de l’épreuve Workfront n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of November 29, 2021</a>.</p>
-->

## Améliorations des Objectifs Workfront

Aucune mise à jour des Objectifs Workfront n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API version 14

Pour l’API version 14, nous avons modifié certaines ressources et points d’entrée. Certaines des modifications participent à la prise en charge des nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, consultez les [Nouveautés de l’API version 14](../../../wf-api/api/new-api-version-14.md).

Pour plus d’informations sur les versions d’API, consultez [Contrôle de version des API et planification de la prise en charge](../../../wf-api/api/api-version-support-schedule.md).

## Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version 22.3, consultez [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=fr).

## Webinaire sur la version 22.3

Le webinaire de la version 22.3 a été présenté le 23 juin 2022. Vous pouvez afficher l&#39;enregistrement [ici](https://webinars.on24.com/adobe_workfront/whatsnew223?partnerref=WF1).
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

## Mises à jour de formation

Découvrez les dernières mises à jour apportées aux programmes de formation, aux parcours de formation, aux vidéos et aux guides de chaque version de produit Adobe Workfront. Pour plus d’informations, consultez la [page des mises à jour de la version de formation](https://one.workfront.com/s/training-release-updates).

## Fonctionnalité non prise en charge

### Internet Explorer 11

Avec la suppression de la prise en charge d’Internet Explorer, Workfront prend désormais officiellement en charge Microsoft Edge.

Pour plus d’informations sur les navigateurs pris en charge, voir [ Configurations requises des navigateurs Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).
