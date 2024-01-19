---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Activité Publication de fusion Workfront : semaine du 11 janvier 2021"
description: Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion durant la semaine du 11 janvier 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Activité Publication de fusion Workfront : Semaine du 11 janvier 2021

Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion durant la semaine du 11 janvier 2021.

Pour obtenir la liste de toutes les modifications récentes, voir [Activité Publication de fusion Adobe Workfront](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Pour obtenir la liste des correctifs récents dans Workfront Fusion, reportez-vous à la section [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) et recherchez toutes les mises à jour intitulées Mise à jour de maintenance de la fusion Workfront.

## Connecteur et modules étendus désormais disponibles

Vous pouvez désormais utiliser Workfront Fusion pour vous connecter à votre compte Widen. Avec les modules Windows, vous pouvez :

* Ajout de ressources à une collection ou suppression de ressources
* Téléchargement ou chargement de fichiers
* Lecture ou mise à jour de métadonnées de ressource
* Recherche de ressources en fonction des critères que vous spécifiez
* Récupération d’une liste de ressources dans une collection
* Effectuez un appel API personnalisé.

Pour plus d’informations, voir [Modules étendus](../../../workfront-fusion/apps-and-their-modules/widen-modules.md).

## Connecteur et modules de données désormais disponibles

Vous pouvez désormais utiliser Workfront Fusion pour vous connecter à votre compte Datadog.

Avec les modules Datadog, vous pouvez :

* Points d’horodatage des publications
* Exécution d’un appel API personnalisé

Pour plus d’informations sur les modules DataManager, voir [Modules de données](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md).

## Connecteur Cvent et modules désormais disponibles

Vous pouvez désormais utiliser Workfront Fusion 2.0 pour vous connecter à votre compte Cvent.

Avec les modules Cvent, vous pouvez :

* Créer une demande de réunion
* Lire des enregistrements tels que des contacts, des événements ou des invitations
* Répertorier les enregistrements en fonction des critères que vous spécifiez
* Enregistrement ou ajout d’invitations à des événements spécifiques
* Mettre à jour ou supprimer des contacts
* Effectuer un appel API personnalisé

Pour plus d’informations sur les modules Cvent disponibles, voir [Modules d’événement](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md).

## Connecteur et modules Microsoft Dynamics 365 désormais disponibles

Vous pouvez désormais utiliser Workfront Fusion 2.0 pour vous connecter à votre compte Microsoft Dynamics 365. Avec les modules Microsoft Dynamics 365, vous pouvez :

* Déclenchez un scénario lorsque des enregistrements sont ajoutés ou mis à jour dans Microsoft Dynamics 365
* Créer, lire, mettre à jour ou supprimer un enregistrement Microsoft Dynamics 365
* Exécution d’un appel API personnalisé

Pour plus d’informations sur les modules Microsoft Dynamics 365 disponibles, voir [Modules Microsoft Dynamics 365](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

## Connecteur et modules DocuSign désormais disponibles

Vous pouvez désormais utiliser Workfront Fusion 2.0 pour vous connecter à votre compte Document. Avec les modules Document, vous pouvez :

* Déclencher un scénario lorsqu’une enveloppe modifie son état
* Création d’une enveloppe
* Lecture, envoi ou ajout d’un destinataire à une enveloppe existante
* Ajouter ou modifier des champs personnalisés dans des documents
* Téléchargement d’un document sous la forme d’un champ
* Transfert d’un fichier vers une enveloppe
* Exécution d’un appel API personnalisé

Pour plus d’informations, voir [Modules DocuSign](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md).

## Recherche de l’historique d’exécution des scénarios

Nous vous avons facilité la recherche d’informations spécifiques provenant d’exécutions de scénarios précédentes. La nouvelle recherche de texte intégral de Fusion permet de rechercher dans l’historique d’exécution toutes les données contenues dans un lot. Par exemple, pour identifier l’exécution qui a créé une tâche spécifique, vous pouvez utiliser la recherche de texte intégral pour rechercher cet ID de tâche.

Auparavant, la recherche d’informations d’exécution spécifiques nécessitait d’afficher chaque exécution individuellement.

Pour plus d’informations, voir [Affichage de l’historique d’exécution d’un scénario dans Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Mises à jour du magasin de données Fusion 2.0

Afin que vous puissiez plus facilement personnaliser vos entrepôts de données, nous avons ajouté de nouvelles fonctionnalités. Maintenant, lorsque vous affichez un entrepôt de données, vous pouvez :

* Effectuez un glisser-déposer pour réorganiser les colonnes.
* Modifier une seule cellule
* Ajout de plusieurs lignes

Pour plus d’informations sur les entrepôts de données, voir [Modules Data Store](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## Effectuer une demande d’autorisation de clé API via le connecteur HTTP

Afin d’accroître la flexibilité d’accès aux API, nous avons ajouté un nouveau module au connecteur HTTP. Désormais, vous pouvez utiliser le connecteur HTTP pour effectuer une requête lorsque le service Web auquel vous accédez nécessite l’utilisation d’une clé API.

Pour plus d’informations, voir [Modules HTTP](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

## Nouvelles fonctions disponibles dans le panneau Mappage

Pour vous aider à personnaliser et simplifier les formules de vos modules, nous avons ajouté de nouvelles fonctions.

* Le/la/les

  ```
  omit
  ```

  est une fonction générale qui omet les clés données de l’objet et renvoie le reste.
* Le/la/les

  ```
  pick
  ```

  est une fonction générale qui sélectionne uniquement les clés données de l’objet .
* Le/la/les

  ```
  escapeMarkdown
  ```

  est une fonction de chaîne qui échappe toutes les balises Markdown d’un texte.

Pour plus d’informations sur les fonctions d’omit et de sélection, voir [Fonctions générales dans Adobe Workfront Fusion](../../../workfront-fusion/functions/general-functions.md).

Pour plus d’informations sur la fonction escapeMarkdown, voir [Fonctions de chaîne dans Adobe Workfront Fusion](../../../workfront-fusion/functions/string-functions.md).
