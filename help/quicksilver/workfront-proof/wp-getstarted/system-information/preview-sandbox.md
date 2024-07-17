---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Aperçu de l’environnement de test Sandbox - [!DNL Workfront Proof]
description: L’environnement de test Aperçu est un environnement de test qui sert de réplique à votre environnement en ligne et qui est actualisé chaque week-end par  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 5%

---

# Aperçu de l’environnement de test Sandbox - [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

L’environnement de test Aperçu Sandbox est un environnement de test qui sert de réplique de votre environnement en ligne et qui est actualisé chaque week-end par [!DNL Workfront Proof].

## Présentation de l’aperçu de l’environnement de test

L’environnement de test Aperçu sert d’environnement dans lequel les utilisateurs de votre entreprise peuvent tester et utiliser en toute sécurité les données de l’environnement de production sans affecter l’environnement de production. Il est idéal pour exécuter des sessions de formation, tester de nouvelles fonctionnalités et déterminer les fonctionnalités de configuration.

En outre, de nouvelles fonctionnalités de produit sont chargées dans l’environnement de prévisualisation Sandbox avant d’être diffusées dans l’environnement de production. Vos utilisateurs peuvent y essayer de nouvelles fonctionnalités sans affecter leur workflow habituel dans l’environnement de production.

L’environnement de test Aperçu contient vos données de production réelles. Flux de données de la production à la prévisualisation, et non inverse. Il s’actualise chaque week-end, de sorte que les données peuvent se trouver jusqu’à une semaine après l’environnement de production. Les éléments créés depuis la dernière actualisation sont placés dans l’environnement Aperçu de l’environnement de test jusqu’à l’actualisation suivante.

## Accès à l’environnement de test d’aperçu

Par défaut, en tant qu’administrateur système, vous avez accès à l’environnement Preview Sandbox . Si vous ne pouvez pas accéder à l’environnement Preview Sandbox comme décrit dans cette section, contactez votre administrateur [!DNL Workfront] ou notre équipe d’assistance.

* [Accès à l’environnement de test d’aperçu en tant que client autonome [!DNL Workfront Proof] ](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [Accès à Preview Sandbox as a [!DNL Workfront]+[!DNL Workfront Proof] Customer](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### Accès à l’environnement de test d’aperçu en tant que client [!DNL Workfront Proof] autonome

1. Accédez à cette URL : `https://preview.proofhq.com`.
1. Connectez-vous à l’aide de vos informations d’identification de prévisualisation.\
   Vos informations d’identification d’aperçu doivent être identiques à celles de vos informations d’identification de production, sauf si vous les avez modifiées dans Production après l’actualisation de l’aperçu. Les connexions ne sont synchronisées que lorsqu’une actualisation a lieu chaque week-end. Elles ne se synchronisent pas automatiquement.

### Accès à l’environnement de test d’aperçu en tant que client de BAT [!DNL Workfront+Workfront]

En tant qu’administrateur système, vous pouvez accéder à l’environnement de test de prévisualisation [!DNL Workfront Proof] via l’interface [!DNL Workfront].

Pour accéder à l’environnement de test de prévisualisation [!DNL Workfront Proof] :

1. Connectez-vous à votre environnement [!DNL Workfront].
1. Cliquez sur **[!UICONTROL Configuration]** dans la barre de navigation globale.
1. Cliquez sur **[!UICONTROL Système]** > **[!UICONTROL Préférences]**.

1. Dans la section **[!UICONTROL Test Environments]**, cliquez sur **[!UICONTROL Sandbox Preview]**.

1. Connectez-vous à l’aide de vos informations d’identification d’aperçu.\
   Vos informations d’identification d’aperçu doivent être identiques à celles de vos informations d’identification de production, sauf si vous les avez modifiées dans Production après l’actualisation de l’aperçu. Les connexions ne sont synchronisées que lorsqu’une actualisation se produit. Elles ne se synchronisent pas automatiquement.
1. Cliquez sur l’icône [!DNL Workfront Proof] dans la barre de navigation globale.\
   ![BAT_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   L’environnement de prévisualisation [!DNL Workfront Proof] s’affiche.

## Réception d’emails à partir de l’environnement de test de prévisualisation

Les notifications électroniques ne sont jamais déclenchées à partir de l’environnement d’aperçu [!DNL Workfront Proof].
