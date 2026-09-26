---
product-area: documents
navigation-topic: documents-navigation-topic
title: Métadonnées C2PA dans Adobe Workfront
description: Découvrez ce que sont les métadonnées C2PA et comment Adobe Workfront les conserve sur les documents que vous téléchargez, stockez et téléchargez.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%
---
# Métadonnées C2PA dans Adobe Workfront

Les métadonnées C2PA sont des informations sécurisées et infalsifiables qui voyagent avec un élément de contenu. Lorsque l’IA générative (GenAI) est utilisée pour créer ou modifier une image, une vidéo ou un fichier audio, les métadonnées C2PA enregistrent ce fait afin que toute personne qui reçoit le fichier puisse voir comment il a été créé.

Les métadonnées C2PA sont basées sur la norme ouverte [C2PA](https://c2pa.org/).

## Ce que contiennent les métadonnées C2PA

Les métadonnées C2PA incluent :

* Nom du fournisseur qui a fourni l’outil GenAI.
* Nom et numéro de version du système GenAI utilisé pour créer ou modifier le contenu.
* Date et heure auxquelles le contenu a été créé ou modifié.
* Identifiant unique.

Les métadonnées C2PA n’incluent aucune information d’identification personnelle (PII).

## Gestion des métadonnées C2PA par Workfront

Adobe Workfront ne modifie pas les métadonnées des fichiers que vous utilisez. Lorsque vous téléchargez un fichier qui contient déjà des métadonnées C2PA, Workfront conserve ces informations inchangées, car le fichier est stocké dans et téléchargé à partir de Workfront.

Comme les métadonnées sont incorporées dans le fichier lui-même, elles restent intactes dans vos workflows Workfront, de sorte que les informations de provenance restent avec le contenu lorsqu’il quitte Workfront.
