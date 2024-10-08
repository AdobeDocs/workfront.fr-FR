---
product-area: resource-management
navigation-topic: resource-pools
title: Créer des groupes de ressources
description: Les pools de ressources sont des ensembles d’utilisateurs qui vous aident à gérer plus facilement les ressources dans Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: 2f5e0b8ba4ec4f32ae0457a6a901a43d03389773
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 76%

---

# Créer des groupes de ressources {#create-resource-pools}

>[!CONTEXTUALHELP]
>id="wf_resource_pools"
>title="Pools de ressources"
>abstract="Un pool de ressources est un ensemble d’utilisateurs qui sont nécessaires en même temps pour la fin d’un projet. Après avoir créé un pool de ressources, vous pouvez l’associer à des projets et des modèles."

{{preview-and-fast-release-Q424}}

Les groupes de ressources sont des groupes d’utilisateurs et utilisatrices qui facilitent la gestion des ressources dans Adobe Workfront. Pour plus d’informations sur les groupes de ressources, voir [Vue d’ensemble des groupes de ressources](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td><p>Nouveau : Tous</p>
       <p>ou</p>
       <p>Actuel : Pro ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès à la gestion des ressources qui inclut l’accès à Gérer les groupes de ressources</p> <p>Modifier l’accès aux projets, aux modèles et aux utilisateurs et utilisatrices</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Gérez les autorisations des projets, modèles et utilisateurs auxquels vous souhaitez associer les groupes de ressources.</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un groupe de ressources {#create-a-resource-pool}

{{step1-to-resourcing}}

1. Cliquez sur **Groupes de ressources** dans le panneau de gauche.

   <span class="preview">Exemple d’image dans l’environnement de prévisualisation :</span>
   <span class="preview">![Pools de ressources](assets/list-of-resource-pools.png)</span>

   Exemple d’image dans l’environnement de production :
   ![Pools de ressources](assets/resource-pools-tab-350x198.png)

1. Cliquez sur **Nouveau groupe de ressources**.
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
        </ul><p>Conseil : vous ne pouvez ajouter que des utilisateurs et utilisatrices, des équipes, des <span>rôles,</span> ou des entreprises actifs.</p><br>Vous devrez peut-être faire défiler la page vers le bas de la boîte de dialogue pour afficher tous les utilisateurs dans le pool de ressources.
        <p>Remarque : si un utilisateur ou une utilisatrice devient membre d’un groupe, d’une équipe, d’une entreprise ou est associé à une fonction après que le groupe, l’équipe, l’entreprise ou la fonction ont été ajoutés au groupe de ressources, le nouveau membre n’est pas automatiquement ajouté au groupe de ressources. <br>Si un utilisateur ou une utilisatrice appartient à l’équipe, au groupe, à l’entreprise et à la fonction que vous ajoutez, cette personne n’est ajoutée qu’une seule fois au groupe de ressources.<br>Les utilisateurs et utilisatrices qui sont désactivés après avoir été ajoutés au groupe de ressources sont grisés dans la liste des utilisateurs et utilisatrices et sont marqués comme étant désactivés.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Facultatif) Utilisez le lien **Annuler** pour supprimer les utilisateurs et utilisatrices ajoutés par le biais d’un groupe, d’une équipe, d’une entreprise ou d’une fonction.

   >[!NOTE]
   >
   >Il n’y a pas de limite au nombre d’utilisateurs et utilisatrices que vous pouvez avoir dans un groupe de ressources. Cependant, nous recommandons de ne pas ajouter trop d’utilisateurs et utilisatrices à un groupe de ressources, car cela pourrait compliquer la gestion des ressources. La liste des utilisateurs et utilisatrices n’affiche que les 2 000 premières personnes du groupe de ressources et celles-ci sont classées par ordre alphabétique.

   <span class="preview">Exemple d’image dans l’environnement de prévisualisation :</span>
   <span class="preview">![Utilisateurs ajoutés au pool de ressources](assets/users-in-resource-pool2.png)</span>

   Exemple d’image dans l’environnement de production :
   ![Utilisateurs ajoutés au pool de ressources](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (Facultatif) Cliquez sur l’icône X située à droite du nom d’un utilisateur pour le supprimer. Pour plus d’informations sur la suppression des utilisateurs d’un pool de ressources, voir [Suppression des utilisateurs des pools de ressources](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Facultatif) Utilisez l’option **Recherche** pour trouver un utilisateur ou une utilisatrice dans le groupe de ressources.
1. Cliquez sur **Créer**.
