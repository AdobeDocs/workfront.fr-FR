---
title: Accorder l’accès aux portfolios
user-type: administrator
product-area: system-administration;portfolios
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur aux portefeuilles dans Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f4a9c4f3-8ed4-4629-aced-9cc09b8acd3f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 17%

---

# Accorder l’accès aux portfolios

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur aux portefeuilles, comme expliqué dans la [présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## Configuration de l’accès des utilisateurs aux portefeuilles à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d&#39;accès, comme expliqué dans la section [Créer ou modifier des niveaux d&#39;accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** situé à droite de Portfolio, puis sélectionnez les fonctionnalités que vous souhaitez accorder sous **{Affiner vos paramètres**.

   ![](assets/fine-tune-portfolios.png)

   >[!NOTE]
   >
   >Lorsque vous configurez un paramètre de niveau d’accès pour un certain type d’objet, cette configuration n’affecte pas l’accès des utilisateurs aux objets de rang inférieur. Par exemple, vous pouvez empêcher les utilisateurs de supprimer des portfolios dans leur niveau d’accès, mais cela ne les empêche pas de supprimer des projets, qui sont de rang inférieur à ceux des portfolios. Pour plus d’informations sur la hiérarchie des objets, reportez-vous à la section [Interdépendance et hiérarchie des objets](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) de l’article [Comprendre les objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, passez à l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), tels que [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’affecter à un utilisateur. Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accès aux portefeuilles par type de licence

Pour plus d’informations sur ce que les utilisateurs de chaque niveau d’accès peuvent faire avec les portefeuilles, reportez-vous à la section [Portfolios](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#portfoli) de l’article [Fonctionnalité disponible pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accès aux portefeuilles partagés

En tant que propriétaire ou créateur d’un portfolio, vous pouvez le partager avec d’autres utilisateurs en leur accordant des autorisations, comme expliqué dans la section [Partager un portfolio](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).

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

Pour plus d’informations sur les autorisations que les utilisateurs peuvent accorder à un portfolio lors de son partage, voir [Partager un portfolio](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).
