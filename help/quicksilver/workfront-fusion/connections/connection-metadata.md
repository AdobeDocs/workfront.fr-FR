---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Métadonnées de connexion dans Adobe Workfront Fusion
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion et une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: af260c63-3385-4d5c-abc2-d5c23175be40
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 6%

---

# Métadonnées de connexion dans Adobe Workfront Fusion

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une licence [!DNL Adobe Workfront Fusion] en plus d’une licence [!DNL Adobe Workfront].

Toutes les connexions ne sont pas les mêmes. Comprendre les différences entre les connexions est très important pour connaître leur contexte d’entreprise. Fusion utilise des métadonnées pour identifier les attributs importants d’une connexion.

Les métadonnées de connexion peuvent être définies lors de la création d’une connexion. Ces attributs se trouvent dans la boîte de dialogue utilisée pour configurer une connexion :

![Métadonnées de connexion](assets/connection-metadata-setup.png)

Les utilisateurs de fusion peuvent afficher et modifier les connexions à partir de la zone Connexions .

![Métadonnées de connexion dans la zone Connexions](assets/connections-area-metadata.png)

## Type d’environnement

Les connexions de fusion peuvent être utilisées à la fois par les systèmes de production et les systèmes hors production. Connaître la différence est très important pour la protection des environnements de production. Veuillez noter que le type d’environnement, comme les autres métadonnées de connexion, est utilisé à titre d’information uniquement. Les utilisateurs sont toujours responsables de la définition précise de cet attribut.

## Type d&#39;authentification

Les connexions de fusion peuvent être utilisées à la fois pour les comptes de service et les comptes personnels. Les comptes de service sont utilisés pour l’authentification lorsqu’un scénario s’automatise en tant que Fusion. Les comptes personnels sont une authentification basée sur une personne spécifique. Le type d’authentification utilisé dépend des exigences du scénario. Les comptes personnels doivent être utilisés pour les actions utilisateur automatisées. Par exemple, si un scénario de fusion automatise l’approbation par une personne spécifique, le type d’authentification doit être pour cette personne. Sinon, Fusion agit comme Fusion et le type doit être &quot;Compte de service&quot;.

Veuillez noter que le type, comme les autres métadonnées de connexion, est utilisé à titre d’information uniquement. Les utilisateurs sont toujours responsables de la définition manuelle de cet attribut.

Pour plus d’informations sur les types d’authentification, consultez [Authentification](https://developer.adobe.com/developer-console/docs/guides/authentication/) dans le guide d’authentification de l’Adobe.
