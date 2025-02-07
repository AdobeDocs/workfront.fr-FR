---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Désactivation ou réactivation d’un groupe
description: Vous pouvez désactiver un groupe que vous gérez et que vous n’utilisez plus.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 91%

---

# Désactiver ou réactiver un groupe

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

Vous pouvez désactiver un groupe que vous gérez et que vous n’utilisez plus.

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

## Désactiver ou réactiver un groupe

>[!IMPORTANT]
>
>Lorsque vous désactivez un groupe, tous les sous-groupes situés en dessous sont également désactivés.
>
>Si vous devez réactiver l’un d’entre eux, vous pouvez le faire après avoir effectué l’une des opérations suivantes :
>
>* Le retirer de son groupe parent. Pour plus d’informations, voir la section [Supprimer un sous-groupe de son groupe parent et en faire un groupe de niveau supérieur](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) dans l’article [Gérer un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Le déplacer dans un groupe actif. Pour plus d’informations, voir la section [Créer, déplacer, afficher, modifier, copier, renommer, exporter ou supprimer un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) dans l’article [Gérer un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).

{{step-1-to-setup}}

1. Dans le panneau de gauche, sélectionnez **Groupes**.

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe pour ouvrir sa page.

1. Cliquez sur le menu Plus ![icône Plus](assets/more-icon.png) en regard du nom du groupe, puis cliquez sur **Désactiver** ou **Réactiver**.

   >[!NOTE]
   >
   >L’option Est actif (option Réactiver dans la prévisualisation) n’est pas disponible si le groupe est un sous-groupe d’un groupe désactivé. Avant de pouvoir le réactiver, vous devez le supprimer de son groupe parent ou le déplacer sous un groupe actif, comme décrit dans la note importante ci-dessus.

1. (Le cas échéant) Si vous désactivez le groupe, cliquez sur **Désactiver** dans la zone **Désactiver le groupe** qui s’affiche.

## Considérations relatives aux groupes inactifs

Considérez ce qui suit à propos d’un groupe que vous avez désactivé en désactivant l’option Est actif expliquée dans la section [Désactiver ou réactiver un groupe](#View) de cet article.

* La désactivation d’un groupe entraîne la désactivation de tous les sous-groupes qui lui sont subordonnés. Cela inclut les sous-groupes que vous ajoutez après l’avoir désactivé.

  Pour plus d’informations sur la réactivation d’un sous-groupe dans cette situation, voir [Réactivation d’un sous-groupe sous un groupe parent inactif](#about-reactivating-a-subgroup-below-an-inactive-parent-group) dans cet article.

* Lorsque vous accédez à la zone Groupes dans Configuration, vous ne pouvez voir que les groupes actifs dans la liste, car Actif est le filtre par défaut ![icône Filtre](assets/filter-nwepng.png). Si vous souhaitez afficher tous les groupes que vous gérez, y compris les groupes inactifs, vous pouvez utiliser le filtre Tous. Vous pouvez également utiliser le filtre Inactifs pour ne répertorier que les groupes inactifs.

  Pour plus d’informations sur les filtres dans les listes, voir [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* La désactivation d’un groupe ne modifie pas les éléments suivants :

   * Les associations du groupe à des objets. Les objets associés continuent de fonctionner comme avant, sans aucune modification.

     Par exemple, si un projet est associé à un groupe que vous désactivez, le projet continue d’utiliser les préférences et les statuts du groupe sans aucune modification.

   * Votre capacité à créer un nouvel objet, tel qu’une approbation, une équipe ou une entreprise, à partir de la page du groupe dans la configuration. Par défaut, le nouvel objet est associé au groupe inactif.
   * Votre capacité, en tant qu’administrateur ou administratrice, à trouver le groupe dans les filtres et les rapports.

     Vous le trouverez également dans les champs de type de groupe où vous pouvez vouloir gérer les paramètres du groupe dans la zone Configuration. Il s’agit des zones Préférences, Notifications d’événements et Licences système.

     Par exemple, si vous allez dans Configuration > Préférences de projet > Projets et que vous supprimez le champ de type au-dessus des options, vous pouvez toujours trouver un groupe inactif et configurer ses préférences de projet.

## Réactivation d’un sous-groupe sous un groupe parent inactif {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

La désactivation d’un groupe entraîne la désactivation de tous les sous-groupes qui lui sont subordonnés. Si vous devez réactiver l’un des sous-groupes d’un groupe inactif, vous pouvez procéder de deux manières :

* Déplacez le sous-groupe sous un groupe actif. Activez ensuite l’option Est actif pour le groupe déplacé, comme expliqué dans la section [Désactiver ou réactiver un groupe](#View) de cet article.

  Pour savoir comment déplacer un groupe, voir [Déplacer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Supprimez le sous-groupe de son groupe parent (ce qui convertit le sous-groupe en un groupe de niveau supérieur). Activez ensuite l’option Est actif pour le groupe déplacé, comme expliqué dans la section [Désactiver ou réactiver un groupe](#View) de cet article.

  Pour savoir comment supprimer un sous-groupe de son groupe parent, voir la section [Supprimer un sous-groupe de son groupe parent et en faire un groupe de niveau supérieur](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) dans l’article [Gérer un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
