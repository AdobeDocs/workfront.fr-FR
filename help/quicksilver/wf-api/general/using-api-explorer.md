---
content-type: api
navigation-topic: general-api
title: Utilisation de l’explorateur d’API
description: Utilisation de l’explorateur d’API
author: John
feature: Workfront API
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Utilisation de l’explorateur d’API

Lors de l’utilisation de l’API Core d’Adobe Workfront, l’explorateur d’API est un outil de référence hérité qui catalogue les relations entre les ressources, les paramètres et les variables pris en charge.

## Accédez à l’explorateur d’API :

1. Utilisez un navigateur Web pour accéder à la variable [Explorateur d’API](https://one.workfront.com/s/api-explorer)\
   ![](assets/mceclip1-350x149.png)

1. Dans l’angle supérieur droit de l’explorateur d’API, sélectionnez l’interface de travail de votre choix. **Version de l’API**, par défaut, la version la plus récente est automatiquement sélectionnée.
1. Le **Filtrer** , peut être utilisé pour filtrer les objets répertoriés par nom et tronque la liste des objets affichés en conséquence :

   ![](assets/mceclip2-350x147.png)

   * **Champs**: Champs disponibles dans l’objet spécifié.
   * **Références**: Variables de référence disponibles pour l’objet spécifié. Une référence est un alias pour une variable. Une fois initialisée, une référence peut être utilisée de manière interchangeable avec le nom de variable. Une référence utilise la mémoire initialisée.
   * **Collections**: Collections disponibles pour l’objet. Les collections sont des variables qui représentent une relation de type &quot;un à plusieurs&quot; entre l’objet et la ressource.
   * **Rechercher**: Ressources de recherche disponibles pour l’objet. Les résultats d’une recherche sont basés sur les paramètres de requête spécifiés par la ressource de recherche dans la requête API.
   * **Actions**: Actions prises en charge pour l’objet . Les actions peuvent être des procédures simples ou complexes qui s’exécutent sur une ressource ou un ensemble de ressources. Une action donnée peut également affecter les ressources associées.

1. Ouvrez un onglet, puis cliquez sur ID d’objet pour afficher les variables applicables.\
   ![](assets/approval-350x89.png)\
   Selon l’objet sélectionné, les variables suivantes peuvent s’appliquer :

   | Variable | Définition |
   |---|---|
   | Nom de champ | Nom d’un champ utilisé dans une opération de l’API Workfront. |
   | Type de champ | Type de valeurs pouvant être renseignées dans un champ spécifique d’un tableau de données. Les valeurs de type de champ possibles sont string, double, int, dateTime. |
   | Type énuméré | Type de valeurs pouvant être utilisé pour identifier un type de données. |
   | Valeurs possibles | Valeurs acceptables pour l’objet. |
   | Type d’attribut ObjCode | Attributs pouvant être utilisés pour modifier la classe d’objet. |
   | URL | Chemin d’accès qui permet à votre application de communiquer avec l’API Workfront. |
   | Arguments | Les variables de l’objet qui peuvent être transmises entre votre application et Workfront. |
   | Type de résultat | Types de données autorisés qui peuvent être renvoyés à partir d’une méthode. |
