---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Synchronisation des utilisateurs entre Adobe Workfront et Workfront Proof
description: Les informations utilisateur sont synchronisées d’Adobe Workfront vers Workfront BAT ; il n’est pas synchronisé de Workfront BAT vers Workfront. C’est pourquoi, chaque fois que vous créez ou modifiez des utilisateurs, vous devez apporter ces modifications dans Workfront. Vous ne pouvez pas apporter de modifications aux utilisateurs dans Workfront BAT.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Synchronisation des utilisateurs entre Adobe Workfront et Workfront Proof

Les informations utilisateur sont synchronisées d’Adobe Workfront vers Workfront BAT ; il n’est pas synchronisé de Workfront BAT vers Workfront. C’est pourquoi, chaque fois que vous créez ou modifiez des utilisateurs, vous devez apporter ces modifications dans Workfront. Vous ne pouvez pas apporter de modifications aux utilisateurs dans Workfront BAT.

Les sections suivantes fournissent des informations sur la synchronisation des utilisateurs de Workfront vers Workfront BAT :

## Informations synchronisées

Workfront synchronise les informations utilisateur suivantes avec Workfront BAT :

* Nom (prénom et nom de l’utilisateur)
* Adresse e-mail

## Lorsque la synchronisation survient

Les informations utilisateur sont synchronisées de Workfront vers Workfront Proof dans les cas suivants :

* Les informations d’un utilisateur sont mises à jour dans Workfront
* Un utilisateur est créé dans Workfront

Selon qu’il existe un utilisateur disposant de la même adresse électronique dans le bon à tirer Workfront, l’une des actions suivantes se produit :

* **S’il n’existe aucun utilisateur avec un email correspondant dans Workfront Proof et**

   * **La vérification est activée pour l’utilisateur :** L’utilisateur est créé en tant qu’utilisateur dans le bon à tirer Workfront.
   * **La vérification n’est pas activée pour l’utilisateur :** L’utilisateur est créé en tant que contact dans le bon à tirer Workfront.

* **Si un utilisateur avec un email correspondant existe dans le bon à tirer Workfront :** La vérification est activée pour cet utilisateur dans Workfront (si elle n’était pas déjà activée) et les informations sont synchronisées entre les deux utilisateurs.

   Pour plus d’informations, voir [Configuration de l’accès de vérification de l’utilisateur](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [Configuration de l’accès de vérification de l’utilisateur](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

   >[!IMPORTANT]
   >
   >Lorsqu’un utilisateur possède un email correspondant, dans son propre environnement ou dans un autre environnement de vérification, Workfront crée une adresse email d’alias en ajoutant l’ID de compte de l’utilisateur comme suffixe à son email. Par exemple : *username+accountid@domain.com*. Les utilisateurs recevront toujours des notifications de BAT en cas de création d’un email d’alias.
