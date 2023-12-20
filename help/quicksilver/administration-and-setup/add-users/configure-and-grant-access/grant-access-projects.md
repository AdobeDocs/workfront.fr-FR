---
title: Accorder l’accès aux projets
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur aux projets dans Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: e47f5d06d0c7d72c171583b53b69f951e4e99afe
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Accorder l’accès aux projets

<!-- Audited: 12/2023 -->

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur aux projets, comme expliqué dans les articles suivants :
* [Présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)
* [Nouveaux niveaux d’accès - Aperçu](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)

Pour plus d’informations sur l’utilisation de niveaux d’accès personnalisés pour gérer l’accès des utilisateurs à d’autres types d’objets dans Workfront, voir [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Quelconque</td> 
  </tr> 
    <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard </p>
 <p>ou</p> 
<p>Actuel : formule </p> 
</td> 
  </tr>

<tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configuration de l’accès des utilisateurs aux projets à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d’accès, comme expliqué dans la section [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le **Affichage** ou **Modifier** à droite de la console Projets, puis sélectionnez les fonctionnalités sous lesquelles vous souhaitez accorder des **Ajuster vos paramètres**.

   ![](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* Les utilisateurs disposant d’une licence de travail disposent de droits de projet limités. Ils peuvent contribuer à un projet, mais pas en gérer un.
   >* Les utilisateurs disposant d’une licence de révision disposent de droits d’affichage sur les projets issus de problèmes convertis, mais leurs droits d’affichage sont limités.
   >* Pour plus d’informations sur les autorisations que les utilisateurs peuvent accorder lors du partage de projets avec d’autres personnes, voir [Partage d’un projet dans Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
   >* Lorsque vous configurez un paramètre de niveau d’accès pour un certain type d’objet, cette configuration n’affecte pas l’accès des utilisateurs aux objets de rang inférieur. Par exemple, vous pouvez empêcher les utilisateurs de supprimer des projets dans leur niveau d’accès, mais cela ne les empêche pas de supprimer des tâches, qui sont de rang inférieur à celui des projets. Pour plus d’informations sur la hiérarchie des objets, consultez la section . [Interdépendance et hiérarchie des objets](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) dans l’article [Présentation des objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Facultatif) Cliquez sur **définir les paramètres de partage** à droite de l’option Créer , puis **Ajouter une règle** pour ajouter une règle de partage pour les nouveaux projets.

   Lorsque l’utilisateur disposant de ce niveau d’accès crée un projet, celui-ci est automatiquement partagé avec les utilisateurs que vous sélectionnez dans le menu de gauche.

   ![](assets/project-sharing-menu.png)

   Dans le menu de droite, indiquez comment le projet doit être partagé avec ces utilisateurs :

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >Si un utilisateur disposant de ce niveau d’accès utilise un modèle d’accès au projet, le modèle remplace les paramètres de partage au niveau d’accès. Pour plus d’informations sur les modèles d’accès aux projets, voir [Partage d’un projet dans Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   Vous pouvez répéter cette étape pour ajouter autant de règles de partage de projet que nécessaire pour le niveau d’accès.

1. Cliquez sur le X pour fermer la **Ajuster vos paramètres** de la boîte.
1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans la section [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), par exemple [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’affecter à un utilisateur. Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accès aux rapports, tableaux de bord et calendriers par type de licence

Pour plus d’informations sur ce que les utilisateurs de chaque niveau d’accès peuvent faire avec les problèmes, voir la section [Projets](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accès aux projets partagés

En tant que propriétaire ou créateur d’un problème, vous pouvez le partager avec d’autres utilisateurs en leur accordant des autorisations, comme expliqué dans la section [Partage d’un projet dans Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Lorsque vous partagez un objet avec un autre utilisateur, les droits du destinataire le concernant sont déterminés par une combinaison de deux éléments :

* Autorisations que vous accordez à votre destinataire pour l’objet
* Paramètres du niveau d&#39;accès du destinataire pour le type d&#39;objet
