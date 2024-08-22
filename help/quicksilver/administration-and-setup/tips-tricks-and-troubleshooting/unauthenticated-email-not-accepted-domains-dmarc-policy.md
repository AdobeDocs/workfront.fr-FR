---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Le message non authentifié n’est pas accepté en raison de la stratégie DMARC du domaine
description: Si un email envoyé depuis le système  [!DNL Workfront] n'est pas accepté en raison de la stratégie DMARC du domaine, votre administrateur de messagerie peut résoudre le problème en configurant votre système de messagerie pour autoriser tous les emails provenant de workfront.com.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 1%

---

# Les emails non authentifiés ne sont pas acceptés en raison de la politique DMARC du domaine.

## Problème

[Test] J’ai reçu le retour de mails suivant :

550-5.7.1 Les emails non authentifiés de &quot;domaine client.com&quot; ne sont pas acceptés en raison de\
550-5.7.1 - Politique DMARC du domaine. Veuillez contacter l’administrateur de &quot;customer domain.com&quot;.\
Domaine 550-5.7.1 s’il s’agissait d’un courrier légitime. Veuillez consulter\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) pour en savoir plus sur DMARC\
550 5.7.1.

## Solution

DMARC est configuré dans le système de messagerie de votre entreprise et ne fait pas partie de [!DNL Adobe Workfront]. Si vous recevez cet email, vous devez contacter votre administrateur de messagerie.

Votre administrateur de messagerie doit configurer votre système de messagerie pour autoriser/approuver les courriers électroniques de noreply@workfront.com ou, de préférence, tous les courriers électroniques de workfront.com.

Pour plus d’informations sur DMARC, voir [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
