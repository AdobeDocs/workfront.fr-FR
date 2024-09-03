---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Exporter des données historiques d’Adobe Workfront : avantages et inconvénients"
description: Cet article explique les avantages et les inconvénients de 4 options que vous pouvez utiliser pour exporter des données historiques à partir de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 72%

---

# Exporter des données historiques à partir d’[!DNL Adobe Workfron]t : avantages et inconvénients

Cet article explique les avantages et inconvénients de quatre options que vous pouvez utiliser pour exporter des données historiques à partir de [!DNL Workfront].

## Faire appel à l’un de nos partenaires

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) dispose d’une application conviviale (leur [solution d’instantané de Workfront](https://store.atappstore.com/product/workfront-snapshot/)) qui vous permet de télécharger vos données vous-même. Une visionneuse facultative (leur solution [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)) vous permet d’afficher facilement vos données hors ligne.

* **Avantages :** Tous vos objets [!DNL Workfront] principaux sont exportés, y compris les champs personnalisés et les notes, qui sont tous ensuite stockés dans une base de données [!DNL MS Access] facilement accessible. L’interface de la visionneuse est facile à utiliser et à lire. L’extraction de documents est également disponible séparément en tant que service. La sortie est organisée en une structure de dossiers logique qui mappe chaque document (et éventuellement, ses versions précédentes).

* **Inconvénients :** Il existe une limitation technique de 2 Go de données, mais AtAppStore vous permet d’acheter uniquement ce dont vous avez besoin.

* **Coûts :** Pour plus d’informations, rendez-vous sur [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).

## Demander un fichier dump de données [!DNL Postgres] à notre équipe chargée des bases de données

Votre personne représentante de compte peut demander à notre équipe chargée des bases de données d’exporter un fichier dump de la base de données (fichier [!DNL Postgres] .dmp) contenant vos données. Une demande supplémentaire sera adressée à notre équipe AOS pour récupérer tous les documents stockés.

* **Avantages** : vous obtenez l’ensemble de vos données, y compris les champs personnalisés, ainsi que les documents stockés dans le système.

* **Inconvénients** : le fichier de base de données est difficile à lire : il est impossible de lire ce fichier à moins de le charger dans une base de données [!DNL Postgres] et de rétablir les relations entre les tableaux. Les documents sont stockés sur un serveur de fichiers distinct et doivent être extraits séparément par l’équipe AOS. Ce faisant, les documents ne sont pas organisés et sont tous référencés par leur GUID.

* **Coût** : ce téléchargement a un coût, qui dépend du temps nécessaire à l’équipe pour créer le fichier. Consultez votre personne représentante de compte pour plus d’informations ou pour entamer ce processus.

## Exporter via des [!UICONTROL Kickstarts]

Que vous disposiez ou non d’heures de conseil à distance, vous pouvez faire appel à l’une de nos personnes consultantes pour exporter vos données sous la forme de rapports ou de [!UICONTROL Kickstarts], ou vous pouvez exécuter ces rapports vous-même :

* **Avantages** : les rapports sont faciles à lire et peuvent être importés dans une variété d’applications ; ils peuvent être personnalisés pour inclure les regroupements et les vues que vous souhaitez.

* **Inconvénients** : les documents devront être téléchargés séparément.

* **Coût** : cela est gratuit si vous pouvez exécuter les rapports vous-même (tout ce dont vous avez besoin est d’une connexion en tant qu’administrateur ou administratrice système), ou si vous pouvez utiliser les heures de conseil à distance restantes. Si l’achat d’un service de conseil à distance vous intéresse, veuillez en parler à votre personne représentante de compte.

  Pour plus d’informations sur l’utilisation de Kickstarts pour exporter des données, voir [Exporter des données à partir d’ [!DNL Adobe Workfront]  via des [!UICONTROL Kickstarts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Utiliser notre API ouverte

Si vous avez les bonnes ressources dans votre organisation, elles peuvent créer une API personnalisée pour récupérer toutes vos données à partir de Workfront :

* **Avantages** : vous contrôlez ce qui est exporté par le système.

* **Inconvénients** : le temps que cela prend est à votre charge, et vous devrez trouver des ressources pour coder l’API et effectuer l’export.

* **Coût** : interne à votre organisation.
