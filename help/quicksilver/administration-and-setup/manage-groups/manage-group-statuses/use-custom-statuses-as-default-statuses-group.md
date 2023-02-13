---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Utiliser un état personnalisé comme état par défaut pour un groupe
description: En tant qu’administrateur de groupe, vous pouvez configurer un état personnalisé comme état par défaut pour un groupe ou un sous-groupe que vous gérez. Cela s’avère utile lorsque le système doit attribuer automatiquement un état Workfront à un projet, une tâche ou un problème. Un projet, une tâche ou un problème affiche toujours l’état personnalisé que vous définissez comme état par défaut au lieu d’afficher l’état Workfront auquel il correspond.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Utiliser un état personnalisé comme état par défaut pour un groupe

En tant qu’administrateur de groupe, vous pouvez configurer un état personnalisé comme état par défaut pour un groupe ou un sous-groupe que vous gérez. Cela s’avère utile lorsque le système doit attribuer automatiquement un état Workfront à un projet, une tâche ou un problème. Un projet, une tâche ou un problème affiche toujours l’état personnalisé que vous définissez comme état par défaut au lieu d’afficher l’état Workfront auquel il correspond.

L’état que vous configurez peut être tout état personnalisé créé pour le groupe, hérité d’un groupe situé au-dessus du groupe ou hérité au niveau du système.

S’il existe des groupes au-dessus du groupe que vous gérez, leurs administrateurs peuvent également le faire pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

>[!INFO]
>
>**Exemple :** Vous pouvez créer un état personnalisé nommé Terminé et le définir comme un état par défaut associé à l’état Workfront Terminé.
>
>Ensuite, pour les tâches définies pour passer à l’état Terminé lorsqu’elles atteignent 100 %, l’état s’affiche comme Terminé au lieu de Terminé.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur de groupe du groupe ou un administrateur Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Statuts des problèmes

Si l’état personnalisé est un état de problème, les quatre types de problème doivent être activés pour celui-ci (rapport de bogue, ordre de modification, problème et requête). Par exemple, dans l’état ci-dessous, l’état Réouvert ne peut pas être utilisé comme état par défaut, car le type de problème Modifier l’ordre n’est pas sélectionné :

![](assets/all-4-issue-types-enabled.png)

## Définition d’un état personnalisé comme état par défaut pour un groupe

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).
1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png), puis cliquez sur le nom du groupe dans lequel vous souhaitez créer ou personnaliser des états.
1. Dans le panneau de gauche, cliquez sur **Statuts** ![](assets/gear-icon-settings.png).
1. Ouvrez le **Projet**, **Tâches** ou **Problèmes** selon le type d’état que vous souhaitez définir comme état par défaut.
1. Cliquez sur **Définition des états par défaut** près du coin supérieur droit.
1. Dans la liste déroulante qui s’affiche, en regard de l’état dans lequel vous souhaitez définir l’état par défaut, sélectionnez l’état par défaut à définir.
1. Cliquer sur **Enregistrer**.

   L’état est désormais disponible comme état par défaut pour une utilisation avec les projets associés au groupe.

1. Associez l’état personnalisé au projet dans lequel vous souhaitez l’utiliser.

   Vous associez le statut au projet en associant le groupe où il réside au projet. Les utilisateurs ne peuvent utiliser l’état personnalisé que si le groupe où réside l’état est associé au projet.

   >[!NOTE]
   >
   >Si vous affectez le projet à un autre groupe, l’état du projet se recharge et peut changer.

   1. Accédez au projet dans lequel vous souhaitez utiliser l’état personnalisé.
   1. Cliquez sur le menu Plus ![](assets/more-icon.png), puis cliquez sur **Modifier**.
   1. Dans le **Modifier le projet** qui s’affiche, dans la **Groupe** champ sous **Association de projets**, sélectionnez le groupe auquel l’état personnalisé est associé.

   1. Cliquez sur **Enregistrer les modifications**.

## Les groupes héritent des configurations d’état par défaut.

Lorsqu’un administrateur Workfront configure un état personnalisé comme état par défaut, les nouveaux groupes créés héritent de cette configuration.

De même, lorsqu’un administrateur de groupe définit un état personnalisé comme état par défaut, les nouveaux sous-groupes créés directement sous le groupe héritent de cette configuration.

Pour plus d’informations, voir [Comment les groupes héritent des états](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## Lorsqu’un état par défaut est masqué

Si vous masquez un état par défaut (en activant l’option Masquer l’état ), le système tente plutôt de définir un autre état du type équivalent comme valeur par défaut.

S’il n’existe aucun état disponible du type équivalent, le type d’état s’affiche comme **Masqué** et n’est pas disponible pour les tâches.

![](assets/when-hide-default-status-no-equivalent.png)
