---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Synchronisation des utilisateurs entre Adobe Workfront et Workfront Proof
description: Les informations sur les utilisateurs et utilisatrices sont synchronisées d’Adobe Workfront sur Workfront Proof ; elles ne sont pas synchronisées de Workfront Proof sur Workfront. Pour cette raison, chaque fois que vous créez ou modifiez des utilisateurs et utilisatrices, vous devez apporter ces modifications dans Workfront. Vous ne pouvez pas modifier les utilisateurs et utilisatrices dans Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 97%

---

# Synchronisation des utilisateurs et utilisatrices entre Adobe Workfront et Workfront Proof

Les informations sur les utilisateurs et utilisatrices sont synchronisées d’Adobe Workfront sur Workfront Proof ; elles ne sont pas synchronisées de Workfront Proof sur Workfront. Pour cette raison, chaque fois que vous créez ou modifiez des utilisateurs et utilisatrices, vous devez apporter ces modifications dans Workfront. Vous ne pouvez pas modifier les utilisateurs et utilisatrices dans Workfront Proof.

Les sections suivantes fournissent des informations sur la synchronisation des utilisateurs et utilisatrices de Workfront sur Workfront Proof :

## Informations synchronisées

Workfront synchronise les informations suivantes sur les utilisateurs et utilisatrices sur Workfront Proof :

* Nom (prénom et nom de l’utilisateur ou de l’utilisatrice)
* Adresse e-mail

## Moment de la synchronisation

Les informations sur l’utilisateur ou l’utilisatrice sont synchronisées de Workfront sur Workfront Proof dans les situations suivantes :

* Les informations d’un utilisateur ou d’une utilisatrice sont mises à jour dans Workfront.
* Une personne est créée dans Workfront.

Selon qu’une personne avec la même adresse e-mail existe ou non dans Workfront Proof, l’un ou l’autre des cas suivants se produit :

* **Si aucune personne avec une adresse e-mail correspondante n’existe dans Workfront Proof et que**

   * **la relecture est activée pour la personne :** la personne est créée en tant qu’utilisateur ou utilisatrice dans Workfront Proof.
   * **la relecture n’est pas activée pour la personne :** la personne est créée en tant que contact dans Workfront Proof.

* **Si une personne avec une adresse e-mail correspondante existe dans Workfront Proof :** la relecture est activée pour cette personne dans Workfront (si elle ne l’était pas déjà) et les informations sont synchronisées entre les deux personnes.

  Pour plus d’informations, voir [Configurer l’accès d’un utilisateur ou d’une utilisatrice à la relecture](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) dans [Configurer l’accès d’un utilisateur ou d’une utilisatrice à la relecture](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >Lorsqu’une personne avec une adresse e-mail correspondante existe, que ce soit dans son propre environnement ou dans un autre environnement de relecture, Workfront crée un alias d’adresse e-mail en ajoutant l’identifiant du compte de la personne en tant que suffixe à son adresse e-mail. Par exemple, *nomutilisateur+identifiantcompte@domaine.com*. Les utilisateurs et utilisatrices continueront à recevoir des notifications d’épreuve si un alias d’e-mail est créé.
