---
title: Accorder l’accès aux problèmes
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’une personne aux problèmes dans Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3c15f90f-ce87-484d-93a7-9eeb2963a798
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 99%

---

# Accorder l’accès aux problèmes

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’une personne aux problèmes, comme expliqué dans la section [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Pour plus d’informations sur l’utilisation de niveaux d’accès personnalisés pour gérer l’accès des personnes à d’autres types d’objets dans Workfront, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Accorder à des personnes l’accès aux problèmes à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou à modifier le niveau d’accès, comme expliqué dans la section [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** à droite de Problèmes, puis sélectionnez les autorisations que vous souhaitez accorder dans **Ajuster vos paramètres**.

1. (Facultatif) Pour restreindre les autorisations héritées des problèmes issus d’objets de rang supérieur, cliquez sur **Définir des restrictions supplémentaires**, puis sélectionnez **Ne jamais hériter de l’accès aux documents depuis des projets, des tâches, des problèmes, etc.**.

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans la section [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), par exemple [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’attribuer à un utilisateur ou à une utilisatrice. Pour plus d’informations, consultez la section [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accéder aux problèmes par type de licence

Pour plus d’informations sur les actions disponibles pour chaque niveau d’accès, consultez la section [Problèmes](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#issues) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accéder aux problèmes partagés

Si vous possédez ou créez un problème, vous pouvez le partager avec d’autres personnes en leur accordant des autorisations, comme expliqué dans la section [Partager un problème](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

<!--
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
-->

Lorsque vous partagez un objet avec un autre utilisateur ou une autre utilisatrice, les droits des personnes destinataires sur cet objet sont déterminés par une combinaison de deux éléments :

* Les autorisations que vous accordez à votre personne destinataire pour l’objet.
* Les paramètres du niveau d’accès des personnes destinataires pour le type d’objet.

En outre, si leur niveau d’accès le leur autorise, les personnes peuvent accéder à un problème par le biais de la hiérarchie des objets : si une personne dispose déjà d’une autorisation sur le projet ou la tâche parent d’un problème, elle dispose également d’une autorisation sur le problème (voir l’étape 3 ci-dessus). Lorsque vous partagez un problème, vous pouvez consulter la liste des personnes qui ont hérité des autorisations d’accès à celui-ci.

![](assets/inherited-permissions.png)
