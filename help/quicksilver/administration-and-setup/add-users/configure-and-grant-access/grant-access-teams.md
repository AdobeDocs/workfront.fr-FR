---
title: Accorder l’accès aux équipes
description: En tant que personne membre de l’administration Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’utilisation des équipes dans Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 99%

---

# Accorder l’accès aux équipes

En tant que personne membre de l’administration Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’utilisation des équipes dans Workfront, comme expliqué dans [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurer l’accès des utilisateurs et utilisatrices à la modification des utilisateurs et utilisatrice à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou à modifier le niveau d’accès, comme expliqué dans [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône en forme d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** à droite d’« Équipes », puis sélectionnez les droits que vous souhaitez accorder sous **Ajuster vos paramètres**.

   * **Afficher** : si vous configurez la façon dont les utilisateurs et les utilisatrices, quelle que soit leur licence, peuvent afficher les équipes, modifiez l’une des options suivantes :

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Afficher les équipes associées à mes groupes</td>
         <td>
          <p><b>Activé</b> : lorsque les utilisateurs et les utilisatrices recherchent des équipes dans un champ de suggestion automatique « Équipe », les équipes associées à leurs groupes sont visibles, que l’équipe leur soit affectée ou non. </p>
          <p><b>Désactivé</b> : lorsque les utilisateurs et les utilisatrices recherchent des équipes dans un champ de suggestion automatique « Équipe », les équipes associées à leurs groupes sont visibles uniquement si elles leur sont affectées.</p><p>Cette option est activée par défaut.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">Afficher toutes les équipes</td>
         <td><p>Lorsque cette option est activée, n’importe quelle équipe peut être affichée et sélectionnée lorsque les utilisateurs et les utilisatrices recherchent des équipes dans un champ de saisie semi-automatique « Équipe ».</p><p>Cette option est activée par défaut. </p></td>
        </tr>
       </tbody>
      </table>

   * **Modifier** : si vous configurez la manière dont les utilisateurs et les utilisatrices disposant des licences Plan et Travail peuvent gérer des équipes, modifiez l’une des options suivantes :

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Créer</td>
         <td><p>Permet aux utilisateurs et aux utilisatrices disposant soit d’une licence Plan, soit d’une licence Travail de créer des équipes.</p><p>Cette option est activée par défaut.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Supprimer</td>
         <td><p> Permet aux utilisateurs et aux utilisatrices disposant d’une licence Plan de supprimer les équipes qui ont des droit de modification (non disponible pour les utilisateurs et les utilisatrices disposant d’une licence Travail).</p><p>Cette option est activée par défaut.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Modifier les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</td>
         <td><p>Permet aux utilisateurs et aux utilisatrices de licences Plan responsables de l’administration de groupes de modifier les équipes affectées aux groupes dont ils assurent la gestion.</p><p>Cette option est activée par défaut.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Modifier les équipes dont je suis membre</td>
         <td><p>Permet aux utilisateurs et aux utilisatrices de licences Plan et Travail de modifier les équipes dont ils sont membres.</p><p>Cette option est désactivée par défaut.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Afficher les équipes associées à mes groupes</td>
         <td>
         <p><b>Activé</b> : lorsque les utilisateurs et les utilisatrices recherchent des équipes dans un champ de suggestion automatique « Équipe », les équipes associées à leurs groupes sont visibles, que l’équipe leur soit affectée ou non. </p>
         <p><b>Désactivé</b> : lorsque les utilisateurs et les utilisatrices recherchent des équipes dans un champ de saisie semi-automatique « Équipe », les équipes associées à leurs groupes sont visibles uniquement si elles leur sont affectées.</p><p>Cette option est activée par défaut.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">Afficher toutes les équipes</td>
         <td><p>Lorsque cette option est activée, n’importe quelle équipe peut être affichée et sélectionnée lorsque les utilisateurs et les utilisatrices recherchent des équipes dans un champ de saisie semi-automatique « Équipe ».</p><p>Cette option est activée par défaut. </p></td>
        </tr>
       </tbody>
      </table>

1. Cliquez sur le X pour fermer la zone **Ajuster vos paramètres**.
1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et domaines dans le niveau d’accès sur lequel vous travaillez, poursuivez avec l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), tels que [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

>[!NOTE]
>
>* Les énoncés suivants sont vrais, quels que soient les paramètres du niveau d’accès :
>
>   * Les personnes propriétaires d’équipes peuvent toujours afficher et modifier leurs équipes.
>   * Les utilisateurs et les utilisatrices ont toujours accès aux équipes qui leur sont affectées.
>
>* La configuration de toute option disponible à la fois pour « Afficher » et pour « Modifier » (telle que « Afficher les équipes associées à mes groupes ») est conservée si vous décidez de sélectionner « Afficher » au lieu de « Modifier » ou « Modifier » au lieu d’« Afficher » dans un niveau d’accès.
>

## Accès aux équipes par type de licence

Pour plus d’informations sur ce que les utilisateurs et les utilisatrices de chaque niveau d’accès peuvent faire avec les problèmes, consultez la section [Équipes](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
