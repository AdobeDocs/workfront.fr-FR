---
title: Vue d’ensemble
description: Vue d’ensemble
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 1%

---

# Vue d’ensemble

**Bienvenue dans l’API Workfront Proof**

L’API Workfront Proof est un service HTTP simple sécurisé à l’aide de SSL. L’API vise à vous fournir toutes les fonctionnalités utilisées dans notre propre application.

## Formats pris en charge

L’interface publique est SOAP 1.1 conforme à la prise en charge WSDL. Toutes les requêtes sont donc exécutées à l’aide de XML sur HTTPS.

## Contrôle de version des API

Afin de préserver la compatibilité avec les intégrations client existantes, nous avons introduit le contrôle de version des API à partir de notre version 12.1. Veuillez consulter la  [Mises à jour de l’API](https://api.proofhq.com/new-updates.html) pour plus d’informations. Si une méthode ou un paramètre ne contient aucune information de version, cela signifie que vous trouverez cela dans notre API standard, reportez-vous à la section &quot;Prise en main de l’API&quot; ci-dessous.

## Prise en main de l’API

Point d’entrée de l’API :

`https://soap.proofhq.com/soap` (notez l’utilisation de HTTPS)

Le fichier WSDL se trouve ici :

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Ce fichier WSDL contient toutes les modifications jusqu’à la version 12.1, après laquelle nous avons introduit le contrôle de version des API. Pour plus d’informations sur les différentes versions WSDL et les modifications à venir, consultez la page Mises à jour de l’API**

Chaque requête d’API nécessite une clé de session. Cette clé de session identifie l’utilisateur Workfront Proof effectuant la ou les actions. Elle est obtenue en appelant la méthode doLogin() et en transmettant l’adresse électronique et le mot de passe de l’utilisateur. La méthode doLogin() ne doit être appelée qu’une seule fois avant une séquence de requêtes API. La clé de session reste active pendant une courte période et est renouvelée à chaque appel de méthode. *Nous ajouterons très bientôt la prise en charge de l’authentification basée sur les jetons.*

Toutes les requêtes utilisent le format d’enveloppe, d’en-tête et de corps suivant :

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

