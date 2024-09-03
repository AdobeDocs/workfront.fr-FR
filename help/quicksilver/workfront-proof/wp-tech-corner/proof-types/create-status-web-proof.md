---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Créer une épreuve statique de site web à l’aide de  [!DNL Workfront Proof]
description: Vous pouvez créer des épreuves statiques à partir de vos pages web. En outre, vous pouvez simuler divers appareils en définissant la résolution des captures d’écran.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 100%

---

# Créer une épreuve statique de site web à l’aide de [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Vous pouvez créer des épreuves statiques à partir de vos pages web. En outre, vous pouvez simuler divers appareils en définissant la résolution des captures d’écran.

## Créer une épreuve statique de site web

1. Ouvrez la page [!UICONTROL Nouvelle épreuve], comme décrit dans la section [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Collez ou entrez votre URL dans la zone **www.shareyourlink.com**.
1. Vous pouvez répéter cette étape pour ajouter plusieurs URL.
1. Juste en dessous de cette zone, cliquez sur la résolution (la valeur par défaut est 1366 x 768), puis sélectionnez les résolutions de votre choix dans la zone **[!UICONTROL Résolution de capture d’écran]**.
Sélectionnez une résolution plus petite si vous souhaitez réviser des conceptions pour appareils mobiles. En règle générale, les conceptions se chargent selon la résolution de l’écran/de la fenêtre du navigateur.

1. Cliquez sur **[!UICONTROL Rechercher des sous-pages]** si vous souhaitez inclure des pages connectées qui se trouvent dans le même domaine/sous-domaine que l’URL saisie.
   [!DNL Workfront Proof] analyse les pages connectées et les répertorie sous l’option **[!UICONTROL Rechercher des sous-pages]**. Vous pouvez sélectionner les pages à inclure.

1. Grâce à la fonctionnalité [!UICONTROL Combiner des épreuves], vous pouvez soumettre toutes les pages web sous la forme d’une épreuve à plusieurs pages.
1. Cliquez sur **[!UICONTROL Terminé]**, puis terminez la configuration de votre épreuve, comme expliqué dans [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## À propos des pages protégées par mot de passe et des pages nécessitant une autorisation

[!DNL Workfront Proof] ne peut pas capturer un site web protégé par mot de passe comme une épreuve statique.

Pour créer des épreuves à partir de pages nécessitant une autorisation, votre équipe informatique doit ajouter l’une des URL suivantes à la liste autorisée de votre entreprise, via laquelle notre outil de capture web est connecté :

**Clusters AWS aux États-Unis** : webcapture.proofhq.com

**Clusters GCP aux États-Unis** : webcapture.gcp.proofhq.com

**Clusters EMEA** : webcapture.proofhq.eu

>[!NOTE]
>
>Nous vous recommandons de procéder à la relecture interactive plutôt qu’à la relecture statique des pages internes nécessitant des sites web protégés par une autorisation et un mot de passe. Pour plus d’informations, voir [Vue d’ensemble des épreuves de contenu interactif](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## À propos du traitement des épreuves statiques de site web

* Les animations, les vidéos intégrées, les scripts et les interactions ne peuvent pas être inclus dans les épreuves statiques de site web. Si vous souhaitez réviser du contenu interactif, voir [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) dans [Générer des épreuves dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Les pages de l’épreuve sont généralement préparées et capturées à une vitesse d’environ 20 secondes par page. Toutefois, le temps de préparation global dépend également des serveurs sur lesquels les pages sont hébergées. L’outil attend 60 secondes pour que chaque URL envoyée soit chargée. Si ce délai d’attente est dépassé, l’épreuve échoue.
* Pour les épreuves combinées, si l’une des URL ne répond pas à l’outil de capture, l’épreuve échoue.
* [!DNL Workfront Proof] capture les pages web d’une longueur maximale de 195 pouces après le tramage. Si la page web dépasse cette limite, l’épreuve échoue.
* L’extraction de texte est disponible sur tous les éléments de texte, mais le texte placé en tant qu’images n’est pas extrait.
* Vous pouvez cliquer sur les hyperliens figurant sur les épreuves, et les pages liées s’ouvrent dans de nouveaux onglets du navigateur.
* Il n’est pas possible de cliquer sur les hyperliens des images si les éléments style=&quot;display:block&quot; sont utilisés dans les balises `<a>`. Nous vous recommandons d’ajuster ces parties de la conception de la page.
* Pour de meilleurs résultats, il est recommandé de créer les pages à l’aide des bonnes pratiques de codage et des normes reconnues.
