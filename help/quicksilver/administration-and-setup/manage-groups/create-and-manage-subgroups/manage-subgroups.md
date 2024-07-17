---
user-type: administrator
product-area: system-administration;user-management
keywords: manage,subgroup,edit
navigation-topic: create-and-manage-subgroups
title: Gérer un sous-groupe
description: En tant qu’administrateur de groupe d’un sous-groupe, vous pouvez créer, déplacer, afficher, modifier, copier, renommer, exporter et supprimer le sous-groupe. Vous pouvez également faire d’un sous-groupe un groupe de niveau supérieur en le supprimant de son groupe parent.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1272'
ht-degree: 16%

---

# Gérer un sous-groupe

En tant qu’administrateur de groupe d’un sous-groupe, vous pouvez créer, déplacer, afficher, modifier, copier, renommer, exporter et supprimer le sous-groupe.

Vous pouvez également faire d’un sous-groupe un groupe de niveau supérieur en le supprimant de son groupe parent.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs ou administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

Pour plus d’informations sur les sous-groupes, voir [Présentation des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## Créer, déplacer, afficher, modifier, copier, renommer, exporter ou supprimer un sous-groupe

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

   Dans la liste qui s’affiche, vous pouvez voir les groupes que vous gérez, ainsi que les sous-groupes qu’ils possèdent. Les administrateurs Adobe Workfront peuvent voir tous les groupes.

1. Cliquez sur le nom du groupe contenant le sous-groupe sur lequel vous souhaitez travailler.

   Ou

   Si vous déplacez un ou plusieurs sous-groupes, cliquez sur le nom du groupe de destination (vous indiquez les sous-groupes que vous souhaitez déplacer ultérieurement).

1. Dans le menu de gauche, cliquez sur **Sous-groupes**.

1. Effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Créer un sous-groupe</td> 
      <td> <p>Si vous souhaitez créer le nouveau sous-groupe d’un niveau vers le bas à partir du groupe que vous affichez, cliquez sur <strong>Ajouter un sous-groupe</strong>.</p> <p>Ou, si vous souhaitez créer le nouveau sous-groupe sous un autre sous-groupe de la liste, sélectionnez ce sous-groupe, puis cliquez sur <strong>Ajouter s</strong><strong>sous-groupe</strong>.</p> <p>Pour plus d’informations sur les options que vous pouvez utiliser pour configurer le sous-groupe, consultez le tableau de la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Création d’un sous-groupe</a>.</p> <p>Une hiérarchie de groupe ne peut pas dépasser 15 niveaux, mais un seul niveau peut comporter un nombre illimité de groupes parallèles.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Déplacer un sous-groupe </td> 
      <td> <p>Vous pouvez déplacer des sous-groupes existants sous un autre groupe que vous administrez.</p> <p>Une hiérarchie de groupe ne peut pas dépasser 15 niveaux, mais un seul niveau peut comporter un nombre illimité de groupes parallèles.</p> 
       <ol> 
        <li value="1"> <p>(Facultatif) Sélectionnez un sous-groupe pour en faire le groupe de destination.</p> <p>Si vous ignorez cette étape, le groupe sélectionné à l’étape 3 est le groupe de destination.</p> </li> 
        <li value="2">Cliquez sur <strong>Ajouter un sous-groupe</strong> &gt; <strong>Groupe existant</strong>.</li> 
        <li value="3"> <p>Dans la zone <strong>Groupe existant</strong> qui s’affiche, commencez à saisir le nom d’un sous-groupe que vous souhaitez déplacer.</p> <p>Les résultats qui s’affichent ne contiennent pas de groupes au-dessus du groupe de destination.</p> <p>Vous pouvez vous assurer que vous sélectionnez le bon groupe en le survolant et en cliquant sur l’icône d’information <img src="assets/info-icon.png"> qui s’affiche en regard. Cette option permet d’afficher une infobulle contenant des informations sur le groupe, telles que la hiérarchie des groupes qui le précèdent et ses administrateurs et administratrices.</p> </li> 
        <li value="4"> <p>Cliquez sur le nom du sous-groupe que vous souhaitez déplacer lorsque celui-ci s’affiche dans la liste.</p> </li> 
        <li value="5"> <p>Répétez les étapes c-d pour tous les autres sous-groupes que vous souhaitez déplacer vers le groupe de destination.</p> </li> 
        <li value="6">Cliquer sur <strong>Enregistrer</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifier un sous-groupe</td> 
      <td> <p>Sélectionnez le sous-groupe que vous souhaitez modifier, puis cliquez sur l’icône Modifier <img src="assets/edit-icon.png">.</p> <p>Pour plus d’informations sur les options que vous pouvez utiliser pour configurer le sous-groupe, consultez le tableau de la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Création d’un groupe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exporter un ou plusieurs sous-groupes</td> 
      <td> 
       <ol> 
        <li value="1">Sélectionnez le ou les sous-groupes à exporter.</li> 
        <li value="2">Cliquez sur l'icône Exporter <img src="assets/export.png">, puis sélectionnez le format de fichier souhaité.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copier un sous-groupe pour créer un nouveau groupe de niveau supérieur</td> 
      <td> <p>(Disponible uniquement pour les administrateurs Workfront.) Lorsque vous copiez un sous-groupe, il devient un groupe parent. Tous les membres de groupe et sous-groupes sont copiés avec. Les membres du groupe conservent toutes leurs affectations dans le groupe d’origine.</p> <p>Pour plus d’informations sur la copie d’un sous-groupe, voir <a href="#about-copying-a-subgroup" class="MCXref xref">À propos de la copie d’un sous-groupe</a> dans cet article.</p> 
       <ol> 
        <li value="1">Sélectionnez un sous-groupe, puis cliquez sur l’icône Copier <img src="assets/copy-icon.png"> pour créer un nouveau groupe de niveau supérieur en fonction du groupe sélectionné.</li> 
        <li value="2"> <p>Configurez les paramètres du nouveau groupe.</p> <p>Pour obtenir de l’aide sur ces paramètres, reportez-vous au tableau de la section <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Créer un groupe de niveau supérieur en copiant un groupe ou un sous-groupe existant</a> dans l’article <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Créer un groupe de niveau supérieur en copiant un groupe ou un sous-groupe existant</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suppression d’un sous-groupe</td> 
      <td> <p><b>IMPORTANT</b> : lorsque vous supprimez un groupe ou un sous-groupe, vous devez conserver les utilisateurs, les éléments de travail et les sous-groupes qui lui sont actuellement affectés. Pour vous assurer qu’elles sont conservées, une invite vous invite à réaffecter les objets du groupe à un autre groupe à l’étape ci-dessous.</p> 
       <ol> 
        <li value="1">Sélectionnez le sous-groupe, puis cliquez sur l’icône Supprimer <img src="assets/delete.png">.</li> 
        <li value="2">Dans la zone <strong>Supprimer le groupe</strong> qui s’affiche, en commençant par saisir , puis sélectionnez le nom du groupe dans lequel vous souhaitez déplacer les membres, les tâches et les sous-groupes du groupe que vous supprimez.</li> 
        <li value="3">Cliquez Sur <strong>Les Supprimer</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>Lorsque vous gérez un groupe qui contient des sous-groupes, il est utile de pouvoir identifier et filtrer les données de l’ensemble du groupe et de tous ses sous-groupes. Pour ce faire, utilisez le champ Identifiant principal dans un rapport ou une liste.
>
>Imaginez par exemple que vous gérez un grand service marketing et que vous souhaitez obtenir la liste de tous les projets sur lesquels travaille l’ensemble du service.
>
>Dans Workfront, ce service marketing est représenté par un groupe appelé Marketing, avec 3 sous-groupes appelés Marketing des champs, Marketing des produits et Marketing numérique. Pour répertorier les projets appartenant à l’ensemble du service marketing (les 4 groupes), vous pouvez créer un filtre pour la zone Projets avec la règle de filtrage suivante :
>
>```
>Group: Top Parent ID > Equal > Marketing
>```
>
>Vous pouvez également utiliser le champ Nom du parent supérieur pour identifier les données associées à un groupe de niveau supérieur, mais uniquement dans les vues, et non dans les filtres ou les groupes.

## Supprimer un sous-groupe de son groupe parent et en faire un groupe de niveau supérieur

Vous pouvez faire d’un sous-groupe un groupe de niveau supérieur en le supprimant de son groupe parent.

>[!TIP]
>
>Lorsque vous désactivez un groupe dont les sous-groupes sont situés en dessous, ces sous-groupes deviennent également inactifs. Si vous souhaitez que l’un d’eux soit actif, vous pouvez utiliser ces instructions pour le supprimer de son groupe parent, puis le réactiver.
>
>Pour plus d’informations sur la désactivation et la réactivation des groupes, reportez-vous aux sections [Affichage et gestion des détails d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) et [Affichage et gestion des détails d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) dans l’article [Affichage et gestion des détails d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Sélectionnez le groupe parent du groupe que vous souhaitez créer un groupe de niveau supérieur, puis cliquez sur l’icône Modifier ![](assets/edit-icon.png).
1. Dans la zone **Modifier le groupe** qui s’affiche, sous **Membres du groupe et administrateurs de groupe**, commencez à saisir le nom du sous-groupe que vous souhaitez créer un groupe de niveau supérieur, puis cliquez sur le X à droite de son nom lorsqu’il apparaît.
1. Cliquer sur **Enregistrer**.

## Affichage et gestion des membres du sous-groupe d’un groupe

Lorsque vous affichez la page principale d’un groupe que vous administrez, vous pouvez afficher et gérer tous les utilisateurs des sous-groupes du groupe. Pour obtenir des instructions, voir [Affichage et gestion des membres de sous-groupe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## A propos de la copie d’un sous-groupe {#about-copying-a-subgroup}

Tenez compte de ce qui suit lorsque vous copiez un sous-groupe.

* Si un sous-groupe que vous copiez possède ses propres sous-groupes, ils sont inclus dans la copie et leurs noms sont formatés comme suit :

  ```
  Original subgroup name (Copy)
  ```

* Tout sous-groupe appartenant à un groupe public est également public, de sorte que tout utilisateur disposant d’un accès utilisateur d’édition, au sein ou en dehors du groupe, peut ajouter des utilisateurs au sous-groupe.
