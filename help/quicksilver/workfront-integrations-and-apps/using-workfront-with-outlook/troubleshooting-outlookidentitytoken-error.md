---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Dépannage : erreur outlookIdentityToken lors de l’utilisation de Workfront pour Outlook'
description: Si vous obtenez une erreur outlookIdentityToken lors de l’utilisation de Workfront pour Outlook, vous devez activer les jetons hérités Microsoft 365 pour votre organisation.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 31%

---

# Dépannage : erreur outlookIdentityToken lors de l’utilisation de Workfront pour Outlook

>[!IMPORTANT]
>
>[Microsoft est en train de désactiver la prise en charge des jetons Exchange Online hérités](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) actuellement utilisés par le complément Workfront Outlook pour l&#39;authentification. Cette modification apportée par Microsoft a déjà commencé à affecter les clients et continuera à être déployée par phases jusqu’en octobre 2025.
>
>* **Une fois que Microsoft a complètement désactivé ces jetons, l’intégration de Workfront pour Microsoft Outlook ne fonctionne plus.**
>
>Dans le cadre de cette modification, Microsoft a pris la décision de modifier la manière dont les jetons sont réactivés. Après le **30 juin 2025**, les administrateurs ne pourront plus réactiver les jetons eux-mêmes. Seule la prise en charge de Microsoft peut accorder des exceptions. **Le 1er octobre 2025, les jetons hérités seront désactivés pour tous les clients. Les exceptions ne seront pas accordées.**


Lors de l’utilisation de Workfront pour Outlook, l’erreur suivante peut s’afficher :

```
Unexpected error
Unable to get the outlookIdentityToken
```

Pour résoudre cette erreur, vous devez activer les jetons Microsoft 365 hérités pour votre organisation. Cela devant être effectué dans Microsoft 365, Workfront ne peut pas activer ces jetons pour votre organisation.

Pour obtenir des instructions sur l’activation des jetons Microsoft 365 hérités, voir la section [Activer ou désactiver des jetons Exchange Online hérités](https://learn.microsoft.com/fr-fr/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) dans la documentation Microsoft.

Pour plus d&#39;informations sur les jetons hérités, voir la section [Puis-je réactiver les jetons hérités Exchange Online ?](https://learn.microsoft.com/fr-fr/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) dans la documentation Microsoft.
