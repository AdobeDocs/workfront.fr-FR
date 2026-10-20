---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: Configuration des abonnements aux événements dans Workfront
description: Les administrateurs et administratrices de Workfront peuvent créer, afficher et supprimer des abonnements à des événements de la Configuration. Les utilisateurs et utilisatrices disposant de l’accès requis peuvent également gérer les abonnements aux événements dans la portée autorisée par leurs autorisations et la configuration du système.
feature: System Setup and Administration
role: Admin
author: Courtney
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 8%
---

# Configuration des abonnements aux événements dans Workfront

{{highlighted-preview-article-level}}

En tant qu’administrateur Adobe Workfront, vous pouvez créer, afficher et supprimer des abonnements à des événements dans la zone Configuration . Les abonnements aux événements envoient les informations d’événement Workfront à un point d’entrée externe lorsque des événements spécifiés se produisent.

Vous pouvez créer et supprimer des abonnements à des événements dans Workfront, mais vous ne pouvez pas modifier un abonnement existant. Si vous devez modifier un abonnement, supprimez-le et créez-en un nouveau.

Les utilisateurs et utilisatrices disposant de l’accès requis peuvent également gérer les abonnements aux événements dans Workfront, mais uniquement dans la limite autorisée par leurs autorisations et la configuration du système. Pour plus d’informations, voir [Gérer les abonnements aux événements en tant qu’utilisateur non administrateur](/help/quicksilver/wf-api/general/event-subs-non-admin.md).

Pour plus d’informations sur les abonnements aux événements, consultez les articles sous [Abonnements aux événements](/help/quicksilver/wf-api/api/event-subscriptions.md).

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
    <p>Les utilisateurs non administrateurs ne peuvent accéder à que dans la portée autorisée par leurs autorisations et la configuration du système.</p>
   </td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Création d’un abonnement à un événement

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **Système**, puis sur **Abonnements aux événements**.
1. Cliquez sur **Nouvel abonnement à l’événement**.
1. Dans le champ **Objet**, sélectionnez l’objet Workfront que vous souhaitez surveiller.
1. Dans le champ **Type d&#39;événement**, indiquez si vous souhaitez que l&#39;abonnement à l&#39;événement se déclenche lorsque l&#39;objet est créé, mis à jour, supprimé ou partagé.
1. Dans le champ **URL Webhook**, saisissez le point d’entrée qui doit recevoir la payload de l’événement.
1. Dans le champ **Jeton d’authentification**, saisissez le jeton utilisé pour authentifier la requête sur votre point d’entrée.
1. Si vous souhaitez que Workfront code la payload avant de l’envoyer, activez l’option permettant d’envoyer la payload en tant que Base64.
1. Si nécessaire, ajoutez un ou plusieurs filtres pour limiter les événements qui déclenchent l’abonnement. Les filtres disponibles sont basés sur l’objet sélectionné.
1. Cliquez sur **Créer**.

Pour plus d’informations sur les exigences en matière de point d’entrée, voir [Exigences de diffusion des abonnements aux événements](/help/quicksilver/wf-api/general/setup-event-sub-endpoint.md).

## Afficher les abonnements aux événements

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **Système**, puis sur **Abonnements aux événements**.

La page Abonnements aux événements vous permet de consulter les abonnements configurés pour votre environnement. Vous pouvez également consulter le nombre total d’abonnements dont dispose votre entreprise et le nombre de ceux qui sont actifs, désactivés ou gelés.

* **Abonnements désactivés** : ces abonnements ont été automatiquement désactivés en raison d’échecs de diffusion répétés.
* **Abonnements gelés** : ces abonnements sont temporairement gelés en raison de problèmes de diffusion.

## Supprimer un abonnement à un événement

{{step-1-to-setup}}

1. Dans le panneau de navigation de gauche, cliquez sur **Système**, puis sur **Abonnements aux événements**.
1. Sélectionnez l’abonnement à l’événement à supprimer.
1. Cliquez sur **Supprimer**.
