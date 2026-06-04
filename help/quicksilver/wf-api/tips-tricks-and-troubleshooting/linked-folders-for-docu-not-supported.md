---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Les dossiers liés ne sont pas pris en charge pour l’objet DOCU.
description: Les dossiers liés ne sont pas pris en charge pour l’objet DOCU.
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
TQID: https://experienceleague.adobe.com/iPjiffn9QLDldjWRdxMyf8RTaZaB9X6axc7UVY1B3Bg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 118
ht-degree: 100%

---

# L’utilisation de l’API pour ajouter un dossier lié n’est pas prise en charge.

L’utilisation de l’API pour ajouter un dossier lié au tableau de dossiers pour un objet Document (DOCU) n’est pas prise en charge. La requête aboutira, mais le document risque d’être supprimé du système par certains fournisseurs externes. La raison en est que le système externe sera utilisé comme source ultime de vérité. Par conséquent, si le document est supprimé du fournisseur externe, il est alors considéré comme inexistant. Les documents qui ne figurent pas dans le dossier (externe) lié peuvent être supprimés automatiquement de [!DNL Workfront], sans moyen de les récupérer.
