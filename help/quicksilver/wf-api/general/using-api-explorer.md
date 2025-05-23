---
content-type: api
navigation-topic: general-api
title: Utiliser l’explorateur d’API
description: Utiliser l’explorateur d’API
author: Becky
feature: Workfront API
role: Developer
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 97%

---


# Utiliser l’explorateur d’API

Lors de l’utilisation de l’API principale de Workfront, l’explorateur d’API est un outil de référence hérité qui répertorie les relations entre les ressources, les paramètres et les variables pris en charge.

## Accédez à l’explorateur d’API :

1. Utiliser un navigateur web pour accéder à l’[Explorateur d’API](https://developer.adobe.com/workfront/api-explorer/)\
   ![Accéder à l’explorateur d’API](assets/mceclip1-350x149.png)

1. Dans l’angle supérieur droit de l’explorateur d’API, sélectionnez la **version de l’API** de votre choix. Par défaut, la version la plus récente est automatiquement sélectionnée.
1. Le champ **Filtrer** peut être utilisé pour filtrer les objets répertoriés par nom et raccourcir la liste des objets affichés en conséquence :

   ![champs de l’explorateur d’API](assets/mceclip2-350x147.png)

   * **Champs** : champs disponibles dans l’objet spécifié.
   * **Références** : variables de référence disponibles pour l’objet spécifié. Une référence est un alias pour une variable. Une fois initialisée, une référence peut être utilisée de manière interchangeable avec le nom de la variable. Une référence utilise la mémoire initialisée.
   * **Collections** : collections disponibles pour l’objet. Les collections sont des variables qui représentent une relation un-à-multiple entre l’objet et la ressource.
   * **Recherche** : ressources de recherche disponibles pour l’objet. Les résultats d’une recherche sont basés sur les paramètres de requête spécifiés par la ressource de recherche dans la requête API.
   * **Actions** : actions prises en charge pour l’objet. Les actions peuvent être des procédures simples ou complexes qui s’exécutent sur une ressource ou un ensemble de ressources. Une action donnée peut également affecter les ressources associées.

1. Ouvrez un onglet, puis cliquez sur « ID d’objet » pour afficher les variables applicables.\
   ![Afficher les variables](assets/approval-350x89.png)\
   Selon l’objet sélectionné, les variables suivantes peuvent s’appliquer :

   | Variable | Définition |
   |---|---|
   | Nom de champ | Nom d’un champ utilisé dans une opération de l’API Workfront. |
   | Type de champ | Type de valeurs pouvant être entrées dans un champ spécifique d’un tableau de données. Les valeurs de type de champ possibles sont string, double, int, dateTime. |
   | Type énuméré | Type de valeurs pouvant être utilisées pour identifier un type de données. |
   | Valeurs possibles | Valeurs acceptables pour l’objet. |
   | Type d’attribut ObjCode | Attributs pouvant être utilisés pour modifier la classe de l’objet. |
   | URL | Chemin d’accès qui permet à votre application de communiquer avec l’API Workfront. |
   | Arguments | Variables de l’objet qui peuvent être transmises entre votre application et Workfront. |
   | Type de résultat | Types de données autorisés qui peuvent être renvoyés à partir d’une méthode. |
