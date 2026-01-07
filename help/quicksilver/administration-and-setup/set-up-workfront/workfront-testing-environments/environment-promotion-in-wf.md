---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Déplacement d’objets d’un environnement à un autre dans Workfront
description: La fonctionnalité Promotion environnementale est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Elle ne permet pas de déplacer des objets transactionnels (à quelques exceptions près).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 50%

---

# Vue d’ensemble du déplacement d’objets entre les environnements Workfront (promotion environnementale)

La fonctionnalité de promotion d’environnement vous permet de déplacer des objets d’un environnement Workfront à un autre. Par exemple, vous pouvez créer un modèle et le configurer dans votre environnement de sandbox, en sachant que les tests que vous effectuez n’affecteront pas les données réelles de votre organisation. Une fois le modèle configuré et testé, vous pouvez le déplacer vers votre environnement de production, prêt à l’emploi.

Ce processus est appelé « promotion de l’environnement ».

Vous pouvez effectuer ce processus dans Workfront en créant un package d’objets à déplacer, puis en installant ce package dans le nouvel environnement.

* Pour obtenir des instructions spécifiques sur l’exécution de ce processus dans Workfront, voir :

   * [Créer ou modifier un package de promotion environnementale](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Installer un package de promotion environnementale](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Pour obtenir des instructions sur l’exécution de ce processus par le biais de l’API Workfront, voir [Déplacer des objets entre  [!DNL Workfront]  environnements à l’aide de l’API  [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3429735/){target=_blank}

## Objets pris en charge pour la promotion environnementale

La fonctionnalité de promotion d’environnement est destinée à fournir la possibilité de déplacer des objets liés à la configuration d’un environnement à un autre. Il s’agit d’objets qui peuvent être configurés, tels que des projets, des équipes ou des formulaires personnalisés.

Étant donné que la promotion d’environnement traite de la configuration des objets, les objets transactionnels (objets qui changent fréquemment ou qui dépendent fortement du cas d’utilisation) ne sont pas inclus. Les documents, les événements, les demandes, les mises à jour et les décisions liées aux épreuves sont des exemples d’objets transactionnels.

* [Objets de travail](#work-objects)
* [Objets de création de rapports](#reporting-objects)
* [Objets de données personnalisées](#custom-data-objects)
* [Objets d’organisation](#organization-objects)
* [Autres objets de configuration](#other-configuration-objects)


### Objets de travail

| Objet pouvant être promu | Objets liés pouvant être promus inclus |
| --- | --- |
| Projet (PROJ) | Projet<br>Tâche<br>Affectation<br>Tâche antérieure<br>Entreprise<br>Taux de remplacement<br>Groupe<br>Rôle<br>Équipe<br>Processus d’approbation<br>Chemin d’approbation<br>Étape d’approbation<br>Approbateur ou approbatrice d’étape<br>Planning<br>Jour non ouvrable<br>Définition de file d’attente<br>Groupe de rubriques de file d’attente<br>Rubrique de file d’attente<br>Règle de transmission<br>Chemin jalonné<br>Jalon<br>Type d’heure<br>Groupe de ressources<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories |
| Modèle (TMPL) | Modèle<br>Tâche de modèle<br>Affectation de tâches de modèle<br>Tâche de modèle antérieure<br>Entreprise<br>Taux de remplacement<br>Groupe<br>Rôle<br>Équipe<br>Processus d’approbation<br>Chemin d’approbation<br>Étape d’approbation<br>Approbateur ou approbatrice d’étape<br>Planning<br>Jour non ouvrable<br>Définition de file d’attente<br>Groupe de rubriques de file d’attente<br>Rubrique de file d’attente<br>Règle de transmission<br>Chemin jalonné<br>Jalon<br>Type d’heure<br>Groupe de ressources<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories |

### Objets de création de rapports

| Objet pouvant être promu | Objets liés pouvant être promus inclus |
| --- | --- |
| Modèle de mise en page (UITMPL) | Modèle<br>Tableau De Bord<br>Calendrier<br>Section Calendrier<br>Page Externe<br>Rapport<br>Filtrer<br>Regroupement<br>Vue<br>Paramètre<br>Groupe De Mises En Page |
| Tableau de bord (PTLTAB) | Tableau de bord<br>Calendrier<br>Section du calendrier<br>Page externe<br>Rapport<br>Filtre<br>Regroupement<br>Vue<br>Paramètre |
| Calendrier (CALEND) | Calendrier<br>Section du calendrier |
| Page externe (EXTSEC) | Page externe |
| Rapport (PTLSEC) | Rapport<br>Filtre<br>Regroupement<br>Vue<br>Paramètre |
| Filtre (UIFT) | Filtre<br>Paramètre |
| Regroupement (UIGB) | Regroupement<br>Paramètre |
| Vue (UIVW) | Vue<br>Paramètre |

### Objets de données personnalisées

| Objet pouvant être promu | Objets liés pouvant être promus inclus |
| --- | --- |
| Catégorie (CTGY) | Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories<br>Groupe |
| Paramètre (PARAM) | Paramètre<br>Option de paramètre |
| Groupe de paramètres (PGRP) | Groupe de paramètres |

### Objets d’organisation

| Objet pouvant être promu | Objets liés pouvant être promus inclus |
| --- | --- |
| Groupe (GROUP) | Groupe <br>Sous-groupes (jusqu’à 5 niveaux)*<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories |
| Rôle (ROLE) | Rôle |
| Équipe (TEAM) | Équipe<br>Groupe |
| Entreprise (CMPY) | Entreprise<br>Taux de remplacement<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Paramètre<br>Logique d’affichage des catégories<br>Groupe |
| Portfolio (PORT) | Portfolio<br>Programme<br>Groupe<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories |
| Programme (PRGM) | Programme<br>Portfolio<br>Groupe<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories |

### Autres objets de configuration

| Objet pouvant être promu | Objets liés pouvant être promus inclus |
| --- | --- |
| Processus d’approbation (ARVPRC) | Processus d’approbation<br>Chemin d’approbation<br>Étape de validation<br>Approbateur ou approbatrice d’étape<br>Rôle<br>Équipe<br>Groupe |
| Planning (SCHED) | Planning<br>Jour non ouvrable<br>Groupe |
| Chemin jalonné (MPATH) | Chemin jalonné<br>Jalon |
| Profil de feuille de temps (TSPRO) | Profil de feuille de temps<br>Type d’heure |
| Type d’heure (HOURT) | Type d’heure |
| Type de dépense (EXPTYP) | Type de frais |
| Type de risque (RSKTYP) | Type de risque |
| Groupe de ressources (RSPL) | Pool de ressources |
| Niveau d’accès (ACSLVL) | Niveau d’accès |
| Carte tarifaire (RTCRD) | Carte tarifaire |
| Emplacement / Classificateur (CLSF) | Emplacement / Classificateur |
| Règles métier (BNRUL) | Règles métier |

\* Non disponible actuellement

<!--

>[!NOTE]
>
>Actions (ignore, select existing, and create new) are available on the following objects:
>
>* Role
>* Team
>* Company
>* Group

-->

## Statuts de promotion d’environnement

Les packages de promotion d’environnement passent par plusieurs statuts lorsqu’ils sont créés et préparés à passer d’un environnement à l’autre. Ces statuts apparaissent dans la liste des packages de Workfront ou dans les réponses de l’API si vous utilisez l’API Workfront.

Ces statuts sont les suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>NON ASSEMBLÉ</td> 
   <td><p>Ce statut est automatiquement attribué et représente un package qui a été enregistré mais pas encore assemblé. </p><p>Ce statut ne peut pas être défini directement par un utilisateur.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING</td> 
   <td><p>Ce statut est automatiquement attribué lors de l’assemblage des objets. </p><p>L’assemblage fait référence au processus automatisé d’identification des objets et des sous-objets à inclure dans un package et d’ajout de ces objets et de leurs données au package.</p><p>Ce statut ne peut pas être défini directement par un utilisateur.</p></td> 
  </tr> 
  <tr> 
   <td>DRAFT</td> 
   <td><p>Ce statut est attribué à la fin d'un processus d'assemblage ou lors de la création d'un package de promotion vide.</p><p>Il est possible pour un utilisateur ou une utilisatrice de ramener le package de promotion à ce statut.</p><p>Tant que vous disposez de ce statut, le package de promotion ne peut être installé dans aucun environnement.</p></td> 
  </tr> 
  <tr> 
   <td>TESTING</td> 
   <td><p>Ce statut permet d’installer un package de promotion dans n’importe quel sandbox de prévisualisation ou à actualisation personnalisée. Tant que vous disposez de ce statut, le package ne peut pas être installé en production.</p></td> 
  </tr> 
  <tr> 
   <td>ACTIVE</td> 
   <td><p>Ce statut permet d’installer un package de promotion dans n’importe quel environnement, y compris l’environnement de production.</p><p>Lorsque le statut d’un package est défini sur ACTIVE, la date <code>publishedAt</code> est automatiquement définie sur l’horodatage actuel de la requête.</p></td> 
  </tr> 
  <tr> 
   <td>DISABLED</td> 
   <td><p>Ce statut est utilisé pour masquer les packages de promotion utilisés précédemment qui ne seront plus installés dans aucun environnement à l’avenir.</p><p>Lorsqu’un package a ce statut, il ne peut être installé dans aucun environnement.</p><p>Lorsque le statut d’un package est défini sur DISABLED, la date <code>retiredAt</code> est automatiquement définie sur l’horodatage actuel de la requête.</p><p>L’utilisation de ce statut est recommandée par rapport à l’utilisation du point d’entrée <code>DELETE /package</code>, car il est récupérable et l’historique d’installation est conservé pour tous les déploiements effectués avec ce package.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Le package de promotion est automatiquement placé dans ce statut si l’étape ASSEMBLING échoue.</p><p>Pour renvoyer le package à l'étape ASSEMBLAGE, vous devez déclencher à nouveau le processus d'assemblage.</p><p>Pour plus d’informations sur l’assemblage d’un package, voir la section <a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package">Modifier ou assembler un package existant</a> dans l’article Créer ou modifier un package de promotion d’environnement.</td> 
  </tr> 
  </tbody> 
</table>

## Ressources

* Pour les questions fréquentes concernant la promotion de l’environnement, voir [FAQ sur la promotion de l’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-faq.md)
* Pour obtenir des recommandations de dépannage, voir [&#x200B; Dépannage de la promotion de l’environnement &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-troubleshooting.md)


