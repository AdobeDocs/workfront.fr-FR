---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Exporter des données historiques depuis Adobe Workfront : avantages et inconvénients'
description: Cet article explique les avantages et les inconvénients de 4 options que vous pouvez utiliser pour exporter des données historiques à partir de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: bbd00374a6b291582cd03b9d0471d8547eb6ab7f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 42%

---

# Exporter les données historiques depuis [!DNL Adobe Workfront] : avantages et inconvénients

<!-- Audited: 5/2025 -->

Cet article explique les avantages et inconvénients de quatre options que vous pouvez utiliser pour exporter des données historiques à partir d’Adobe Workfront.

## Faire appel à l’un de nos partenaires

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) dispose d’une application facile à utiliser (sa solution [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/)) qui vous permet de télécharger vos données vous-même. Une visionneuse facultative (sa solution [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)) vous permet d’afficher facilement vos données hors ligne.

* **Avantages :** tous vos objets [!DNL Workfront] principaux sont exportés, y compris les champs personnalisés et les notes, et stockés dans une base de données [!DNL MS Access] facilement accessible. L’interface de la visionneuse est facile à utiliser et à lire. L’extraction de documents est également disponible séparément en tant que service, avec une sortie organisée en une structure de dossiers logique qui mappe à chaque document et à ses versions précédentes.

* **Inconvénients :** il existe une limite technique de 2 Go de données, mais AtAppStore vous permet d’acheter uniquement ce dont vous avez besoin.

* **Coûts :** Pour plus d’informations, rendez-vous sur [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).



## Exporter via des [!UICONTROL Kickstarts]

Que vous disposiez ou non d’heures de conseil à distance, vous pouvez faire appel à l’une de nos personnes consultantes pour exporter vos données sous la forme de rapports ou de [!UICONTROL Kickstarts], ou vous pouvez exécuter ces rapports vous-même :

* **Avantages** : les rapports sont faciles à lire et peuvent être importés dans diverses applications. Ils peuvent être personnalisés pour inclure les regroupements et les vues souhaités.

* **Inconvénients** : les documents devront être téléchargés séparément.

* **Coût** : ce service est gratuit si vous pouvez exécuter les rapports vous-même (tout ce dont vous avez besoin est une connexion d’administrateur système) ou si vous pouvez utiliser les heures restantes de consultation à distance. Si l’achat d’un service de conseil à distance vous intéresse, veuillez en parler à votre personne représentante de compte.

  Pour plus d’informations sur l’utilisation de Kickstarts pour exporter des données, voir [Exporter des données à partir d’ [!DNL Adobe Workfront]  via des [!UICONTROL Kickstarts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Utiliser notre API ouverte

Si vous avez les bonnes ressources dans votre organisation, elles peuvent créer une API personnalisée pour récupérer toutes vos données à partir de Workfront :

* **Avantages** : vous contrôlez ce qui est exporté par le système.

* **Inconvénients** : le temps que cela prend est à votre charge, et vous devrez trouver des ressources pour coder l’API et effectuer l’export.

* **Coût** : il est interne à votre organisation.
