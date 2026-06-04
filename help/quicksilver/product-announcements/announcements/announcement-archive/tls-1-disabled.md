---
content-type: reference
navigation-topic: announcements
title: TLS 1.2 requis dans Adobe Workfront
description: Pour assurer une sécurité maximale, Adobe Workfront exige que toutes les connexions de navigateur et les intégrations d’API utilisant TLS 1.0 ou une version antérieure soient mises à niveau pour utiliser TLS 1.2. Dans l’environnement de prévisualisation, TLS 1.0 est déjà désactivé.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
TQID: https://experienceleague.adobe.com/23UVEvZitUFvhkTkgOnubLK76Lzl8QKiyz-R4svWcc8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 380
ht-degree: 93%

---

# TLS 1.2 requis dans Adobe Workfront

Pour assurer une sécurité maximale, Adobe Workfront exige que toutes les connexions de navigateur et les intégrations d’API utilisant TLS 1.0 ou une version antérieure soient mises à niveau pour utiliser TLS 1.2. Dans l’environnement de prévisualisation, TLS 1.0 est déjà désactivé.

Workfront a officiellement arrêté la prise en charge de TLS 1.0 en mars 2018. Toutes les intégrations exploitant TLS 1.0 ont cessé de fonctionner à compter du 9 janvier 2019.  TLS 1.1 sera désactivé au 4e trimestre 2019.

Les sections suivantes donnent plus de détails sur ces étapes importantes et expliquent comment vous pouvez vous préparer à cette mise à niveau dans votre entreprise :

## Workfront met fin à la prise en charge officielle de TLS 1.0 (5 mars 2018).

Workfront a mis fin à la prise en charge officielle de TLS 1.0 en mars 2018.

Les connexions des navigateurs et les intégrations d’API qui utilisent TLS 1.0 sont toujours opérationnelles, mais Workfront ne résoudra pas les problèmes de l’application Workfront liés à TLS 1.0.

## Intégrations Workfront utilisant TLS 1.0 désactivées (9 janvier 2019)

Le 9 janvier 2019, toutes les connexions de navigateur et intégrations d’API Workfront qui exploitent TLS 1.0 devront être mises à niveau pour utiliser TLS 1.1 ou une version ultérieure. Les connexions de navigateur et les intégrations d’API qui continuent à utiliser TLS 1.0 (connexions entrantes ou sortantes) ne pourront plus communiquer avec l’application Workfront après ce délai. 

## TLS 1.1 sera désactivé au quatrième trimestre 2019

Dans l’environnement de production, TLS 1.1 a été désactivé le 21 octobre 2019. Après cette période, toutes les intégrations utilisant TLS 1.1 cesseront de fonctionner.

Cette modification sera active dans les environnements de prévisualisation et de sandbox le 7 août pour aider les organisations à se préparer à cet arrêt.

## Se préparer à la mise à niveau de TLS

* [Lors de l’accès à Workfront via le navigateur](#when-accessing-workfront-via-the-browser)
* [Lors de la connexion à Workfront via l’API](#when-connecting-to-workfront-via-the-api)

### Lors de l’accès à Workfront via le navigateur {#when-accessing-workfront-via-the-browser}

Assurez-vous que les utilisateurs et utilisatrices de votre entreprise accèdent à Workfront via un navigateur pris en charge. (Pour plus d’informations sur les navigateurs pris en charge, consultez la section [Configuration requise pour le navigateur Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).)

Tous les navigateurs pris en charge par Workfront sont compatibles avec TLS 1.2.

### Lors de la connexion à Workfront via l’API {#when-connecting-to-workfront-via-the-api}

Si vous intégrez des applications tierces à Workfront via l’API (entrante ou sortante), assurez-vous que TLS 1.2 (et les protocoles de chiffrement TLS 1.2) sont activés dans vos intégrations.
