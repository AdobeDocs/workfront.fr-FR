---
content-type: reference
navigation-topic: announcements
title: Supprimer le SMTP personnalisé en tant qu’option d’email sortant
description: Avec la version 20.3 (prévue pour août 2020), Adobe Workfront passe à un nouveau système de messagerie qui améliorera considérablement la fiabilité de votre diffusion de courrier électronique pour les mises à jour et notifications Workfront. De ce fait, les clients ne pourront plus utiliser leur propre serveur de messagerie SMTP pour relayer leurs emails de la plateforme Workfront vers le destinataire prévu. Tous les courriers électroniques seront envoyés directement à partir du serveur de messagerie Workfront.
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
source-git-commit: 9bc394c718becbac2848c2d91ba3202483699b6f
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Supprimer le SMTP personnalisé en tant qu’option d’email sortant

Avec la version 20.3 (prévue pour août 2020), Adobe Workfront passe à un nouveau système de messagerie qui améliorera considérablement la fiabilité de votre diffusion de courrier électronique pour les mises à jour et notifications Workfront. De ce fait, les clients ne pourront plus utiliser leur propre serveur de messagerie SMTP pour relayer leurs emails de la plateforme Workfront vers le destinataire prévu. Tous les courriers électroniques seront envoyés directement à partir du serveur de messagerie Workfront.

Pour accéder à cette fonction, connectez-vous en tant qu’administrateur système et accédez à Configuration > Email > Configuration. Voici une capture d’écran mettant en évidence cette fonctionnalité :

![](assets/email-server-settings-350x226.png)

Le paramètre mis en évidence dans cette capture d’écran est automatiquement migré pour utiliser l’option Serveur de messagerie Workfront avec la version 20.3.

Si vous avez configuré un serveur de messagerie SMTP personnalisé, **Nous vous recommandons vivement de contacter votre équipe informatique.** pour vous assurer que les courriers électroniques de notifications@my.workfront.com ne seront pas bloqués pour les courriers électroniques entrants sur votre système. Vous pouvez également vous reporter à Configuration de votre pare-feu pour plus d’informations sur les adresses IP d’où viennent notre trafic et nos courriers électroniques.

Si vous avez d’autres questions ou des questions, veuillez contacter [Équipe d’assistance Workfront](https://one.workfront.com/s/support?language=en_US).
