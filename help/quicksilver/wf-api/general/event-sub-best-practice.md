---
content-type: api
navigation-topic: general-api
title: Bonnes pratiques en matière d’abonnement aux événements
description: Bonnes pratiques en matière d’abonnement aux événements
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 100%

---


# Bonnes pratiques en matière d’abonnement aux événements

Les messages d’abonnement à un événement Adobe Workfront sont automatiquement envoyés depuis Workfront une fois que vous avez correctement configuré votre service et créé un abonnement à un événement pour déclencher ces diffusions de messages. Pour en savoir plus sur la bonne configuration des abonnements à un événement, consultez [Exigences en matière de diffusion d’abonnements aux événements](../../wf-api/general/setup-event-sub-endpoint.md).


Vous trouverez ci-dessous quelques bonnes pratiques pour vous aider à créer efficacement des abonnements à un événement.

## Fournir tous les champs obligatoire du corps de la requête

Assurez-vous que tous les champs du corps de requête obligatoires sont fournis à l’API. Pour plus d’informations sur tous les attributs de requête obligatoires, consultez [API d’abonnement aux événements](../../wf-api/general/event-subs-api.md).

## Éviter d’inclure des champs de corps supplémentaires

N’incluez pas de champs de corps supplémentaires dans la requête, car cela entraînera l’échec de l’API lors de la création de l’abonnement.

## Terminer le test dans le délai de grâce

Essayez d’effectuer tous les tests d’abonnement pendant le délai de grâce de 100 messages. Pour en savoir plus sur ce délai de grâce, consultez [Questions fréquentes - Abonnements aux événements](../../wf-api/general/event-subs-faq.md).

## Respecter les exigences de diffusion des messages d’abonnement à un événement standard

Assurez-vous que votre point d’entrée pour l’abonnement est conforme aux exigences de diffusion des messages d’abonnement à un événement standard. Pour en savoir plus sur ces exigences, consultez [Exigences en matière de diffusion d’abonnements aux événements](../../wf-api/general/setup-event-sub-endpoint.md).

## Liste autorisée d’adresses IP par région globale

Pour que votre pare-feu ne bloque pas les payloads d’abonnement aux événements, vous devez ajouter les adresses IP à la liste autorisée par région globale. Pour en savoir plus, consultez [API d’abonnement aux événements](../../wf-api/general/event-subs-api.md).

## Avoir un niveau d’accès et une clé API appropriés

Pour créer, interroger ou supprimer un abonnement à un événement, votre utilisateur ou utilisatrice Workfront a besoin des éléments suivants :

* Un niveau d’accès **Administrateur ou administratrice système**
Pour en savoir plus, consultez [Attribuer un accès administratif complet à un utilisateur ou une utilisatrice](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) ou [Attribuer aux utilisateurs et utilisatrices un accès administratif à certaines zones](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Une clé API

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
