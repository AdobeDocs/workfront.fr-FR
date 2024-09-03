---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Enregistrements SPF de Workfront Proof
description: Workfront Proof envoie des notifications par e-mail aux personnes chargées de la révision à partir d’une adresse e-mail de Workfront Proof telle que notification@proofing.yourdomain.com. Afin de s’assurer que les serveurs de messagerie de vos destinataires font confiance à toutes les notifications par e-mail de Workfront Proof, vous devez configurer un  [!DNL Sender Policy] enregistrement SPF (« Sender Policy Framework ») pour votre domaine personnalisé connecté au compte  [!DNL Workfront Proof]  (par exemple, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 100%

---

# Enregistrements SPF de Workfront Proof

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] envoie des notifications par e-mail aux personnes chargées de la révision à partir d’une adresse e-mail [!DNL Workfront Proof] telle que notification@proofing.yourdomain.com. Afin de s’assurer que les serveurs de messagerie de vos destinataires font confiance à toutes les notifications par e-mail de [!DNL Workfront Proof], vous devez configurer un [!UICONTROL enregistrement SPF (« Sender Policy Framework »)] pour votre domaine personnalisé connecté au compte [!DNL Workfront Proof] (par exemple, **proofing.yourdomain.com**).

Pour configurer un enregistrement SPF, vous devrez inclure l’enregistrement SPF utilisé pour notre domaine principal.

1. Ajoutez une entrée **[!UICONTROL DNS TXT]** pour votre domaine avec la valeur suivante :

   `v=spf1 a:mx.proofhq.com -all`

   Votre administrateur ou administratrice de messagerie ou votre personnel informatique peut vous aider à configurer cette fonction.

   >[!TIP]
   >
   >Vous pouvez utiliser l’outil gratuit disponible à l’adresse [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) pour examiner les enregistrements SPF de [!DNL Workfront].
