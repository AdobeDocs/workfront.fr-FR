---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Le message non authentifié n’est pas accepté en raison de la stratégie DMARC du domaine
description: Si un e-mail envoyé depuis le système  [!DNL Workfront]  n’est pas accepté en raison de la politique DMARC du domaine, votre administrateur ou administratrice de messagerie peut résoudre le problème en configurant votre système de messagerie pour autoriser tous les e-mails provenant de workfront.com.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 93%

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
