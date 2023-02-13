---
product-area: resource-management
navigation-topic: resource-pools
title: Suppression des utilisateurs des pools de ressources
description: Bien qu’il n’existe aucune limite au nombre d’utilisateurs pouvant appartenir à un pool de ressources, la liste des utilisateurs n’affiche que les 2 000 premiers utilisateurs, classés par ordre alphabétique.
author: Alina
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Suppression des utilisateurs des pools de ressources

Bien qu’il n’existe aucune limite au nombre d’utilisateurs pouvant appartenir à un pool de ressources, la liste des utilisateurs n’affiche que les 2 000 premiers utilisateurs, classés par ordre alphabétique.

Nous vous recommandons de supprimer les utilisateurs qui ont été désactivés ou qui ont déplacé des rôles ou des services, afin de vous assurer que vous disposez toujours d’une liste précise d’utilisateurs dans tous les pools de ressources.

Pour plus d’informations sur les pools de ressources, voir [Présentation des pools de ressources](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès à la gestion des ressources qui inclut l’accès à Gérer les groupes de ressources</p> <p>Affichage ou accès supérieur aux utilisateurs</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>(NOTE:&nbsp;I don't think this is needed for removing users from the pool)</p> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Suppression d’utilisateurs d’un pool de ressources

Vous pouvez supprimer des utilisateurs d’un pool de ressources lorsque ces utilisateurs ne sont plus nécessaires dans ce pool.

Pour supprimer un utilisateur d’un pool de ressources :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Ressource**.
1. Cliquez sur **Groupes de ressources** dans le panneau de gauche.
1. Sélectionnez un pool de ressources et cliquez sur **Modifier.**Ou\
   Cliquez sur le nom d’un pool de ressources.

1. Commencez à saisir le nom d’un utilisateur que vous souhaitez supprimer dans la variable **Recherche dans ce pool de ressources** champ .\
   Ou\
   Commencez à saisir le nom d’une entreprise, d’un rôle de tâche, d’une équipe ou d’un groupe si vous souhaitez supprimer tous les utilisateurs associés à ces entités.\
   ![search_inside_NEW_resource_pool.png](assets/search-inside-new-resource-pool-350x314.png)

1. Cliquez sur l’icône &quot;x&quot; au niveau de l’utilisateur pour supprimer un utilisateur du pool de ressources. Ils sont supprimés de toutes les listes dans lesquelles ils apparaissent.\
   Ou\
   Pour supprimer tous les utilisateurs associés à un rôle de tâche, à un groupe, à une équipe ou à une entreprise, cliquez sur **Supprimer** au niveau du rôle de tâche, du groupe, de l’équipe ou de la société. Cela supprime tous les utilisateurs associés à ce rôle de tâche, ce groupe, cette équipe ou cette société du pool de ressources.

1. Cliquer sur **Enregistrer**.
