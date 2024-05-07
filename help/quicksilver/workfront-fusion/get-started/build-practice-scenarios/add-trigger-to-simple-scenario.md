---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Ajouter un module de déclenchement à un scénario de base
description: Découvrez comment ajouter un module de déclenchement pour permettre au scénario de rechercher périodiquement de nouvelles requêtes et de les convertir en projets.
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Ajouter un module de déclenchement à un scénario de base

Les modules de déclenchement sont placés au début d’un scénario. Ces modules commencent une exécution de scénario lorsque des critères spécifiques ont été modifiés dans un service donné. La modification peut être la création de nouveaux enregistrements, la suppression d’un enregistrement, la mise à jour d’un enregistrement, etc.

Les modules d’interrogation vérifient le service à un intervalle de temps défini et renvoient des informations sur les modifications qui se sont produites au cours de cet intervalle. Si aucune modification n’a été apportée, le déclencheur n’exécute pas le scénario.

Dans cet exemple, vous allez ajouter un module de déclenchement qui s’exécute toutes les 15 minutes et lance un scénario si des demandes ont été envoyées à une file d’attente spécifique. Le scénario convertit ensuite ces requêtes dans un projet.

Cet exemple modifie le scénario créé dans [Création d’un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Conditions préalables

Vous devez créer le scénario décrit dans la section [Création d’un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) avant de suivre cette procédure.

## Ajouter et configurer le module déclencheur

### Ajouter le module déclencheur

1. Ouvrez le scénario dans l’éditeur de scénarios.
1. Cliquez avec le bouton droit sur le premier module (Recherche) et sélectionnez **Supprimer le module**.

   Le module est supprimé, laissant un espace réservé vide.

1. Cliquez sur le module vierge, puis sélectionnez **Adobe Workfront** dans la liste des applications.
1. Sélectionner **Surveiller les enregistrements**.
1. Assurez-vous que le module utilise la même connexion que le reste des modules dans le scénario.
1. Dans le champ Filtre , sélectionnez **Nouveaux enregistrements uniquement**.
1. Dans la zone Outputs, sélectionnez `ID`, `Name`, et `Project ID`.
1. Cliquez sur **OK** pour enregistrer les paramètres du module.

   Une fenêtre Choisir où commencer s’affiche.

1. Sélectionner **Désormais**.

### Planification du module de déclenchement

1. Cliquez sur l’horloge du module Enregistrements de contrôle.

   La fenêtre Paramètres de planification s’ouvre.

1. Dans le champ Exécuter le scénario , sélectionnez **À intervalles réguliers**.

1. Cliquez sur **OK**.

### Mettre à jour le deuxième module

Le premier module ayant été remplacé, le deuxième module doit être mappé au nouveau premier module.

1. Ouvrez le module d’objet Convert .
1. Dans le champ ID du problème , supprimez le bloc ID noir. Le bloc est noir car le module à partir duquel il a été mappé n’est plus disponible.
1. Sélectionnez le bloc ID sous le premier module (Enregistrements de contrôle) pour le mapper au second module.
1. Cliquez sur **OK**.

### Tester et activer

1. Accédez à l’environnement Workfront auquel Fusion se connecte et ajoutez un problème.
1. Cliquez sur **[!UICONTROL Exécuter une seule fois]** dans le coin inférieur gauche de l’éditeur de scénarios.
1. Examinez la sortie pour vous assurer que le scénario s’est exécuté comme prévu.
1. Lorsque vous êtes satisfait que le scénario fonctionne comme prévu, cliquez sur le bouton **Planification** basculez le curseur dans le coin inférieur gauche de l’écran sur **Activé**.

   Cela active le scénario.
1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** près du coin inférieur gauche pour enregistrer la progression sur le scénario.

   >[!IMPORTANT]
   >
   >Enregistrez souvent lorsque vous affinez et testez un scénario.

## Ressources

* Pour plus d’informations sur les webhooks, voir [Déclencheurs instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
