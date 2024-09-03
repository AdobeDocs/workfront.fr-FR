---
title: autres mises à jour pendant la période de publication de la version 22.3
description: autres mises à jour pendant la période de publication de la version 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 100%

---

# 22.3 Autres améliorations

Cette page décrit toutes les autres améliorations apportées à l’environnement de prévisualisation avec la version 22.3. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 juillet 2022. Pour obtenir la liste de toutes les modifications disponibles avec la version 22.3, voir [Vue d’ensemble de la version 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Mise à jour des feuilles de temps

Nous continuons à améliorer et à mettre à jour votre expérience lorsque vous utilisez des feuilles de temps. Voici quelques-unes des fonctionnalités incluses dans cette mise à jour :

* Un nouvel aspect qui correspond à la nouvelle expérience Workfront.

* Fonctionnalité d’enregistrement automatique afin d’enregistrer automatiquement vos heures consignées et vos commentaires sur les heures à la seconde où vous les ajoutez.

* Une mise en page plus intuitive pour correspondre à d’autres pages d’objet. Par exemple, nous avons ajouté un panneau de gauche à la feuille de temps. Les mises à jour de la feuille de temps sont désormais affichées dans la section Mises à jour du panneau de gauche. Vous pouvez également supprimer une feuille de temps de la page des feuilles de temps et l’ajouter à la liste Favoris.

* Une meilleure expérience lors de la recherche et de l’ajout de projets, de tâches ou de problèmes à la feuille de temps. Cela correspond à l’expérience dans toutes les autres listes de Workfront.

* Le panneau Résumé est disponible pour les tâches et les problèmes et permet d’ajouter des commentaires ou de mettre à jour des informations directement depuis la feuille de temps.


Avec la mise à jour actuelle, nous avons également abandonné les fonctionnalités suivantes :

* Il n’est plus possible de créer une tâche à partir d’une mise à jour. Cette fonctionnalité a été supprimée depuis la version 2018.2 des zones Mises à jour de tous les autres objets, mais elle était toujours disponible dans le flux de mise à jour de la feuille de temps.

* La préférence « Ajouter des dépenses à partir d’une feuille de temps ». a été supprimée de la zone Préférences de la feuille de temps et des heures de Configuration et vous ne pouvez plus enregistrer les dépenses à partir de la feuille de temps. Vous pouvez toujours enregistrer les dépenses à partir des pages des tâches et des projets.


Pour plus d’informations, consultez les articles suivants :

* [Comprendre la mise en page de la feuille de temps](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Configurer les préférences des feuilles de temps et des heures](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Améliorations du panneau de navigation de gauche

Plusieurs améliorations ont été apportées au panneau de navigation de gauche dans Adobe Workfront.

* L’aspect du panneau de navigation de gauche a été mis à jour selon les normes de conception d’Adobe, notamment en ce qui concerne les couleurs et les polices.

* Le lien « Ajouter une section personnalisée » au bas du panneau a été renommé « Ajouter un tableau de bord » afin de mieux expliquer sa fonction.

## Activer la rotation automatique des jetons d’actualisation dans vos applications OAuth2 personnalisées

Pour vous permettre de mieux contrôler la sécurité de vos applications OAuth2 personnalisées, nous avons ajouté une option permettant d’activer la rotation du jeton d’actualisation. Lorsque cette option est activée, chaque fois qu’un jeton d’actualisation est utilisé, votre application crée et envoie automatiquement un nouveau jeton d’actualisation, puis désactive l’ancien.

Votre application doit stocker le nouveau jeton d’actualisation après chaque actualisation. Workfront ne stocke pas ce jeton d’actualisation.

Auparavant, les jetons d’actualisation expiraient après un délai défini configuré dans les paramètres personnalisés de l’application OAuth2.

Pour plus d’informations, voir [Créer des applications OAuth2 pour les intégrations Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Utiliser PKCE dans vos intégrations OAuth2 personnalisées pour les applications web d’une seule page

Vous pouvez désormais créer des applications web d’une seule page dans vos intégrations personnalisées à l’aide de PKCE. PKCE est un flux d’autorisation sécurisé qui fonctionne bien avec les applications à actualisation dynamique, telles que les applications mobiles, mais qui est utile pour tous les clients OAuth2. Au lieu d’utiliser un secret client statique, PKCE emploie une chaîne générée dynamiquement, éliminant ainsi le risque de fuite d’un secret client.

Auparavant, les options disponibles pour les applications OAuth2 personnalisées utilisaient le nom et le mot de passe d’un utilisateur ou d’une utilisatrice ou un secret client.

Pour plus d’informations, voir [Créer des applications OAuth2 pour les intégrations Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
