---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Enregistrements SPF de l’épreuve Workfront
description: Workfront Proof envoie des notifications par courrier électronique aux réviseurs à partir d’une adresse électronique Workfront Proof telle que notification@proofing.yourdomain.com. Pour vous assurer que les serveurs de messagerie de vos destinataires font confiance à toutes les notifications par e-mail Workfront Proof, vous devez configurer un enregistrement [!DNL Sender Policy] Framework (SPF) pour votre domaine personnalisé connecté au compte  [!DNL Workfront Proof] (par exemple, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 4%

---

# Enregistrements SPF de l’épreuve Workfront

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d&#39;informations sur la vérification à l&#39;intérieur de [!DNL Adobe Workfront], voir [Proofing](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] envoie des notifications électroniques à vos réviseurs à partir d’une adresse électronique [!DNL Workfront Proof] telle que notification@proofing.yourdomain.com. Pour vous assurer que les serveurs de messagerie de vos destinataires font confiance à toutes les notifications par e-mail [!DNL Workfront Proof], vous devez configurer un enregistrement [!UICONTROL Sender Policy Framework] (SPF) pour votre domaine personnalisé connecté au compte [!DNL Workfront Proof] (par exemple, **proofing.yourdomain.com**).

Pour configurer un enregistrement SPF, vous devez inclure l’enregistrement SPF utilisé pour notre domaine principal.

1. Ajoutez une entrée **[!UICONTROL DNS TXT]** pour votre domaine avec la valeur suivante :

   `v=spf1 a:mx.proofhq.com -all`

   Votre administrateur de messagerie ou votre personnel informatique peut vous aider à configurer cette fonctionnalité.

   >[!TIP]
   >
   >Vous pouvez utiliser l’outil gratuit sur [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) pour consulter les [!DNL Workfront] enregistrements SPF.
