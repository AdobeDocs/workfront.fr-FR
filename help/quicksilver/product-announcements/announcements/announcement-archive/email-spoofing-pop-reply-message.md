---
content-type: reference
navigation-topic: announcements
title: usurpation des emails et suppression des réponses POP
description: Nous apportons deux modifications à la façon dont Adobe Workfront envoie et reçoit des emails avec la version 20.3 (prévue en août 2020).
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# usurpation d’email et réponse POP

Nous apportons deux modifications à la façon dont Adobe Workfront envoie et reçoit des emails avec la version 20.3 (prévue en août 2020).

## Courrier électronique sortant de Workfront

Afin d&#39;améliorer la diffusion des emails, nous allons éliminer l&#39;usurpation des emails, souvent balisés comme spam (voir la section usurpation d&#39;email). Tous les courriers électroniques de Workfront seront envoyés depuis notifications@my.workfront.com, y compris les alertes automatisées et la communication utilisateur-utilisateur. Voici un exemple de courrier électronique de Joan Harris dans la zone de votre courrier électronique :

![](assets/noreply.png)

*Nous vous recommandons vivement de contacter votre équipe informatique.* pour vous assurer que les courriers électroniques de notifications@my.workfront.com ne seront pas bloqués pour les courriers électroniques entrants sur votre système. Vous pouvez également référencer [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) pour plus d’informations sur les adresses IP de notre trafic et de nos courriers électroniques.

## Réponses électroniques entrantes aux notifications (réponse POP)

Certaines notifications électroniques permettent aux utilisateurs de répondre par email et de faire copier la réponse dans Workfront en tant que réponse de commentaire dans le système Workfront. Les administrateurs système de Workfront ont toujours pu choisir entre fournir leur propre serveur de messagerie POP pour recevoir ces réponses ou utiliser le système de réponse Workfront intégré. Le choix du serveur de messagerie POP personnalisé est supprimé avec la version 20.3. Tous les comptes configurés pour utiliser un serveur personnalisé seront automatiquement transférés afin d’utiliser le système de réponse aux courriers électroniques natif de Workfront. Aucune action n’est requise pour les administrateurs système ou les autres utilisateurs de Workfront.

Les emails provenant directement du système de BAT Workfront ne seront pas modifiés. Vous continuerez à recevoir ces emails comme vous l’avez fait par le passé.

Si vous avez d’autres questions ou préoccupations, veuillez contacter la [Équipe d’assistance Workfront](https://one.workfront.com/s/support?language=en_US).
