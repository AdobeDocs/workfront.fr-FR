---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Environnement de test Sandbox de prévisualisation- [!DNL Workfront Proof]
description: L’environnement de prévisualisation de sandbox est un environnement de test qui sert de réplique à votre environnement réel et qui est actualisé chaque week-end par  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 100%

---

# Environnement de test Sandbox de prévisualisation- [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

L’environnement de prévisualisation de sandbox est un environnement de test qui sert de réplique à votre environnement réel et qui est actualisé chaque week-end par [!DNL Workfront Proof].

## Comprendre l’environnement de sandbox de prévisualisation

L’environnement de prévisualisation de sandbox sert d’environnement dans lequel les utilisateurs et les utilisatrices de votre organisation peuvent tester et travailler en toute sécurité avec les données de l’environnement de production sans affecter ce dernier. Il est idéal pour exécuter des sessions de formation, tester de nouvelles fonctionnalités et déterminer les fonctionnalités de configuration.

En outre, de nouvelles fonctionnalités de produit sont chargées dans l’environnement de sandbox de prévisualisation avant d’être diffusées dans l’environnement de production. Vos utilisateurs et utilisatrices peuvent y essayer de nouvelles fonctionnalités sans affecter leur workflow habituel dans l’environnement de production.

L’environnement de sandbox de prévisualisation contient vos données de production réelles. Les données passent de la production à la prévisualisation, et non l’inverse. Il s’actualise chaque week-end, de sorte que les données peuvent avoir jusqu’à une semaine de retard sur l’environnement de production. Les éléments créés depuis la dernière actualisation sont dans l’environnement de prévisualisation de sandbox jusqu’à l’actualisation suivante.

## Accéder à l’environnement de prévisualisation de sandbox

Par défaut, en tant qu’administrateur ou administratrice système, vous avez accès à l’environnement de sandbox de prévisualisation. Si vous ne pouvez pas accéder à l’environnement de sandbox de prévisualisation comme décrit dans cette section, contactez votre administrateur ou adminsitratrice [!DNL Workfront] ou notre équipe d’assistance.

* [Accéder à l’environnement de sandbox de prévisualisation en tant que client ou cliente  [!DNL Workfront Proof]  autonome](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [Accéder à l’environnement de sandbox de prévisualisation en tant que client ou cliente  [!DNL Workfront]+[!DNL Workfront Proof] ](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### Accéder à l’environnement de sandbox de prévisualisation en tant que client ou cliente [!DNL Workfront Proof] autonome

1. Accédez à cette URL : `https://preview.proofhq.com`.
1. Connectez-vous à l’aide de vos identifiants de prévisualisation.\
   Vos identifiants de prévisualisation doivent être les mêmes que vos identifiants de production, à moins que vous ne les ayez modifiés dans la production après l’actualisation de la prévisualisation. Les connexions ne sont synchronisées que lorsqu’une actualisation a lieu, ce qui se produit chaque week-end. Elles ne se synchronisent pas automatiquement.

### Accéder à l’environnement de sandbox de prévisualisation en tant que client ou cliente [!DNL Workfront+Workfront] Proof

En tant que personne membre de l’équipe d’administration [!DNL Workfront Proof], vous pouvez accéder à l’environnement de prévisualisation de sandbox via l’interface [!DNL Workfront].

Pour accéder à l’environnement de sandbox de prévisualisation [!DNL Workfront Proof] :

1. Connectez-vous à votre environnement [!DNL Workfront].
1. Cliquez sur **[!UICONTROL Configuration]** dans la barre de navigation globale.
1. Cliquez sur **[!UICONTROL Système]** >**[!UICONTROL Préférences]**.

1. Dans la section **[!UICONTROL Environnements de test]**, cliquez sur **[!UICONTROL Prévisualisation de sandbox]**.

1. Connectez-vous avec vos identifiants de prévisualisation.\
   Vos identifiants de prévisualisation doivent être les mêmes que vos identifiants de production, à moins que vous ne les ayez modifiés dans la production après l’actualisation de la prévisualisation. Les connexions ne sont synchronisées que lorsqu’une actualisation a lieu. Elles ne se synchronisent pas automatiquement.
1. Cliquez sur l’icône [!DNL Workfront Proof] dans la barre de navigation globale.\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   L’environnement de prévisualisation [!DNL Workfront Proof] s’affiche.

## Recevoir des e-mails à partir de la prévisualisation de sandbox

Les notifications par e-mail ne sont jamais déclenchées à partir de l’environnement de prévisualisation [!DNL Workfront Proof].
