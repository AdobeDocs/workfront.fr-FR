---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Corriger le jour de début de la semaine de travail pour les feuilles de temps
description: Le jour de début de la semaine sur ma feuille de temps ne correspond pas au jour de début de la semaine configuré sur mon profil de feuille de temps.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 92%

---

# Corriger le jour de début de la semaine de travail pour les feuilles de temps

## Problème

Le jour de début de la semaine sur ma feuille de temps ne correspond pas au jour de début de la semaine configuré sur mon profil de feuille de temps (comme décrit dans la section [Créer, modifier et attribuer des profils de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)).

## Solution

Le jour de début de la semaine d’une feuille de temps dans Adobe Workfront utilise les paramètres de langue et régionaux de votre navigateur pour déterminer le jour de la semaine. Pour cette raison, vous devez mettre à jour les paramètres de langue et régionaux de votre navigateur.

Par exemple, lorsque la langue du navigateur est définie sur Anglais et les paramètres régionaux sur États-Unis, la semaine commence le dimanche. Sinon, lorsque la langue du navigateur est définie sur Anglais et les paramètres régionaux sur Royaume-Uni, le jour de début est le lundi.

Ce paramètre affecte également le jour de début de la semaine dans les calendriers contextuels du système.

Le changement de paramètres régionaux n’a aucune incidence sur le jour de début de la semaine dans la grille des ressources (ou la vue de grille des ressources). La semaine commence toujours le dimanche.

Vous trouverez ci-dessous les instructions relatives au changement de langue et de paramètres régionaux pour divers navigateurs pris en charge par Workfront.

* **Chrome :** Copiez et collez le lien suivant dans votre navigateur Chrome : `chrome://settings/languages` puis accédez à Langues.
* **Firefox :** copiez et collez le lien suivant dans votre navigateur Firefox : `about:preferences#content`, puis accédez à Langues.
* **IE 11 :** Outils -> Options Internet -> Général -> Langues.
* **Safari :** Safari ne permet malheureusement pas de modifier les langues de navigation web sans modifier la langue de l’ensemble de votre système d’exploitation. Il sera probablement plus simple d’installer un autre navigateur tel que Chrome ou Firefox.


