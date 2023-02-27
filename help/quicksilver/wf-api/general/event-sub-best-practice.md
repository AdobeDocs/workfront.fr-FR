---
content-type: api
navigation-topic: general-api
title: Bonnes pratiques relatives à l’abonnement aux événements
description: Bonnes pratiques relatives à l’abonnement aux événements
author: Becky
feature: Workfront API
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Bonnes pratiques relatives à l’abonnement aux événements

Les messages d’abonnement à un événement Adobe Workfront sont automatiquement envoyés depuis Workfront une fois que vous avez correctement configuré votre service et créé un abonnement à un événement pour déclencher ces diffusions de messages. Pour en savoir plus sur la configuration correcte des abonnements à un événement, voir [Exigences de diffusion de l’abonnement à un événement](../../wf-api/general/setup-event-sub-endpoint.md).


Vous trouverez ci-dessous quelques bonnes pratiques pour vous aider à créer efficacement des abonnements à un événement.

## Fournir tous les champs requis du corps de la requête

Assurez-vous que tous les champs de corps de requête requis sont fournis à l’API. Pour plus d’informations sur tous les attributs de requête requis, voir [API d’abonnement à un événement](../../wf-api/general/event-subs-api.md).

## Éviter d’inclure des champs de corps supplémentaires

N’incluez pas de champs de corps supplémentaires dans la requête, car cela entraînera l’échec de l’API à créer un abonnement.

## Terminer le test dans la période de grâce

Essayez d’effectuer tous les tests d’abonnement pendant la période de grâce de 100 messages. Pour en savoir plus sur cette période de grâce, voir [Questions fréquentes - Abonnements à un événement](../../wf-api/general/event-subs-faq.md).

## Respectez les exigences de diffusion des messages d’abonnement à un événement standard.

Assurez-vous que votre point de terminaison d’abonnement est conforme aux exigences de diffusion des messages d’abonnement à un événement standard. Pour en savoir plus sur ces exigences, voir [Exigences de diffusion de l’abonnement à un événement](../../wf-api/general/setup-event-sub-endpoint.md).

## Liste autorisée des adresses IP par région globale

Pour recevoir les payloads d’abonnement aux événements par le biais de votre pare-feu, vous devez ajouter les adresses IP à la liste autorisée par région globale. Pour en savoir plus, voir [API d’abonnement à un événement](../../wf-api/general/event-subs-api.md).

## Posséder le niveau d’accès approprié et une clé API

Pour créer, interroger ou supprimer un abonnement à un événement, votre utilisateur Workfront a besoin des éléments suivants :

* Un niveau d’accès à **Administrateur système**
Pour en savoir plus, voir [Octroi d’un accès administratif complet à un utilisateur](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) ou [Octroi aux utilisateurs un accès administratif à certaines zones](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Une clé API

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
