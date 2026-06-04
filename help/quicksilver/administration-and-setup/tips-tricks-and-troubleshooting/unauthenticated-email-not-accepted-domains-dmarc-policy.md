---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Les e-mails non authentifiés ne sont pas acceptés en raison de la politique DMARC du domaine
description: Si un e-mail envoyé depuis le système  [!DNL Workfront]  n’est pas accepté en raison de la politique DMARC du domaine, votre administrateur ou administratrice de messagerie peut résoudre le problème en configurant votre système de messagerie pour autoriser tous les e-mails provenant de workfront.com.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
TQID: https://experienceleague.adobe.com/f44Wkid-gwfXgHKmSKa6oevhN5jA6720JTlOcH8kJKY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 177
ht-degree: 94%

---

# Les e-mails non authentifiés ne sont pas acceptés en raison de la politique DMARC du domaine.

## Problème

[Test] J’ai reçu l’e-mail de rebond suivant :

550-5.7.1 L’email non authentifié de « customer domain.com » n’est pas accepté en raison de\
550-5.7.1 la politique DMARC du domaine. Veuillez contacter l’administrateur ou l’administratrice du domaine « customer domain.com »\
550-5.7.1 s’il s&#39;agit d’un e-mail légitime. Veuillez consulter la page\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) pour en savoir plus sur l’initiative\
550 5.7.1 DMARC.

## Solution

DMARC est configuré dans le système de messagerie de votre entreprise et ne fait pas partie d’[!DNL Adobe Workfront]. Si vous recevez cet e-mail, vous devez contacter votre administrateur ou administratrice de messagerie.

Votre administrateur ou administratrice de messagerie doit configurer votre système de messagerie pour autoriser/approuver les e-mails provenant de noreply@workfront.com ou, de préférence, tous les e-mails provenant de workfront.com.

Pour plus d’informations sur DMARC, voir [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
