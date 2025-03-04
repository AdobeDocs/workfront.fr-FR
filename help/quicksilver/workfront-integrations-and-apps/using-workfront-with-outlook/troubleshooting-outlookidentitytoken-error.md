---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Dépannage : erreur outlookIdentityToken lors de l’utilisation de Workfront pour Outlook'
description: Si vous obtenez une erreur outlookIdentityToken lors de l’utilisation de Workfront pour Outlook, vous devez activer les jetons hérités Microsoft 365 pour votre organisation.
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 77cc1acde87b2ada96117daa06e98ba38e64fa8a
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Dépannage : erreur outlookIdentityToken lors de l’utilisation de Workfront pour Outlook

Lors de l’utilisation de Workfront pour Outlook, l’erreur suivante peut s’afficher :

```
Unexpected error
Unable to get the outlookIdentityToken
```

Pour résoudre cette erreur, vous devez activer les jetons Microsoft 365 hérités pour votre organisation. Comme cela doit être effectué dans Microsoft 365, Workfront ne peut pas activer ces jetons pour votre organisation.

Pour obtenir des instructions sur l’activation des jetons hérités de Microsoft 365, voir [Activation ou désactivation des jetons Exchange Online hérités](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) dans la documentation de Microsoft.

Pour plus d&#39;informations sur les jetons de logique, voir [Puis-je réactiver les jetons hérités d&#39;Exchange Online ?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) dans la documentation de Microsoft.
