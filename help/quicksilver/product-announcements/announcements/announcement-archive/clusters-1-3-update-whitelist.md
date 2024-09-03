---
content-type: reference
navigation-topic: announcements
title: Les clientes et clients des clusters 1, 2 et 3 doivent mettre à jour tous les blocs d’adresses IP de liste autorisée pour empêcher le blocage des services Adobe Workfront.
description: Pour améliorer notre infrastructure de base, nous migrerons bientôt les clients Adobe Workfront sur les clusters 1, 2 et 3 vers le cloud public AWS.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 100%

---

# Les clientes et clients des clusters 1, 2 et 3 doivent mettre à jour tous les blocs d’adresses IP de liste autorisée pour empêcher le blocage des services Adobe Workfront.

Pour améliorer notre infrastructure de base, nous migrerons bientôt les clients Adobe Workfront sur les clusters 1, 2 et 3 vers le cloud public AWS.

Dans le cadre de cette migration, vous devez ajouter les adresses IP suivantes à vos blocs d’adresses IP de liste autorisée afin d’empêcher le blocage des services Workfront :

Pour les comptes SSO et POP :

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

Pour les e-mails :

* 54.240.60.174
* 54.240.60.175

Assurez-vous de mettre à jour vos blocs d’adresses IP de liste autorisée d’ici le 13 mai 2019. Pour plus d’informations, voir [Configurer la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Nous vous remercions de votre soutien constant à Workfront. Nous travaillons sans relâche à créer une expérience plus fiable et robuste pour nos clientes et clients.

Si vous avez d’autres questions, contactez notre équipe d’assistance par le biais du site web experience.workfront.com ou en appelant le 844.306.4357 (États-Unis) ou le +44.1256.274200 (EMEA).

## Questions fréquentes

### Pourquoi Workfront procède-t-il à ce changement ?

Afin de fournir à nos clientes et clients le meilleur service possible à chaque instant, Workfront cherche constamment des moyens d’améliorer l’expérience client. Cette migration permet de tirer parti des nouvelles technologies afin de fournir la meilleure expérience possible et d’améliorer notre modèle de sécurité déjà robuste.

### Quelles actions dois-je entreprendre en tant qu’administrateur ou administratrice Workfront ?

Contactez votre service informatique ou de sécurité interne pour obtenir de l’aide afin de passer en revue vos blocs d’adresses IP de liste autorisée et d’ajouter les adresses IP répertoriées ci-dessus.

### Que se passera-t-il pour mon organisation si nous ne procédons pas au changement ?

Vous ne pourrez pas accéder aux services Workfront, car nous migrons les services vers les nouvelles adresses IP.
