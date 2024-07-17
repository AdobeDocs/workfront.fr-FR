---
content-type: reference
navigation-topic: announcements
title: Suppression du serveur SMTP personnalisé en tant qu’option d’e-mail sortant
description: Avec la version 20.3 (prévue pour août 2020), Adobe Workfront passe à un nouveau système de messagerie qui améliorera considérablement la fiabilité de votre diffusion de courrier électronique pour les mises à jour et notifications Workfront. De ce fait, les clients ne pourront plus utiliser leur propre serveur de messagerie SMTP pour relayer leurs emails de la plateforme Workfront vers le destinataire prévu. Tous les courriers électroniques seront envoyés directement à partir du serveur de messagerie Workfront.
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
source-git-commit: 9bc394c718becbac2848c2d91ba3202483699b6f
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 5%

---

# Suppression du serveur SMTP personnalisé en tant qu’option d’e-mail sortant

Avec la version 20.3 (prévue pour août 2020), Adobe Workfront passe à un nouveau système de messagerie qui améliorera considérablement la fiabilité de votre diffusion de courrier électronique pour les mises à jour et notifications Workfront. De ce fait, les clients ne pourront plus utiliser leur propre serveur de messagerie SMTP pour relayer leurs emails de la plateforme Workfront vers le destinataire prévu. Tous les courriers électroniques seront envoyés directement à partir du serveur de messagerie Workfront.

Pour accéder à cette fonction, connectez-vous en tant qu’administrateur système et accédez à Configuration > Email > Configuration. Voici une capture d’écran mettant en évidence cette fonctionnalité :

![](assets/email-server-settings-350x226.png)

Le paramètre mis en évidence dans cette capture d’écran est automatiquement migré pour utiliser l’option Serveur de messagerie Workfront avec la version 20.3.

Si vous avez configuré un serveur de messagerie SMTP personnalisé, **nous vous recommandons vivement de contacter votre équipe informatique** pour vous assurer que les emails de notifications@my.workfront.com ne seront pas bloqués pour les emails entrants sur votre système. Vous pouvez également vous reporter à Configuration de votre pare-feu pour plus d’informations sur les adresses IP d’où viennent notre trafic et nos courriers électroniques.

Si vous avez d’autres questions ou préoccupations, contactez l’ [équipe d’assistance Workfront](https://one.workfront.com/s/support?language=en_US).
