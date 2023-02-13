---
content-type: reference
navigation-topic: announcements
title: Les clients des grappes 1, 2 et 3 doivent mettre à jour tous les blocs IP de liste autorisée pour empêcher le blocage des services Adobe Workfront.
description: Pour améliorer notre infrastructure de base, nous migrerons bientôt les clients Adobe Workfront sur les grappes 01, 02 et 03 vers le cloud public AWS.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 4%

---

# Les clients des grappes 1, 2 et 3 doivent mettre à jour tous les blocs IP de liste autorisée pour empêcher le blocage des services Adobe Workfront.

Pour améliorer notre infrastructure de base, nous migrerons bientôt les clients Adobe Workfront sur les grappes 01, 02 et 03 vers le cloud public AWS.

Dans le cadre de cette modification, vous devez ajouter les adresses IP suivantes à vos blocs IP de liste autorisée afin d’empêcher le blocage des services Workfront :

Pour SSO et POP :

* 34.215.145.168
* 54.69.155.48
* 35.160.44.226
* 34.213.96.218
* 3.16.210.22
* 3.16.229.153
* 18.224.117.99
* 3.18.123.153
* 3.211.159.196
* 3.85.255.45
* 3.210.78.197
* 3.211.23.183

Pour l’e-mail :

* 54.240.60.174
* 54.240.60.175

Assurez-vous que vos blocs IP de liste autorisée sont mis à jour d’ici le 13 mai 2019. Pour plus d’informations, voir [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Merci pour votre soutien constant à Workfront alors que nous travaillons à créer une expérience plus fiable et robuste pour nos clients.

Pour toute question, contactez notre équipe d’assistance en consultant experience.workfront.com ou en appelant le 844.306.4357 (Etats-Unis) ou le +44.1256.274200 (EMEA).

## FAQ

### Pourquoi Workfront apporte-t-il cette modification ?

Afin de fournir constamment à nos clients le meilleur service possible, Workfront cherche constamment des moyens d’améliorer l’expérience utilisateur. Ce changement fait appel à de nouvelles technologies qui nous permettent de fournir la meilleure expérience possible et d’améliorer notre modèle de sécurité déjà robuste.

### Quelles actions dois-je entreprendre en tant qu’administrateur Workfront ?

Contactez votre service informatique ou de sécurité interne pour obtenir de l’aide afin de passer en revue vos blocs IP de liste autorisée et d’ajouter les adresses IP répertoriées ci-dessus.

### À quoi peut s’attendre mon organisation si nous ne faisons pas ce changement ?

Vous ne pourrez pas accéder aux services Workfront lorsque nous migrons les services vers les nouvelles adresses IP.
