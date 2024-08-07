---
content-type: release-notes
keywords: notes,trimestriel,mise à jour
navigation-topic: 2021-4-release-activity
title: Vue d’ensemble de la version 21.4
description: Cette page fournit des informations sur les fonctionnalités d’Adobe Workfront Classic et de la nouvelle expérience Adobe Workfront incluse dans la version 21.4. pour vous aider à déverrouiller la productivité et la collaboration.[Une ligne de conduite marketing pour la version]
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0897b269-c6f3-4b63-8956-b7f9fbe0a553
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '4717'
ht-degree: 3%

---

# Vue d’ensemble de la version 21.4

Cette page fournit des informations sur les fonctionnalités d’Adobe Workfront Classic et de la nouvelle expérience Adobe Workfront incluse dans la version 21.4.

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
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 21.4 release nears its planned Production release the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 21.4.</p>
-->

Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 4 octobre 2021.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of October 4, 2021
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
,
</MadCap:conditionalText>
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
unless otherwise specifiedthe week of May 10, 2021.
</MadCap:conditionalText>


For specific release dates and times for each cluster, see the [Adobe Workfront status page](https://status.adobe.com/en/products/5943) on [status.adobe.com](http://status.adobe.com/). You must log in to see specific release times.

-->

## Améliorations Adobe Workfront

* [Améliorations de l’administrateur](#administrator-enhancements)
* [Améliorations pratiques](#agile-enhancements)
* [Améliorations apportées au projet](#project-enhancements)
* [Améliorations de la gestion des ressources](#resource-management-enhancements)
* [Améliorations du reporting](#reporting-enhancements)
* [Améliorations des requêtes](#requests-enhancements)
* [ Améliorations de la vérification](#proofing-enhancements)
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#for" class="MCXref xref" xrefformat="{para}">Pour les administrateurs : voir les groupes associés à un processus d’approbation</a> </p> <p>Pour vous aider à déterminer les groupes qui sont associés aux processus de validation de votre système, nous avons ajouté une colonne Nom de groupe à la vue Standard sur la page Validations de la configuration. Vous pouvez désormais afficher ces informations sans avoir à créer une vue personnalisée.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouveau pour les administrateurs : les groupes peuvent configurer leurs propres préférences de feuille de temps et d’heure</a> </p> <p>Dans une grande entreprise, certains groupes peuvent avoir besoin de configurer les préférences de la feuille de temps et de l’heure indépendamment pour s’adapter à leurs workflows uniques, plutôt que d’hériter des préférences configurées par un administrateur au niveau du système. Désormais, les administrateurs de Workfront peuvent déverrouiller les préférences de feuille de temps et d’heure pour tous les groupes du système afin de pouvoir les configurer eux-mêmes.</p> <p>Cette fonctionnalité a également été ajoutée récemment pour les préférences de projet et de tâche et de problème.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4 <span style="color: #ff0000;"> (initialement disponible en production uniquement pour les clients sur la grappe 4)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nouveau pour les administrateurs de Workfront : Configuration de modèles de mise en page pour les utilisateurs à configuration automatique dans la nouvelle expérience Workfront</a> </p> <p>Vous pouvez maintenant configurer des modèles de mise en page dans la nouvelle expérience Workfront pour les utilisateurs avec mise en service automatique. Dans le menu déroulant Attribut utilisateur Workfront, dans lequel vous mappez les attributs utilisateur (Configuration &gt; Système &gt; Authentification unique), un nouvel élément de menu "Nouveau modèle de mise en page" est désormais disponible pour effectuer cette configuration. Auparavant, vous pouviez configurer des modèles de mise en page pour les utilisateurs avec approvisionnement automatique uniquement dans Workfront Classic.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Le nouveau champ affiche les groupes auxquels vos utilisateurs appartiennent</a> </p> <p>Il est maintenant facile de déterminer à quels groupes vos utilisateurs appartiennent. Dans un rapport ou une vue qui répertorie les utilisateurs, vous pouvez créer une colonne à l’aide du nouveau champ Autres groupes . Ce champ répertorie les groupes auxquels chaque utilisateur est membre.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">La page de détails des plans directeurs affiche désormais une image</a> </p> <p>La page de détails de chaque plan directeur affiche désormais une image du modèle de projet installé avec le plan directeur. L’image fournit un aperçu du contenu du plan directeur afin que vous sachiez ce que vous êtes sur le point d’installer. Vous pouvez éventuellement prévisualiser l’image complète dans le navigateur ou télécharger l’image.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">Préférences de plans directeurs pour les nouveaux problèmes</a> </p> <p>De nouvelles préférences de problème sont désormais disponibles pour certains plans directeurs. Ils sont installés par défaut, mais vous pouvez choisir de ne pas installer les préférences lorsque vous configurez les détails de l’installation.</p> <p>Les préférences incluent les groupes de rubriques de la file d’attente, les rubriques de la file d’attente et les règles de routage pour collecter les informations correctes lorsqu’un problème ou une requête est envoyé, et envoyer le problème ou la requête au rôle de tâche ou à l’équipe appropriée. L’utilisation des préférences permet de créer une cohérence dans la manière dont les nouveaux problèmes ou requêtes sont capturés sur vos projets.</p> <p>Notez que l’utilisation de ces préférences ne fait pas des projets créés à partir du modèle des files d’attente de requêtes.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Nouveau pour les administrateurs de groupe : affichez et gérez les éléments récemment supprimés et restaurés d’un groupe</a> </p> <p>Nous continuons à faciliter la gestion de vos groupes et de leurs objets associés au même endroit. Vous pouvez désormais afficher et utiliser les éléments récemment supprimés et restaurés d’un groupe dans la zone Groupes . Cela vous évite d’avoir à accéder à la zone Récemment supprimés ou Récemment restaurés dans Configuration pour gérer ces éléments. Et il conserve la liste des éléments de groupe avec lesquels vous travaillez séparément des autres éléments supprimés et restaurés dans le système.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 26 août 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">Nouveau pour les administrateurs de groupe : les préférences de groupe affectent désormais les modèles de groupe</a> </p> <p>Il est désormais plus facile de vous assurer que les modèles de projet de votre groupe répondent aux besoins de votre groupe. Lorsque vous attribuez un nouveau modèle de projet à un groupe au moment de sa création, celui-ci hérite de divers paramètres issus des préférences de projet et de tâche du groupe.</p> <p>Lorsque vous créez une tâche de modèle dans un modèle de projet associé à un groupe, la tâche de modèle hérite de divers paramètres des préférences de tâche du groupe.</p> <p>Auparavant, les modèles de projet et les tâches de modèle de projet héritaient de ces paramètres des préférences de projet et de tâche définies au niveau du système.</p> <p>Si vous créez une tâche de modèle ou de modèle sans groupe (par exemple, à partir de la page Modèles principale), les paramètres ci-dessus sont hérités des préférences de projet et de tâche au niveau du système. Cependant, si vous attribuez par la suite un groupe à la tâche de modèle ou de modèle, les préférences du groupe ne l’affectent pas.</p> </td> 
   <td> <p>Version d’aperçu : 26 août 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new6" class="MCXref xref" xrefformat="{para}">Nouveau pour les administrateurs : découvrez quels formulaires personnalisés utilisent un champ personnalisé</a> </p> <p>Il est désormais plus facile de modifier un champ personnalisé dans un formulaire personnalisé. En un seul clic dans le formulaire personnalisé, vous pouvez découvrir d’autres formulaires personnalisés qui utilisent également le champ . Il est important d’évaluer si ces formulaires devront être ajustés afin de continuer à fonctionner correctement après avoir apporté la modification.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 19 août 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new7" class="MCXref xref" xrefformat="{para}">Nouveau pour les administrateurs de groupe : verrouillage et déverrouillage des préférences de projet, de tâche et de problème pour un groupe</a> </p> <p>Vous pouvez désormais vous assurer que tous les membres de votre groupe et de ses sous-groupes utilisent le même paramètre pour un projet, une tâche ou une préférence de problème. Une fois qu’un administrateur Workfront a déverrouillé une préférence au niveau du système, vous pouvez la configurer, puis la verrouiller pour votre groupe. Bien que vous puissiez toujours reconfigurer une préférence de groupe verrouillé, les administrateurs des sous-groupes inférieurs ne peuvent pas le faire séparément pour leurs groupes.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 12 août 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new8" class="MCXref xref" xrefformat="{para}">Nouveau pour les administrateurs de groupe : créer et modifier des modèles à partir de la zone Groupes</a> </p> <p>Nous continuons à faciliter la gestion de vos groupes et de leurs objets associés au même endroit. Vous pouvez désormais afficher et utiliser les modèles d’un groupe à partir de la zone Groupes de la section Configuration. Cela vous évite d’avoir à accéder à la zone Modèles pour gérer les modèles d’un groupe. Et il conserve la liste des modèles de groupe sur lesquels vous travaillez séparément des autres dans tout le système.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 12 août 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#enter" class="MCXref xref" xrefformat="{para}">Saisissez et enregistrez des informations dans un formulaire personnalisé joint à la fois</a> </p> <p>Il est désormais plus facile de fournir des informations dans la section Détails pour un objet : saisissez et enregistrez les informations dans un champ personnalisé unique ou une zone extensible (comme Aperçu et Finance), même si les champs requis dans d’autres formulaires personnalisés de l’objet ne sont pas encore remplis.</p> <p>Auparavant, lorsque vous saisissiez des informations dans un formulaire personnalisé ou une zone extensible pour un objet, tous les formulaires personnalisés associés à l’objet étaient passés en mode d’édition et tous leurs champs obligatoires devaient être renseignés avant que vous puissiez enregistrer vos modifications. Il s’agissait d’un problème si vous ne pouviez pas remplir un champ obligatoire, car il était destiné à un autre utilisateur.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 22 juillet 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new9" class="MCXref xref" xrefformat="{para}">Nouveau pour les administrateurs de groupe : créer et gérer des états pour un groupe à n’importe quel niveau</a> </p> <p>Afin de faciliter la gestion et le contrôle indépendants des workflows pour tous les niveaux d’une organisation, nous avons introduit la possibilité de créer et de gérer des états pour les sous-groupes. </p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 3 juin 2021 (durant le cycle de publication 21.3)<br></p> <p>Version de production : 22 juillet 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#new10" class="MCXref xref" xrefformat="{para}">Nouveau pour les administrateurs de Workfront : migrez vous-même les modèles de mise en page de Workfront Classic vers la nouvelle expérience Workfront</a> </p> <p>Pour vous aider à gérer les modèles de mise en page pendant que vos utilisateurs passent à l’utilisation de la nouvelle expérience Workfront, nous avons créé un bouton que vous pouvez utiliser pour migrer les modèles de mise en page de Workfront Classic vers la nouvelle expérience sans faire appel au service clientèle de Workfront.</p> <p>Auparavant, seul le service clientèle de Workfront pouvait migrer vos modèles de mise en page de Workfront Classic vers la nouvelle expérience Workfront.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 1er juillet 2021<br></p> <p>Version de production : 15 juillet 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-admin-enhancements.md#when" class="MCXref xref" xrefformat="{para}">Lors de l’association d’un modèle à un groupe, sélectionnez un processus d’approbation de groupe dans Détails de la file d’attente et Rubriques de la file d’attente</a> </p> <p>Nous avons ajouté une nouvelle option au processus d’association d’un modèle à un groupe. Vous pouvez désormais sélectionner des processus d’approbation spécifiques à un groupe pour les problèmes dans les détails de la file d’attente du modèle ou dans l’une de ses rubriques de file d’attente.</p> <p>Dans la version 21.3, lorsque nous avons ajouté la possibilité d’associer un modèle de groupe à un groupe, vous pouvez sélectionner un processus d’approbation spécifique au groupe dans le modèle, mais vous ne pouvez pas le faire dans les détails de la file d’attente ou les rubriques de la file d’attente du modèle.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 1er juillet 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#include" class="MCXref xref" xrefformat="{para}">Inclure des images dans les mises à jour</a> </p> <p>Dans l’onglet Mises à jour d’un objet, vous pouvez désormais ajouter des images en cliquant sur l’icône Image de la barre d’outils. Vous pouvez également faire glisser et déposer une image dans la zone de mise à jour. Notez que votre administrateur Workfront doit activer l’ajout d’images avant que l’icône Image ne s’affiche.</p> <p>Vous pouvez ajouter des images dans les mises à jour et les réponses. Une miniature d’image dans la mise à jour indique que les destinataires peuvent prévisualiser l’image dans le navigateur ou la télécharger, et les notifications par e-mail et in-app indiquent que les images sont jointes à la mise à jour.</p> <p>Auparavant, le seul moyen de partager une image dans Workfront était de la joindre à un objet en tant que document. Les images ajoutées sous l’onglet Mises à jour ne sont disponibles que dans cet onglet et non dans l’onglet Documents .</p> <p>Pour que les utilisateurs de Workfront puissent inclure des images dans les mises à jour, cette fonctionnalité doit d’abord être activée par l’administrateur Adobe Workfront.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">Algorithme mis à jour pour les affectations intelligentes</a> </p> <p>Nous avons amélioré l’algorithme utilisé lors d’affectations intelligentes. Grâce à cette nouvelle amélioration, Workfront examine les 30 affectations les plus récentes effectuées par l’utilisateur connecté afin d’effectuer des suggestions lorsqu’il affecte des tâches et des problèmes. La liste de suggestions peut contenir jusqu’à 50 utilisateurs. </p> <p>Avant cette amélioration, Workfront prenait en compte les affectations sur les tâches parents et d’autres attributs utilisateur associés à ces affectations lors de la suggestion d’utilisateurs.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de la création d’un projet à partir d’un modèle</a> </p> <p>Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface de création d’un projet à partir d’un modèle. La fonctionnalité de création d’un projet à l’aide d’un modèle n’a pas changé. Toutefois, voici quelques améliorations apportées à cette nouvelle interface :</p> 
    <ul> 
     <li> <p>Prévisualiser les informations du modèle avant de les joindre</p> </li> 
     <li> <p>Ajouter des modèles à une liste de favoris pendant le processus de création du projet</p> </li> 
    </ul> <p>Nous avons mis à jour l’interface de création du projet, à la fois lorsque vous le créez à partir des projets et de la zone Modèles .</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de l’association de modèles à des projets</a> </p> <p>Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface permettant de joindre un modèle à un projet. La fonctionnalité d’association d’un modèle n’a pas changé. Certaines des améliorations apportées à cette nouvelle interface ont été apportées :</p> 
    <ul> 
     <li> <p>Prévisualiser les informations du modèle avant de les joindre</p> </li> 
     <li> <p>Ajouter des modèles à une liste de favoris pendant le processus de pièce jointe</p> </li> 
     <li> <p>Afficher toutes les options de gestion des paramètres de modèle et de projet sur une page continue</p> </li> 
    </ul> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 26 août 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#unified" class="MCXref xref" xrefformat="{para}"> Valeurs unitaires de durée et durée unifiées pour les tâches </a> </p> <p>Pour une expérience utilisateur plus propre et plus simple, nous avons fusionné la valeur du champ Durée avec l’unité de temps de durée. Avant cette amélioration, l’unité de temps s’affichait dans un champ déroulant distinct après le champ Durée .</p> <p>Outre les champs Durée des zones Détails de la tâche, Modifier les tâches et Nouvelle tâche, nous mettons également à jour les champs suivants pour qu’ils correspondent à cette expérience :</p> 
    <ul> 
     <li> <p>Champ Durée lors d’affectations avancées</p> </li> 
     <li> <p>Champ de délai d'ajustement lors de la création ou de la modification d'une tâche</p> </li> 
     <li> <p>Champ Fréquence lors de la création d'une tâche récurrente (disponible prochainement)</p> </li> 
     <li> <p>Champ de libellé lors de l’ajout d’un prédécesseur (disponible prochainement)</p> </li> 
    </ul> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 19 août 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#disable" class="MCXref xref" xrefformat="{para}">Désactiver l’ajout de problèmes en ligne sur les projets</a> </p> <p>Pour vous assurer que les utilisateurs fournissent des informations précises lors de l’ajout de problèmes à des projets en remplissant un formulaire de problèmes, nous avons introduit un nouveau paramètre qui vous permet de gérer s’ils peuvent ajouter des problèmes à un projet ou à ses tâches intégrées. Ce paramètre est activé par défaut dans la nouvelle zone Paramètres du problème de la boîte de dialogue Modifier le projet . La désactivation réduit l’option Ajouter d’autres problèmes de la section Problèmes d’un projet afin que les utilisateurs ne puissent pas ajouter d’autres problèmes dans la liste. Les utilisateurs peuvent toujours ajouter des problèmes aux projets à l’aide de l’option Nouveau problème de la section Problèmes ou à l’aide d’une file d’attente de demandes si celle-ci est configurée pour le projet.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 5 août 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-project-enhancements.md#custom" class="MCXref xref" xrefformat="{para}">Amélioration de l’affichage des champs personnalisés pour les cases à cocher et les boutons radio</a> </p> <p>L’affichage et la sélection des options de cases à cocher et de boutons radio dans les formulaires personnalisés sont devenus plus simples : un champ personnalisé avec de nombreuses options de cases à cocher ou de boutons radio s’affiche désormais dans plusieurs colonnes sur la page. Auparavant, ils s’affichaient dans une seule colonne, ce qui nécessitait un défilement supplémentaire pour les utilisateurs qui remplissaient le formulaire.</p> <p>Cela dépend de la position des champs dans le formulaire personnalisé. Si vous placez un autre champ dans la même ligne avec la case à cocher ou le champ de bouton radio, les options peuvent n’avoir qu’un espace horizontal suffisant pour s’afficher dans une seule colonne.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 29 juillet 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#make" class="MCXref xref" xrefformat="{para}">Effectuer des affectations rapides dans l’équilibreur de charge de travail</a> </p> <p>Vous pouvez désormais équilibrer efficacement les ressources de l’équilibreur de charge de travail avec un minimum de clics en faisant glisser un élément de la zone Non affecté et en le déposant sur la ligne d’un utilisateur dans la zone Affecté. À l’aide du glisser-déposer, vous pouvez également annuler l’affectation d’éléments à des utilisateurs et les déplacer à nouveau vers la zone Non affecté, ainsi que les déplacer vers d’autres utilisateurs. </p> <p>Avant cette amélioration, vous ne pouviez affecter des éléments qu’en cliquant sur le menu Plus d’une tâche ou d’un problème, puis en utilisant l’option Attribuer . Désormais, les Heures planifiées allouées à l’utilisateur sont mises à jour en temps réel tout en faisant glisser les tâches.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouvelle option par défaut pour l’équilibreur de charge de travail</a> </p> <p>Dans le cadre de nos efforts pour abandonner la planification et rendre l’outil principal d’affectation des ressources de l’équilibreur de charge de travail Workfront obsolète, nous avons fait de l’équilibreur Workfront l’option par défaut pour tous les nouveaux utilisateurs. Actuellement, l’option Planification est l’option par défaut. Cette modification s’applique à toutes les zones dans lesquelles vous pouvez accéder à la Planification, y compris la zone Ressource (dans la nouvelle expérience Adobe Workfront) ou la zone Personnes (dans Adobe Workfront Classic), ainsi qu’au niveau du projet et de l’équipe.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-resource-management-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nouvelle expérience de filtrage dans l’équilibreur de charge de travail</a> </p> <p>Nous avons repensé l’expérience de filtrage dans l’équilibreur de charge de travail afin d’inclure les fonctionnalités supplémentaires suivantes :</p> 
    <ul> 
     <li> <p>Interface utilisateur plus simple et plus rationalisée qui correspond à la nouvelle expérience Workfront</p> </li> 
     <li> <p>Champs supplémentaires par lesquels vous pouvez filtrer</p> </li> 
     <li> <p>Possibilité de dupliquer un filtre</p> </li> 
     <li> <p>Partage de filtres avec d'autres utilisateurs</p> </li> 
    </ul> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 16 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations rapides {#agile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#user" class="MCXref xref" xrefformat="{para}">Affectations d’utilisateurs sur les panoramas Kanban et Scrum</a> </p> <p>Nous avons mis à jour les fiches d'information sur les panoramas Kanban et Scrum afin de faciliter l'affectation d'un utilisateur à l'histoire. Vous pouvez désormais cliquer sur l’avatar d’une équipe ou d’un utilisateur pour ajouter une attribution lorsque la carte d’article est développée. Auparavant, vous deviez localiser et cliquer sur une icône plus distincte.</p> </td> 
   <td> <p>Version d’aperçu : 9 septembre 2021 <br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Configurer la manière dont les dates sont appliquées lors de l’ajout d’éléments de travail à une itération Scrum</a> </p> <p>Par défaut, lorsque vous ajoutez un élément de travail à une itération, la Date de début planifiée et la Date de fin planifiée de l’élément de travail sont modifiées pour correspondre aux dates de début et de fin de l’itération. Vous pouvez maintenant choisir de conserver la date de début planifiée et la date de fin planifiée d’origine pour toutes les tâches d’une équipe.</p> <p>Cette option s’applique uniquement aux équipes Scrum et non aux équipes Kanban.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#changes" class="MCXref xref" xrefformat="{para}">Modifications de l’affichage agile sur les projets</a> </p> <p>Dans le cadre de la version 21.3, nous avons apporté des améliorations à l’en-tête de carte agile et aux panoramas d’histoires (voir la section <a href="../../../product-announcements/product-releases/21.3-release-activity/21-3-project-enhancements.md#agile" class="MCXref xref" xrefformat="{para}"> En-tête de carte agile et mises à jour du panorama d’histoires</a>). Ces mises à jour s’appliquaient aux itérations ainsi qu’à la vue agile des projets.</p> <p>Avec la version 21.4, ces améliorations ont été apportées à l’affichage agile des projets. Aucune modification n’est apportée aux itérations agiles.</p> <p>Voici les modifications qui sont annulées concernant l’affichage agile sur les projets :</p> 
    <ul> 
     <li> <p>Les cartes d’histoire et les colonnes de tableau ont des largeurs ajustables.</p> </li> 
     <li> <p>Les colonnes n’ont pas d’ombrage en arrière-plan.</p> </li> 
     <li> <p>Les cartes ne comportent pas de libellés d’identifiant (article parent, sous-tâche, article, tâche ou problème).</p> </li> 
     <li> <p>La colonne Article parent a été renommée Articles.</p> </li> 
    </ul> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 16 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-agile-enhancements.md#add" class="MCXref xref" xrefformat="{para}"> Ajoutez de nouveaux articles et problèmes à partir du panorama Kanban </a> </p> <p>Vous pouvez maintenant créer un article ou un problème directement à partir du panorama de Kanban. Cela facilite l’ajout rapide d’un nouvel article sans avoir à accéder à un projet, un rapport ou un tableau de bord pour créer une tâche.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 22 juillet 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouveau look et nouvelle ambiance pour le champ Affectations dans les listes et rapports mis à jour</a> </p> <p>Pour correspondre à l’aspect moderne d’autres zones de la nouvelle expérience Workfront, le style du champ Affectations a été modifié dans les listes et les rapports mis à jour. La reconception comprend une nouvelle icône de rôle de tâche, une nouvelle icône de personnes pour les affectations avancées, une nouvelle icône d’accès restreint, etc.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu de Beta : 8 avril 2021 (avec la version 21.2)<br></p> <p>Version de production : 15 juillet 2021<span class="uitext" style="color: #dc143c;"> (initialement publiée en production avec la version 21.2)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-reporting-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nouveau look et nouvelle ambiance pour les champs de type anticipé dans les listes et les rapports mis à jour</a> </p> <p>Pour correspondre à l’aspect moderne d’autres zones de la nouvelle expérience Workfront, la mise en forme des champs de saisie anticipée a été modifiée dans les listes et les rapports mis à jour. Ces modifications comprennent diverses améliorations.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu de Beta : 8 avril 2021 (avec la version 21.2)<br></p> <p>Version de production : 15 juillet 2021 <span class="uitext" style="color: #dc143c;"> (initialement publiée en production avec la version 21.2)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations des requêtes {#requests-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">La recherche améliorée pour les requêtes inclut désormais des caractères spéciaux</a> </p> <p>Afin de faciliter et accélérer la recherche des files d’attente de demandes lors de l’envoi de demandes, nous avons amélioré l’algorithme de recherche pour trouver désormais les files d’attente pouvant contenir des caractères spéciaux.</p> <p>Par exemple, vous pouvez trouver une file d’attente de requêtes nommée "*Workfront" en saisissant "*Workfront" ou "Workfront" dans le champ Type de requête.</p> <p>Tous les caractères spéciaux sont pris en charge.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 9 septembre 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-requests-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouvelle apparence des files d’attente de requêtes incorporées dans la nouvelle expérience Workfront</a> </p> <p>Pour conserver l’aspect nécessaire à l’envoi des requêtes identiques partout dans la nouvelle expérience Workfront, nous avons repensé l’interface permettant d’ajouter des requêtes à une file d’attente de requêtes incorporée. Avant cette amélioration, l’interface d’ajout de requêtes d’un tableau de bord correspondait à l’environnement Workfront Classic.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 26 août 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Améliorations de la vérification {#proofing-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Fonctionnalité</strong> </p> </td> 
   <td> <p><strong>Dates de publication et environnements</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-proofing-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Amélioration des capacités de vérification pour les réviseurs et les demandeurs</a> </p> <p>Pour offrir une expérience plus intégrée entre Workfront et BAT, nous avons apporté plusieurs améliorations aux fonctionnalités de vérification pour les réviseurs et les demandeurs :</p> 
    <ul> 
     <li> <p>Vous pouvez accorder des rôles de modérateur ou d’auteur à n’importe quel utilisateur de Workfront, qu’il dispose d’une licence de vérification, en lui accordant des droits supplémentaires, comme l’application d’actions ou la résolution de commentaires.</p> </li> 
     <li> <p>Vous pouvez ajouter des réviseurs et des demandeurs aux BAT qui nécessitent une connexion ou qui doivent être signés électroniquement.</p> </li> 
     <li> <p>Tous les utilisateurs bénéficient également d’une meilleure connectivité entre Workfront et BAT. Désormais, lorsque vous désactivez un utilisateur ou mettez à jour son adresse électronique, vos mises à jour sont correctement répercutées dans la vérification lorsqu’elles sont modifiées dans Workfront.</p> </li> 
    </ul> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 5 août 2021 <br></p> <p>Version de production : avec la version 21.4 <span class="uitext" style="color: #dc143c;"> (supprimée de l’aperçu et de la production le 20 octobre 2021. Disponible initialement uniquement pour les clients EMEA entièrement intégrés. Cette fonctionnalité sera réintroduite pour tous les clients ultérieurement.)</span></p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#link" class="MCXref xref" xrefformat="{para}">Lier des documents de Dropbox Business</a> </p> <p>Nous avons ajouté Dropbox Business en tant qu’intégration de document disponible. Vous pouvez désormais accéder aux documents que vous avez stockés dans Dropbox Business directement depuis Workfront.</p> <p>Dropbox Business vous permet de lier des documents partagés et de télécharger des documents vers des dossiers partagés. Dropbox (et non Dropbox Business) permet uniquement au propriétaire des documents d’afficher le document dans Workfront.</p> <p>Votre administrateur Workfront peut activer cette intégration pour votre organisation.</p> </td> 
   <td> <p><b>Disponible sur ces dates :</b> </p> <p>Aperçu de la version : S.O.<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Mises à jour de Workfront pour Slack</a> </p> <p>Les mises à jour suivantes sont désormais visibles dans l’intégration Workfront for Slack :</p> <p>L’intégration Workfront for Slack a désormais une nouvelle apparence. En outre, vous recevez désormais votre Workfront pour les notifications de Slack en temps réel. </p> <p>Par exemple, si vous êtes affecté à une tâche, vous recevez cette notification dès que vous êtes affecté. </p> <p>Auparavant, il pouvait y avoir un délai avant que la notification n’apparaisse en Slack.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 29 juillet 2021<br></p> <p>Version de production : 29 juillet 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#more" class="MCXref xref" xrefformat="{para}">Pour plus d’informations sur l’accès au compte lors de l’obtention du consentement aux intégrations Adobe Workfront, voir les détails</a> </p> <p>Les écrans de consentement pour les intégrations Adobe Workfront sont désormais mis à jour. Vous pouvez désormais voir les actions et les zones spécifiques auxquelles les intégrations ont accès, afin de mieux comprendre ce à quoi vous accordez l’accès à l’intégration ou à l’application.</p> <p>Ce nouvel écran de consentement s’applique à toute intégration Adobe Workfront qui utilise OAuth 2.0. </p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 29 juillet 2021<br></p> <p>Version de production : 29 juillet 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-integration-enhancements.md#api" class="MCXref xref" xrefformat="{para}"> L’authentification de clé API n’est plus nécessaire pour les intégrations</a> </p> <p>Les intégrations Workfront ont récemment commencé à utiliser OAuth2 pour une sécurité et une convivialité plus grandes. Dans le cadre de ce déplacement, Workfront ne nécessite plus de clés d’API pour l’authentification des intégrations.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 5 août 2021<br></p> <p>Version de production : 5 août 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> <p>Nouvelle expérience Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#review" class="MCXref xref" xrefformat="{para}">Vérifier et approuver les bons à tirer dans l’application mobile</a> </p> <p>L’application mobile Adobe Workfront affiche désormais toutes les validations de BAT qui vous ont été attribuées, dans votre liste de validations dans Mon travail. Vous pouvez consulter un document de BAT directement dans l’application et prendre une décision à ce sujet.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Aperçu de la version : S.O.<br></p> <p>Version de production : semaine du 11 octobre 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Boutique d’applications iOS</p> </li> 
     <li> <p>Boutique d’applications Android</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-mobile-enhancements.md#create" class="MCXref xref" xrefformat="{para}"> Créez une requête à partir de la zone d'accueil de l'application mobile </a> </p> <p>Vous pouvez désormais créer une requête à partir de la zone d’accueil dans l’application mobile Adobe Workfront. Appuyez sur le bouton "Ajouter" dans la barre de navigation flottante pour afficher une option Request en plus de Task (Demande). Auparavant, vous deviez accéder à la page Demandes pour créer une requête.</p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Aperçu de la version : S.O.<br></p> <p>Version de production : 4 août 2021</p> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Boutique d’applications iOS</p> </li> 
     <li> <p>Boutique d’applications Android</p> </li> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.4-release-activity/21-4-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Nouveaux raccourcis clavier pour mettre en retrait et mettre en retrait dans les listes</a> </p> <p>Pour offrir une expérience accessible à tous les utilisateurs système et respecter les principes de navigation standard du clavier, les commandes de retrait/retrait du clavier ont été modifiées. </p> <p>Pour Mac, appuyez sur Option + &gt; pour mettre en retrait un élément de liste et sur Option + &lt; pour mettre en retrait. </p> <p>Pour Windows, appuyez sur Alt + &gt; pour mettre un élément de liste en retrait et sur Alt + &lt; pour le retrait négatif.</p> <p>Auparavant, le raccourci clavier pour mettre en retrait dans une liste était Tab et la mise en retrait était Maj + Tab. Toutefois, l’utilisation de la touche de tabulation pour mettre en retrait et mettre en retrait rendait impossible la possibilité de passer d’un champ actif à l’autre dans l’interface.</p> <p>Cette modification s’applique uniquement aux listes mises à jour et non aux listes héritées. </p> </td> 
   <td><strong>Disponible sur ces dates :</strong> <p>Version d’aperçu : 12 août 2021<br></p> <p>Version de production : avec la version 21.4</p> <p><strong>Disponible dans ces environnements :</strong> </p> 
    <ul> 
     <li> <p>Nouvelle expérience Adobe Workfront </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent du calendrier de version 21.4. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Améliorations du planificateur de scénarios Workfront

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are no Scenario Planner updates at this point in the release. This area will be updated when updates are available.</p>
-->

De nouvelles fonctionnalités sont disponibles dans la version 21.4 de Workfront Scenario Planner. Pour plus d’informations sur ces nouvelles fonctionnalités désormais disponibles dans Aperçu, voir [Activité de publication du planificateur de scénario Adobe Workfront](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof enhancements</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-may-17.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of May 17, 2021</a>.</p>
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

## Webinaire sur la version 21.4

Le webinaire sur la version 21.4 de Workfront a été présenté le 23 septembre 2021. Vous pouvez afficher l’enregistrement du webinaire à partir de la page [Événements sur Workfront One](https://one.workfront.com/s/event).

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
