---
title: Affichage et gestion des détails d’un groupe
description: Vous pouvez afficher et modifier la page Détails du groupe d’un groupe ou d’un sous-groupe que vous gérez.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 96%

---

# Afficher et gérer les détails d’un groupe

Vous pouvez afficher et modifier la page Détails du groupe d’un groupe ou d’un sous-groupe que vous gérez. Cette page comprend les éléments suivants :

* Description du groupe.
* Noms du chef ou de la cheffe d’entreprise et des administrateurs et administratrices de groupe.
* Option vous permettant de rendre le groupe et ses sous-groupes publics ou privés.

  <!--
  <li>An option that allows you to deactivate or reactivate a group and its subgroups.
  DRAFTED IN FLARE:
  Make this change when Callisto adds the
  <b>Is active</b>
   option to the Details pag
  </li>
  -->

Pour plus d’informations sur les autres méthodes de gestion d’un groupe, voir [Créer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Pour plus d’informations sur la désactivation ou la réactivation d’un groupe, voir [Désactiver ou réactiver un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

<!--
DRAFTED IN FLARE:
Delete this paragraph when Callisto adds the
<b>Is active</b>
 option to the Details pag
-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher et gérer les détails d’un groupe

{{step-1-to-setup}}

1. Cliquez sur **Groupes**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe de niveau supérieur que vous souhaitez modifier.
1. Si vous souhaitez désactiver ou réactiver le groupe :
1. Dans le menu de gauche, cliquez sur **Détails du groupe**, puis effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td> <p>Vous pouvez saisir jusqu’à 512 caractères.</p> <p>Si le champ est vide, cliquez sur <strong>Ajouter</strong> pour saisir une description.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Est active</td> 
      <td> <p>(Activé par défaut) Active le groupe dans votre instance Workfront.</p> <p>Dans les champs à remplissage automatique comme celui illustré ci-dessous, lorsque des utilisateurs et utilisatrices ordinaires recherchent un groupe pour le joindre à un objet ou pour partager un objet avec celui-ci, seuls les groupes actifs s’affichent dans la liste.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Pour simplifier cette opération pour vos utilisateurs et utilisatrices, vous pouvez désactiver l’option Est actif pour les groupes qui ne sont pas actuellement utilisés.</p> <p>Vous pouvez facilement afficher, filtrer et regrouper la liste des groupes en fonction de l’état actif ou inactif à l’aide de ce champ. Pour plus d’informations sur l’utilisation des vues, des filtres et des regroupements dans les listes, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Éléments de création de rapports : filtres, vues et regroupements</a>.</p> <p>Pour plus d’informations sur les groupes inactifs, voir la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">Remarques relatives aux groupes inactifs</a> dans l’article <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">Supprimer ou désactiver un formulaire personnalisé</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accessibilité du groupe</td> 
      <td> <p>(Disponible uniquement si vous consultez les détails d’un groupe et non d’un sous-groupe.) Activez ou désactivez l’option <strong>Rendre ce groupe et ses sous-groupes privés</strong>.</p> <p>Pour un groupe public, toute personne (faisant partie ou non du groupe) disposant d’un accès d’édition peut ajouter le groupe au profil d’autres utilisateurs et utilisatrices. Cette personne ne peut pas effectuer cette action pour un groupe privé.</p> <p>Vous ne pouvez modifier cette option que pour le groupe parent situé au niveau le plus haut d’une hiérarchie de groupes à plusieurs niveaux. Tous les sous-groupes du groupe parent héritent de ce paramètre.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Parties prenantes du groupe</td> 
      <td> 
       <ul> 
        <li><strong>Administrateurs et administratrices de groupes</strong> : ajoutez ou supprimez des utilisateurs et utilisatrices disposant d’une licence de planification en tant qu’administrateurs et administratrices de groupes pour le groupe. Commencez à saisir le nom d’un utilisateur ou d’une utilisatrice, puis cliquez sur le nom lorsqu’il apparaît dans le menu déroulant.</li> 
        <li><strong>Chef ou cheffe d’entreprise</strong> : effectuez l’une des opérations suivantes :
         <ul>
          <li>Si vous n’avez pas encore désigné de chef ou cheffe d’entreprise pour le groupe, cliquez sur <strong>Ajouter</strong>, commencez à saisir le nom de l’utilisateur ou de l’utilisatrice que vous souhaitez désigner, puis cliquez sur le nom de la personne lorsqu’il apparaît.</li>
          <li>Si le groupe possède déjà un chef ou une cheffe d’entreprise et que vous souhaitez en changer, double-cliquez sur le nom du chef ou de la cheffe d’entreprise existant. Supprimez le nom, commencez à saisir le nom de l’utilisateur ou de l’utilisatrice que vous souhaitez affecter, puis cliquez sur le nom de la personne lorsqu’il apparaît.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ajouter un formulaire personnalisé</td> 
      <td>Si votre niveau d’accès vous permet de gérer des formulaires personnalisés, ajoutez un formulaire personnalisé au groupe. Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Formulaires personnalisés</a>.</td> 
     </tr> 
    </tbody> 
   </table>
