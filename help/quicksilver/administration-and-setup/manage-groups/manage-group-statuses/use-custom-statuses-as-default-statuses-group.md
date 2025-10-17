---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Utiliser un statut personnalisé comme statut par défaut pour un groupe
description: En tant qu’administrateur de groupes, vous pouvez configurer un statut personnalisé comme statut par défaut pour un groupe ou un sous-groupe que vous gérez.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 85%

---

# Utiliser un statut personnalisé comme statut par défaut pour un groupe

En tant qu’administrateur ou administratrice de groupe, vous pouvez configurer un statut personnalisé comme statut par défaut pour un groupe ou un sous-groupe que vous gérez. Cela se révèle utile lorsque le système doit affecter automatiquement un statut Workfront à un projet, une tâche ou un problème. Un projet, une tâche ou un problème affiche toujours le statut personnalisé que vous définissez comme statut par défaut au lieu d’afficher le statut Workfront auquel il correspond.

Le statut que vous configurez peut être tout statut personnalisé créé pour le groupe, hérité d’un groupe situé au-dessus du groupe ou hérité au niveau du système.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs et administratrices peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

>[!INFO]
>
>**Exemple :** vous pouvez créer un statut personnalisé nommé Fini et le définir comme statut par défaut équivalent au statut Terminé de Workfront.
>
>Ensuite, pour les tâches programmées pour passer au statut Terminé lorsqu’elles atteignent 100 %, le statut s’affiche comme Fini au lieu de Terminé.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Statuts des problèmes

Si le statut personnalisé est un statut de problème, les quatre types de problèmes doivent être activés pour celui-ci (rapport de bug, ordre de modification, problème et requête). Par exemple, dans le statut de problème ci-dessous, le statut Réouvert ne peut pas être utilisé comme statut par défaut, car le type de problème Ordre de modification n’est pas sélectionné :

![Tous les types d&#39;événements activés](assets/all-4-issue-types-enabled.png)

## Définir un statut personnalisé comme statut par défaut pour un groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png), puis cliquez sur le nom du groupe dans lequel vous souhaitez créer ou personnaliser des statuts.
1. Dans le panneau de gauche, cliquez sur **Statuts** ![Icône des paramètres d’engrenage](assets/gear-icon-settings.png).
1. Ouvrez l’onglet **Projet**, **Tâches**, ou **Problèmes** selon le type de statut que vous souhaitez définir comme statut par défaut.
1. Cliquez sur **Définir des statuts par défaut** en haut à droite.
1. Dans la liste déroulante qui s’affiche, en regard du statut que vous souhaitez définir par défaut, sélectionnez le statut par défaut à définir.
1. Cliquer sur **Enregistrer**.

   Le statut est désormais disponible comme statut par défaut pour une utilisation avec les projets associés au groupe.

1. Associez le statut personnalisé au projet sur lequel vous souhaitez l’utiliser.

   Vous associez le statut au projet en associant au projet le groupe où le statut réside. Les utilisateurs et utilisatrices ne peuvent utiliser le statut personnalisé que si le groupe où réside le statut est associé au projet.

   >[!NOTE]
   >
   >Si vous affectez le projet à un autre groupe, le statut du projet se recharge et pourrait changer.

   1. Accédez au projet dans lequel vous souhaitez utiliser le statut personnalisé.
   1. Cliquez sur le menu Plus ![icône Plus](assets/more-icon.png), puis sur **Modifier**.
   1. Dans la zone **Modifier le projet** qui s’affiche, dans le champ **Groupe** sous **Association de projets**, sélectionnez le groupe auquel le statut personnalisé est associé.

   1. Cliquez sur **Enregistrer les modifications**.

## Les groupes héritent de configurations de statuts par défaut.

Lorsqu’un administrateur ou une administratrice Workfront configure un statut personnalisé comme statut par défaut, les nouveaux groupes créés héritent de cette configuration.

De même, lorsqu’un administrateur ou une administratrice de groupe définit un statut personnalisé comme statut par défaut, les nouveaux sous-groupes créés directement sous le groupe héritent de cette configuration.

Pour plus d’informations, voir la section [Comment les groupes héritent des statuts](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## Lorsqu’un statut par défaut est masqué

Si vous masquez un statut par défaut (en activant l’option Masquer le statut), le système tente plutôt de définir un autre statut du type équivalent comme valeur par défaut.

S’il n’existe aucun statut disponible du type équivalent, le type de statut s’affiche comme étant **Masqué** et il n’est pas disponible pour les éléments de travail.

![Aucun statut disponible](assets/when-hide-default-status-no-equivalent.png)
