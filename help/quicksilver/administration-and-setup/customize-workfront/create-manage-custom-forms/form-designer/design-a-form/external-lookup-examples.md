---
title: Exemples de champs de recherche externe dans un formulaire personnalisé
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Un champ Recherche externe dans un formulaire personnalisé appelle une API externe et renvoie des valeurs sous forme d’options dans un champ déroulant. Cet article fournit des exemples d’utilisation du champ Recherche externe pour appeler la même instance de Workfront ou une API publique.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
source-git-commit: 101a5a80d00a8113ce31222b92f77300a5b0ce8a
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 11%

---

# Exemples de champs de recherche externe dans un formulaire personnalisé

Un champ Recherche externe dans un formulaire personnalisé appelle une API externe et renvoie des valeurs sous forme d’options dans un champ déroulant. Les utilisateurs qui utilisent l’objet auquel le formulaire personnalisé est joint peuvent sélectionner une ou plusieurs de ces options dans la liste déroulante.

Cet article fournit des exemples d’utilisation du champ Recherche externe pour appeler la même instance de Workfront ou une API publique. Vous pouvez également utiliser la recherche externe pour communiquer avec un système externe tel que Jira, Salesforce ou ServiceNow.

Les champs de recherche externe sont disponibles uniquement dans le nouveau concepteur de formulaire, et non dans l’ancien créateur de formulaires. Pour plus d’informations sur l’ajout d’un champ de recherche externe à un formulaire personnalisé et des définitions supplémentaires des composants de recherche externe, voir [Concevoir un formulaire avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Configuration d’un champ de recherche externe pour la même instance de Workfront

Vous pouvez utiliser la recherche externe pour importer les données de votre instance Workfront dans le formulaire personnalisé.

Cet exemple montre comment appeler l’API Workfront et importer les données du champ existant &quot;Requête d’état&quot; dans votre champ Recherche externe .

1. Ouvrez le formulaire personnalisé.
1. Dans la partie gauche de l’écran, recherchez **Recherche externe** et faites-le glisser vers une section de la zone de travail.
1. Saisissez les **Libellé** et **Nom** pour le champ.
1. Sélectionnez le **Format** correspondant au champ.
1. Saisissez l’appel d’URL d’API dans le champ **URL de l’API de base** .

   * Vous pouvez ajouter $$HOST pour référencer la même instance.
   * Vous pouvez ajouter $$QUERY pour filtrer les résultats en fonction de l’interrogation d’un autre champ.

   **Exemple**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. Examinez les **dépendances** pour connaître les champs référencés par ce champ de recherche dans l’API.

   Un champ de dépendance peut être n’importe quel champ personnalisé ou natif existant dans la page de détails de l’objet.

   Dans cet exemple, `{DE:StatusQuery}` sera remplacé par la valeur du champ personnalisé StatusQuery .

1. Sélectionnez la **méthode HTTP**.

   Il s’agira probablement de **Get**.

1. Saisissez le **chemin JSON** pour obtenir les résultats de votre appel API.

   **Exemple**
   `$.data[*].name`

   >[!NOTE]
   >
   >Les informations **Header** ne sont pas requises pour un appel vers la même instance Workfront.

1. Cliquez sur **Appliquer**.

   ![Configuration de l’appel API à Workfront sous forme personnalisée](assets/external-lookup-to-workfront.png)

   Lorsque le formulaire personnalisé est ajouté à un objet Workfront (dans cet exemple, un projet), il ressemble à ceci.

   ![Formulaire personnalisé avec champ de recherche externe](assets/external-lookup-project-status-example1.png)

   ![Options de recherche externe basées sur l’état](assets/external-lookup-project-status-example2.png)

## Configuration d’un champ de recherche externe pour une API publique

Vous pouvez utiliser la recherche externe pour appeler une API publique externe et récupérer des données.

Cet exemple montre comment appeler une API de pays (comme <https://api.first.org/data/v1/countries>) afin que vous n&#39;ayez pas à coder en dur tous les noms de pays dans les options de liste déroulante.

1. Ouvrez le formulaire personnalisé.
1. Dans la partie gauche de l’écran, recherchez **Recherche externe** et faites-le glisser vers une section de la zone de travail.
1. Saisissez les **Libellé** et **Nom** pour le champ.
1. Sélectionnez le **Format** correspondant au champ.
1. Saisissez l’appel d’URL d’API dans le champ **URL de l’API de base** .

   * Vous pouvez ajouter $$QUERY pour implémenter le filtrage des requêtes pour vos utilisateurs finaux.

   **Exemples**
Liste de tous les pays : <https://api.first.org/data/v1/countries>

   Permet à l’utilisateur de rechercher n’importe quel pays dans le champ déroulant : <https://api.first.org/data/v1/countries?q=$$QUERY>

   Permet à l’utilisateur de rechercher un pays dans une région : <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * Les régions disponibles sont définies dans un champ personnalisé distinct dans Workfront.
   * Lorsque l’utilisateur sélectionne une région sur le formulaire, le champ Recherche externe affiche uniquement les pays de cette région (le pays dans lequel la région est définie dans l’API). L’utilisateur peut également rechercher un pays dans la région sélectionnée.

1. Examinez les **dépendances** pour connaître les champs référencés par ce champ de recherche dans l’API.

   Un champ de dépendance peut être n’importe quel champ personnalisé ou natif existant dans la page de détails de l’objet.

   Dans cet exemple, `{DE:Region}` sera remplacé par la valeur du champ personnalisé Région .

1. Sélectionnez la **méthode HTTP**.

   Il s’agira probablement de **Get**.

1. Saisissez le **chemin JSON** pour obtenir les résultats de votre appel API.

   Cette option permet d’extraire des données du code JSON renvoyé par l’URL de l’API. Elle permet de sélectionner les valeurs qui, à l’intérieur du fichier JSON, apparaîtront dans les options de liste déroulante.

   **Exemple**
   `$.data[*].country`

1. (Facultatif) Cliquez sur **Ajouter un en-tête** et saisissez ou collez la paire clé-valeur requise pour l’authentification avec l’API.

   >[!NOTE]
   >
   >Les champs En-tête ne sont pas un lieu sécurisé pour stocker les informations d’identification. Vous devez donc veiller à ce que vous saisissiez et enregistrez.

1. (Facultatif) Sélectionnez **Liste déroulante à sélection multiple** pour permettre à l’utilisateur de sélectionner plusieurs valeurs dans la liste déroulante.

1. Cliquez sur **Appliquer**.

   ![Configuration de l’appel API à l’API publique sous forme personnalisée](assets/external-lookup-to-api-for-countries.png)

   Lorsque le formulaire personnalisé est ajouté à un objet Workfront (dans cet exemple, un projet), il ressemble à ceci.

   ![Formulaire personnalisé avec champ de recherche externe](assets/external-lookup-countries-example1.png)

   ![Options de recherche externe pour un pays en fonction de la région](assets/external-lookup-countries-example2.png)
