---
title: Exemples de champ de recherche externe dans un formulaire personnalisé
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Un champ de recherche externe dans un formulaire personnalisé appelle une API externe et renvoie les valeurs sous forme d’options dans un champ déroulant. Cet article fournit des exemples d’utilisation du champ de recherche externe pour appeler la même instance de Workfront ou une API publique.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
source-git-commit: 40d9455fe3b14006817c784a4d3c8dea8a601839
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 49%

---

# Exemples de champs de recherche externe dans un formulaire personnalisé

Un champ de recherche externe dans un formulaire personnalisé appelle une API externe et renvoie les valeurs sous forme d’options dans un champ déroulant. Les personnes qui travaillent avec l’objet auquel le formulaire personnalisé est attaché peuvent sélectionner une ou plusieurs de ces options dans la liste déroulante.

Cet article fournit des exemples d’utilisation du champ de recherche externe pour appeler la même instance de Workfront ou une API publique. Vous pouvez également utiliser la recherche externe pour communiquer avec un système externe tel que Jira, Salesforce ou ServiceNow.

Pour plus d’informations sur l’ajout d’un champ de recherche externe à un formulaire personnalisé et des définitions supplémentaires des composants de recherche externe, voir [Concevoir un formulaire avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Configuration d’un champ de recherche externe pour la même instance de Workfront

Vous pouvez utiliser la recherche externe pour importer les données de votre instance Workfront dans le formulaire personnalisé.

### Utilisation de valeurs de champ Workfront natives dans la recherche externe

Cet exemple montre comment appeler l’API Workfront et importer les données du champ existant &quot;Requête d’état&quot; dans votre champ de recherche externe.

1. Ouvrez le formulaire personnalisé.
1. Dans la partie gauche de l’écran, recherchez **Recherche externe** et faites glisser le champ vers une section du canevas.
1. Saisissez l’**étiquette** et le **nom** pour le champ.
1. Sélectionnez le **format** pour le champ.
1. Saisissez l’appel API dans le champ **URL de l’API de base**.

   * Pour référencer la même instance de Workfront que celle du formulaire personnalisé, utilisez $$HOST pour l’URL.
   * Pour filtrer les résultats en fonction de l’interrogation d’un autre champ, ajoutez $$QUERY.

   **Exemple**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. Consultez le site **Dépendances** pour connaître les champs auxquels ce champ de recherche fait référence dans l’API.

   Un champ de dépendance peut être n’importe quel champ personnalisé ou natif existant dans la page de détails de l’objet.

   Dans cet exemple, le site `{DE:StatusQuery}` sera remplacé par la valeur du champ personnalisé StatusQuery.

1. Sélectionnez la **méthode HTTP** .

   Il s’agira le plus souvent de **Get**.

1. Saisissez le **chemin JSON** pour obtenir les résultats de votre appel API.

   **Exemple**
   `$.data[*].name`

   >[!NOTE]
   >
   >Les informations de l’**en-tête** ne sont pas nécessaires pour un appel à la même instance de Workfront.

1. Cliquez sur **Appliquer**.

   ![Mettre en place un appel API vers Workfront dans un formulaire personnalisé](assets/external-lookup-to-workfront.png)

   Lorsque le formulaire personnalisé est ajouté à un objet Workfront (dans cet exemple, un projet), il ressemble à ceci.

   ![Formulaire personnalisé avec champ de recherche externe](assets/external-lookup-project-status-example1.png)

   ![Options de recherche externe basées sur le statut](assets/external-lookup-project-status-example2.png)

### Utilisation de valeurs de champ personnalisées dans la recherche externe

Cet exemple vous montre comment appeler l’API Workfront et importer les données d’un champ personnalisé dans votre champ de recherche externe. L’exemple de champ personnalisé est appelé &quot;Couleurs personnalisées&quot;.

1. Ouvrez le formulaire personnalisé.
1. Dans la partie gauche de l’écran, recherchez **Recherche externe** et faites glisser le champ vers une section du canevas.
1. Saisissez l’**étiquette** et le **nom** pour le champ.
1. Sélectionnez le **format** pour le champ.
1. Saisissez l’appel à l’URL de l’API dans le champ **URL API de base**.

   **Exemple**
   `$$HOST/attask/api/v18.0/PORT/search?ID={portfolioID}&fields=parameterValues`

1. Consultez le site **Dépendances** pour connaître les champs auxquels ce champ de recherche fait référence dans l’API.

   Un champ de dépendance peut être n’importe quel champ personnalisé ou natif existant dans la page de détails de l’objet.

1. Sélectionnez la **méthode HTTP** .

   Il s’agira le plus souvent de **Get**.

1. Saisissez le **chemin JSON** pour obtenir les résultats de votre appel API.

   **Exemple**
   `$.data[*].parameterValues.["DE:Combo Colors"]`

   * &quot;parameterValues&quot; fait référence à tout champ personnalisé dans Workfront pour l’objet que vous utilisez.
   * Pour cet exemple, &quot;DE:Combo Colors&quot; est le champ personnalisé spécifique contenant les valeurs que vous souhaitez récupérer.

   >[!NOTE]
   >
   >Les informations de l’**en-tête** ne sont pas nécessaires pour un appel à la même instance de Workfront.

1. Cliquez sur **Appliquer**.

   Lorsque le formulaire personnalisé est ajouté à un objet Workfront, toutes les valeurs du champ &quot;Couleurs de la boîte de dialogue&quot; apparaissent dans la liste déroulante du champ de recherche externe.

## Configuration d’un champ de recherche externe pour l’API de planification Workfront

Un point de terminaison est disponible dans l’API Workfront Planning pour rechercher des enregistrements par identifiant de type d’enregistrement via la méthode Get . Vous pouvez utiliser ce point de terminaison pour référencer des enregistrements de planification dans des champs de recherche externes.

* **URL de l’API de base :** `$$HOST/maestro/api/v1/records/search?recordTypeId={recordTypeID}`
* **Méthode HTTP :** Get
* **Chemin JSON :** `$.records[*].data.{fieldID}`

  **{fieldID}** est le champ à afficher dans les résultats de recherche externe sur le formulaire personnalisé pour les utilisateurs finaux.

Pour plus d’informations, voir [API de planification Workfront](/help/quicksilver/planning/general/planning-api-basics.md).

## Configuration d’un champ de recherche externe pour une API publique

Vous pouvez utiliser la recherche externe pour appeler une API publique externe et récupérer des données.

Cet exemple montre comment appeler une API de pays (telle que <https://api.first.org/data/v1/countries>) afin de ne pas avoir à coder en dur tous les noms de pays dans les options de la liste déroulante.

1. Ouvrez le formulaire personnalisé.
1. Dans la partie gauche de l’écran, recherchez **Recherche externe** et faites glisser le champ vers une section du canevas.
1. Saisissez l’**étiquette** et le **nom** pour le champ.
1. Sélectionnez le **format** pour le champ.
1. Saisissez l’appel à l’URL de l’API dans le champ **URL API de base**.

   * Vous pouvez ajouter $$QUERY pour mettre en œuvre le filtrage des requêtes pour vos utilisateurs finaux et utilisatrices finales.

   **Exemples**
Liste de tous les pays : <https://api.first.org/data/v1/countries>

   Permet de rechercher n’importe quel pays dans le champ déroulant : <https://api.first.org/data/v1/countries?q=$$QUERY>

   Permet de rechercher un pays dans une région : <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * Les régions disponibles sont définies dans un champ personnalisé distinct dans Workfront.
   * Lorsque l’utilisateur sélectionne une région sur le formulaire, le champ de recherche externe affiche uniquement les pays de cette région (le pays dans lequel la région est définie dans l’API). La personne peut également rechercher un pays dans la région sélectionnée.

1. Consultez le site **Dépendances** pour connaître les champs auxquels ce champ de recherche fait référence dans l’API.

   Un champ de dépendance peut être n’importe quel champ personnalisé ou natif existant dans la page de détails de l’objet.

   Dans cet exemple, l’élément `{DE:Region}` sera remplacé par la valeur du champ personnalisé Zone géographique.

1. Sélectionnez la **méthode HTTP**.

   Il s’agira le plus souvent de **Get**.

1. Saisissez le **chemin JSON** pour obtenir les résultats de votre appel API.

   Cette option permet d’extraire des données du JSON renvoyé par l’URL de l’API. Elle permet de sélectionner les valeurs du JSON qui apparaîtront dans les options de la liste déroulante.

   **Exemple**
   `$.data[*].country`

1. (Facultatif) Cliquez sur **Ajouter un en-tête**, et saisissez ou collez la paire clé-valeur requise pour l’authentification avec l’API.

   >[!NOTE]
   >
   >Les champs de l’en-tête ne sont pas un endroit sûr pour stocker des informations d’identification, et vous devez faire attention à ce que vous saisissez et enregistrez.

1. (Facultatif) Sélectionnez **Menu déroulant multi-sélection** pour permettre à la personne de sélectionner plusieurs valeurs dans la liste déroulante.

1. Cliquez sur **Appliquer**.

   ![Configurer un appel API à l’API public dans un formulaire personnalisé](assets/external-lookup-to-api-for-countries.png)

   Lorsque le formulaire personnalisé est ajouté à un objet Workfront (dans cet exemple, un projet), il ressemble à ceci.

   ![Formulaire personnalisé avec champ de recherche externe](assets/external-lookup-countries-example1.png)

   ![Options de recherche externe pour un pays en fonction de la zone géographique](assets/external-lookup-countries-example2.png)

## Cas d’utilisation supplémentaires pour les champs de recherche externes

Il existe de nombreux autres cas d’utilisation pour la création d’une recherche externe.

**Cas d’utilisation :** Remplacez les champs de type caractère , car ils peuvent entraîner des problèmes dans la création de rapports.
**Solution :** Utilisez un appel API pour accéder aux objets existants dans le système.

Exemple d’URL d’API de base pour les modèles, pour remplacer un champ de type :
`$$HOST/attask/api/v17.0/tmpl/search?isActive=true&name_Sort=asc`

**Cas d’utilisation :** Créez des champs de liste déroulante avec plus de fonctionnalités (par exemple, il y a un retour automatique à la ligne dans le champ de recherche externe).
**Solution :** Utilisez un appel API pour les objets existants dans le système, ou créez un objet et utilisez un appel API pour cet objet.

**Cas d’utilisation :** définissez un moyen pour que les utilisateurs conservent leurs propres champs en dehors de la zone de formulaires personnalisée. Configurez le champ Recherche externe et vous pouvez donner aux utilisateurs les objets qui composent le champ. Cette option est adaptée aux équipes et aux champs de maintenance élevés.
**Solution :** Créez un objet et utilisez un appel API vers cet objet.

**Cas pratique :** intégration à des objets en dehors de Workfront. Par exemple, l’accès à un autre système pour obtenir le nom de chaque utilisateur, plutôt que d’être limité dans un champ de saisie anticipée.
**Solution :** Automatisation webhook/Fusion pour se connecter à d’autres systèmes.

