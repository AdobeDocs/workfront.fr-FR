---
title: Activité Publication de fusion Workfront :&nbsp;Semaine du 30 août 2021
description: Activité Publication de fusion Workfront :&nbsp;Semaine du 30 août 2021
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Activité Publication de fusion Workfront : semaine du 30 août 2021

Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion au cours de la semaine du 30 août 2021.

Pour obtenir la liste de toutes les modifications récentes, voir [Activité Publication de fusion Adobe Workfront](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Pour obtenir la liste des correctifs récents dans Workfront Fusion, reportez-vous à la section [Mises à jour de maintenance de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) et recherchez toutes les mises à jour intitulées Mise à jour de maintenance de la fusion Workfront.

## Filtrage des événements qui déclenchent le module Workfront > Evénements de contrôle

1. Configurer un filtre personnalisé pour les événements qui déclenchent le module Workfront > Evénements de contrôle

   Pour réduire le nombre d’exécutions de scénarios superflues, nous avons mis à jour le module Workfront > Enregistrements de contrôle afin d’activer le filtrage des événements. Vous pouvez maintenant définir un filtre lors de la création d’un webhook. Cela permet au scénario de se déclencher uniquement lorsque l’événement répond à certains critères.

   Le filtre d’événement propose actuellement les opérations suivantes :

   * Equal : Déclenchez un scénario uniquement lorsqu’un événement correspond aux conditions du filtre. Par exemple, vous pouvez configurer un filtre qui déclenche un scénario uniquement si l’événement se produit dans un projet spécifique.
   * Not Equal : Déclenchez un scénario uniquement si un événement ne correspond pas aux conditions du filtre. Par exemple, vous pouvez créer un filtre qui déclenche un scénario uniquement si le problème qui se produit dans n’a pas l’état Fermé.

   Auparavant, le module Watch records récupérait tous les enregistrements. Les utilisateurs peuvent filtrer uniquement en configurant des filtres ultérieurement dans le scénario.

   Pour tirer parti du filtrage des événements, créez un webhook dans votre module Watch events. Il n’est actuellement pas possible de modifier les webhooks existants pour inclure cette fonctionnalité. Nous vous recommandons vivement de créer de nouveaux webhooks à l’aide de filtres d’événement pour vos scénarios existants.

1. Filtrez les événements déclenchés par la connexion actuelle.

   Pour faciliter la configuration de vos webhooks pour le module Workfront > Evénements de contrôle , nous avons inclus le filtre d’événement le plus courant. Désormais, le webhook dispose d’une option pour filtrer toute modification apportée par les modules à l’aide de la connexion spécifiée pour le module de surveillance des événements. En d’autres termes, avec ce filtre activé, les modifications effectuées par l’utilisateur Workfront associé à cette connexion ne peuvent pas déclencher le scénario.

   Auparavant, ce filtre n’était pas disponible. Par conséquent, il était plus facile pour les modifications apportées aux modules Workfront de déclencher des scénarios contenant ces modules, ce qui pouvait entraîner le déclenchement de scénarios dans une boucle infinie.

Pour plus d’informations sur les filtres d’événements dans le module Workfront > Evénements de contrôle, voir [Modules Adobe Workfront](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

