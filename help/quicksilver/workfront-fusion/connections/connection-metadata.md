---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Métadonnées de connexion dans Adobe Workfront Fusion
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion en plus d’une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: af260c63-3385-4d5c-abc2-d5c23175be40
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 100%

---

# Métadonnées de connexion dans Adobe Workfront Fusion

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une licence [!DNL Adobe Workfront Fusion] en plus d’une licence [!DNL Adobe Workfront].

Toutes les connexions ne sont pas identiques. Il est très important de comprendre les différences entre les connexions pour connaître leur contexte métier. Fusion utilise des métadonnées pour identifier les attributs importants d’une connexion.

Les métadonnées de connexion peuvent être définies lors de la création d’une nouvelle connexion. Ces attributs se trouvent dans la même boîte de dialogue que celle utilisée pour établir une connexion :

![Métadonnées de connexion](assets/connection-metadata-setup.png)

Les utilisateurs et utilisatrices de Fusion peuvent afficher et modifier les connexions à partir de la zone Connexions.

![Métadonnées de connexion dans la zone Connexions](assets/connections-area-metadata.png)

## Type d’environnement

Les connexions Fusion peuvent être utilisées par les systèmes de production et non-production. Il est très important de connaître la différence pour protéger les environnements de production. Veuillez noter que le type d’environnement, tout comme les autres métadonnées de connexion, n’est utilisé qu’à titre informatif. Les utilisateurs et utilisatrices sont toujours responsables de l’exactitude du paramétrage de cet attribut.

## Type d&#39;authentification

Les connexions Fusion peuvent être utilisées à la fois pour les comptes de service et les comptes personnels. Les comptes de service sont utilisés pour l’authentification lorsqu’un scénario s’automatise comme Fusion. Les comptes personnels sont des authentifications basées sur une personne spécifique. Le type d’authentification dépend des exigences du scénario. Les comptes personnels doivent être utilisés pour les actions automatisées des utilisateurs et utilisatrices. Par exemple, si un scénario Fusion automatise l’approbation par une personne spécifique, le type d’authentification doit être celui de cette personne. Sinon, Fusion agit en tant que Fusion et le type devrait être « Compte de service ».

Veuillez noter que le type, tout comme les autres métadonnées de connexion, n’est utilisé qu’à titre informatif. Les utilisateurs et utilisatrices sont toujours responsables de l’exactitude du paramétrage manuel de cet attribut.

Pour plus d’informations sur les types d’authentification, voir [Authentification](https://developer.adobe.com/developer-console/docs/guides/authentication/) dans le guide de l’authentification Adobe.
