---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Aperçu du statut d'achèvement de l'itération
description: Les informations d’achèvement décrites dans cet article s’affichent au-dessus du graphique d’avancement.
author: Jenny
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 84%

---

# Vue d’ensemble de l’état d’achèvement d’une itération

Les informations d’achèvement décrites dans cet article s’affichent au-dessus du graphique d’avancement.

Pourcentage d’achèvement d’une itération :

![panneau détails de l’itération](assets/burndown-percentcomplete-350x47.png)

ces informations indiquent l’état d’achèvement de l’itération pour le jour actuellement sélectionné dans le graphique d’avancement. Par défaut, l’état d’achèvement s’affiche en fonction de la date du jour actuel.

Les informations suivantes sont disponibles :

* **[!UICONTROL Pourcentage terminé] :** progression globale de l’itération.

  Le [!UICONTROL pourcentage terminé] s’ajuste en fonction du pourcentage terminé de chaque histoire ou tâche dans l’itération, y compris les histoires ou les tâches qui ne sont que partiellement achevées.

  La barre d’état du [!UICONTROL pourcentage terminé] s’affiche en rouge ou en vert pour correspondre à la couleur du taux d’avancement réel. Elle s’affiche en rouge lorsque le taux d’avancement est inférieur au taux idéal (plus de points ou d’heures restants par jour que le calcul d’avancement idéal) et elle s’affiche en vert lorsque le taux d’avancement est égal ou supérieur au taux idéal (autant ou moins de points par jour restants que le calcul d’avancement idéal).

* **[!UICONTROL Histoires terminées] :** (disponible uniquement dans les itérations) le nombre d’histoires marquées avec le statut [!UICONTROL Terminé]. Ce nombre est affiché par rapport au nombre total d’histoires dans l’itération. Par exemple, « 3 sur 6 » indique que 3 des 6 histoires de l’itération ont été marquées avec le statut [!UICONTROL Terminé].
* **[!UICONTROL Points/heures terminés] :** (disponible uniquement pour les itérations) le nombre de points ou d’heures marqué(e)s avec le statut [!UICONTROL Terminé]. Ce nombre est affiché par rapport au nombre total de points ou d’heures dans l’itération. Par exemple, « 5 sur 11 » indique que 5 des 11 histoires de l’itération ont été marquées avec le statut [!UICONTROL Terminé]. Ce nombre est directement lié au calcul du [!UICONTROL pourcentage terminé] et se met à jour en même temps que le [!UICONTROL pourcentage terminé].

  Les points et les heures sont associés aux histoires. Lorsqu’une histoire est marquée avec le statut [!UICONTROL Terminé], les points ou heures associé(e)s à cette histoire sont marqué(e)s avec le statut Terminé.

  Par défaut, les points sont utilisés. Vous pouvez modifier ce paramètre en modifiant les paramètres de votre équipe, comme décrit dans la section [Créer une équipe Agile](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Points/heures par jour] :** (disponible uniquement pour les itérations) le nombre moyen de points ou d’heures marqué(e)s avec le statut [!UICONTROL Terminé] chaque jour depuis le début de l’itération jusqu’au jour actuel.

  Ce nombre est calculé en prenant le total des points ou des heures terminé(e)s, divisé par le nombre total de jours jusqu’au jour actuel. (Les jours partiels sont considérés comme des jours entiers.)

  Ces informations peuvent s’avérer utiles lors de la planification d’une prochaine itération.

* **[!UICONTROL Estimation d’achèvement] :** date estimée à laquelle l’itération sera terminée, en fonction du taux d’avancement actuel de la mesure Points/heures par jour (pour les itérations).

  Lorsque l’[!UICONTROL Estimation d’achèvement] est postérieure à la date de fin définie pour l’itération, le nombre de jours ouvrés restants est affiché en rouge entre parenthèses à côté de l’[!UICONTROL Estimation d’achèvement].

  Lorsque l’[!UICONTROL Estimation d’achèvement] est antérieure à la date de fin prévue de l’itération, le nombre de jours ouvrés restants est affiché en vert. (La date de fin de l’itération est spécifiée lors de la planification de l’itération, comme décrit dans la section [Créer une itération](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md). La date de fin du projet est la [!UICONTROL Date d’achèvement prévue], ou la date actuelle si la [!UICONTROL Date d’achèvement prévue] est dépassée. La [!UICONTROL Date d&#39;achèvement prévue] pour le projet est calculée en fonction de la durée des tâches du projet.) Lors de la planification de l&#39;itération, si vous définissez la date de fin de l&#39;itération pour un jour non ouvré et que l&#39;itération suit son avancement pour se terminer à temps, la date d&#39;achèvement estimée est définie pour le dernier jour ouvré précédant la date de fin de l&#39;itération que vous avez définie (car il n&#39;est pas prévu que le travail soit consommé les jours non ouvrés).

  Par exemple, « (+9 jours) » indique que la date d’achèvement estimée est de 9 jours ouvrés après la date de fin prévue de l’itération.

  Pour plus d’informations, consultez [Vue d’ensemble de l’état d’achèvement d’une itération](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
