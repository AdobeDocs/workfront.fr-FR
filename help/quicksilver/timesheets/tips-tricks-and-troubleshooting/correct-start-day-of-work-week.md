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
ht-degree: 7%

---

# Corriger le jour de début de la semaine de travail pour les feuilles de temps

## Problème

Le jour de début de la semaine sur ma feuille de temps ne correspond pas au jour de début de la semaine configuré sur mon profil de feuille de temps (comme décrit dans la section [Créer, modifier et attribuer des profils de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)).

## Solution

Le jour de début de la semaine d’une feuille de temps dans Adobe Workfront utilise la langue et les paramètres régionaux de votre navigateur pour déterminer le jour de la semaine. Pour cette raison, vous devez mettre à jour les paramètres de langue et de paramètres régionaux de votre navigateur.

Par exemple, avec la langue du navigateur définie sur Anglais et le paramètre régional défini sur Etats-Unis, la semaine commence le dimanche. Sinon, la langue du navigateur est l’anglais et la langue est le Royaume-Uni. Le jour de début est le lundi.

Ce paramètre affecte également le jour de début de la semaine dans les calendriers contextuels du système.

Le changement de paramètres régionaux n’a aucune incidence sur le jour de début de la semaine dans la grille de ressources (ou l’affichage de la grille de ressources). La semaine commence toujours le dimanche.

Vous trouverez ci-dessous les instructions relatives à la modification de la langue et des paramètres régionaux pour divers navigateurs pris en charge par Workfront.

* **Chrome :** Copiez et collez le lien suivant dans votre navigateur Chrome : `chrome://settings/languages` puis accédez à Langues.
* **Firefox :**Copiez et collez le lien suivant dans votre navigateur Firefox : `about:preferences#content`, puis accédez à Langues.
* **IE 11 :** Outils -> Options Internet -> Général -> Langues
* **Safari :** Malheureusement, Safari ne permet pas de modifier les langues de navigation web sans modifier la langue de votre système d’exploitation. Il est probablement plus facile d’installer un autre navigateur comme Chrome ou Firefox.


