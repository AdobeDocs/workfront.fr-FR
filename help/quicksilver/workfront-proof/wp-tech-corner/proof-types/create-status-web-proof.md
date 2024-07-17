---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Création d’un BAT de site web statique à l’aide de  [!DNL Workfront Proof]
description: Vous pouvez créer des BAT statiques à partir de vos pages web. En outre, vous pouvez simuler divers appareils en définissant la résolution d’écran des captures d’écran.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Création d’un BAT de site web statique à l’aide de [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Vous pouvez créer des BAT statiques à partir de vos pages web. En outre, vous pouvez simuler divers appareils en définissant la résolution d’écran des captures d’écran.

## Création d’un BAT de site web statique

1. Ouvrez la page [!UICONTROL New BAT], comme décrit dans la section [Générer des bons à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Collez ou saisissez votre URL dans la zone **www.shareyourlink.com**.
1. Vous pouvez répéter cette étape pour ajouter plusieurs URL.
1. Juste en dessous de cette case, cliquez sur la résolution (la résolution par défaut est 1366x768), puis sélectionnez toutes les résolutions souhaitées dans la zone **[!UICONTROL Résolution Screens]**.
Sélectionnez une résolution plus petite si vous souhaitez tester des conceptions pour les appareils mobiles. En règle générale, les conceptions se chargent selon la résolution de l’écran/de la fenêtre du navigateur.

1. Cliquez sur **[!UICONTROL Rechercher des sous-pages]** si vous souhaitez inclure des pages connectées qui se trouvent dans le même domaine/sous-domaine que l’URL entrée.
   [!DNL Workfront Proof] analyse les pages connectées et les répertorie sous l’option **[!UICONTROL Rechercher des sous-pages]** . Vous pouvez sélectionner les pages à inclure.

1. Avec la fonction [!UICONTROL Combiner les bons à tirer], vous pouvez envoyer toutes les pages web en tant que BAT multi-page unique.
1. Cliquez sur **[!UICONTROL Terminé]**, puis terminez la configuration de votre BAT, comme expliqué dans la section [Générer un bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## À propos des pages et pages protégées par un mot de passe nécessitant une autorisation

[!DNL Workfront Proof] ne peut pas capturer un site web protégé par mot de passe comme BAT statique.

Pour créer des bons à tirer à partir de pages qui requièrent une autorisation, votre équipe informatique doit ajouter l’une des URL suivantes à la Liste autorisée de votre entreprise par le biais de laquelle notre outil de capture web se connecte :

**Grappes AWS aux États-Unis** : webcapture.proofhq.com

**Grappes GCP aux États-Unis** : webcapture.gcp.proofhq.com

**Grappes EMEA{1: webcapture.proofhq.eu**

>[!NOTE]
>
>Nous vous recommandons de procéder à la vérification interactive plutôt que de procéder à la vérification statique des pages internes nécessitant des sites web protégés par une autorisation et un mot de passe. Pour plus d’informations, voir [Présentation des BAT de contenu interactif](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## A propos du traitement des BAT de site web statiques

* Les animations, les vidéos intégrées, les scripts et les interactions ne peuvent pas être inclus dans les bons à tirer de site web statique. Si vous souhaitez tester le contenu interactif, reportez-vous à la section [Générer un bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) de la section [Générer un bon à tirer dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Les pages de BAT sont généralement préparées et capturées à une vitesse d’environ 20 secondes par page. Toutefois, le temps de préparation global dépend également des serveurs sur lesquels les pages sont hébergées. L’outil attend 60 secondes pour que chaque URL envoyée soit chargée. Si ce délai d’attente est dépassé, le BAT échoue.
* Pour les bons à tirer combinés, si l’une des URL ne répond pas à l’outil de capture, le BAT échoue.
* [!DNL Workfront Proof] capture les pages web jusqu’à 195 pouces longtemps après la pixellisation. Si la page web est plus longue que celle-ci, le BAT échoue.
* L’extraction de texte est disponible sur tous les éléments de texte, mais le texte placé en tant qu’images n’est pas extrait.
* Les liens hypertextes peuvent être cliqués sur les bons à tirer et les pages liées s’ouvrent dans les nouveaux onglets du navigateur.
* Il n’est pas possible de cliquer sur les hyperliens des images si les éléments style=&quot;display:block&quot; sont utilisés à l’intérieur des balises `<a>`. Nous vous recommandons d’ajuster ces parties de la conception de la page.
* Pour de meilleurs résultats, il est recommandé de créer les pages à l’aide des bonnes pratiques de codage et des normes reconnues.
