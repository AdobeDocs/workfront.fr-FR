---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Activité Publication de fusion Workfront : semaine du 16 novembre 2020"
description: Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion la semaine du 16 novembre 2020.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 9221a69e-2482-478b-95a9-f62dd28538d6
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 8%

---

# Activité Publication de fusion Workfront : semaine du 16 novembre 2020

Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion la semaine du 16 novembre 2020.

Pour obtenir la liste de toutes les modifications récentes, voir [Activité de publication d’Adobe Workfront Fusion](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Pour obtenir la liste des correctifs récents dans Workfront Fusion, reportez-vous à la page [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=fr) et recherchez toutes les mises à jour intitulées Mise à jour de maintenance de Workfront Fusion.

## Mises à jour du connecteur Jira Cloud

Pour développer les façons d’utiliser le connecteur Jira Cloud, nous avons ajouté trois nouveaux modules :

* Ajout d’un problème au sprint
* Enregistrements de liste
* Recherche d’enregistrements

Nous avons également mis à jour les modules existants pour prendre en charge le type d’objet &quot;Sprint&quot;. Auparavant, l’objet &quot;Sprint&quot; n’était accessible que par le biais du module d’appel API personnalisé.

Pour plus d’informations, voir [Jira Software modules](../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md).

## L’identifiant d’exécution est désormais disponible pour le mappage dans les scénarios.

L’ID d’exécution d’un scénario est désormais disponible dans le panneau de mappage. Cet identifiant représente une exécution spécifique du scénario et peut être utilisé comme métadonnées. Par exemple, l’ID d’exécution peut être enregistré avec un enregistrement créé par Fusion, de sorte que vous puissiez déterminer ultérieurement quelle exécution Fusion a créé l’enregistrement. L’identifiant d’exécution se trouve dans le panneau de mappage sous Fonctions générales.

Pour plus d’informations sur les exécutions de scénarios, voir [Exécution de scénarios, cycles et phases dans Adobe Workfront Fusion](../../../../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Raccourcis clavier pour les scénarios Workfront Fusion 2.0

Pour faciliter la création de scénarios, nous avons ajouté quelques raccourcis clavier :

* Ctrl/Cmd+Maj+Entrée : exécutez un scénario une fois.
* Ctrl/Cmd + Maj + S : enregistrer un scénario

Pour plus d’informations sur la création de scénarios Workfront Fusion 2.0, voir [Création d’un scénario dans Adobe Workfront Fusion](../../../../../workfront-fusion/scenarios/create-a-scenario.md).

## Mises à jour du connecteur Excel Office 365

Pour étendre les possibilités d&#39;utilisation du connecteur Excel Office 365, nous avons ajouté de nouveaux modules. Vous pouvez désormais :

* Déclencher un module des modifications apportées aux classeurs
* Recherche ou téléchargement de classeurs
* Liste des feuilles de calcul, des lignes de feuille de calcul, des tableaux ou des lignes de tableau
* Mise à jour d’un tableau ou d’une ligne de feuille de calcul
* Suppression d’un tableau ou d’une ligne de feuille de calcul
* Récupération des métadonnées d’un tableau
* Effectuer un appel API personnalisé

Les modules précédemment disponibles sont toujours présents dans l’application.

Pour plus d’informations, voir [Modules Excel Microsoft Office 365](../../../../../workfront-fusion/apps-and-their-modules/microsoft-365-excel-modules.md).

## Utilisation d’OAuth 2.0 dans vos connexions d’applications Workfront

Nous avons mis à jour le connecteur Workfront pour utiliser OAuth 2.0. Cette mise à jour signifie qu’il est plus facile d’apporter des modifications à vos connexions d’applications Workfront. Par exemple, si quelque chose à propos de vos modifications de connexion (un mot de passe, par exemple), vous n’avez plus besoin de mettre à jour chaque connexion individuelle dans vos scénarios. En outre, OAuth2 offre d’autres avantages, tels que l’amélioration de la sécurité et la possibilité d’utiliser l’authentification unique (SSO).

Pour le moment, les connexions existantes ne nécessitent aucune modification. Vous pouvez toutefois réautoriser les connexions existantes si vous souhaitez profiter des avantages d’OAuth 2.0.

Pour plus d’informations, voir [Modules Adobe Workfront](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).
