---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Désactivation ou réactivation d’un groupe
description: Vous pouvez désactiver un groupe que vous gérez et que vous n’utilisez plus.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Désactivation ou réactivation d’un groupe

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

Vous pouvez désactiver un groupe que vous gérez et que vous n’utilisez plus.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur de groupe du groupe ou un administrateur Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Désactivation ou réactivation d’un groupe

>[!IMPORTANT]
>
>Lorsque vous désactivez un groupe, tous les sous-groupes situés au-dessous sont également désactivés.
>
>Si vous devez réactiver l’un d’eux, vous pouvez le faire après avoir effectué l’une des opérations suivantes :
>
>* Supprimez-le de son groupe parent. Pour plus d’informations, voir la section [Supprimer un sous-groupe de son groupe parent et en faire un groupe de niveau supérieur](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) dans l’article [Gestion d’un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Déplacez-la sous un principal groupe. Pour plus d’informations, voir la section [Créer, déplacer, afficher, modifier, copier, renommer, exporter ou supprimer un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) dans l’article [Gestion d’un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>


1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, sélectionnez **Groupes**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils possèdent. Les administrateurs Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe pour ouvrir sa page.

1. Cliquez sur le menu Plus ![](assets/more-icon.png) en regard du nom du groupe, puis cliquez sur **Désactiver** ou **Réactiver**.

   >[!NOTE]
   >
   >L’option Est Principal (option Réactiver dans l’aperçu) n’est pas disponible si le groupe est un sous-groupe d’un groupe désactivé. Avant de pouvoir la réactiver, vous devez la supprimer de son groupe parent ou la déplacer sous un groupe principal, comme décrit dans la remarque importante ci-dessus.

1. (Conditionnel) Si vous désactivez le groupe, cliquez sur **Désactiver** dans le **Désactiver le groupe** qui s’affiche.

## Considérations pour les groupes inactifs

Tenez compte des points suivants au sujet d’un groupe que vous désactivez en désactivant l’option Est Principal décrite dans la section . [Désactivation ou réactivation d’un groupe](#View) dans cet article.

* La désactivation d’un groupe désactive également tous les sous-groupes situés en dessous. Cela inclut les sous-groupes que vous ajoutez après l’avoir désactivé.

   Pour plus d’informations sur la réactivation d’un sous-groupe dans ce cas, voir [À propos de la réactivation d’un sous-groupe sous un groupe parent inactif](#about-reactivating-a-subgroup-below-an-inactive-parent-group) dans cet article.

* Lorsque vous accédez à la zone Groupes dans Configuration, vous ne pouvez afficher que les groupes principaux dans la liste, car Principal est le filtre par défaut. ![](assets/filter-nwepng.png) pour cela. Si vous souhaitez afficher tous les groupes que vous gérez, y compris les groupes inactifs, vous pouvez utiliser le filtre Tous . Vous pouvez également utiliser le filtre Inactif pour répertorier uniquement les inactifs.

   Pour plus d’informations sur les filtres dans les listes, voir [Présentation des filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* La désactivation d’un groupe ne modifie pas les éléments suivants :

   * Les associations du groupe avec les objets. Les objets associés continuent de fonctionner comme auparavant, sans aucune modification.

      Par exemple, si un projet est associé à un groupe que vous désactivez, il continue à utiliser les préférences et les états du groupe sans aucune modification.

   * Votre capacité à créer un objet, tel qu’une approbation, une équipe ou une entreprise, à partir de la page du groupe dans la configuration. Par défaut, le nouvel objet est associé au groupe inactif.
   * Votre capacité, en tant qu’administrateur, à trouver le groupe dans les filtres et les rapports.

      Vous pouvez également le trouver dans les champs de type avant du groupe dans lesquels vous souhaiterez peut-être gérer les paramètres du groupe dans la zone Configuration . Cela inclut les zones Préférences, Notifications d’événement et Licences système .

      Par exemple, si vous accédez à Configuration > Préférences du projet > Projets et que vous effacez le champ de type avant au-dessus des options, vous pouvez toujours trouver un groupe inactif et configurer ses préférences de projet.

## À propos de la réactivation d’un sous-groupe sous un groupe parent inactif {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

La désactivation d’un groupe désactive également tous les sous-groupes situés en dessous. Si vous devez réactiver l’un des sous-groupes sous un groupe inactif, vous pouvez effectuer l’une des deux opérations suivantes :

* Déplacez le sous-groupe sous un groupe principal. Activez ensuite l’option Est Principal pour le groupe déplacé, comme expliqué dans la section . [Désactivation ou réactivation d’un groupe](#View) dans cet article.

   Pour obtenir des instructions sur le déplacement d’un groupe, voir [Déplacer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Supprimez le sous-groupe de son groupe parent (ce qui fait du sous-groupe un groupe de niveau supérieur). Activez ensuite l’option Est Principal pour le groupe déplacé, comme expliqué dans la section . [Désactivation ou réactivation d’un groupe](#View) dans cet article.

   Pour obtenir des instructions sur la suppression d’un sous-groupe de son groupe parent, reportez-vous à la section . [Supprimer un sous-groupe de son groupe parent et en faire un groupe de niveau supérieur](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) dans l’article [Gestion d’un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
