---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Ajouter un webhook à un scénario de base
description: Les webhooks, également appelés déclencheurs instantanés, sont un type spécifique de module de déclenchement qui peut démarrer un scénario chaque fois qu’une modification est effectuée, au lieu d’une planification donnée.
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Ajouter un webhook à un scénario de base dans [!DNL Adobe Workfront Fusion]

Les webhooks, également appelés déclencheurs instantanés, sont un type spécifique de module de déclenchement qui peut démarrer un scénario chaque fois qu’une modification est effectuée, au lieu d’une planification donnée.

Dans cet exemple, vous allez ajouter un webhook pour démarrer un scénario dès que des requêtes ont été envoyées à une file d’attente spécifique. Le scénario convertit ensuite ces requêtes dans un projet.

Cet exemple modifie le scénario créé dans [Créer un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Conditions préalables

Vous devez créer le scénario décrit dans [Créer un scénario de base](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) avant de suivre cette procédure.

## Ajout et configuration du webhook

1. Ouvrez le module d’objet Convert .
1. Dans le champ ID du problème , supprimez le bloc ID noir. Le bloc est noir car le module à partir duquel il a été mappé n’est plus disponible.
1. Sélectionnez le bloc d’identifiant sous le premier module (événements de contrôle) pour le mapper au deuxième module.
1. Cliquez sur **OK**.

### Ajout du module webhook

1. Ouvrez le scénario dans l’éditeur de scénarios.
1. Cliquez avec le bouton droit sur le premier module et sélectionnez **Supprimer le module**.

   Le module est supprimé, laissant un espace réservé vide.

1. Cliquez sur le module vierge, puis sélectionnez **Adobe Workfront** dans la liste des applications.
1. Sélectionnez **Événements de contrôle**.
1. Cliquez sur **Ajouter** en regard du champ Webhook.
1. dans le champ Type d’enregistrement , sélectionnez **Problème**, de sorte que le module se déclenche pour les modifications apportées aux problèmes.
1. Dans le champ État , sélectionnez **Nouvel état**. Il s’agit d’un champ obligatoire utilisé pour le filtre, que cet exemple ne couvre pas.
1. Dans le champ Record Origin, sélectionnez **New Record Only**. Cela permet au scénario de se déclencher lorsqu’un problème est ajouté, et non lorsqu’il est mis à jour ou supprimé.
1. Cliquez sur **Enregistrer** pour enregistrer la configuration du module.
