---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Enregistrements SPF de Workfront Proof
description: Workfront Proof envoie des notifications par e-mail aux personnes chargées de la révision à partir d’une adresse e-mail de Workfront Proof telle que notification@proofing.yourdomain.com. Pour vous assurer que les serveurs de messagerie de vos destinataires font confiance à toutes les notifications par e-mail de Workfront Proof, vous devez configurer un enregistrement [!DNL Sender Policy] Framework (SPF) pour votre domaine personnalisé connecté au compte [!DNL Workfront Proof] (par exemple, proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
TQID: 'https://experienceleague.adobe.com/LTZzs99Zzsn5dbOlu4wP1coyJAMDnnCZZ1pTTbEjT24'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
    internal-label: Workfront Proof
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 80%
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

