---
title: Afficher et gérer les détails d’un groupe
description: Vous pouvez afficher et modifier la page Détails du groupe pour un groupe ou un sous-groupe que vous gérez.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 16%

---

# Afficher et gérer les détails d’un groupe

Vous pouvez afficher et modifier la page Détails du groupe pour un groupe ou un sous-groupe que vous gérez. Cette page comprend :

* Description du groupe
* Les noms des chefs d’entreprise et des administrateurs de groupe
* Option permettant de rendre le groupe et ses sous-groupes publics ou privés

  <!--
  <li>An option that allows you to deactivate or reactivate a group and its subgroups.
  DRAFTED IN FLARE:
  Make this change when Callisto adds the
  <b>Is active</b>
   option to the Details pag
  </li>
  -->

Pour plus d’informations sur les autres façons de gérer un groupe, voir [Création d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Pour plus d’informations sur la façon dont vous pouvez désactiver ou réactiver un groupe, voir [Désactivation ou réactivation d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

<!--
DRAFTED IN FLARE:
Delete this paragraph when Callisto adds the
<b>Is active</b>
 option to the Details pag
-->

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan Workfront*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur ou une administratrice de groupe pour le groupe ou un administrateur ou une administratrice de Workfront. Pour plus d’informations, consultez les sections <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à une personne</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir votre plan ou type de licence, contactez l’administration de Workfront.

## Afficher et gérer les détails d’un groupe

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Groups**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils possèdent. Les administrateurs Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe de niveau supérieur que vous souhaitez modifier.
1. Si vous souhaitez désactiver ou réactiver le groupe,
1. Dans le menu de gauche, cliquez sur **Détails du groupe**, puis effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td> <p>Vous pouvez saisir jusqu’à 512 caractères.</p> <p>Si le champ est vide, cliquez sur <strong>Ajouter</strong> pour saisir une description.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Est actif</td> 
      <td> <p>(Activé par défaut) Active le groupe dans votre instance Workfront.</p> <p>Dans des champs de type anticipé comme celui illustré ci-dessous, lorsque des utilisateurs ordinaires recherchent un groupe pour le joindre à un objet ou pour le partager avec lui, seuls les groupes actifs s’affichent dans la liste.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Pour rationaliser cette opération pour vos utilisateurs, vous pouvez désactiver l’option Est active pour les groupes qui ne sont pas actuellement utilisés.</p> <p>Vous pouvez facilement afficher, filtrer et regrouper la liste Groupes en fonction de l’état actif ou inactif à l’aide de ce champ. Pour plus d’informations sur l’utilisation des vues, des filtres et des regroupements dans des listes, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Éléments de reporting : filtres, vues et regroupements</a>.</p> <p>Pour plus d’informations sur les groupes inactifs, reportez-vous à la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">Considérations relatives aux groupes inactifs</a> de l’article <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">Suppression ou désactivation d’un formulaire personnalisé</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accessibilité du groupe</td> 
      <td> <p>(Disponible uniquement si vous affichez les détails d’un groupe, et non d’un sous-groupe.) Activez ou désactivez l’option <strong>Rendez ce groupe et ces sous-groupes privés</strong>.</p> <p>Pour un groupe public, tout utilisateur (dans ou hors du groupe) disposant d’un accès utilisateur d’édition peut ajouter le groupe au profil d’autres utilisateurs. Ils ne peuvent pas le faire pour un groupe privé.</p> <p>Vous ne pouvez modifier cette option que sur le groupe parent supérieur d’une hiérarchie de groupes comportant plusieurs niveaux. Tous les sous-groupes du groupe parent héritent de son paramètre.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Parties prenantes du groupe</td> 
      <td> 
       <ul> 
        <li><strong>Administrateurs de groupe</strong> : ajoutez ou supprimez des utilisateurs disposant d’une licence de planificateur en tant qu’administrateurs de groupe pour le groupe. Commencez à saisir le nom d’un utilisateur, puis cliquez sur celui-ci lorsqu’il apparaît dans le menu déroulant.</li> 
        <li><strong>Business Leader</strong> : effectuez l’une des opérations suivantes :
         <ul>
          <li>Si vous n’avez pas encore affecté de chef d’entreprise au groupe, cliquez sur <strong>Ajouter</strong>, commencez à saisir le nom de l’utilisateur à affecter, puis cliquez sur le nom de la personne lorsqu’il apparaît.</li>
          <li>Si le groupe dispose déjà d’un chef d’entreprise et que vous souhaitez le modifier, double-cliquez sur le nom du chef d’entreprise existant. Supprimez le nom, commencez à saisir le nom de l’utilisateur que vous souhaitez affecter, puis cliquez sur le nom de la personne lorsqu’il apparaît.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ajouter un formulaire personnalisé</td> 
      <td>Si votre niveau d’accès vous permet de gérer des formulaires personnalisés, ajoutez un formulaire personnalisé au groupe. Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Formulaires personnalisés</a>.</td> 
     </tr> 
    </tbody> 
   </table>
