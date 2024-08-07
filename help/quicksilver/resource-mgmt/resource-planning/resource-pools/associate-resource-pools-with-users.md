---
product-area: resource-management
navigation-topic: resource-pools
title: Associer des pools de ressources à des utilisateurs et utilisatrices
description: Vous devez créer un pool de ressources avant de pouvoir l’associer à des utilisateurs. Vous pouvez associer des utilisateurs à des pools de ressources lors de la création de vos pools de ressources.
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: 36599722aafadcbbc630650a94005fd73b3e517e
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 32%

---

# Associer des pools de ressources à des utilisateurs et utilisatrices

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Les pools de ressources sont des groupes d’utilisateurs qui vous aident à gérer les ressources dans Adobe Workfront.

Vous devez créer un pool de ressources avant de pouvoir l’associer à des utilisateurs.

Vous pouvez associer des utilisateurs à des pools de ressources lors de la création de vos pools de ressources.

Si vous créez des pools de ressources sans les remplir avec des utilisateurs, vous pouvez les associer ultérieurement à des utilisateurs au fur et à mesure que vous modifiez ou créez de nouveaux utilisateurs.

Pour plus d’informations sur les pools de ressources, voir [Présentation des pools de ressources](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Pour plus d’informations sur la création de pools de ressources, voir [Création de pools de ressources](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès à la gestion des ressources qui inclut l’accès à Gérer les groupes de ressources</p> <p>Modifier l’accès aux projets, aux modèles et aux utilisateurs</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérez les autorisations des projets, modèles et utilisateurs auxquels vous associez les pools de ressources</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Associer des pools de ressources à un utilisateur

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Users**.
1. Cochez la case en regard du nom d’un utilisateur dans la liste, puis cliquez sur **Modifier**.
1. Cliquez sur **Resource Planning**.
1. Commencez à saisir le nom d’un pool de ressources que vous souhaitez associer à l’utilisateur dans le champ **Pools de ressources**, puis sélectionnez-le dans la liste, lorsqu’il s’affiche.\
   Vous pouvez associer plusieurs pools de ressources à un seul utilisateur.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Cliquez sur **Enregistrer les modifications**.

Pour plus d’informations sur la modification des utilisateurs, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Pour plus d’informations sur la création d’utilisateurs et d’utilisatrices, voir [Ajouter des utilisateurs et des utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Associer les pools de ressources aux utilisateurs en bloc

Vous pouvez modifier plusieurs utilisateurs en bloc et associer les mêmes pools de ressources à tous en même temps.

Pour associer des pools de ressources à plusieurs utilisateurs en bloc :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Users**.
1. Sélectionnez plusieurs utilisateurs dans la liste, puis cliquez sur **Modifier**.
1. Cliquez sur **Resource Planning**.
1. Commencez à saisir le nom d’un pool de ressources que vous souhaitez associer aux utilisateurs dans le champ **Pools de ressources**, puis sélectionnez-le dans la liste, lorsqu’il s’affiche.\
   Vous pouvez associer plusieurs pools de ressources à plusieurs utilisateurs.

   >[!NOTE]
   >
   >Seuls les pools de ressources communs à tous les utilisateurs sélectionnés s’affichent dans ce champ. Si les utilisateurs et utilisatrices sélectionnés n’ont pas de pools de ressources partagés, ce champ est vide. Si ce champ est vide, les pools de ressources que vous spécifiez ici remplaceront leurs pools de ressources individuels.

1. Cliquez sur **Enregistrer les modifications**.

Pour plus d’informations sur la modification des utilisateurs en masse, voir [Modification des profils utilisateur en masse](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
