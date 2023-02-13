---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Enregistrements SPF de preuve Workfront
description: Le Bon à tirer Workfront envoie des notifications par courrier électronique aux réviseurs à partir d’une adresse électronique de bon à tirer Workfront telle que notification@proofing.yourdomain.com. Pour vous assurer que les serveurs de messagerie de vos destinataires font confiance à toutes les notifications par e-mail de BAT Workfront, vous devez configurer une [!DNL Sender Policy] Enregistrement SPF (Framework) pour votre domaine personnalisé connecté à [!DNL Workfront Proof] (par exemple, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Enregistrements SPF de preuve Workfront

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome. [!DNL Workfront Proof]. Pour plus d’informations sur la vérification à l’intérieur [!DNL Adobe Workfront], voir [Vérification](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] envoie des notifications par courrier électronique à vos réviseurs à partir d’une [!DNL Workfront Proof] adresse électronique, par exemple notification@proofing.yourdomain.com. Pour vous assurer que les serveurs de messagerie de vos destinataires font confiance à tous les [!DNL Workfront Proof] notifications par e-mail, vous devez configurer une [!UICONTROL Structure de la stratégie d’expéditeur] Enregistrement (SPF) pour votre domaine personnalisé connecté au [!DNL Workfront Proof] compte (par exemple, **proofing.yourdomain.com**).

Pour configurer un enregistrement SPF, vous devez inclure l’enregistrement SPF utilisé pour notre domaine Principal.

1. Ajouter un **[!UICONTROL TXT DNS]** entrée pour votre domaine avec la valeur suivante :

   `v=spf1 a:mx.proofhq.com -all`

   Votre administrateur de messagerie ou votre personnel informatique peut vous aider à configurer cette fonctionnalité.

   >[!TIP]
   >
   >Vous pouvez utiliser l’outil gratuit à l’adresse [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) pour la révision [!DNL Workfront] Enregistrements SPF.
