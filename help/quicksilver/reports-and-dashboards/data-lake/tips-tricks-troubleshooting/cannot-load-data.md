---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop ne peut pas établir de connexion
description: Lorsque vous essayez de connecter Tableau Desktop à Data Connect, vous obtenez une erreur.
author: Courtney
feature: Reports and Dashboards
exl-id: 2a25d99a-a05e-4f60-ae1a-51ee137ad5f3
TQID: https://experienceleague.adobe.com/-V1TT-X0FjMm2PIKDy0JVFkvt-A-a7f8fRbVzGzy1jg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 253
ht-degree: 5%

---

# Tableau Desktop ne peut pas établir de connexion

## Problème

Lorsque vous essayez de connecter Tableau Desktop à Data Connect, le message d&#39;erreur suivant s&#39;affiche :

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## Cause

Cette erreur est due à un paramètre de proxy sur votre ordinateur local qui empêche le chargement des données à partir de Data Connect.

Data Connect est fourni par le biais de services cloud Snowflake tiers. Tableau nécessite l&#39;ouverture de la mise en réseau pour communiquer avec Snowflake.

## Solution

Vous pouvez essayer les méthodes suivantes pour résoudre ce problème :

* **Dépannage en désactivant votre outil de sécurité** : désactivez votre outil de sécurité, comme Zscaler ou Cisco, pour voir s’il résout le problème de connectivité. Si cela résout le problème de connexion, assurez-vous que votre outil de sécurité est mis à niveau vers la dernière version, ajoutez l’adresse IP Data Connect (Snowflake) à la liste autorisée VPN avec votre équipe réseau interne.

* **Ajouter des adresses IP à la Liste autorisée** : assurez-vous que les paramètres de votre pare-feu autorisent les adresses IP utilisées par Data Connect. Utilisez la `SYSTEM$ALLOWLIST()` de commande pour obtenir l’adresse IP, que vous pouvez ensuite dans le VPN.

* **Vérification des paramètres de pare-feu et de proxy** : vérifiez si des configurations de pare-feu ou de proxy sur votre réseau bloquent l’accès aux points d’entrée de Snowflake. Vous devrez peut-être contacter votre administrateur réseau pour ajouter les adresses IP et les ports Snowflake requis à la place sur la liste autorisée de données de votre société.

* **Option de solution** : créez un extrait à partir d&#39;un écran de feuille de calcul au lieu du volet Source de données dans Tableau. La connexion n’est pas perdue et le processus d’extraction se termine.
