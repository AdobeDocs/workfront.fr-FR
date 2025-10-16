---
product-area: resource-management
navigation-topic: resource-pools
title: Créer des pools de ressources
description: Les pools de ressources sont des ensembles d'utilisateurs qui vous aident à gérer plus facilement les ressources dans Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 80%

---

# Créer des groupes de ressources {#create-resource-pools}

>[!CONTEXTUALHELP]
>id="wf_resource_pools"
>title="Pools de ressources"
>abstract="Pour achever un projet, un groupe de ressources rassemble dans une collection les utilisateurs et les utilisatrices qui sont nécessaires au même moment. Après avoir créé un groupe de ressources, vous pouvez l’associer à des projets et des modèles."

Les groupes de ressources sont des groupes d’utilisateurs et utilisatrices qui facilitent la gestion des ressources dans Adobe Workfront. Pour plus d’informations sur les groupes de ressources, voir [Vue d’ensemble des groupes de ressources](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès à la gestion des ressources qui inclut l’accès à la gestion des pools de ressources</p> <p>Modifier l’accès aux projets, aux modèles et aux utilisateurs et utilisatrices</p></td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Gérez les autorisations des projets, modèles et utilisateurs auxquels vous souhaitez associer les pools de ressources</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un groupe de ressources {#create-a-resource-pool}

{{step1-to-resourcing}}

1. Cliquez sur **Groupes de ressources** dans le panneau de gauche.
1. Cliquez sur **Nouveau groupe de ressources**.

   ![Pools de ressources](assets/list-of-resource-pools.png)

1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nom</strong></td>
      <td>Il s’agit du nom du groupe de ressources.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Description</strong></td>
      <td>Il s’agit d’une brève description de ce groupe de ressources. Par exemple, vous pouvez spécifier son utilité.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Membres du pool</strong></td>
      <td><p> Ajoutez des utilisateurs et utilisatrices un par un au groupe de ressources.<br>Ou <br>Pour ajouter un grand nombre d’utilisateurs et utilisatrices au groupe de ressources en une seule fois. Vous pouvez ajouter l’une des entités suivantes associées à des utilisateurs et utilisatrices ou à un ensemble d’utilisateurs et utilisatrices :
        <ul>
         <li><strong>Équipes</strong> : tous les membres de l’équipe sont ajoutés au groupe de ressources.</li>
         <li><strong>Groupes</strong> : tous les membres du groupe sont ajoutés au groupe de ressources.</li>
         <li><strong>Rôles</strong> : tous les utilisateurs et utilisatrices associés à ce rôle sont ajoutés au groupe de ressources.</li>
         <li><strong>Entreprises</strong> : tous les utilisateurs et utilisatrices de l’entreprise sont ajoutés au groupe de ressources.</li>
        </ul><p>Conseil : vous ne pouvez ajouter que des utilisateurs et utilisatrices, des équipes, des <span>rôles,</span> ou des entreprises actifs.</p><br>Vous devrez peut-être faire défiler la boîte de dialogue vers le bas pour afficher tous les utilisateurs du pool de ressources.
        <p>Remarque : si un utilisateur ou une utilisatrice devient membre d’un groupe, d’une équipe, d’une entreprise ou est associé à une fonction après que le groupe, l’équipe, l’entreprise ou la fonction ont été ajoutés au groupe de ressources, le nouveau membre n’est pas automatiquement ajouté au groupe de ressources. <br>Si un utilisateur ou une utilisatrice appartient à l’équipe, au groupe, à l’entreprise et à la fonction que vous ajoutez, cette personne n’est ajoutée qu’une seule fois au groupe de ressources.<br>Les utilisateurs et utilisatrices qui sont désactivés après avoir été ajoutés au groupe de ressources sont grisés dans la liste des utilisateurs et utilisatrices et sont marqués comme étant désactivés.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Facultatif) Utilisez le lien **Annuler** pour supprimer les utilisateurs et utilisatrices ajoutés par le biais d’un groupe, d’une équipe, d’une entreprise ou d’une fonction.

   >[!NOTE]
   >
   >Il n’y a pas de limite au nombre d’utilisateurs et utilisatrices que vous pouvez avoir dans un groupe de ressources. Cependant, nous recommandons de ne pas ajouter trop d’utilisateurs et utilisatrices à un groupe de ressources, car cela pourrait compliquer la gestion des ressources. La liste des utilisateurs et utilisatrices n’affiche que les 2 000 premières personnes du groupe de ressources et celles-ci sont classées par ordre alphabétique.

   ![Utilisateurs ajoutés au pool de ressources](assets/users-in-resource-pool2.png)

1. (Facultatif) Cliquez sur l’icône X à droite du nom d’un utilisateur pour supprimer un utilisateur. Pour plus d&#39;informations sur la suppression d&#39;utilisateurs d&#39;un pool de ressources, voir [Supprimer des utilisateurs des pools de ressources](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Facultatif) Utilisez l’option **Recherche** pour trouver un utilisateur ou une utilisatrice dans le groupe de ressources.
1. Cliquez sur **Créer**.
