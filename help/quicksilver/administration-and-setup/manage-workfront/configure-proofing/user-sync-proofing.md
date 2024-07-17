---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Synchronisation des utilisateurs entre Adobe Workfront et Workfront Proof
description: Les informations utilisateur sont synchronisées d’Adobe Workfront vers Workfront Proof ; elles ne sont pas synchronisées de Workfront Proof vers Workfront. C’est pourquoi, chaque fois que vous créez ou modifiez des utilisateurs, vous devez apporter ces modifications dans Workfront. Vous ne pouvez pas apporter de modifications aux utilisateurs dans Workfront Proof.
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

Les informations utilisateur sont synchronisées d’Adobe Workfront vers Workfront Proof ; elles ne sont pas synchronisées de Workfront Proof vers Workfront. C’est pourquoi, chaque fois que vous créez ou modifiez des utilisateurs, vous devez apporter ces modifications dans Workfront. Vous ne pouvez pas apporter de modifications aux utilisateurs dans Workfront Proof.

Les sections suivantes fournissent des informations sur la synchronisation des utilisateurs de Workfront vers Workfront Proof :

## Informations synchronisées

Workfront synchronise les informations utilisateur suivantes avec Workfront Proof :

* Nom (prénom et nom de l’utilisateur)
* Adresse e-mail

## Lorsque la synchronisation survient

Les informations utilisateur sont synchronisées de Workfront vers Workfront Proof dans les cas suivants :

* Les informations d’un utilisateur sont mises à jour dans Workfront
* Un utilisateur est créé dans Workfront

Selon qu’un utilisateur disposant de la même adresse électronique existe dans Workfront Proof, l’une des situations suivantes se produit :

* **Si aucun utilisateur avec un email correspondant n’existe dans Workfront Proof et**

   * **La vérification est activée pour l’utilisateur :** l’utilisateur est créé en tant qu’utilisateur dans Workfront Proof.
   * **La vérification n’est pas activée pour l’utilisateur :** l’utilisateur est créé en tant que contact dans Workfront Proof.

* **Si un utilisateur avec un courrier électronique correspondant existe dans Workfront Proof :** La vérification est activée pour cet utilisateur dans Workfront (s’il n’a pas déjà été activé) et les informations sont synchronisées entre les deux utilisateurs.

  Pour plus d’informations, voir [Configuration de l’accès de vérification de l’utilisateur](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) dans [ Configuration de l’accès de vérification de l’utilisateur](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >Lorsqu’un utilisateur possède un email correspondant, dans son propre environnement ou dans un autre environnement de vérification, Workfront crée une adresse email d’alias en ajoutant l’ID de compte de l’utilisateur comme suffixe à son email. Par exemple, *username+accountid@domain.com*. Les utilisateurs recevront toujours des notifications de BAT en cas de création d’un email d’alias.
