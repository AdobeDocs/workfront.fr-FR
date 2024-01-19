---
title: autres mises à jour pendant la période de la version 22.3
description: autres mises à jour pendant la période de la version 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 22.3 Autres améliorations

Cette page décrit toutes les autres améliorations apportées à la version 22.3 de l’environnement Aperçu. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 juillet 2022. Pour obtenir la liste de toutes les modifications disponibles avec la version 22.3, voir [Présentation de la version 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Feuilles de temps mises à jour

Nous continuons à améliorer et à mettre à jour votre expérience lorsque vous utilisez des feuilles de temps. Voici quelques-unes des fonctionnalités incluses dans cette mise à jour :

* Une nouvelle apparence qui correspond à la nouvelle expérience Workfront.

* Fonction d’enregistrement automatique afin d’enregistrer automatiquement vos commentaires d’heures et d’heures consignés à la seconde où vous les ajoutez.

* Disposition de page plus intuitive pour correspondre à d’autres pages d’objet. Par exemple, nous avons ajouté un panneau de gauche à la feuille de temps. Les mises à jour de la feuille de temps sont désormais affichées dans la section Mises à jour du panneau de gauche. Vous pouvez également supprimer une feuille de temps de la page de la feuille de temps et l’ajouter à la liste Favoris.

* Une meilleure expérience lors de la recherche et de l’ajout de projets, de tâches ou de problèmes à la feuille de temps. Cela correspond à l’expérience dans toutes les autres listes de Workfront.

* Le panneau Résumé est disponible pour les tâches et les problèmes permettant d’ajouter des commentaires ou de mettre à jour des informations directement depuis la feuille de temps.


Avec la mise à jour actuelle, nous avons également abandonné les fonctionnalités suivantes :

* La création d’une tâche à partir d’une mise à jour a été supprimée. Cette fonctionnalité a été supprimée depuis la version 2018.2 des zones Mises à jour de tous les autres objets, mais elle était toujours disponible dans le flux de mise à jour de la feuille de temps.

* &quot;Ajoutez des dépenses à partir d’une feuille de temps. &quot;La préférence a été supprimée de la zone Préférences de la feuille de temps et des heures de la configuration et vous ne pouvez plus consigner les dépenses à partir de la feuille de temps. Vous pouvez toujours consigner les dépenses à partir des pages de la tâche et du projet.


Pour plus d’informations, voir les articles suivants :

* [Présentation de la disposition de la feuille de calcul](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Configuration des préférences de feuille de temps et d’heure](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Améliorations du panneau de navigation de gauche

Plusieurs améliorations ont été apportées au panneau de navigation de gauche dans Adobe Workfront.

* L’aspect du panneau de navigation de gauche a été mis à jour pour Adobe les normes de conception, notamment les couleurs et les polices.

* Le lien &quot;Ajouter une section personnalisée&quot; au bas du panneau a été renommé &quot;Ajouter un tableau de bord&quot; afin de mieux expliquer sa fonction.

## Activation de la rotation automatique des jetons d’actualisation dans vos applications OAuth2 personnalisées

Pour vous permettre de mieux contrôler la sécurité de vos applications OAuth2 personnalisées, nous avons ajouté à l’option permettant d’activer la rotation du jeton d’actualisation. Lorsque cette option est activée, chaque fois qu’un jeton d’actualisation est utilisé, votre application crée et envoie automatiquement un nouveau jeton d’actualisation, puis désactive l’ancien.

Votre application doit stocker le nouveau jeton d’actualisation après chaque actualisation. Workfront ne stocke pas ce jeton d’actualisation.

Auparavant, les jetons d’actualisation expiraient après un délai défini configuré dans les paramètres personnalisés de l’application OAuth2.

Pour plus d’informations, voir [Création d’applications OAuth2 pour les intégrations Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Utilisation de PKCE dans vos intégrations OAuth2 personnalisées pour les applications web d’une seule page

Vous pouvez désormais créer des applications web d’une seule page dans vos intégrations personnalisées à l’aide de PKCE. PKCE est un flux d’autorisation sécurisé qui fonctionne bien avec les applications d’actualisation dynamique telles que les applications mobiles, mais qui est utile pour tous les clients OAuth2. Au lieu d’un secret client statique, PKCE utilise une chaîne générée dynamiquement, éliminant ainsi le risque de fuite d’un secret client.

Auparavant, les options disponibles pour les applications OAuth2 personnalisées utilisaient le nom et le mot de passe d’un utilisateur ou un secret client.

Pour plus d’informations, voir [Création d’applications OAuth2 pour les intégrations Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
