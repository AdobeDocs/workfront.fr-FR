---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Déplacement d’objets d’un environnement à un autre dans Workfront
description: La fonctionnalité Promotion environnementale vise à permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Elle n’offre pas la possibilité de déplacer des objets transactionnels (à quelques exceptions près).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: e9df34c206dd65ccc2edec00087248eb4ed16f54
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 8%

---

# Vue d’ensemble du déplacement d’objets entre les environnements Workfront (promotion environnementale)

La fonctionnalité de promotion de l’environnement vous permet de déplacer des objets d’un environnement Workfront vers un autre. Par exemple, vous pouvez créer un modèle et le configurer dans votre environnement de test, tout en sachant que les tests que vous effectuez n’auront aucune incidence sur les données réelles de votre entreprise. Une fois le modèle configuré et testé, vous pouvez le déplacer vers votre environnement de production, prêt à l’emploi.

Ce processus est appelé &quot;promotion de l’environnement&quot;.

Vous pouvez effectuer ce processus dans Workfront en créant un package d’objets à déplacer, puis en installant ce package dans le nouvel environnement.

* Pour obtenir des instructions spécifiques sur l’exécution de ce processus dans Workfront, voir :

   * [Créer ou modifier un package de promotion environnementale](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Installer un package de promotion environnementale](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Pour plus d’informations sur l’exécution de ce processus via l’API Workfront, voir [Déplacement d’objets entre  [!DNL Workfront] environnements à l’aide de l’ [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

[Voir une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3429735/){target=_blank}

## Objets pris en charge pour la promotion environnementale

La fonctionnalité de promotion de l’environnement est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Il s’agit d’objets qui peuvent être configurés, tels que des projets, des équipes ou des formulaires personnalisés.

Dans la mesure où la promotion de l’environnement traite de la configuration des objets, les objets transactionnels (objets qui changent fréquemment ou qui dépendent fortement du cas d’utilisation) ne sont pas inclus. Parmi les exemples d’objets transactionnels, citons des documents, des problèmes, des demandes, des mises à jour et des décisions de BAT.

* [Objets de travail](#work-objects)
* [Objets de création de rapports](#reporting-objects)
* [Objets de données personnalisés](#custom-data-objects)
* [Objets d’organisation](#organization-objects)
* [Autres objets de configuration](#other-configuration-objects)


### Objets de travail

| Objet Promotable | Objets liés promotionnels inclus |
| --- | --- |
| Project (PROJ) | Projet<br>Tâche<br>Attribution<br>Predecessor<br>Société<br>Taux de remplacement<br>Groupe<br>Rôle<br>Équipe<br>Processus d’approbation<br>Chemin d’approbation<br>Étape d’approbation<br>Approbateur d’étape<br>Planifier<br>Fête de non-travail<br>Définition de file d’attente<br>Groupe de rubriques<br>Groupe de sujets d’approbation Rubrique De File D’Attente <br>Règle De Routage<br>Chemin Milestone<br>Milestone<br>Type D’Heure<br>Pool De Ressources<br>Catégorie<br>Paramètre De Catégorie<br>Paramètre<br>Groupe De Paramètre<br>Option D’Affichage De Catégorie<br> |
| Template (TMPL) | Tâche de modèle<br>Tâche de modèle<br>Attribution de tâche de modèle<br>Predecessor de tâche de modèle<br>Société<br>Taux de remplacement<br>Groupe<br>Rôle<br>Équipe<br>Processus d’approbation<br>Chemin d’approbation<br>Étape d’approbation<br>Approbateur d’étape<br>Rubrique de file d’attente de non de travail<br> <br>Rubrique de la file d’attente<br>Règle de routage<br>Chemin Milestone<br>Milestone<br>Type d’heure<br>Pool de ressources<br>Catégorie<br>Paramètre de catégorie<br>Paramètre de groupe<br>Option de paramètre<br>Logique d’affichage de catégorie<br><br><br> |

### Objets de création de rapports

| Objet Promotable | Objets liés promotionnels inclus |
| --- | --- |
| Modèle de mise en page (UITMPL) | Modèle de mise en page<br>Tableau de bord<br>Calendrier<br>Section Calendrier<br>Page externe<br>Rapport<br>Filtre<br>Groupement<br>Affichage<br>Paramètre<br>Groupe |
| Tableau de bord (PTLTAB) | Tableau de bord<br>Calendrier<br>Section Calendrier<br>Page externe<br>Rapport<br>Filtre<br>Groupement<br>Affichage<br>Paramètre |
| Calendrier (CALENDE) | Calendrier<br>Section Calendrier |
| Page externe (EXTSEC) | Page externe |
| Rapport (PTLSEC) | Rapport<br>Filtre<br>Groupement<br>Affichage<br>Paramètre |
| Filtre (UIFT) | Paramètre Filter<br> |
| Regroupement (UIGB) | Paramètre de groupement<br> |
| Vue (UIVW) | Paramètre View<br> |

### Objets de données personnalisés

| Objet Promotable | Objets liés promotionnels inclus |
| --- | --- |
| Category (CTGY) | Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage de catégorie<br>Groupe |
| Paramètre (PARAM) | Paramètre <br>Option de paramètre |
| Groupe de paramètres (PGRP) | Groupe de paramètres |

### Objets d’organisation

| Objet Promotable | Objets liés promotionnels inclus |
| --- | --- |
| Groupe (GROUP) | Groupe <br>Sous-groupes (jusqu’à 5 niveaux) *<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage de catégorie |
| Rôle (RÔLE) | Rôle |
| Equipe (EQUIPE) | Team<br>Group |
| Société (CMPY) | Société<br>Taux de remplacement<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Paramètre <br>Logique d’affichage de catégorie<br>Groupe |
| Portfolio (PORT) | Portfolio<br>Programme<br>Groupe<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage de catégorie |
| Programme (PRGM) | Programme<br>Portfolio<br>Groupe<br>Catégorie<br>Paramètre de catégorie<br>Paramètre<br>Groupe de paramètres<br>Option de paramètre<br>Logique d’affichage de catégorie |

### Autres objets de configuration

| Objet Promotable | Objets liés promotionnels inclus |
| --- | --- |
| Processus d’approbation (ARVPRC) | Processus d’approbation<br>Chemin d’approbation<br>Étape d’approbation<br>Approbateur d’étape<br>Rôle<br>Équipe<br>Groupe |
| Planification (SCHED) | Planification<br>Jour sans travail<br>Groupe |
| Chemin Milestone (MPATH) | Chemin Milestone<br>Milestone |
| Profil de feuille de temps (TSPRO) | Profil de la feuille de temps<br>Type d’heure |
| Type d’heure (HEURE) | Type d’heure |
| Type de dépense (EXPTYP) | Type de frais |
| Type de risque (RSKTYP) | Type de risque |
| Pool de ressources (RSPL) | Pool de ressources |

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

Les packages de promotion d’environnement passent par plusieurs états lorsqu’ils sont créés et préparés pour se déplacer entre les environnements. Vous pouvez voir ces états dans votre liste de packages dans Workfront ou dans les réponses de l’API si vous utilisez l’API Workfront.

Ces statuts sont les suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>UNASSEMBLÉ</td> 
   <td><p>Ce statut est automatiquement attribué et représente un package qui a été enregistré mais pas encore assemblé. </p><p>Cet état ne peut pas être défini directement par un utilisateur.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLAGE</td> 
   <td><p>Cet état est automatiquement attribué lors de l’assemblage des objets. </p><p>L’assemblage fait référence au processus automatisé d’identification des objets et des sous-objets à inclure dans un package et d’ajout de ces objets et de leurs données au package.</p><p>Cet état ne peut pas être défini directement par un utilisateur.</p></td> 
  </tr> 
  <tr> 
   <td>version préliminaire</td> 
   <td><p>Ce statut est attribué à la fin d’un processus d’assemblage ou lors de la création d’un package de promotion vide.</p><p>Il est possible pour un utilisateur de replacer le package de promotion dans cet état.</p><p>Dans cet état, le package de promotion ne peut être installé dans aucun environnement.</p></td> 
  </tr> 
  <tr> 
   <td>TEST</td> 
   <td><p>Ce statut permet d’installer un package de promotion dans n’importe quel environnement de test Aperçu ou Actualisation personnalisée. Dans cet état, le package ne peut pas être installé dans Production.</p></td> 
  </tr> 
  <tr> 
   <td>ACTIF</td> 
   <td><p>Ce statut permet d’installer un package de promotion dans n’importe quel environnement, y compris Production.</p><p>Lorsqu’un état de package est défini sur ACTIF, la date <code>publishedAt</code> est automatiquement définie sur l’horodatage actuel de la requête.</p></td> 
  </tr> 
  <tr> 
   <td>DISABLED</td> 
   <td><p>Cet état est utilisé pour masquer les packages de promotion précédemment utilisés qui ne seront plus installés dans aucun environnement à l’avenir.</p><p>Lorsqu’un package est dans cet état, il ne peut être installé dans aucun environnement.</p><p>Lorsqu’un état de package est défini sur DISABLED, la date <code>retiredAt</code> est automatiquement définie sur l’horodatage actuel de la requête.</p><p>L’utilisation de cet état est recommandée plutôt que d’utiliser le point d’entrée <code>DELETE /package</code>, car il est récupérable et l’historique d’installation est conservé pour tous les déploiements effectués avec ce package.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Le package de promotion est automatiquement placé dans ce statut si l'étape ASSEMBLEMENT échoue.</p><p>Pour renvoyer le package à l’étape ASSEMBLEMENT, vous devez relancer le processus d’assemblage.</p><p>Pour plus d'informations sur l'assemblage d'un package, reportez-vous à la section <a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package">Modification ou assemblage d'un package existant</a> de l'article Créer ou modifier un package de promotion d'environnement.</td> 
  </tr> 
  </tbody> 
</table>

