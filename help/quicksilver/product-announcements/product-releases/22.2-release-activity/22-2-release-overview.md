---
title: Vue d’ensemble de la version 22.2
description: Vue d’ensemble de la version 22.2
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: e490a955-b2cb-4b9b-9794-12ff2a2c2338
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '3973'
ht-degree: 8%

---

# Vue d’ensemble de la version 22.2

Cette page fournit des informations sur les fonctionnalités incluses dans la version 22.2. Toutes les fonctionnalités répertoriées sont disponibles dans la nouvelle expérience Adobe Workfront. Certaines fonctionnalités sont également disponibles dans Adobe Workfront Classic. Toutefois, [Workfront Classic sera interrompu en mars 2022](https://one.workfront.com/s/new-workfront-experience), suivi de la date de fin de vie de Workfront Classic en juillet 2022.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
to help you unlock productivity and collaboration.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 22.2 release nears its planned Production release later this year
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
the week of January 17, 2022
</MadCap:conditionalText>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 22.2. </p>
-->

Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 4 avril 2022.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment and will be made available in the Production environment
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
later this year
</MadCap:conditionalText>
the week of April 4, 2022, unless otherwise specified. For specific release dates and times for each cluster, see the <a href="https://status.adobe.com/en/products/5943" target="_blank">Adobe Workfront status page</a> on <a href="http://status.adobe.com/" target="_blank">status.adobe.com</a>. You must log in to see specific release times. </p>
-->

## Améliorations Adobe Workfront

* [Améliorations de l’administrateur](#administrator-enhancements)
* [Améliorations apportées au projet](#project-enhancements)
* [Améliorations de la gestion des ressources](#resource-management-enhancements)
* [Améliorations de l’accueil](#home-enhancements)
* [ Améliorations mobiles ](#mobile-enhancements)
* [Améliorations des intégrations](#integrations-enhancements)
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configurer un formulaire personnalisé pour qu’il fonctionne avec plusieurs types d’objets</a> </p> <p>Vous pouvez maintenant configurer un formulaire personnalisé nouveau ou existant pour qu’il fonctionne avec plusieurs types d’objets, ce qui rend le formulaire beaucoup plus utile. Les utilisateurs pourront joindre et remplir le formulaire sur les objets de tous les types pour lesquels vous le configurez.</p> <p>Auparavant, vous pouviez configurer un formulaire personnalisé pour qu’il fonctionne avec un seul type d’objet.</p> <p>Cette fonctionnalité fonctionne avec tous les formulaires personnalisés créés précédemment dans votre système Workfront. Par exemple, si vous disposez déjà d’un formulaire personnalisé créé pour le type d’objet Tâche , vous pouvez maintenant le configurer pour qu’il fonctionne avec d’autres types d’objets, tels que Projet et Problème.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}"> Le catalogue de plans directeurs est disponible pour tous les utilisateurs et les administrateurs peuvent autoriser les requêtes</a> </p> <p>Tous les utilisateurs d’Adobe Workfront peuvent désormais parcourir le catalogue des plans directeurs disponibles. </p> <p>En outre, l’administrateur système peut permettre aux utilisateurs de demander l’installation de plans directeurs. L’affectation d’une file d’attente de requêtes pour stocker les requêtes permet aux utilisateurs d’effectuer des requêtes à partir du catalogue de plans directeurs. </p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#add" class="MCXref xref" xrefformat="{para}">Ajouter une image à un formulaire personnalisé</a> </p> <p>Dans un formulaire personnalisé que vous créez ou modifiez, vous pouvez désormais ajouter une image et inclure une info-bulle informative ou instructive que les utilisateurs peuvent lire lorsqu’ils la survolent.</p> <p>Cela peut s’avérer utile, par exemple, pour afficher l’identité graphique d’un nouveau produit ou pour fournir des informations visuelles dont les utilisateurs ont besoin lorsqu’ils remplissent le formulaire.</p> <p>Auparavant, les formulaires personnalisés étaient entièrement basés sur du texte.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#deactiva" class="MCXref xref" xrefformat="{para}">Désactiver un groupe</a> </p> <p>À mesure que vos organisations internes changent, vous devrez peut-être cesser d’utiliser certains groupes dans Workfront et en créer de nouveaux. Pour faciliter cette opération, nous avons ajouté la possibilité de désactiver un groupe sans perdre ses données historiques. Pour les utilisateurs réguliers qui n’ont pas besoin de les voir, les groupes inactifs sont effacés des champs de type anticipé de groupe.</p> <p>Vous pouvez toujours rechercher et configurer des options, des préférences et des associations d’objets pour les groupes inactifs que vous gérez. Et la désactivation d'un groupe ne change rien aux objets auxquels il est attaché.</p> <p>Auparavant, il n’était pas possible de désactiver un groupe.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouvelles configurations de niveau d’accès par défaut</a> </p> <p>Pour mieux répondre aux besoins de la plupart des administrateurs qui créent des niveaux d’accès, nous avons modifié la configuration par défaut de plusieurs des options "Ajuster vos paramètres" qui s’affichent lorsque vous cliquez sur l’icône d’engrenage d’un bouton Modifier.</p> <p>Les options, précédemment activées par défaut, sont désormais désactivées. Si cela ne correspond pas aux besoins de votre entreprise, vous pouvez les activer lorsque vous configurez un nouveau niveau d’accès, ou ultérieurement.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 27 janvier 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic sera interrompu en mars 2022 </a>, suivi de la date de fin de vie de Workfront Classic en juillet 2022).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">Améliorations de l’historique d’installation des plans directeurs</a> </p> <p>Lorsque vous installez un plan directeur, un message affiche désormais les objets spécifiques (tels que les rôles, les équipes ou les groupes) qui ont été correctement installés avec le plan directeur et les objets qui n’ont pas pu être installés. Vous pouvez également afficher la liste des objets installés sur la page Détails du plan directeur en cliquant sur Afficher les détails en regard d’une installation spécifique dans le tableau de l’historique d’installation.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 février 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#a" class="MCXref xref" xrefformat="{para}">Un avertissement s’affiche maintenant lors de l’installation d’un plan directeur Aperçu uniquement dans Production</a> </p> <p>Certains plans directeurs ne peuvent être installés que dans l’environnement Aperçu à des fins de test.</p> <p>Si vous accédez au contenu Aperçu uniquement dans votre environnement de production, sandbox 1 ou sandbox 2, le bouton d’installation n’est pas actif et un message d’avertissement peut s’afficher.</p> </td> 
   <td><b>Disponible sur ces dates :</b> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 février 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">Les panoramas Adobe Workfront sont désormais disponibles ! </a> </p> <p>Les panoramas sont des outils flexibles qui permettent la collaboration des équipes en permettant d’accéder à un panorama partagé contenant des colonnes et des cartes. </p> <p>Les panoramas vous permettent de configurer rapidement un tableau de tâches avec plusieurs colonnes, de configurer des colonnes pour afficher un statut ou une catégorie, d’ajouter d’autres utilisateurs au panorama et de les affecter à des cartes, etc.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#addition" class="MCXref xref" xrefformat="{para}">Autres améliorations apportées aux panoramas Workfront</a></p> <p>Les améliorations supplémentaires suivantes sont désormais disponibles pour les panoramas Workfront :</p> 
    <ul> 
     <li> <p>Balisage des cartes sur les panoramas</p> </li> 
     <li> <p>Déplacer des cartes</p> </li> 
     <li> <p>Copie de cartes</p> </li> 
     <li> <p>Recherche dans les panoramas</p> </li> 
     <li> <p>Définition de la date d’échéance d’une carte dans les panoramas</p> </li> 
    </ul> </td> 
   <td><b>Disponible sur ces dates :</b> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 24 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#undo" class="MCXref xref" xrefformat="{para}">Option Annuler pour mettre à jour des publications</a> </p> <p>Il est désormais plus facile de repérer les erreurs lors de la publication d’une mise à jour. La finalisation d’un commentaire dans l’onglet Mise à jour d’un objet crée désormais une fenêtre contextuelle de 7 secondes qui vous permet d’annuler la publication et de revenir à la modification, avant l’horodatage du système ou l’envoi d’emails et de notifications in-app. Si vous ignorez la fenêtre contextuelle, quittez la page ou patientez 7 secondes pendant l’expiration de la fenêtre, la publication est effectuée normalement.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de la copie d’un projet</a> </p> <p>Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Adobe Workfront, nous avons repensé l’interface pour la copie de projets. Cette option est actuellement disponible lors de la copie d’un projet à partir de la page du projet ou lors de la copie d’un projet à partir d’une liste ou d’un rapport. Avant cette mise à jour, vous ne pouviez copier qu’un projet à partir de la page du projet.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#ability" class="MCXref xref" xrefformat="{para}">Possibilité de gérer des projets à partir de listes et de rapports à partir d’un nouveau menu Plus</a> </p> <p>Nous avons ajouté un nouveau menu Plus dans les listes de projets et les rapports pour vous permettre d’effectuer les actions suivantes à partir de ces zones :</p> 
    <ul> 
     <li> <p>Pour plusieurs projets à la fois :</p> </li> 
     <li> <p>Recalculer chronologie</p> </li> 
     <li> <p>Recalculer finances</p> </li> 
     <li> <p>Recalculer les expressions personnalisées</p> </li> 
     <li> <p>Pour un seul projet :</p> </li> 
     <li> <p>Joindre modèle</p> </li> 
     <li> <p>Exporter vers MS Project</p> </li> 
     <li> <p>S'abonner</p> </li> 
    </ul> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de la conversion d’un problème en projet à l’aide d’un modèle au niveau du problème</a> </p> <p>Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface permettant de convertir un problème en projet lors de l’utilisation d’un modèle lorsque vous le convertissez à partir de la page de problèmes.</p> <p>Vous pouvez désormais accéder plus facilement à votre liste de favoris immédiatement après avoir sélectionné pour convertir le problème.</p> <p>L’interface repensée correspond à l’expérience lors de la création d’un projet à partir d’un modèle que nous avons également mis à jour récemment.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : 8 décembre 2021<br></p> </li> 
     <li> <p>Version de production : avec la version 22.1 <span style="color: #ff0000; font-weight: bold;">Cette fonctionnalité a été temporairement supprimée de l’environnement de production le 4 mars 2022. Il a ensuite été lancé dans un déploiement progressif à partir du 28 avril 2022. Le déploiement a été achevé le 5 mai 2022. Cette option est désormais disponible dans Aperçu et Production pour tous les clients.</span></p> </li> 
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
     <li> <p>Version de production : avec la version 22.1 <span style="color: #ff0000; font-weight: bold;">Cette fonctionnalité a été temporairement supprimée de l’environnement de production le 4 mars 2022. Il a ensuite été lancé dans un déploiement progressif à partir du 28 avril 2022. Le déploiement a été achevé le 5 mai 2022. Cette option est désormais disponible dans Aperçu et Production pour tous les clients.</span></p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}"> Expérience mise à jour lors de la copie et du déplacement de problèmes</a> </p> <p>Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Adobe Workfront, nous avons repensé l’interface pour la copie et le déplacement des problèmes. Cette option est actuellement disponible lors de la copie ou du déplacement d’un seul problème ou lors de la copie ou du déplacement de problèmes en masse à partir d’une liste ou d’un rapport.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : samedi 18 février 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#keep" class="MCXref xref" xrefformat="{para}">Conserver les utilisateurs sur le tableau de bord, la liste ou le rapport après la conversion d’un problème en projet</a> </p> <p>Pour accroître l’efficacité et éliminer le nombre de clics, nous avons publié une amélioration lors de la conversion de problèmes en projets à partir d’une liste, d’un rapport ou d’un tableau de bord.</p> <p>Les utilisateurs restent dans la liste, le rapport ou un tableau de bord après avoir converti un problème en projet au lieu d’être redirigés vers la page du projet. Une notification de réussite avec le lien vers le projet s’affiche une fois la conversion terminée, afin que vous puissiez facilement accéder au projet, si nécessaire. </p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 février 2022<br></p> </li> 
     <li> <p>Version de production : 24 février 2022</p> </li> 
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
     <li> <p>Les heures planifiées sont conservées lors de la suppression de tous les cessionnaires. <span style="color: #ff0000;">(Supprimé de la version. Désormais, les heures planifiées seront définies sur 0 après la suppression de tous les cessionnaires.)</span></p> </li> 
    </ul> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 février 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 <span style="color: #ff0000; font-weight: bold;">Cette fonctionnalité sera publiée en production peu de temps après la version 22.2</span></p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic sera interrompu en mars 2022 </a>, suivi de la date de fin de vie de Workfront Classic en juillet 2022).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Partager des dossiers uniquement dans les cinq premiers niveaux d’une hiérarchie de dossiers</a> </p> <p>Afin d’optimiser les performances pour les utilisateurs partageant des dossiers, nous limitons actuellement le partage aux cinq premiers niveaux d’une hiérarchie de dossiers sur un objet.</p> <p>Chaque dossier au sixième niveau ou au-dessous hérite de ses configurations de partage à partir du dossier situé directement au-dessus.</p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Amélioration de la navigation de l’équilibreur de charge de travail</a> </p> <p>Pour améliorer votre expérience lors de l’utilisation de l’équilibreur de charge de travail, nous avons introduit les améliorations suivantes :</p> 
    <ul> 
     <li> <p>Les boutons Annuler et Enregistrer lors de l’ajustement des allocations sont désormais collants, même si la tâche est plus longue que la période incluse à l’écran ou lorsque le panneau Résumé s’affiche.</p> </li> 
     <li> <p>Le panneau de gauche qui affiche les noms des utilisateurs et des éléments de travail est maintenant collant. Il vous permet de faire défiler horizontalement les éléments pendant plus longtemps et de toujours pouvoir lire les noms des éléments répertoriés dans le panneau.</p> </li> 
     <li> <p>Vous pouvez réduire et développer tous les éléments répertoriés dans le panneau de gauche d’un seul clic au lieu de l’utilisateur ou du projet.</p> </li> 
     <li> <p>Le panneau de gauche peut désormais également être redimensionné.</p> </li> 
     <li> <p>Il existe désormais un mode plein écran pour l’équilibreur de charge de travail.</p> </li> 
    </ul> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#access" class="MCXref xref" xrefformat="{para}">Accès aux affectations avancées dans l’équilibreur de charge de travail</a> </p> <p>Pour faciliter l’affectation des tâches et la rendre plus précise, vous pouvez désormais effectuer des affectations avancées lorsque vous attribuez des tâches manuellement dans l’équilibreur de charge de travail. Avant cette amélioration, vous pouviez accéder aux affectations avancées lors de la modification d’éléments, à partir des en-têtes des éléments ou dans des listes.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouvelle formule pour calculer la disponibilité de l’utilisateur lorsque la préférence Planification par défaut est sélectionnée</a> </p> <p>Pour fournir des informations plus précises dans les outils de gestion des ressources, nous avons modifié la formule utilisée par Workfront pour calculer la disponibilité des utilisateurs lorsque l’administrateur de Workfront sélectionne Le planning par défaut dans les préférences de gestion des ressources. Avec la nouvelle mise à jour, Workfront utilise la formule suivante pour calculer la disponibilité de l’utilisateur :</p> <p>Heures disponibles de l’utilisateur = (Heures de planification par défaut - Exceptions) * ETR - Heures de congé</p> <p>Avant cette mise à jour, Workfront utilisait la formule suivante pour calculer la disponibilité de l’utilisateur lorsque la planification par défaut était sélectionnée :</p> <p>Heures disponibles de l’utilisateur = (Heures de planification par défaut - (exceptions de planification + heures de congé) * Valeur de l’éditeur de texte enrichi de l’utilisateur</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic sera interrompu en mars 2022 </a>, suivi de la date de fin de vie de Workfront Classic en juillet 2022).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations de la page d’accueil {#home-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-home-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">Améliorations apportées aux filtres dans la liste de travail à domicile</a> </p> <p>Pour mieux contrôler et se concentrer sur votre liste de travail, nous avons mis en place plusieurs améliorations des filtres dans la zone Accueil . Grâce aux nouvelles améliorations, vous pouvez sélectionner des filtres par type d’objet et affiner davantage vos résultats en fonction de l’état de vos tâches (par exemple, Prêt à démarrer, Travailler ou Demandé). Les nouveaux filtres d’accueil fournissent désormais un nombre correct de tâches, de problèmes, d’éléments de travail personnels et d’approbations lorsque vous appliquez une combinaison de filtres de type d’objet et d’état de l’élément de travail.</p> <p>Avant cette expérience, les filtres de la zone Accueil ne fournissaient pas un décompte précis du nombre d’éléments de travail dans la liste lorsque vous sélectionniez un ou plusieurs filtres, ce qui créait une confusion quant à l’état des éléments de travail.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-mobile-enhancements.md#drawings" class="MCXref xref" xrefformat="{para}">Dessins et commentaires sur les documents de BAT dans l’application mobile</a></p> <p>L’application mobile Adobe Workfront vous permet désormais d’ajouter des dessins et des commentaires sur les documents de BAT. Une nouvelle barre d'outils sur le BAT contient des outils de dessin pour les formes. Vous pouvez choisir des paramètres tels que l’épaisseur de la couleur et de la ligne pour chaque forme. En dessinant une forme sur le BAT, votre commentaire se connecte à cette zone du document du BAT.</p> <p>Vous pouvez également répondre aux commentaires que d'autres ont fait sur le BAT.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Aperçu de la version : S.O.<br></p> </li> 
     <li> <p>Version de production : mi-avril à fin avril 2022 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Application mobile iOS</p> </li> 
     <li> <p>Application mobile Android</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-mobile-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">Améliorations des fonctionnalités de BAT dans l’application mobile</a> </p> <p>Dans l’application mobile Adobe Workfront, vous pouvez désormais :</p> 
    <ul> 
     <li> <p>Partage de BAT avec des destinataires internes et externes</p> </li> 
     <li> <p>Afficher les commentaires du BAT</p> </li> 
     <li> <p>Téléchargement de BAT</p> </li> 
    </ul> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Aperçu de la version : S.O.<br></p> </li> 
     <li> <p>Version de production : début février 2022 (ces améliorations ont été communiquées à l’origine avec la version 22.1.)</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Application mobile iOS</p> </li> 
     <li> <p>Application mobile Android</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations des intégrations {#integrations-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">Adobe Workfront avec intégration Anaplan désormais disponible</a> </p> <p>Pour vous offrir une meilleure flexibilité et une meilleure compréhension des aspects financiers de vos projets Workfront, Workfront peut désormais s’intégrer à votre compte Anaplan. En liant les objets Workfront aux objets Anaplan, vous pouvez mettre à jour automatiquement les informations entre les deux comptes, en vous assurant qu’elles sont à jour et identiques. </p> <p>Vous pouvez également déclencher des processus automatisés dans Anplan en fonction d’actions dans Workfront (ou vice versa).</p> <p>Vous pouvez par exemple créer une campagne dans Anaplan, puis créer un projet ou un programme Workfront lié à la campagne. Tous les coûts suivis dans Workfront peuvent ensuite être transférés à nouveau vers Anaplan pour passer en revue les performances de la campagne.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront pour les mises à jour de connecteur améliorées par Experience Manager</a> </p> <p>Workfront pour le connecteur amélioré Experience Manager comprend désormais les mises à jour suivantes :</p> 
    <ul> 
     <li> <p>Vous pouvez désormais créer des dossiers liés entre Adobe Workfront et Adobe Experience Manager Assets as a Cloud Service même s’il existe plusieurs configurations de dossiers liés à un projet.</p> </li> 
     <li> <p>Ajout de la prise en charge de la pagination des abonnements aux événements</p> </li> 
     <li> <p>Ajout de la prise en charge d’AEM 6.4.x</p> </li> 
     <li> <p>Ajout de la prise en charge des environnements proxy</p> </li> 
     <li> <p>Plusieurs correctifs basés sur les commentaires des partenaires et des clients</p> </li> 
    </ul> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Aperçu de la version : S.O.<br></p> </li> 
     <li> <p>Version de production : mardi 28 mars 2022</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see" class="MCXref xref" xrefformat="{para}">Voir les détails du secret client pour les intégrations OAuth2 ou JWT personnalisées</a> </p> <p>Pour garantir la transparence de l’utilisation de vos intégrations OAuth2 et JWT personnalisées, nous vous avons permis d’afficher les détails des secrets client que vos intégrations utilisent. Vous pouvez maintenant voir les dates de création et d’utilisation du secret client pour la dernière fois. Vous pouvez également ajouter et afficher vos propres notes sur le secret client.</p> <p>Auparavant, ces détails n’étaient pas disponibles.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 3 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe2" class="MCXref xref" xrefformat="{para}">Les intégrations Adobe Creative Cloud utilisent désormais OAuth2</a> </p> <p>Pour une sécurité accrue et pour offrir une expérience plus cohérente entre les intégrations, nous avons mis à jour les intégrations Adobe Creative Cloud afin d’utiliser l’authentification OAuth2, un moyen standard d’authentifier les utilisateurs. Désormais, lorsque vos utilisateurs se connectent, ils peuvent voir les actions et les zones auxquelles les intégrations ont accès et y autoriser l’accès. Après cela, il n’est plus nécessaire de se connecter aussi fréquemment.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 24 février 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see2" class="MCXref xref" xrefformat="{para}">Voir type d’authentification dans la liste des applications OAuth2 personnalisées</a> </p> <p>Désormais, lorsque vous affichez la liste des applications OAuth2 personnalisées dans votre entreprise, vous pouvez voir si chaque application utilise l’authentification de l’utilisateur ou l’authentification du serveur.</p> <p>Auparavant, vous pouviez afficher ces informations uniquement en accédant aux options de modification de chaque application.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 17 février 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#set" class="MCXref xref" xrefformat="{para}">Définition de l’expiration des jetons d’actualisation dans vos intégrations OAuth2 personnalisées</a> </p> <p>Pour mieux contrôler l’accès et la sécurité de vos intégrations OAuth2 personnalisées, vous pouvez désormais personnaliser la durée de vie des jetons d’actualisation. Une fois que le jeton d’actualisation d’un utilisateur expire, il doit se reconnecter à l’intégration.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 février 2022 <br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#use" class="MCXref xref" xrefformat="{para}">Utilisez des clés publiques et privées dans vos intégrations OAuth2 personnalisées pour les applications serveur à serveur</a> </p> <p>Vous pouvez désormais configurer des applications OAuth2 serveur à serveur dans vos intégrations personnalisées. En configurant des clés publiques et privées, vous pouvez permettre à Workfront de communiquer avec une autre application sans utiliser d’informations de connexion.</p> <p>Auparavant, toutes les authentifications de vos applications OAuth2 personnalisées utilisaient les informations de connexion de l’utilisateur.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 février 2022 <br></p> </li> 
     <li> <p>Version de production : avec la version 22.2 </p> </li> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-look-and-feel-updates.md#enhancem" class="MCXref xref" xrefformat="{para}">Mises à jour de l’apparence pendant la période de publication de la version 22.2</a> </p> <p>Des mises à jour mineures de l’aspect des différentes zones de l’application Adobe Workfront sont effectuées dans le délai de publication de la version 22.2. Ces améliorations seront rendues disponibles dans l’environnement de production au moins 2 semaines après la publication de la version de prévisualisation. </p> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Aperçu de la version : pendant toute la période de la version 22.2<br></p> </li> 
     <li> <p>Version de production : au moins 2 semaines après la publication de la version de prévisualisation</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">Améliorations apportées à la barre de navigation supérieure</a> </p> <p>Plusieurs améliorations ont été apportées à la barre de navigation supérieure d’Adobe Workfront.</p> 
    <ul> 
     <li> <p>Les options Favoris et Récents comportent désormais des icônes distinctes dans la barre de navigation supérieure. Chacun d’eux affiche toujours le même contenu (pages que vous avez marquées comme favorites et pages que vous avez récemment consultées), et vous pouvez continuer à ajouter et supprimer des pages favorites de la même manière.</p> </li> 
     <li> <p>L’aspect des pin’s et du menu principal a été mis à jour pour Adobe les normes de conception, notamment les couleurs et les polices. La façon dont vous ajoutez et supprimez des pin's et les zones auxquelles vous avez accès dans le menu principal n’ont pas changé.</p> </li> 
     <li> <p>Les icônes situées à droite de la barre de navigation supérieure ont été réorganisées pour être plus intuitives. L’ordre des icônes est : lien d’aide, notifications, favoris, récents, recherche, menu principal.</p> </li> 
    </ul> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#redesign" class="MCXref xref" xrefformat="{para}">Listes de feuilles de temps reconçues</a> </p> <p>Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Adobe Workfront, nous avons repensé les listes de feuilles de temps dans la zone Fiches horaires. Vous pouvez vous attendre à la même fonctionnalité dans la liste des feuilles de temps, mais seulement avec une expérience utilisateur plus propre et plus rationalisée.</p> <p>Voici quelques-uns des points forts de cette reconception :</p> 
    <ul> 
     <li> <p>La liste de feuilles de temps correspond désormais à l’expérience dans toutes les autres listes de Workfront.</p> </li> 
     <li> <p>L’expérience de filtre correspond désormais aux filtres de toutes les autres listes. Vous disposez d’une plus grande flexibilité pour créer vos propres filtres avec les champs et attributs qui vous conviennent le mieux et les partager avec d’autres utilisateurs.</p> </li> 
    </ul> </td> 
   <td><strong>Disponible sur ces dates :</strong> 
    <ul> 
     <li> <p>Version d’aperçu : vendredi 10 mars 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.2</p> </li> 
    </ul> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent du calendrier de version 22.2. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Améliorations du planificateur de scénarios Workfront

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

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version 22.2, consultez [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=fr).

## Webinaire sur la version 22.2

Le webinaire sur la version 22.2 de Workfront sera présenté le 24 mars 2022 à 8h00 MST. Vous pouvez vous inscrire à l’événement sur la page [Événements sur Workfront One](https://webinars.on24.com/adobe_workfront/WF22point2?partnerref=WFOne).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This area will be updated as more information becomes available.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
was presented on January 12, 2022. You can view the webinar recording on the
<a href="https://one.workfront.com/s/event">Events page on Workfront One</a>.
</MadCap:conditionalText>
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
