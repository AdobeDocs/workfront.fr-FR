---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Déplacement d’objets d’un environnement à un autre dans Workfront
description: La fonctionnalité Promotion de l’environnement est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Il ne prend pas en charge la possibilité de déplacer des objets transactionnels (à quelques exceptions près).
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: 5d84d50b8984bbff7bbc02ffc0ce86ec1f486742
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 1%

---

# Présentation du déplacement d’objets entre les environnements Workfront (promotion d’environnement)

La fonctionnalité de promotion de l’environnement est destinée à permettre de déplacer des objets d’un environnement Workfront vers un autre. Par exemple, vous pouvez créer un modèle et le configurer dans votre environnement de test, tout en sachant que les tests que vous effectuez n’auront aucune incidence sur les données réelles de votre entreprise. Une fois le modèle configuré et testé, vous pouvez le déplacer vers votre environnement de production, prêt à l’emploi.

Ce processus est appelé &quot;promotion de l’environnement&quot;.

Vous pouvez effectuer ce processus dans Workfront en créant un package d’objets à déplacer, puis en installant ce package dans le nouvel environnement.

* Pour obtenir des instructions spécifiques sur l’exécution de ce processus dans Workfront, voir :

   * [Créer ou modifier un package de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Installer un package de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Pour obtenir des instructions sur l’exécution de ce processus via l’API Workfront, voir [Déplacer des objets entre [!DNL Workfront] à l’aide des [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

## Objets pris en charge pour la promotion de l’environnement

La fonctionnalité Promotion de l’environnement est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Il ne prend pas en charge la possibilité de déplacer des objets transactionnels (à quelques exceptions près).

* [Objets de travail](#work-objects)
* [Objets de création de rapports](#reporting-objects)
* [Objets de données personnalisés](#custom-data-objects)
* [Objets d’organisation](#organization-objects)
* [Autres objets de configuration](#other-configuration-objects)


### Objets de travail

| Objet Promotable | Objets liés promotionnels inclus |
| --- | --- |
| Projet (PROJ) | Projet<br>Tâche<br>Attribution<br>Prédécesseur<br>Société<br>Taux de remplacement<br>Groupe<br>Rôle<br>Équipe<br>Processus d’approbation<br>Chemin d’approbation<br>Étape de validation<br>Approbateur d’étape<br>Planification<br>Jour sans travail<br>Définition de la file d&#39;attente<br>Groupe de rubriques de la file d’attente<br>Rubrique de la file d’attente<br>Règle de routage<br>Chemin Milestone<br>Milestone<br>Type d’heure<br>Pool de ressources<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories |
| Modèle (TMPL) | Modèle<br>Tâche du modèle<br>Attribution de tâches de modèle<br>Prédécesseur de tâche de modèle<br>Société<br>Taux de remplacement<br>Groupe<br>Rôle<br>Équipe<br>Processus d’approbation<br>Chemin d’approbation<br>Étape de validation<br>Approbateur d’étape<br>Planification<br>Jour sans travail<br>Définition de la file d&#39;attente<br>Groupe de rubriques de la file d’attente<br>Rubrique de la file d’attente<br>Règle de routage<br>Chemin Milestone<br>Milestone<br>Type d’heure<br>Pool de ressources<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories |

### Objets de création de rapports

| Objet Promotable | Objets liés promotionnels inclus |
| --- | --- |
| Modèle de mise en page (UITMPL) | Modèle de mise en page<br>Tableau de bord<br>Calendrier<br>Section Calendrier<br>Page externe<br>Rapport<br>Filtrer<br>Regroupement<br>Affichage<br>Paramètre |
| Tableau de bord (PTLTAB) | Tableau de bord<br>Calendrier<br>Section Calendrier<br>Page externe<br>Rapport<br>Filtrer<br>Regroupement<br>Affichage<br>Paramètre |
| Calendrier (CALENDE) | Calendrier<br>Section Calendrier |
| Page externe (EXTSEC) | Page externe |
| Rapport (PTLSEC) | Rapport<br>Filtrer<br>Regroupement<br>Affichage<br>Paramètre |
| Filtre (UIFT) | Filtrer<br>Paramètre |
| Regroupement (UIGB) | Regroupement<br>Paramètre |
| Vue (UIVW) | Affichage<br>Paramètre |

### Objets de données personnalisés

| Objet Promotable | Objets liés promotionnels inclus |
| --- | --- |
| Catégorie (CTGY) | Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories<br>Groupe |
| Paramètre (PARAM) | Paramètre<br>Option de paramètre |
| Groupe de paramètres (PGRP) | Groupe de paramètres |

### Objets d’organisation

| Objet Promotable | Objets liés promotionnels inclus |
| --- | --- |
| Groupe (GROUP) | Groupe <br>Sous-groupes (jusqu’à 5 niveaux) *<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories |
| Rôle (RÔLE) | Rôle |
| Equipe (EQUIPE) | Équipe<br>Groupe |
| Société (CMPY) | Société<br>Taux de remplacement<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Paramètre <br>Logique d’affichage des catégories<br>Groupe |
| Portfolio (PORT) | Portfolio<br>Programme<br>Groupe<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories |
| Programme (PRGM) | Programme<br>Portfolio<br>Groupe<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage des catégories |

### Autres objets de configuration

| Objet Promotable | Objets liés promotionnels inclus |
| --- | --- |
| Processus d’approbation (ARVPRC) | Processus d’approbation<br>Chemin d’approbation<br>Étape de validation<br>Approbateur d’étape<br>Rôle<br>Équipe<br>Groupe |
| Planification (SCHED) | Planification<br>Jour sans travail<br>Groupe |
| Chemin Milestone (MPATH) | Chemin Milestone<br>Milestone |
| Profil de feuille de temps (TSPRO) | Profil de feuille de calcul<br>Type d’heure |
| Type d’heure (HEURE) | Type d’heure |
| Type de dépense (EXPTYP) | Type de frais |
| Type de risque (RSKTYP) | Type de risque |
| Pool de ressources (RSPL) | Pool de ressources |

\* Non disponible actuellement


## Statuts de promotion d’environnement

Les packages de promotion d’environnement passent par plusieurs états lorsqu’ils sont créés et préparés pour se déplacer entre les environnements. Vous pouvez voir ces états dans votre liste de packages dans Workfront ou dans les réponses de l’API si vous utilisez l’API Workfront.

Ces statuts sont les suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>ASSEMBLAGE</td> 
   <td><p>Cet état est automatiquement attribué lors de l’assemblage des objets. </p><p>L’assemblage fait référence au processus automatisé d’identification des objets et des sous-objets à inclure dans un package et d’ajout de ces objets et de leurs données au package.</p><p>Cet état ne peut pas être défini directement par un client.</p></td> 
  </tr> 
  <tr> 
   <td>version préliminaire</td> 
   <td><p>Ce statut est attribué à la fin d’un processus d’assemblage ou lors de la création d’un package de promotion vide.</p><p>Il est possible pour un client de replacer le package de promotion dans ce statut.</p><p>Dans cet état, le package de promotion ne peut être installé dans aucun environnement.</p></td> 
  </tr> 
  <tr> 
   <td>TEST</td> 
   <td><p>Ce statut permet d’installer un package de promotion dans n’importe quel environnement de test Aperçu ou Actualisation personnalisée. Dans cet état, le package ne peut pas être installé dans Production.</p></td> 
  </tr> 
  <tr> 
   <td>ACTIF</td> 
   <td><p>Ce statut permet d’installer un package de promotion dans n’importe quel environnement, y compris Production.</p><p>Lorsque l’état d’un module est défini sur ACTIF, la variable <code>publishedAt</code> date est automatiquement définie sur l’horodatage actuel de la requête.</p></td> 
  </tr> 
  <tr> 
   <td>DISABLED</td> 
   <td><p>Ce statut sera utilisé pour masquer les packages de promotion précédemment utilisés qui ne seront plus installés dans aucun environnement à l’avenir.</p><p>Lorsqu’un package est dans cet état, il ne peut être installé dans aucun environnement.</p><p>Lorsque l’état d’un package est défini sur DISABLED, la variable <code>retiredAt</code> date est automatiquement définie sur l’horodatage actuel de la requête.</p><p>Il est recommandé d’utiliser ce statut plutôt que d’utiliser la variable<code>DELETE /package</code> point d’entrée, car il est récupérable et l’historique d’installation est conservé pour tous les déploiements effectués avec ce package.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Le package de promotion est automatiquement placé dans ce statut si l'étape ASSEMBLEMENT échoue.</p><p>Pour renvoyer le package à l'étape ASSEMBLEMENT, vous devez relancer le processus d'extraction.</p></td> 
  </tr> 
  </tbody> 
</table>
