---
product-area: templates
navigation-topic: templates-navigation-topic
title: Suppression de modèles de projet
description: Nous vous recommandons de désactiver les modèles que vous n’utilisez plus au lieu de les supprimer afin de conserver des informations historiques sur vos projets au fil du temps.
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: 02d20209b8bf53c84308707a89a5abf399494b64
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Suppression de modèles de projet

Nous vous recommandons de désactiver les modèles que vous n’utilisez plus au lieu de les supprimer afin de conserver des informations historiques sur vos projets au fil du temps. Pour plus d’informations sur la désactivation d’un modèle, voir [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>Lorsque vous supprimez un modèle, les projets qui l’utilisent ne sont en aucune manière modifiés. Cependant, vous ne pouvez plus voir le nom du modèle d’origine dans le champ Modèle du projet. De plus, vous ne pouvez plus afficher les noms des tâches de modèle pour les tâches du projet dans une vue de tâche. Les champs Modèle sur le projet et Tâche de modèle sur les tâches restent vides une fois le modèle initialement associé au projet supprimé.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux modèles qui incluent l’accès à la suppression</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’accès au modèle qui inclut des autorisations de suppression</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Considérations relatives à la suppression de modèles

* Les tâches qui ont été ajoutées aux projets lorsque le modèle a été joint restent sur les projets. Toutefois, les informations de la tâche de modèle associées aux tâches sont supprimées.
* Le nom du modèle n’est plus répertorié dans la **Modèle** sur le champ **Présentation** sous-onglet du projet.

* Vous pouvez récupérer un modèle récemment supprimé dans la Corbeille. Pour plus d’informations sur la récupération d’éléments à partir de la corbeille, voir [Restauration des éléments supprimés](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Supprimer un modèle

{{step1-to-templates}}

La liste des modèles s’affiche alors.

1. Sélectionnez le modèle à supprimer en cochant la case située à gauche du nom du modèle, puis cliquez sur **Supprimer > Oui, Supprimer** pour confirmer la suppression.

   Ou

   Cliquez sur le nom d&#39;un modèle pour y accéder, puis sur le **Plus** menu ![](assets/qs-more-icon-on-an-object.png) , puis **Supprimer le modèle > Oui, supprimer**.

   Le modèle ne peut plus être associé à un projet.
