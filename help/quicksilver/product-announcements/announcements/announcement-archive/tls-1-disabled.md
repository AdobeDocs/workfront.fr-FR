---
content-type: reference
navigation-topic: announcements
title: TLS 1.2 requis dans Adobe Workfront
description: Pour garantir une sécurité optimale, Adobe Workfront exige que toutes les connexions de navigateur et les intégrations d’API qui reposent sur TLS 1.0 ou version antérieure soient mises à niveau pour utiliser TLS 1.2. Dans l’environnement de prévisualisation, TLS 1.0 est déjà désactivé.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# TLS 1.2 requis dans Adobe Workfront

Pour garantir une sécurité optimale, Adobe Workfront exige que toutes les connexions de navigateur et les intégrations d’API qui reposent sur TLS 1.0 ou version antérieure soient mises à niveau pour utiliser TLS 1.2. Dans l’environnement Aperçu, TLS 1.0 est déjà désactivé.

Workfront a officiellement arrêté la prise en charge de TLS 1.0 en mars 2018. Toutes les intégrations exploitant TLS 1.0 ont cessé de fonctionner à compter du 9 janvier 2019.  TLS 1.1 sera désactivé au 4e trimestre 2019.

Les sections suivantes fournissent des informations plus détaillées sur ces jalons importants, ainsi que sur la manière dont vous pouvez vous préparer à cette mise à niveau dans votre entreprise :

## Workfront met fin à la prise en charge officielle de TLS 1.0 (5 mars 2018)

Workfront a mis fin à la prise en charge officielle du protocole TLS 1.0 en mars 2018.

Les connexions des navigateurs et les intégrations d’API qui tirent parti de TLS 1.0 sont toujours opérationnelles, mais Workfront ne résoudra pas les problèmes de l’application Workfront liés à TLS 1.0.

## Intégrations Workfront utilisant TLS 1.0 désactivées (9 janvier 2019)

Le 9 janvier 2019, toutes les connexions de navigateur Workfront et les intégrations d’API qui utilisent TLS 1.0 doivent être mises à niveau pour utiliser TLS 1.1 ou version ultérieure. Les connexions navigateur et les intégrations d’API qui continuent à utiliser TLS 1.0 (connexions entrantes ou sortantes) ne pourront plus communiquer avec l’application Workfront au bout de ce temps. 

## TLS 1.1 à désactiver au quatrième trimestre 2019

Dans l’environnement de production, TLS 1.1 a été désactivé le 21 octobre 2019. Après cette période, toutes les intégrations utilisant TLS 1.1 ne fonctionneront plus.

Cette modification entrera en vigueur dans les environnements Preview et Sandbox le 7 août pour aider les organisations à se préparer à l’arrêt.

## Préparation à la mise à niveau TLS

* [Lors de l’accès à Workfront via le navigateur](#when-accessing-workfront-via-the-browser)
* [Lors de la connexion à Workfront via l’API](#when-connecting-to-workfront-via-the-api)

### Lors de l’accès à Workfront via le navigateur {#when-accessing-workfront-via-the-browser}

Assurez-vous que les utilisateurs de votre entreprise accèdent à Workfront par le biais d’un navigateur pris en charge. (Pour plus d’informations sur les navigateurs pris en charge, voir [Configuration requise pour le navigateur Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).)

Tous les navigateurs pris en charge par Workfront sont compatibles avec TLS 1.2.

### Lors de la connexion à Workfront via l’API {#when-connecting-to-workfront-via-the-api}

Si vous intégrez des applications tierces à Workfront via l’API (entrante ou sortante), assurez-vous que TLS 1.2 (et les protocoles de chiffrement TLS 1.2) sont activés dans vos intégrations.
