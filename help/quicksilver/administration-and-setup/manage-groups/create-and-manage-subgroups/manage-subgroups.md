---
user-type: administrator
product-area: system-administration;user-management
keywords: gérer, sous-groupe, modifier
navigation-topic: create-and-manage-subgroups
title: Gestion d’un sous-groupe
description: En tant qu’administrateur ou administratrice de groupes d’un sous-groupe, vous pouvez créer, déplacer, afficher, modifier, copier, renommer, exporter et supprimer le sous-groupe. Vous pouvez également faire d’un sous-groupe un groupe de niveau supérieur en le supprimant de son groupe parent.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 6c3f5ee43040f81dac734c5e0b4def9021a0d737
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 53%

---

# Gérer un sous-groupe

En tant qu’administrateur de groupe d’un sous-groupe, vous pouvez créer, déplacer, afficher, modifier, copier, renommer, exporter et supprimer le sous-groupe.

Vous pouvez également faire d’un sous-groupe un groupe de niveau supérieur en le supprimant de son groupe parent.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs et administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

Pour plus d’informations sur les sous-groupes, voir [Vue d’ensemble des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

>[!TIP]
>
>Lorsque vous gérez un groupe qui contient des sous-groupes, il est pratique de pouvoir identifier et filtrer les données relatives au groupe entier et à tous ses sous-groupes. Pour ce faire, vous pouvez utiliser le champ ID du parent principal dans un rapport ou une liste.
>
>Imaginez, par exemple, que vous dirigiez un grand service de marketing et que vous souhaitiez obtenir une liste de tous les projets sur lesquels travaille l’ensemble du service.
>
>Dans Workfront, ce service Marketing est représenté par un groupe appelé Marketing, avec 3 sous-groupes nommés Marketing de terrain, Marketing de produit et Marketing numérique. Pour répertorier les projets qui appartiennent à l’ensemble du service marketing (les 4 groupes), vous pouvez créer un filtre pour la zone Projets avec la règle de filtrage suivante :
>
>`Group: Top Parent ID > Equal > Marketing`
>
>Vous pouvez également utiliser le champ Nom du parent principal pour identifier les données associées à un groupe de niveau supérieur, mais uniquement dans les vues, et non dans les filtres ou les regroupements.

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

## Créer un sous-groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe auquel vous souhaitez ajouter un sous-groupe.
1. Dans le menu de gauche, cliquez sur **Sous-groupes**.
1. Pour créer un nouveau sous-groupe un niveau plus bas à partir du groupe que vous consultez, cliquez sur **Ajouter un sous-groupe**.

   Ou, si vous souhaitez créer le nouveau sous-groupe sous un autre sous-groupe de la liste, sélectionnez-le, puis cliquez sur **Ajouter un sous-groupe**.

   Pour plus d’informations sur les options que vous pouvez utiliser pour configurer le sous-groupe, voir [Créer un sous-groupe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

   Une hiérarchie de groupes ne peut dépasser 15 niveaux, mais chaque niveau peut comporter un nombre illimité de groupes parallèles.

## Déplacer un sous-groupe

Vous pouvez déplacer des sous-groupes existants sous un autre groupe que vous administrez.

Une hiérarchie de groupes ne peut dépasser 15 niveaux, mais chaque niveau peut comporter un nombre illimité de groupes parallèles.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe de destination (vous spécifiez les sous-groupes à déplacer à une étape ultérieure).
1. Dans le menu de gauche, cliquez sur **Sous-groupes**.
1. (Facultatif) Sélectionnez un sous-groupe pour en faire le groupe de destination.

   Si vous sautez cette étape, le groupe sélectionné à l’étape 3 est considéré comme le groupe de destination.

1. Cliquez Sur **Ajouter Un Sous-Groupe > Groupe Existant**.
1. Dans la boîte **Groupe existant** qui apparaît, commencez à saisir le nom du sous-groupe que vous souhaitez déplacer.

   Les résultats qui s’affichent ne contiennent pas de groupes supérieurs au groupe de destination.

   Vous pouvez vous assurer de sélectionner le groupe approprié en pointant la souris sur celui-ci et en cliquant sur l’icône d’informations ![icône d’informations](assets/info-icon.png) qui s’affiche en regard de celui-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus et son équipe d’administration.

1. Sélectionnez le nom du sous-groupe que vous souhaitez déplacer lorsque vous le localisez dans la liste.
1. Répétez les étapes 7 à 8 pour tous les autres sous-groupes que vous souhaitez déplacer vers le groupe de destination.
1. Cliquer sur **Enregistrer**.

## Modifier un sous-groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe contenant le sous-groupe à modifier.
1. Dans le menu de gauche, cliquez sur **Sous-groupes**.
1. Sélectionnez le sous-groupe à modifier, puis cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png).

   Pour plus d’informations sur les options que vous pouvez utiliser pour configurer le sous-groupe, voir [Créer un sous-groupe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Copier un sous-groupe

>[!NOTE]
>
>Seul un administrateur système peut copier un sous-groupe.

Lorsque vous copiez un sous-groupe, celui-ci devient un groupe parent. La totalité des personnes membres et des sous-groupes du groupe est copiée avec. Les membres du groupe conservent toutes les affectations qu&#39;ils avaient dans le groupe d&#39;origine.

Tenez compte des points suivants lorsque vous copiez un sous-groupe :

* Si un sous-groupe que vous copiez possède ses propres sous-groupes, ceux-ci sont inclus dans la copie et leurs noms sont formatés comme suit :

  `Original subgroup name (Copy)`

* Tout sous-groupe appartenant à un groupe public est également public. De ce fait, tout utilisateur autorisé à modifier des utilisateurs, qu’ils fassent partie ou non du groupe, peut y ajouter des utilisateurs.

Pour copier un sous-groupe :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe contenant le sous-groupe à copier.
1. Dans le menu de gauche, cliquez sur **Sous-groupes**.
1. Sélectionnez un sous-groupe, puis cliquez sur l’icône **Copier** ![Icône Copier](assets/copy-icon.png) pour créer un groupe de niveau supérieur en fonction du groupe sélectionné.
1. Configurez les paramètres du nouveau groupe.

   Pour obtenir de l’aide sur ces paramètres, voir [Créer un groupe de niveau supérieur en copiant un groupe ou un sous-groupe existant](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) dans l’article [Créer un groupe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

1. Cliquez sur **Créer un groupe**.

## Exporter un sous-groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe contenant le sous-groupe à exporter.
1. Dans le menu de gauche, cliquez sur **Sous-groupes**.
1. Sélectionnez le ou les sous-groupes que vous souhaitez exporter.
1. Cliquez sur l’icône **Exporter** ![Icône Exporter](assets/export.png), puis sélectionnez le format de fichier souhaité.

## Retirer un sous-groupe de son groupe parent et en faire un groupe de niveau supérieur

Vous pouvez faire d’un sous-groupe un groupe de niveau supérieur en le retirant de son groupe parent.

>[!TIP]
>
>Lorsque vous désactivez un groupe qui a des sous-groupes sous-jacents, ces sous-groupes deviennent également inactifs. Si vous souhaitez que l’un d’entre eux soit actif, vous pouvez suivre ces instructions pour le retirer de son groupe parent, puis le réactiver.
>>Pour obtenir des instructions sur la désactivation et la réactivation de groupes, voir [ Désactiver ou réactiver un groupe ](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).
1. Sélectionnez le groupe parent du sous-groupe pour lequel vous souhaitez créer un groupe de niveau supérieur, puis cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png).
1. Dans la zone **Modifier le groupe** qui s’affiche, commencez à saisir le nom du sous-groupe que vous souhaitez transformer en groupe de niveau supérieur dans le champ **Rechercher** (sous **Membres du groupe et administrateurs de groupe**), puis cliquez sur le X à droite de son nom lorsqu’il apparaît.
1. Cliquer sur **Enregistrer**.

## Supprimer un sous-groupe

>[!IMPORTANT]
>
>Lorsque vous supprimez un groupe ou un sous-groupe, vous devez conserver les utilisateurs et utilisatrices, les éléments de travail et les sous-groupes qui lui sont actuellement affectés. Pour vous assurer qu&#39;ils sont conservés, une invite vous demande de réaffecter les objets du groupe à un autre groupe.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe contenant le sous-groupe à supprimer.
1. Dans le menu de gauche, cliquez sur **Sous-groupes**.
1. Sélectionnez le sous-groupe, puis cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/delete.png).

   Dans la zone **Supprimer le groupe** qui s&#39;affiche, commencez à taper, puis sélectionnez le nom du groupe dans lequel vous souhaitez déplacer les membres, les éléments de travail et les sous-groupes du groupe que vous supprimez.

1. Cliquez sur **Supprimer**.

## Afficher et gérer les membres des sous-groupes d’un groupe

Lorsque vous affichez la page principale d’un groupe que vous gérez, vous pouvez voir et gérer toutes les personnes des sous-groupes du groupe. Pour plus d’informations, voir [Afficher et gérer les membres d’un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

