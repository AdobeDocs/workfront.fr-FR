---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Aperçu de l’état d’achèvement de l’itération
description: Les informations d’achèvement décrites dans cet article s’affichent au-dessus du graphique de ventilation.
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# Aperçu de l’état d’achèvement de l’itération

Les informations d’achèvement décrites dans cet article s’affichent au-dessus du graphique de ventilation.

Pourcentage d’achèvement sur une itération :

![](assets/burndown-percentcomplete-350x47.png)

Ces informations indiquent l’état d’achèvement de l’itération pour le jour actuellement sélectionné dans le graphique de ventilation. Par défaut, l’état de fin s’affiche en fonction de la date du jour en cours.

Les informations disponibles sont les suivantes :

* **[!UICONTROL Pourcentage terminé]:** Progression globale de l&#39;itération

   [!UICONTROL Pourcentage terminé] s’ajuste en fonction du pourcentage d’achèvement de chaque article ou tâche dans l’itération, y compris les articles ou les tâches qui ne sont que partiellement terminés.

   La couleur de la variable [!UICONTROL Pourcentage terminé] la barre d’état s’affiche en rouge ou en vert pour correspondre à la couleur du taux de charge réel. Il est affiché en rouge lorsque le taux de charge est inférieur à l’idéal (plus de points ou d’heures restant par jour que le calcul idéal) et s’affiche en vert lorsque le taux de charge est égal ou supérieur à l’idéal (soit moins de points par jour que le calcul idéal).

* **[!UICONTROL Articles terminés]:** (Disponible uniquement en itérations) Le nombre d’articles marqués [!UICONTROL Terminer]. Cela est présenté par rapport au nombre total d’articles dans l’itération. Par exemple, &quot;3 sur 6&quot; indique que 3 des 6 étages de l’itération ont été marqués. [!UICONTROL Terminer].
* **[!UICONTROL Points/heures terminés]:** (Disponible uniquement en itérations) Le nombre de points ou d’heures marqués [!UICONTROL Terminer]. Affiché par rapport au nombre total de points ou d’heures dans l’itération. Par exemple, &quot;5 sur 11&quot; indique que 5 des 11 articles de l’itération ont été marqués [!UICONTROL Terminer]. Ce nombre est directement lié au [!UICONTROL Pourcentage terminé] et est mis à jour simultanément. [!UICONTROL Pourcentage terminé] est mise à jour.

   Les points et les heures sont associés aux histoires. Lorsqu’une histoire est marquée [!UICONTROL Terminer], les points ou heures associés à cet article sont marqués comme étant terminés.

   Par défaut, les points sont utilisés. Vous pouvez modifier ce paramètre en modifiant les paramètres de votre équipe, comme décrit dans la section [Création d’une équipe agile](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Points / Heures par jour]:** (Disponible uniquement en itérations) Le nombre moyen de points ou d’heures marqués [!UICONTROL Terminer] chaque jour depuis le début de l’itération jusqu’au jour en cours.

   Il est calculé par le total des points ou heures terminés, divisé par le nombre total de jours dans la journée en cours. (Les jours partiels sont enregistrés comme une journée entière.)

   Ces informations peuvent s’avérer utiles lors de la planification d’une prochaine itération.

* **[!UICONTROL Achèvement estimé]:** Date estimée à laquelle l’itération sera terminée, en fonction du taux actuel dans la mesure Points/Heures par jour (pour les itérations).

   Lorsque la variable [!UICONTROL Achèvement estimé] date est postérieure à la date de fin définie pour l’itération, le nombre de jours ouvrés restants est affiché en rouge entre parenthèses en regard de la valeur [!UICONTROL Achèvement estimé] date.

   Lorsque la variable [!UICONTROL Achèvement estimé] date est antérieure à la date de fin prévue de l’itération, le nombre de jours ouvrés restants est affiché en vert. (La date de fin de l’itération est spécifiée lors de la planification de l’itération, comme décrit dans la section [Créer une itération](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md); la date de fin du projet est la suivante : [!UICONTROL Date d’achèvement prévue], ou il s’agit de la date courante si la variable [!UICONTROL Date d’achèvement prévue] est dans le passé. Le [!UICONTROL Date d’achèvement prévue] pour le projet est calculé en fonction de la durée des tâches du projet.) Lors de la planification de l’itération, si vous définissez la date de fin de l’itération pour un jour non ouvré et que l’itération est suivie pour se terminer à temps, la date de fin estimée est définie pour le dernier jour ouvrable précédant la date de fin de l’itération que vous avez définie (car le travail n’est pas planifié pour être réduit en cendres pendant les jours non ouvrés).

   Par exemple, &quot;(+9 jours)&quot; indique que la date d’achèvement estimée est de 9 jours ouvrés après la date de fin prévue de l’itération.

   Pour plus d’informations, voir [Aperçu de l’état d’achèvement de l’itération](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
