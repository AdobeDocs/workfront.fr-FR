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
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 98%

---

# Gérer un sous-groupe

En tant qu’administrateur ou administratrice de groupes d’un sous-groupe, vous pouvez créer, déplacer, afficher, modifier, copier, renommer, exporter et supprimer le sous-groupe.

Vous pouvez également faire d’un sous-groupe un groupe de niveau supérieur en le supprimant de son groupe parent.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs et administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

Pour plus d’informations sur les sous-groupes, voir [Vue d’ensemble des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## Créer, déplacer, afficher, modifier, copier, renommer, exporter ou supprimer un sous-groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils comportent. Les administrateurs et administratrices Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe qui contient le sous-groupe sur lequel vous souhaitez travailler.

   Ou

   Si vous déplacez un ou plusieurs sous-groupes, cliquez sur le nom du groupe de destination (vous préciserez les sous-groupes à déplacer dans une étape ultérieure).

1. Dans le menu de gauche, cliquez sur **Sous-groupes**.

1. Effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Créer un sous-groupe</td> 
      <td> <p>Si vous souhaitez créer le nouveau sous-groupe à un niveau inférieur à celui du groupe affiché, cliquez sur <strong>Ajouter un sous-groupe</strong>.</p> <p>Ou, si vous souhaitez créer le nouveau sous-groupe sous un autre sous-groupe de la liste, sélectionnez ce sous-groupe, puis cliquez sur <strong>Ajouter un</strong><strong> sous-groupe</strong>.</p> <p>Pour plus d’informations sur les options que vous pouvez utiliser pour configurer le sous-groupe, voir le tableau dans <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Créer un sous-groupe</a>.</p> <p>Une hiérarchie de groupes ne peut dépasser 15 niveaux, mais chaque niveau peut comporter un nombre illimité de groupes parallèles.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Déplacer un sous-groupe </td> 
      <td> <p>Vous pouvez déplacer des sous-groupes existants sous un autre groupe que vous administrez.</p> <p>Une hiérarchie de groupes ne peut dépasser 15 niveaux, mais chaque niveau peut comporter un nombre illimité de groupes parallèles.</p> 
       <ol> 
        <li value="1"> <p>(Facultatif) Sélectionnez un sous-groupe pour en faire le groupe de destination.</p> <p>Si vous sautez cette étape, le groupe sélectionné à l’étape 3 est considéré comme le groupe de destination.</p> </li> 
        <li value="2">Cliquez sur <strong>Ajouter un sous-groupe</strong> &gt; <strong>Groupe existant</strong>.</li> 
        <li value="3"> <p>Dans la boîte <strong>Groupe existant</strong> qui apparaît, commencez à saisir le nom du sous-groupe que vous souhaitez déplacer.</p> <p>Les résultats qui s’affichent ne contiennent pas de groupes supérieurs au groupe de destination.</p> <p>Vous pouvez vérifier que vous sélectionnez le bon groupe en pointant dessus et en cliquant sur l’icône d’information <img src="assets/info-icon.png"> qui s’affiche à côté. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus et son équipe d’administration.</p> </li> 
        <li value="4"> <p>Cliquez sur le nom du sous-groupe que vous souhaitez déplacer lorsqu’il apparaît dans la liste.</p> </li> 
        <li value="5"> <p>Répétez les étapes c et d pour tous les autres sous-groupes que vous souhaitez déplacer vers le groupe de destination.</p> </li> 
        <li value="6">Cliquer sur <strong>Enregistrer</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifier un sous-groupe</td> 
      <td> <p>Sélectionnez le sous-groupe que vous souhaitez modifier, puis cliquez sur l’icône Modifier <img src="assets/edit-icon.png">.</p> <p>Pour plus d’informations sur les options que vous pouvez utiliser pour configurer le sous-groupe, voir le tableau dans <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Créer un groupe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exporter un ou plusieurs sous-groupes</td> 
      <td> 
       <ol> 
        <li value="1">Sélectionnez le ou les sous-groupes que vous souhaitez exporter.</li> 
        <li value="2">Cliquez sur l’icône Exporter <img src="assets/export.png">, puis sélectionnez le format de fichier souhaité.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copier un sous-groupe pour créer un groupe de niveau supérieur</td> 
      <td> <p>(Disponible uniquement pour les administrateurs et administratrices Workfront) Lorsque vous copiez un sous-groupe, celui-ci devient un groupe parent. La totalité des personnes membres et des sous-groupes du groupe est copiée avec. Les personnes membres du groupe conservent toutes les affectations attribuées dans le groupe d’origine.</p> <p>Pour plus d’informations sur la copie d’un sous-groupe, voir <a href="#about-copying-a-subgroup" class="MCXref xref">À propos de la copie d’un sous-groupe</a> dans cet article.</p> 
       <ol> 
        <li value="1">Sélectionnez un sous-groupe, puis cliquez sur l’icône Copier <img src="assets/copy-icon.png"> pour créer un groupe de niveau supérieur basé sur le groupe sélectionné.</li> 
        <li value="2"> <p>Configurez les paramètres du nouveau groupe.</p> <p>Pour obtenir de l’aide sur ces paramètres, consultez le tableau de la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Créer un groupe de niveau supérieur en copiant un groupe ou un sous-groupe existant</a> dans l’article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Créer un groupe de niveau supérieur en copiant un groupe ou un sous-groupe existant</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer un sous-groupe</td> 
      <td> <p><b>IMPORTANT</b> : lorsque vous supprimez un groupe ou un sous-groupe, vous devez préserver les utilisateurs et utilisatrices, les éléments de travail et les sous-groupes qui lui sont actuellement affectés. Afin de mieux assurer leur préservation, une invite vous demande de réaffecter les objets du groupe à un autre groupe dans l’étape ci-dessous.</p> 
       <ol> 
        <li value="1">Sélectionnez le sous-groupe, puis cliquez sur l’icône Supprimer <img src="assets/delete.png">.</li> 
        <li value="2">Dans la zone <strong>Supprimer groupe</strong> qui apparaît, commencez à saisir puis sélectionnez le nom du groupe dans lequel vous souhaitez déplacer les personnes membres, les éléments de travail et les sous-groupes du groupe que vous supprimez.</li> 
        <li value="3">Cliquez sur <strong>Les supprimer</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>Lorsque vous gérez un groupe qui contient des sous-groupes, il est pratique de pouvoir identifier et filtrer les données relatives au groupe entier et à tous ses sous-groupes. Pour ce faire, vous pouvez utiliser le champ ID du parent principal dans un rapport ou une liste.
>
>Imaginez, par exemple, que vous dirigiez un grand service de marketing et que vous souhaitiez obtenir une liste de tous les projets sur lesquels travaille l’ensemble du service.
>
>Dans Workfront, ce service Marketing est représenté par un groupe appelé Marketing, avec 3 sous-groupes nommés Marketing de terrain, Marketing de produit et Marketing numérique. Pour répertorier les projets appartenant à l’ensemble du service Marketing (les 4 groupes), vous pouvez créer un filtre pour la zone Projets à l’aide de la règle de filtrage suivante :
>
>`Group: Top Parent ID > Equal > Marketing`
>
>Vous pouvez également utiliser le champ Nom du parent principal pour identifier les données associées à un groupe de niveau supérieur, mais uniquement dans les vues, et non dans les filtres ou les regroupements.

## Retirer un sous-groupe de son groupe parent et en faire un groupe de niveau supérieur

Vous pouvez faire d’un sous-groupe un groupe de niveau supérieur en le retirant de son groupe parent.

>[!TIP]
>
>Lorsque vous désactivez un groupe qui a des sous-groupes sous-jacents, ces sous-groupes deviennent également inactifs. Si vous souhaitez que l’un d’entre eux soit actif, vous pouvez suivre ces instructions pour le retirer de son groupe parent, puis le réactiver.
>
>Pour savoir comment désactiver et réactiver les groupes, voir les sections [Afficher et gérer les détails d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) et [Afficher et gérer les détails d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) dans l’article [Afficher et gérer les détails d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Sélectionnez le groupe parent du groupe dont vous voulez faire un groupe de niveau supérieur, puis cliquez sur l’icône Modifier ![](assets/edit-icon.png).
1. Dans la zone **Modifier un groupe** qui apparaît, sous **Personnes membres du groupe et administrateurs et administratrices de groupe**, commencez à saisir le nom du sous-groupe que vous voulez transformer en groupe de niveau supérieur, puis cliquez sur le X à droite de son nom lorsqu’il apparaît.
1. Cliquer sur **Enregistrer**.

## Afficher et gérer les membres des sous-groupes d’un groupe

Lorsque vous affichez la page principale d’un groupe que vous gérez, vous pouvez voir et gérer toutes les personnes des sous-groupes du groupe. Pour plus d’informations, voir [Afficher et gérer les personnes membres d’un sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## À propos de la copie d’un sous-groupe {#about-copying-a-subgroup}

Lorsque vous copiez un sous-groupe, tenez compte des éléments suivants.

* Si un sous-groupe que vous copiez possède ses propres sous-groupes, ceux-ci sont inclus dans la copie et leurs noms sont formatés comme suit :

  `Original subgroup name (Copy)`

* Tout sous-groupe appartenant à un groupe public est également public, de sorte que les utilisateurs et utilisatrices qui disposent d’un accès de modification, qu’ils fassent partie ou non du groupe, peuvent ajouter des utilisateurs et utilisatrices au sous-groupe.
