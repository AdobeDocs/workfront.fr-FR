---
title: Accorder l’accès à la gestion des ressources
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur à la gestion des ressources dans Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 19%

---

# Accorder l’accès à la gestion des ressources

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur à la gestion des ressources, comme expliqué dans la [présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurer l’accès des utilisateurs aux outils de gestion des ressources à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d&#39;accès, comme expliqué dans la section [Créer ou modifier des niveaux d&#39;accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** à droite de la gestion des ressources, puis sélectionnez les fonctionnalités que vous souhaitez accorder sous **Ajuster vos paramètres**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Modifier les priorités et les heures budgétées dans le Planificateur</td> 
      <td> <p>Permet aux utilisateurs disposant de cette licence d’effectuer les opérations suivantes :</p> <p>Définir la priorité des projets dans le planificateur de ressources.</p> <p>Allocation budgétaire pour les ressources dans les outils Resource Planning (section Resource Planner et Resource Budget dans l’ Analyse de cas d’un projet).</p> <p>Cette option est activée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gérer les pools de ressources</td> 
      <td> <p>Permet aux utilisateurs disposant de cette licence de créer, modifier et supprimer des groupes de ressources. Cette option est désactivée par défaut.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Mise à jour des heures planifiées dans l’équilibreur de charge de travail</span> </td> 
      <td> <p>Permet aux utilisateurs disposant de cette licence de mettre à jour les heures planifiées des tâches lorsqu’ils mettent à jour les affectations utilisateur dans l’équilibreur de charge de travail. Le nombre total d’heures allouées devient les Heures planifiées des tâches.</p> <p>Cette option est désactivée par défaut.</p> <p> Pour plus d’informations, voir <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gérer les affectations des utilisateurs et utilisatrices dans l’équilibreur de charge de travail</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, passez à l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), tels que [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’affecter à un utilisateur. Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accès à la gestion des ressources par type de licence

Pour plus d’informations sur ce que les utilisateurs de chaque niveau d’accès peuvent faire avec Resource Management, reportez-vous à la section [Resource Management](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) de l’article [Fonctionnalité disponible pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accès aux problèmes partagés

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Lorsque vous partagez un objet avec un autre utilisateur, les droits du destinataire quant au budget ou à l&#39;affichage de l&#39;allocation de ressources sur cet objet sont déterminés par une combinaison de trois éléments :

* Paramètre du niveau d’accès du destinataire pour la gestion des ressources
* L&#39;accès de l&#39;utilisateur aux données financières, comme expliqué dans la section [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Toute autorisation d’accès aux données financières que le responsable du partage a accordée pour l’objet

Pour plus d’informations sur les autorisations que les utilisateurs peuvent accorder aux données financières sur un objet lors du partage de l’objet, voir [Partage des autorisations financières sur un objet](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
