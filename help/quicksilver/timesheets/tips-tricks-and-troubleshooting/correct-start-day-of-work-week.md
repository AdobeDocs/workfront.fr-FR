---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Corriger le jour de début de la semaine de travail pour les feuilles de temps
description: Le jour de début de la semaine sur ma feuille de temps ne correspond pas à mon jour de début hebdomadaire attendu.
author: Lisa
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 5%

---

# Corriger le jour de début de la semaine de travail pour les feuilles de temps

<!--Audited: 5/2025-->

## Problème

Le jour de début de la semaine sur ma feuille de temps ne correspond pas à mon jour de début hebdomadaire attendu.

Cela se produit généralement lorsque vous n’êtes pas affecté à un profil de feuille de temps et que votre feuille de temps a été créée manuellement.


## Solution

Votre administrateur Workfront doit créer des profils de feuille de temps et affecter chacun à un profil, comme décrit dans la section [Créer, modifier et affecter des profils de feuille de temps](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md). Votre administrateur Workfront peut définir la date de début d’une feuille de temps un jour autre que la date de début hebdomadaire prévue. Contactez-les pour connaître la date de début d’un profil de feuille de temps pour votre feuille de temps.

Si votre feuille de temps a été créée manuellement, le jour de début de la semaine dans la feuille de temps utilise les paramètres régionaux des e-mails dans le profil de votre utilisateur, comme décrit dans l’article [Configurer mes paramètres](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Par exemple, avec le paramètre régional d’e-mail défini sur Anglais (États-Unis), la semaine dans la feuille de temps commence le dimanche. Si les paramètres régionaux des e-mails sont définis sur l’anglais (Royaume-Uni), la semaine sur la feuille de temps commence un lundi.


<!--This is the old content for this article but I found this was not working this way at all, so I changed it to what it is today: 

## Problem

The start day of the week on my timesheet does not match the start day of the week that is configured on my timesheet profile (as described in [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Solution

The start day of the week of a timesheet in Adobe Workfront uses the language and locale settings in your browser to determine the day of the week. Because of this, you need to update the language and locale settings for your browser. 

For example, with the browser language set to English and the locale set to United States, the week starts on Sunday. Alternatively, the browser language set to English and the locale set to United Kingdom, the start day is Monday.

This setting also affects the start day of the week in the pop-up calendars across the system.

The locale change does not affect the start day of the week on the Resource Grid (or resource grid view). The week always starts on Sunday.

Following are the directions for changing language and locale settings for various browsers that are supported with Workfront.

* **Chrome:** Copy and paste the following link into your Chrome browser: `chrome://settings/languages` then go to Languages.
* **Firefox:**Copy and paste the following link into your Firefox browser: `about:preferences#content` then go to Languages.
* **IE 11:** Tools -> Internet Options -> General -> Languages
* **Safari:** Unfortunately, Safari does not allow changing web browsing languages without also changing your entire operating system language. It is probably easier to simply install another browser like Chrome or Firefox.

-->


