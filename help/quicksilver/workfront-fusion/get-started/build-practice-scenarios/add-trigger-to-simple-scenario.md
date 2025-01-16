---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Ajout d’un module de déclenchement à un scénario de base
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 067ee6a1-f4c1-4602-ac39-0283255cced8
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 8%

---

# Ajout d’un module de déclenchement à un scénario de base

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Ajouter un module de déclenchement à un scénario de base](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-trigger-to-basic-scenario.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Les modules Trigger sont placés au début d’un scénario. Ces modules démarrent une exécution de scénario lorsque des critères spécifiques ont été modifiés dans un service donné. La modification peut consister en la création d’enregistrements, la suppression d’un enregistrement, la mise à jour d’un enregistrement, etc.

Les modules d’interrogation vérifient le service à un intervalle de temps défini et renvoient des informations sur les modifications qui se sont produites au cours de cet intervalle de temps. Si aucune modification n’a été apportée, le déclencheur n’exécute pas le scénario.

Dans cet exemple, vous allez ajouter un module déclencheur qui s’exécute toutes les 15 minutes et démarre un scénario si des requêtes ont été envoyées à une file d’attente spécifique. Le scénario convertit ensuite ces requêtes en projet.

Cet exemple montre comment modifier le scénario créé dans [Créer un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Conditions préalables

Vous devez créer le scénario décrit dans [Créer un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) avant de suivre cette procédure.

## Ajout et configuration du module de déclenchement

### Ajout du module de déclenchement

1. Ouvrez le scénario dans l’éditeur de scénarios.
1. Cliquez avec le bouton droit sur le premier module (Rechercher) et sélectionnez **Supprimer le module**.

   Le module est supprimé, laissant un espace réservé vide.

1. Cliquez sur le module vierge, puis sélectionnez **Adobe Workfront** dans la liste des applications.
1. Sélectionnez **Enregistrement de contrôle**.
1. Assurez-vous que le module utilise la même connexion que le reste des modules du scénario.
1. Dans le champ Filtrer , sélectionnez **Nouveaux enregistrements uniquement**.
1. Dans le champ Type d’enregistrement , sélectionnez **Événement**.
1. Dans la zone Sorties, sélectionnez `ID`, `Name` et `Project ID`.
1. Cliquez sur **OK** pour enregistrer les paramètres du module.

   Une fenêtre Choisir où commencer s’affiche.

1. Sélectionnez **À partir de maintenant**.

### Planification du module de déclenchement

1. Cliquez sur l&#39;horloge sur le module Watch Records.

   La fenêtre du paramètre Planification s’ouvre.

1. Dans le champ Exécuter le scénario , sélectionnez **À intervalles réguliers**.

1. Cliquez sur **OK**.

### Mise à jour du deuxième module

Le premier module ayant été remplacé, le second module doit être mappé au nouveau premier module.

1. Ouvrez le module Convertir l’objet .
1. Dans le champ ID de l’événement , supprimez le bloc d’ID noir. Le bloc est noir, car le module à partir duquel il a été mappé n’est plus disponible.
1. Sélectionnez le bloc d’ID sous le premier module (Enregistrements de contrôle) pour le mapper au second module.
1. Cliquez sur **OK**.

### Tester et activer

1. Accédez à l’environnement Workfront auquel Fusion se connecte et ajoutez un problème.
1. Cliquez sur **[!UICONTROL Exécuter une fois]** dans le coin inférieur gauche de l’éditeur de scénario.
1. Examinez la sortie pour vous assurer que le scénario s’est exécuté comme prévu.
1. Lorsque vous êtes convaincu que le scénario fonctionne comme prévu, cliquez sur le bouton (bascule) **Planification** dans le coin inférieur gauche de l’écran pour **Activé**.

   Le scénario est alors activé.
1. Dans [!DNL Workfront Fusion], cliquez sur **[!UICONTROL Enregistrer]** près du coin inférieur gauche pour enregistrer votre progression dans le scénario.

   >[!IMPORTANT]
   >
   >Sauvegardez souvent lorsque vous affinez et testez un scénario.

## Ressources

* Pour plus d’informations sur les webhooks, voir [Déclencheurs instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
