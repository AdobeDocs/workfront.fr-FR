---
title: Octroi de l’accès à la gestion des ressources
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’une personne à la gestion des ressources dans Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 98%

---

# Accorder l’accès à la gestion des ressources

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’une personne à la gestion des ressources, comme expliqué dans la section [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer l’accès des personnes aux outils de gestion des ressources à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou à modifier le niveau d’accès, comme expliqué dans [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** à droite de Gestion des ressources, puis sélectionnez les capacités que vous souhaitez accorder sous **Ajuster vos paramètres**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Modifier les priorités et les heures budgétées dans le Planificateur</td> 
      <td> <p>Permet aux personnes disposant de cette licence d’effectuer les opérations suivantes :</p> <p>Définir la priorité des projets dans le planificateur de ressources.</p> <p>Attribution du budget pour les ressources dans les outils de planification des ressource (sections Planificateur de ressource et Établissement du budget de ressources dans le business case d’un projet).</p> <p>Cette option est activée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gérer les pools de ressources</td> 
      <td> <p>Permet aux personnes disposant de cette licence de créer, modifier et supprimer des groupes de ressources. Cette option est désactivée par défaut.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Mettre à jour le nombre d’heures prévues dans l’équilibreur de charge de travail</span> </td> 
      <td> <p>Permet aux personnes disposant de cette licence de mettre à jour le nombre d’heures prévues des tâches lorsqu’elles mettent à jour les affectations de personnes dans l’équilibreur de charge de travail. Le nombre total d’heures attribuées devient le nombre d’heures prévues des éléments de travail.</p> <p>Cette option est désactivée par défaut.</p> <p> Pour plus d’informations, voir <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gérer les affectations de personnes dans l’équilibreur de charge de travail</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et domaines dans le niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), comme [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’attribuer à un utilisateur ou à une utilisatrice. Pour plus d’informations, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accéder à la gestion des ressources par type de licence

Pour plus d’informations sur ce que les personnes de chaque niveau d’accès peuvent faire avec la gestion des ressources, voir la section [Gestion des ressources](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accéder aux problèmes partagés

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Lorsque vous partagez un objet avec une autre personne, les droits de la personne destinataire quant à l’établissement d’un budget ou l’affichage de l’attribution de ressources sur cet objet sont déterminés par une combinaison de trois éléments :

* Paramètre du niveau d’accès de la personne destinataire pour la gestion des ressources
* Accès de la personne aux données financières, comme expliqué dans la section [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Toute autorisation d’accès aux données financières que la personne à l’origine du partage a accordée pour l’objet.

Pour plus d’informations sur les autorisations que les personnes peuvent accorder aux données financières sur un objet lors du partage, voir [Partager des autorisations financières sur un objet](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
