---
content-type: reference
navigation-topic: announcements
title: Usurpation d’adresses e-mail et suppression des réponses POP
description: Nous apportons deux modifications à la façon dont Adobe Workfront envoie et reçoit des e-mails avec la version 20.3 (prévue en août 2020).
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 84%

---

# Usurpation d’adresses e-mail et réponses POP

Nous apportons deux modifications à la façon dont Adobe Workfront envoie et reçoit des e-mails avec la version 20.3 (prévue en août 2020).

## E-mails sortants de Workfront

Afin d’accroître la diffusion réussie des e-mails, nous allons éliminer l’usurpation d’adresses e-mail, souvent taguées comme spam (voir la section Usurpation d’adresses e-mail). Tous les e-mails provenant de Workfront seront envoyés depuis `notifications@my.workfront.com`, y compris les alertes automatisées et les communications utilisateur à utilisateur. Voici un exemple d’e-mail de Joan Harris dans la zone « De » de votre e-mail :

![Exemple d’e-mail](assets/noreply.png)

*Nous vous recommandons vivement de contacter votre équipe informatique* pour vous assurer que les e-mails provenant de l’adresse `notifications@my.workfront.com` ne seront pas bloqués pour les e-mails entrants sur votre système. Vous pouvez également consulter la section [Configurer la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) pour plus d’informations sur les adresses IP à l’origine de notre trafic et de nos e-mails.

## Réponses électroniques entrantes aux notifications (réponse POP)

Certaines notifications électroniques permettent de répondre par e-mail. La réponse est alors copiée dans Workfront sous forme de réponse de commentaire dans le système Workfront. Les administrateurs et administratrices système de Workfront ont toujours pu choisir entre fournir leur propre serveur de messagerie POP pour recevoir ces réponses ou utiliser le système de réponse Workfront intégré. Le choix du serveur de messagerie POP personnalisé est supprimé dans la version 20.3. Tous les comptes configurés pour utiliser un serveur personnalisé seront automatiquement modifiés afin d’utiliser le système de réponse par e-mail natif de Workfront. Aucune action n’est requise des équipes d’administration système ni des autres utilisateurs et utilisatrices de Workfront.

Les e-mails provenant directement du système Workfront Proof ne seront pas modifiés. Vous continuerez à les recevoir comme par le passé.

Pour toute autre question ou préoccupation, contactez l’[Équipe d’assistance Workfront](https://experienceleague.adobe.com/?support-tab=home#support).
