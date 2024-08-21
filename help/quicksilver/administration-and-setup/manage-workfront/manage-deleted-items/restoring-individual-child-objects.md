---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restaurer des objets enfant individuels
description: Ce document décrit comment obtenir de l’aide pour récupérer des objets enfants individuels qui ont été supprimés de vos environnements de production ou de prévisualisation Adobe Workfront moins de 30 jours auparavant.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 1%

---

# Restaurer des objets enfants individuels

Ce document décrit comment obtenir de l’aide pour récupérer des objets enfants individuels qui ont été supprimés de vos environnements de production ou de prévisualisation Adobe Workfront moins de 30 jours auparavant.

Un administrateur Workfront peut restaurer des projets, des tâches, des problèmes et des documents dans chaque instance Workfront, comme décrit dans la section [Restaurer les éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). Cependant, seule l’équipe de base de données Workfront peut restaurer des objets tels que des tâches, des problèmes, des documents, des formulaires personnalisés, des heures et des notes indépendamment de leur objet parent.

Les données de votre environnement de production sont disponibles dans l’environnement de test de prévisualisation pendant 7 jours au maximum. Cela signifie que vous pouvez exporter les données autonomes à partir de l’environnement Preview Sandbox à l’aide des méthodes suivantes :

* Lancements
* Construire un rapport et exporter les résultats

Pour plus d&#39;informations sur l&#39;export de données depuis Workfront, voir [Export de données](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

Vous pouvez importer les données exportées de la manière suivante :

* Si vous utilisez manuellement des rapports exportés
* En bloc, si vous utilisez des start-ups

  Pour plus d’informations sur l’importation de données dans Workfront à l’aide de démarrage rapide, voir [Importation de données dans Adobe Workfront à l’aide d’un modèle de démarrage rapide](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

L’environnement Preview Sandbox est actualisé pendant les fenêtres de maintenance du week-end.

Pour plus d’informations sur les fenêtres de maintenance pour l’environnement de prévisualisation Sandbox, voir [le site d’état Adobe](https://status.adobe.com/fr).

>[!IMPORTANT]
>
>Les documents constituent une exception à ces méthodes de restauration. Vous pouvez les télécharger manuellement à partir de l’environnement de prévisualisation et les charger à nouveau dans l’environnement de production. Si vous souhaitez télécharger et charger des documents en bloc, vous devez demander une restauration des données à Workfront.

## Informations nécessaires à la restauration des données

Une fois que vous avez déterminé qu’un objet supprimé doit être restauré par notre équipe de base de données, collectez autant d’informations que possible à son sujet. Les informations suivantes sont requises pour que les administrateurs de base de données trouvent l’objet et lancent une restauration :

* Nom de l’objet
* Type d’objet (tâche, problème, projet, etc.)
* Date et heure estimées de suppression
* GUID d’objet (si possible)

  Reportez-vous aux informations suivantes lors de la localisation du GUID d’un objet :

   * Le GUID est accessible en référençant des notifications par e-mail déclenchées en interagissant avec l’objet (affectations, commentaires, etc.)
   * Exemple de GUID trouvé à la fin d&#39;une URL : `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

Une fois que vous avez rassemblé ces informations ou si vous avez besoin d’aide, contactez notre équipe d’assistance clientèle au 844-306-HELP(4357) ou soumettez un ticket en ligne.

## Processus de restauration des données

1. Une fois que notre équipe d’assistance clientèle aura reçu vos informations, elle les transmettra à notre équipe d’assistance clientèle.
1. Notre équipe d’assistance clientèle contactera notre équipe de base de données.
1. Une fois que l’équipe de base de données a eu la possibilité de passer en revue les données restaurées, une estimation plus précise de l’ETA peut être fournie. Une restauration prend généralement trois jours, mais peut prendre plus de temps en fonction du type et du volume des données restaurées.
1. L’équipe de base de données restaurera les informations dans votre environnement de prévisualisation des environnements de test où vous aurez la possibilité de passer en revue les données restaurées. Notre équipe d’assistance clientèle vous indiquera quand les données se trouvent dans l’environnement de test de prévisualisation.
1. Une fois que vous êtes satisfait de la restauration dans l’environnement de test, faites-le savoir à notre équipe d’assistance clientèle. Elle contactera notre équipe de base de données pour l’informer qu’elle peut restaurer les données dans votre environnement de production.
1. Vous aurez la possibilité de consulter les données restaurées avant que la requête ne soit fermée.
