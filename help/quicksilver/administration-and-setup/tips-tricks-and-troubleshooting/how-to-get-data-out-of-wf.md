---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Exporter des données historiques d’Adobe Workfront : avantages et inconvénients"
description: Cet article explique les avantages et inconvénients de 4 options que vous pouvez utiliser pour exporter des données historiques à partir de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Exporter les données historiques de [!DNL Adobe Workfron]t : avantages et inconvénients

Cet article explique les avantages et inconvénients de quatre options que vous pouvez utiliser pour exporter des données historiques à partir de [!DNL Workfront].

## Utilisation de l’un de nos partenaires

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) dispose d’une application conviviale (leur [solution d’instantané de Workfront](https://store.atappstore.com/product/workfront-snapshot/)) qui vous permet de télécharger vos données vous-même. Une visionneuse facultative (leur solution [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)) vous permet d’afficher facilement vos données hors ligne.

* **Avantages :** Tous vos objets [!DNL Workfront] principaux sont exportés, y compris les champs personnalisés et les notes, qui sont tous ensuite stockés dans une base de données [!DNL MS Access] facilement accessible. L’interface de la visionneuse est facile à utiliser et à lire. L’extraction de documents est également disponible séparément en tant que service. La sortie est organisée en une structure de dossiers logique qui mappe chaque document (et éventuellement, ses versions précédentes).

* **Inconvénients :** Il existe une limitation technique de 2 Go de données, mais AtAppStore vous permet d’acheter uniquement ce dont vous avez besoin.

* **Coûts :** Pour plus d’informations, rendez-vous sur [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).

## Demandez un fichier de vidage de données [!DNL Postgres] à notre équipe Base de données

Votre gestionnaire de compte peut envoyer une demande à notre équipe de base de données pour exporter un fichier de vidage de base de données (.dmp [!DNL Postgres]) avec vos données. Une demande supplémentaire sera envoyée à notre équipe AOS pour récupérer tous vos documents stockés.

* **Avantages** : vous obtenez l’intégralité de la charge de données, y compris des champs personnalisés, ainsi que des documents stockés dans le système.

* **Inconvénients** : Le fichier de la base de données est difficile à lire : il n’est pas possible de lire ce fichier, sauf si vous le chargez dans une base de données [!DNL Postgres] et rétablissez les relations entre les tables. Les documents sont stockés sur un serveur de fichiers distinct et doivent être extraits séparément à l’aide d’un processus distinct de l’équipe AOS. Ce faisant, les documents n’ont aucune organisation et ils sont tous référencés par leur GUID.

* **Coût** : un coût est associé à ce téléchargement, selon le temps nécessaire à l’équipe pour créer le fichier. Pour plus d’informations ou pour lancer ce processus, contactez AEM/CAE.

## Exporter via [!UICONTROL Kick-Starts]

Que vous ayez ou non des heures de consulting à distance, vous pouvez utiliser l’un de nos consultants pour exporter vos données sous la forme de rapports ou de [!UICONTROL kick-starts], ou vous pouvez exécuter ces rapports vous-même :

* **Avantages** : les rapports sont faciles à lire et peuvent être importés dans diverses applications. Ils peuvent être personnalisés pour inclure n’importe quel groupe et affichage de votre choix.

* **Inconvénients** : les documents devront être téléchargés séparément.

* **Coût** : gratuit si vous pouvez exécuter vous-même les rapports (vous n’avez besoin que d’une connexion administrateur système) ou si vous pouvez utiliser les heures de consulting à distance qui restent. Si vous souhaitez acheter des services de conseil à distance pour cela, veuillez contacter votre AEM/CAE.

  Pour plus d&#39;informations sur l&#39;utilisation de Kick-Starts pour exporter des données, voir [Exporter des données de [!DNL Adobe Workfront] via [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Utilisation de notre API ouverte

si vous disposez des ressources appropriées dans votre organisation, il peut créer une API personnalisée pour récupérer toutes vos données de Workfront :

* **Avantages** : vous contrôlez les exportations du système.

* **Inconvénients** : le temps passé sur votre côté, et vous devrez trouver des ressources pour coder l’API et effectuer l’exportation.

* **Coût** : interne à votre organisation.
