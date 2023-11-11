---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Exporter les données historiques depuis Adobe Workfront : avantages et inconvénients"
description: Cet article explique les avantages et inconvénients de 4 options que vous pouvez utiliser pour exporter des données historiques à partir de Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Exporter les données historiques depuis [!DNL Adobe Workfron]t : Avantages et inconvénients

Cet article explique les avantages et inconvénients de 4 options que vous pouvez utiliser pour exporter des données historiques à partir de [!DNL Workfront].

## Utilisation de l’un de nos partenaires

[!DNL AtAppStore], un [!DNL Workfront] partenaire certifié, dispose d’une application conviviale qui vous permet de télécharger vos données. Cette application comprend également une visionneuse qui vous permet d’afficher facilement vos données.

* **Avantages :** Tous vos [!DNL Workfront] sont exportés, y compris les champs personnalisés. L’interface de la visionneuse est facile à utiliser et à lire. Elle est facilement identifiable dans une [!DNL MS Access] Base de données.

* **Inconvénients** Les documents ne sont pas exportés. Vous devrez les télécharger séparément. Pour plus d’informations, voir [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Demander une [!DNL Postgres] fichier de vidage de données de notre équipe Base de données

Votre gestionnaire de compte peut envoyer une demande à notre équipe de base de données pour exporter un fichier de vidage de base de données (.dmp). [!DNL Postgres] ) avec vos données. Une demande supplémentaire sera envoyée à notre équipe AOS pour récupérer tous vos documents stockés.

* **Avantages**: vous obtenez l’intégralité de la charge de données, y compris des champs personnalisés, ainsi que des documents stockés dans le système.

* **Inconvénients**: le fichier de la base de données est difficile à lire : vous ne pouvez pas lire ce fichier tant que vous ne l’avez pas téléchargé dans un [!DNL Postgres] et rétablir les relations entre les tables. Les documents sont stockés sur un serveur de fichiers distinct et doivent être extraits séparément à l’aide d’un processus distinct de l’équipe AOS. Ce faisant, les documents n’ont aucune organisation et ils sont tous référencés par leur GUID.
* **Coût**: ce téléchargement engendre un coût, en fonction du temps nécessaire à l’équipe pour créer le fichier. Pour plus d’informations ou pour lancer ce processus, contactez AEM/CAE.

## Exporter via [!UICONTROL Démarrages]

Que vous ayez ou non des heures de consulting à distance, vous pouvez utiliser l’un de nos consultants pour exporter vos données sous la forme de rapports ou [!UICONTROL Démarrages]ou vous pouvez exécuter les rapports suivants vous-même :

* **Avantages**: les rapports sont faciles à lire et peuvent être importés dans différentes applications. Ils peuvent être personnalisés pour inclure n’importe quel groupe ou affichage.

* **Inconvénients**: les documents devront être téléchargés séparément.

* **Coût**: cette option est gratuite si vous pouvez exécuter les rapports vous-même (vous n’avez besoin que d’une connexion administrateur système) ou si vous pouvez utiliser les heures de conseil à distance qui vous restez. Si vous souhaitez acheter des services de conseil à distance pour cela, veuillez contacter votre AEM/CAE.

  Pour plus d’informations sur l’utilisation de start-up pour exporter des données, voir [Exporter les données depuis [!DNL Adobe Workfront] via [!UICONTROL Démarrages]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Utilisation de notre API ouverte

si vous disposez des ressources appropriées dans votre organisation, il peut créer une API personnalisée pour récupérer toutes vos données de Workfront :

* **Avantages**: vous contrôlez les exportations du système.

* **Inconvénients**: le temps passé sur votre côté, et vous devrez trouver des ressources pour coder l’API et effectuer l’exportation.

* **Coût**: interne à votre entreprise.
