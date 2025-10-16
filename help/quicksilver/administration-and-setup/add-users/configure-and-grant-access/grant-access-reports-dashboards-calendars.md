---
title: Accorder l’accès aux rapports, tableaux de bord et calendriers
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’une personne aux rapports, tableaux de bord et calendriers dans Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 98%

---

# Accorder l’accès aux rapports, aux tableaux de bord et aux calendriers

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’une personne aux rapports, tableaux de bord et calendriers, comme expliqué dans [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Cet accès comprend également l’accès aux pages externes. Pour plus d’informations sur les pages externes, voir [Accoder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* Si vous voulez donner aux personnes l’accès aux rapports, aux tableaux de bord et aux calendriers, vous devez également leur donner l’accès aux filtres, aux vues et aux regroupements. Pour plus d’informations, voir [Accorder l’accès aux filtres, aux vues et aux regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* Lorsqu’une personne partage un rapport, un tableau de bord ou un calendrier avec une autre personne, les droits de la personne destinataire sont déterminés par une combinaison de deux éléments : le niveau d’accès de la personne destinataire pour les rapports, les tableaux de bord et les calendriers _et_ toutes les autorisations accordées par la personne partageant le rapport, le tableau de bord ou le calendrier.
>
>Pour plus d’informations sur les autorisations que les personnes peuvent accorder à un rapport, un tableau de bord ou un calendrier lorsqu’elles les partagent, voir [Partager des rapports, des tableaux de bord et des calendriers](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

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

## Configurer l’accès des personnes aux rapports, tableaux de bord et calendriers à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d’accès, comme expliqué dans la section [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône en forme d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** à droite de Rapports, puis sélectionnez les capacités que vous souhaitez accorder sous **Ajuster vos paramètres**.

   ![reports_access.png](assets/reports-access.png)

   Les options suivantes sont activées par défaut :

   * **Créer**
   * **Supprimer**
   * **Afficher les rapports intégrés** : cette option doit être sélectionnée pour afficher les rapports créés par Workfront.
   * **Partager**
   * **Partager les rapports publiquement** : les rapports peuvent être partagés publiquement, en partageant un lien public vers le rapport avec toute personne n’ayant pas de compte Workfront. Cette option doit être sélectionnée pour permettre ce niveau de partage.
   * **Partager sur le système** : les rapports peuvent être partagés avec toutes les personnes du système qui possèdent une licence Workfront. Cette option doit être sélectionnée pour permettre ce niveau de partage.

     Pour plus d’informations sur le partage de rapports, de tableaux de bord et de calendriers, voir [Partager des rapports, des tableaux de bord et des calendriers](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones dans le niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles énumérés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), tels que [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’attribuer à un utilisateur ou à une utilisatrice. Pour plus d’informations, voir [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accéder aux rapports, tableaux de bord et calendriers par type de licence

Pour plus d’informations sur ce que les utilisateurs et utilisatrices de chaque niveau d’accès peuvent faire avec les problèmes, voir la section [Rapports](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accéder aux rapports, tableaux de bord et calendriers partagés

En tant que personne propriétaire ou créatrice d’un rapport, d’un tableau de bord ou d’un calendrier, vous pouvez le partager avec d’autres personnes en leur accordant des autorisations, comme expliqué dans [Partager des rapports, des tableaux de bord et des calendriers](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Lorsque vous partagez un objet avec un autre utilisateur ou une autre utilisatrice, les droits des personnes destinataires sur cet objet sont déterminés par une combinaison de deux éléments :

* Les autorisations que vous accordez à votre personne destinataire pour l’objet.
* Les paramètres du niveau d’accès des personnes destinataires pour le type d’objet.
