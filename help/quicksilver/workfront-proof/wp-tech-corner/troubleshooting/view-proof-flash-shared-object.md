---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problèmes D'Affichage Des Bons À Tirer - Explication Des Objets Partagés De Flash
description: "Remarque : Les informations de cet article font référence à des fonctionnalités actuellement obsolètes et qui seront supprimées de [!DNL Workfront] en 2018. Nous vous recommandons d’utiliser la nouvelle visionneuse de profilage web (comme décrit dans la section Révision de BAT dans la visionneuse de vérification de l’intégrité web) ou la visionneuse de vérification de l’intégrité du bureau (comme décrit dans la section Révision de BAT dans la visionneuse de vérification de l’intégrité du bureau)."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f1f3561e-8660-4c1e-b48f-446eb0eaac06
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Problèmes D&#39;Affichage Des Bons À Tirer - [!DNL Flash] Explication des objets partagés

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

>[!NOTE]
>
>Les informations de cet article font référence à des fonctionnalités actuellement obsolètes et qui seront supprimées de [!DNL Workfront] en 2018. Nous vous recommandons d’utiliser la nouvelle visionneuse de Web Proofing (comme décrit dans la section [Vérification de BAT dans la visionneuse de BAT Web](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer)) ou de la visionneuse de vérification de l’appli de bureau (comme décrit dans la section [Vérification des bons à tirer dans la visionneuse de vérification de l’appli de bureau](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)).

## [!DNL Flash] Objets partagés

Un objet partagé local, parfois appelé &quot;[!DNL Flash] &quot;cookie&quot; est un fichier de données qui peut être créé sur votre ordinateur par les sites que vous visitez. Les objets partagés sont le plus souvent utilisés pour améliorer votre expérience de navigation sur le Web. A [!DNL Flash] cookie est un message utilisé dans [!DNL Adobe Flash] qui est envoyé d’un serveur Web à un navigateur Web, puis stocké en tant que fichier de données dans le navigateur.

Depuis la variable [!DNL Workfront Proof] La visionneuse est basée sur [!DNL Flash], il serait utile de vérifier le stockage autorisé pour [!DNL Flash] sur votre ordinateur.

## [!DNL Flash] Objets partagés - problèmes connus

Si la variable [!DNL Flash] Le stockage est défini sur 0 Ko ou dispose d’un autre paramètre qui bloque [!DNL Flash] à partir de l’enregistrement local des données, cela peut entraîner des problèmes connus dans la variable [!DNL Workfront Proof] Observateur :

* La fenêtre contextuelle d’aperçu &quot;Prise en main&quot; continue d’apparaître bien que l’option de ne plus l’afficher ait été sélectionnée.
* [!DNL Workfront Proof] Les performances de la visionneuse ralentissent en raison de l’augmentation du nombre de commentaires ajoutés aux bons à tirer
* Les bons à tirer ne se chargent pas et vous obtenez un &quot;écran gris&quot; au lieu d’une image réelle.

## Autoriser [!DNL Flash] Objets partagés

Veillez à ce que le stockage [!DNL Flash] Les objets partagés sont autorisés sur l’ordinateur et la limite de stockage n’est pas 0.

Pour vérifier si les objets partagés sont autorisés :

1. Cliquez avec le bouton droit de la souris dans le [!DNL Workfront Proof] Visionneuse.
1. Sélectionner **[!UICONTROL Paramètres globaux]** dans le menu contextuel.
1. Accédez au **[!UICONTROL Stockage]** .
1. Assurez-vous que **[!UICONTROL Autoriser les sites à enregistrer des informations sur cet ordinateur]** est sélectionné (1).
1. ![2017-06-09_1929.png](assets/2017-06-09-1929-350x267.png)

## Augmentation [!DNL Flash] stockage

Par défaut [!DNL Flash] Les applications peuvent stocker jusqu’à 100 Ko de données sur le lecteur de l’utilisateur, mais celles-ci peuvent être facilement modifiées par les utilisateurs. La solution pour le plus grand nombre [!DNL Flash] les problèmes connexes sont les suivants : augmenter les [!DNL Flash] stockage. Vous pouvez le faire directement à partir de la fonction [!DNL Workfront Proof] Observateur :

1. Ouvrez un bon à tirer.
1. Ouvrez le menu contextuel sur le BAT.
1. Cliquez sur **[!UICONTROL Paramètres]** pour ouvrir le [!DNL Flash] s’affiche.
1. Accédez au **[!UICONTROL Local]** stockage .
1. Augmentez le stockage jusqu’à 100 Ko (1, par exemple).
1. Fermez la fenêtre contextuelle des paramètres et rouvrez le BAT .

![2017-06-09_1926.png](assets/2017-06-09-1926-350x274.png)
