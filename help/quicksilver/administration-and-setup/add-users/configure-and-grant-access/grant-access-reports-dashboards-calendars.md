---
title: Accorder l’accès aux rapports, aux tableaux de bord et aux calendriers
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur aux rapports, tableaux de bord et calendriers dans Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 11%

---

# Accorder l’accès aux rapports, aux tableaux de bord et aux calendriers

En tant qu’administrateur d’Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur aux rapports, tableaux de bord et calendriers, comme expliqué dans la [présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Cet accès inclut également l’accès aux pages externes. Pour plus d’informations sur les pages externes, voir [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* Si vous souhaitez accorder aux utilisateurs l’accès aux rapports, aux tableaux de bord et aux calendriers, vous devez également leur donner accès aux filtres, aux vues et aux regroupements. Pour obtenir des instructions, voir [Accorder l’accès aux filtres, aux vues et aux regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* Lorsqu’une personne partage un rapport, un tableau de bord ou un calendrier avec un autre utilisateur, les droits du destinataire le concernant sont déterminés par une combinaison de deux éléments : le paramètre de niveau d’accès du destinataire pour les rapports, les tableaux de bord et les calendriers _et_ toutes les autorisations que le responsable du partage a accordées au rapport, au tableau de bord ou au calendrier
>
>Pour plus d’informations sur les autorisations que les utilisateurs peuvent accorder sur un rapport, un tableau de bord ou un calendrier lorsqu’ils le partagent, voir [Partage de rapports, de tableaux de bord et de calendriers](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

## Conditions d’accès

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

## Configurer l’accès des utilisateurs aux rapports, aux tableaux de bord et aux calendriers à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d&#39;accès, comme expliqué dans la section [Créer ou modifier des niveaux d&#39;accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** à droite de Reports, puis sélectionnez les fonctionnalités que vous souhaitez accorder sous **{Affiner vos paramètres**.

   ![reports_access.png](assets/reports-access.png)

   Les options suivantes sont activées par défaut :

   * **Créer**
   * **Supprimer**
   * **Afficher les rapports intégrés** : cette option doit être sélectionnée pour afficher les rapports créés par Workfront.
   * **Partager**
   * **Partager les rapports publiquement** : les rapports peuvent être partagés publiquement en partageant un lien public vers le rapport avec toute personne qui n’a pas de compte Workfront. Cette option doit être sélectionnée pour autoriser ce niveau de partage.
   * **Partager à l’échelle du système** : les rapports peuvent être partagés avec toutes les personnes du système possédant une licence Workfront. Cette option doit être sélectionnée pour autoriser ce niveau de partage.

     Pour plus d’informations sur le partage de rapports, de tableaux de bord et de calendriers, voir [Partage de rapports, de tableaux de bord et de calendriers](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, passez à l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), tels que [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’affecter à un utilisateur. Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accès aux rapports, tableaux de bord et calendriers par type de licence

Pour plus d’informations sur ce que les utilisateurs de chaque niveau d’accès peuvent faire avec des problèmes, reportez-vous à la section [Rapports](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) de l’article [Fonctionnalité disponible pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accès aux rapports, tableaux de bord et calendriers partagés

En tant que propriétaire ou créateur d’un rapport, d’un tableau de bord ou d’un calendrier, vous pouvez le partager avec d’autres utilisateurs en leur accordant des autorisations, comme expliqué dans la section [Partager des rapports, des tableaux de bord et des calendriers](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Lorsque vous partagez un objet avec un autre utilisateur, les droits du destinataire le concernant sont déterminés par une combinaison de deux éléments :

* Autorisations que vous accordez à votre destinataire pour l’objet
* Paramètres du niveau d&#39;accès du destinataire pour le type d&#39;objet
