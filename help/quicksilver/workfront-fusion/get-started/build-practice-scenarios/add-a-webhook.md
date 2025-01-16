---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Ajout d’un webhook à un scénario de base
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Ajout d’un webhook à un scénario de base dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Ajouter un webhook à un scénario de base](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-a-webhook-to-basic-scenario.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Les Webhooks, également appelés déclencheurs instantanés, sont un type spécifique de module de déclenchement qui peut démarrer un scénario à chaque modification, plutôt que selon un planning donné.

Dans cet exemple, vous allez ajouter un webhook pour démarrer un scénario dès que les requêtes ont été envoyées à une file d’attente spécifique. Le scénario convertit ensuite ces requêtes en projet.

Cet exemple montre comment modifier le scénario créé dans [Créer un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Conditions préalables

Vous devez créer le scénario décrit dans [Créer un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) avant de suivre cette procédure.

## Ajouter et configurer le webhook

1. Ouvrez le module Convertir l’objet .
1. Dans le champ ID de l’événement , supprimez le bloc d’ID noir. Le bloc est noir, car le module à partir duquel il a été mappé n’est plus disponible.
1. Sélectionnez le bloc d’identifiant sous le premier module (Événements Espion) pour le mapper au second module.
1. Cliquez sur **OK**.

### Ajouter le module webhook

1. Ouvrez le scénario dans l’éditeur de scénarios.
1. Cliquez avec le bouton droit sur le premier module et sélectionnez **Supprimer le module**.

   Le module est supprimé, laissant un espace réservé vide.

1. Cliquez sur le module vierge, puis sélectionnez **Adobe Workfront** dans la liste des applications.
1. Sélectionnez **Observer les événements**.
1. Cliquez sur **Ajouter** en regard du champ Webhook.
1. dans le champ Type d’enregistrement , sélectionnez **Problème** afin que le module se déclenche pour les modifications dans les problèmes.
1. Dans le champ Etat , sélectionnez **Nouvel état**. Il s’agit d’un champ obligatoire utilisé pour le filtre, que cet exemple ne couvre pas.
1. Dans le champ Origine de l’enregistrement , sélectionnez **Nouvel enregistrement uniquement**. Cela permet au scénario de se déclencher lorsqu’un événement est ajouté, et non lorsqu’un événement est mis à jour ou supprimé.
1. Cliquez sur **Enregistrer** pour enregistrer la configuration du module.
