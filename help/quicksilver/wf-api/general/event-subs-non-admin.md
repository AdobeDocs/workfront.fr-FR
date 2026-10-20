---
content-type: api
navigation-topic: general-api
title: Gérer les abonnements aux événements en tant qu’utilisateur non administrateur
description: Si votre accès à Workfront le permet, vous pouvez créer, afficher et supprimer des abonnements à des événements qui se trouvent dans la portée autorisée par vos autorisations et votre configuration système.
author: Courtney
feature: Workfront API
role: Developer
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 10%
---

# Gérer les abonnements aux événements en tant qu’utilisateur non administrateur

Si votre accès à Workfront le permet, vous pouvez créer, afficher et supprimer des abonnements à des événements dans la zone Configuration . Cependant, votre accès est limité aux abonnements et aux actions autorisés pour votre rôle et par la configuration du système de votre organisation.

Cette fonctionnalité n’est pas disponible pour tous les utilisateurs de la même manière qu’elle l’est pour les administrateurs Workfront. Les utilisateurs disposant de l’accès requis peuvent gérer les abonnements aux événements uniquement dans la portée qui leur est accordée.

Par exemple, vos autorisations peuvent vous permettre de gérer uniquement certains types d’objets, d’événements ou d’abonnements pour un ensemble de travail défini. Vous ne pouvez pas gérer les abonnements aux événements en dehors de la portée autorisée par votre accès et votre configuration.

Pour la configuration gérée par l’administrateur, voir [Configuration des abonnements aux événements dans Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md).

Pour plus d’informations sur l’API Event Subscriptions, voir [API Event Subscription](/help/quicksilver/wf-api/general/event-subs-api.md).

>[!NOTE]
>
>Les utilisateurs peuvent gérer les abonnements aux événements uniquement dans la portée autorisée par leurs autorisations et la configuration système de l’entreprise. L’accès n’est pas automatiquement équivalent à l’accès administrateur.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Package Adobe Workfront</td>
   <td>Tous</td>
  </tr>
  <tr>
   <td role="rowheader">Licence Adobe Workfront</td>
   <td>
    <p>Standard</p>
    <p>Plan</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Configurations des niveaux d’accès</td>
   <td>
    <p>Vous devez disposer des droits d'accès appropriés pour gérer les abonnements aux événements.</p>
    <p>Votre accès est limité aux abonnements et aux actions autorisés par vos autorisations et la configuration système de votre organisation.</p>
   </td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utiliser les abonnements aux événements

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **Système**, puis sur **Abonnements aux événements**.
1. Passez en revue les abonnements disponibles.
1. Créez, affichez ou supprimez uniquement les abonnements qui entrent dans votre portée autorisée.

Si les options attendues ne s’affichent pas ou si vous ne parvenez pas à créer ou gérer un abonnement, contactez votre administrateur Workfront pour vérifier si votre accès est limité par le rôle, les autorisations ou la configuration du système.

## Articles connexes

* [Configuration des abonnements aux événements dans Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)
* [API d’abonnement aux événements](/help/quicksilver/wf-api/general/event-subs-api.md)
