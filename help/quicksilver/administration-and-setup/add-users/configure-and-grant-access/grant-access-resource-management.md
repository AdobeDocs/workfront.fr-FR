---
title: Accorder l’accès à la gestion des ressources
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur à la gestion des ressources dans Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 3%

---

# Accorder l’accès à la gestion des ressources

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur à la gestion des ressources, comme expliqué dans la section [Présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurer l’accès des utilisateurs aux outils de gestion des ressources à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d’accès, comme expliqué dans la section [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le **Affichage** ou **Modifier** à droite de Resource Management, puis sélectionnez les fonctionnalités que vous souhaitez accorder sous **Ajuster vos paramètres**.

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
      <td role="rowheader"><span>Mettre à jour les heures planifiées dans l'équilibreur de charge de travail</span> </td> 
      <td> <p>Permet aux utilisateurs disposant de cette licence de mettre à jour les heures planifiées des tâches lorsqu’ils mettent à jour les affectations utilisateur dans l’équilibreur de charge de travail. Le nombre total d’heures allouées devient les Heures planifiées des tâches.</p> <p>Cette option est désactivée par défaut.</p> <p> Pour plus d’informations, voir <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestion des affectations utilisateur dans l’équilibreur de charge de travail</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans la section [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), par exemple [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’affecter à un utilisateur. Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accès à la gestion des ressources par type de licence

Pour plus d’informations sur ce que les utilisateurs de chaque niveau d’accès peuvent faire avec la gestion des ressources, voir la section [Gestion des ressources](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accès aux problèmes partagés

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Lorsque vous partagez un objet avec un autre utilisateur, les droits du destinataire quant au budget ou à l&#39;affichage de l&#39;allocation de ressources sur cet objet sont déterminés par une combinaison de trois éléments :

* Paramètre du niveau d’accès du destinataire pour la gestion des ressources
* L’accès de l’utilisateur aux données financières, comme expliqué dans la section [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Toute autorisation d’accès aux données financières que le responsable du partage a accordée pour l’objet

Pour plus d’informations sur les autorisations que les utilisateurs peuvent accorder aux données financières sur un objet lors du partage, voir [Partage des autorisations financières sur un objet](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
