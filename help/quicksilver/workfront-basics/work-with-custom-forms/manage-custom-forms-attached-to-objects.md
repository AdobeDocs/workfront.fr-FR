---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Gérer les formulaires personnalisés associés à des objets
description: Vous pouvez mettre à jour l’ordre dans lequel les formulaires personnalisés associés à un objet s’affichent, les supprimer ou modifier en masse la manière dont les formulaires personnalisés s’affichent sur plusieurs objets.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 97%

---

# Gérer les formulaires personnalisés associés à des objets

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Vous pouvez mettre à jour l’ordre dans lequel les formulaires personnalisés associés à un objet s’affichent, les supprimer ou modifier en masse la manière dont les formulaires personnalisés s’affichent sur plusieurs objets.

## Conditions d’accès

Vous devez disposer des droits d’accès suivants pour effectuer les actions décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux objets pour lesquels vous gérez des formulaires personnalisés</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de contribution ou supérieures aux objets pour lesquels vous gérez des formulaires personnalisés</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

* L’équipe d’administration Workfront ou l’utilisateur ou utilisatrice Plan ayant accès à des formulaires personnalisés doit créer des formulaires personnalisés dans votre environnement. Pour plus d’informations, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Vous devez avoir des formulaires personnalisés joints à un objet.

  Pour plus d’informations sur l’application de formulaires personnalisés à un objet, voir [Ajouter un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Réorganiser plusieurs formulaires personnalisés associés à un objet {#reorder-multiple-custom-forms-attached-to-an-object}

1. Accédez à l’objet dans lequel vous souhaitez modifier l’ordre des formulaires personnalisés ajoutés, puis commencez à modifier l’objet.

   **Exemple :** par exemple, pour gérer les formulaires personnalisés d’un projet, accédez au projet, cliquez sur le menu **Plus** ![](assets/more-icon.png), puis cliquez sur **Modifier**.

1. Dans la section **Formulaires personnalisés** pour les projets, les tâches et les problèmes, cliquez sur l’icône ![](assets/move-icon---dots.png) en regard du nom d’un formulaire personnalisé. Pour tous les autres objets, cliquez sur **Gérer les Formulaires**. Cette option s’affiche uniquement si au moins un formulaire personnalisé est associé à l’objet.
1. Faites glisser un formulaire ![](assets/move-icon---dots.png) à un nouvel emplacement dans la liste.
1. Pour les projets, tâches et problèmes de formulaires personnalisés, cliquez sur **Enregistrer**.

   Pour tous les autres objets, cliquez sur **J’ai fini de gérer** > **Enregistrer les modifications**.

## Supprimer un formulaire personnalisé d’un objet {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Lorsque vous supprimez un formulaire personnalisé d’un objet, toutes les informations saisies dans les champs personnalisés du formulaire sont perdues et ne peuvent pas être récupérées.

1. Accédez à l’objet dans lequel vous souhaitez supprimer le formulaire personnalisé et commencez à modifier l’objet.

   Par exemple, accédez à un projet, cliquez sur le menu **Plus** ![](assets/more-icon.png), puis cliquez sur **Modifier**.

1. Cliquez sur **Formulaires personnalisés**.
1. Pour les projets, tâches et problèmes de formulaires personnalisés, cliquez sur l’icône **X** à droite d’un formulaire pour le supprimer de l’objet.

   Pour tous les autres objets, cliquez sur **Gérer les formulaires**, puis cliquez sur le bouton **X** à droite d’un formulaire pour le supprimer de l’objet.

1. Cliquer sur **Enregistrer**.

## Gérer plusieurs formulaires personnalisés contenant les mêmes champs personnalisés

Il se peut que le même champ s’affiche sur plusieurs formulaires personnalisés associés au même objet. Dans ce cas, tenez compte des points suivants :

* La valeur du champ est identique dans tous les formulaires.

  Vous ne pouvez pas avoir de valeurs différentes pour les mêmes champs sur différents formulaires attachés au même objet.

* Si vous disposez des mêmes champs calculés sur deux objets différents, leurs calculs doivent être identiques pour éviter toute erreur. Pour plus d’informations sur l’ajout de champs calculés à des formulaires personnalisés, y compris plusieurs formulaires, voir [Ajout de champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Gérer plusieurs formulaires personnalisés lors de la modification en masse d’objets

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>La gestion des formulaires personnalisés en objets est identique pour tous les objets, à l’exception des projets.
>
>Pour plus d’informations sur l’ajout en masse de formulaires personnalisés à des projets, reportez-vous à l’article [Modifier des projets](../../manage-work/projects/manage-projects/edit-projects.md).

Lorsque vous modifiez en masse des objets auxquels plusieurs formulaires personnalisés sont appliqués, vous pouvez modifier la façon dont les formulaires personnalisés s’affichent sur ces objets, ainsi que modifier les champs communs aux formulaires personnalisés.

Seuls les formulaires personnalisés joints à tous les objets sélectionnés peuvent être modifiés en masse.

Pour modifier plusieurs formulaires personnalisés lors de la modification d’objets en masse :

1. Dans une liste d’objets, sélectionnez les objets auxquels les formulaires personnalisés sont joints, puis cliquez sur l’icône **Modifier** ![](assets/edit-icon.png).
1. Cliquez sur **Formulaires personnalisés**.

   Vous ne pouvez modifier que les formulaires personnalisés joints à tous les objets sélectionnés.

   Les formulaires personnalisés joints uniquement à certains objets ne s’affichent pas.

1. Commencez à modifier les champs des formulaires personnalisés.

   Lorsque des champs sont modifiés, un indicateur visuel s’affiche sur le champ, indiquant que le champ a été modifié.

   Si un champ est inclus dans plusieurs formulaires personnalisés, toutes les valeurs de ces champs sont mises à jour dans chaque formulaire lorsque vous mettez à jour le champ sur l’un des formulaires.

1. Cliquez sur le menu déroulant **Effectuer une sélection** et sélectionnez des formulaires supplémentaires à ajouter à tous les objets sélectionnés.

   Tenez compte des points suivants lors de l’application de formulaires supplémentaires :

   * Les objets peuvent comporter jusqu’à dix formulaires personnalisés.
   * Vous pouvez appliquer des formulaires uniquement lorsque le formulaire n’est pas déjà appliqué à l’un des objets que vous modifiez. Un formulaire déjà joint à l’un des objets n’apparaît pas dans le menu déroulant.
   * Une fois que vous avez appliqué un formulaire supplémentaire, tous les champs que le formulaire a en commun avec d’autres formulaires s’affichent dans la variable **Champs communs** et ils peuvent être modifiés.

1. (Facultatif) Si vous avez ajouté des formulaires personnalisés à tous les objets, mais que vous n’avez pas encore enregistré les objets, vous pouvez modifier l’ordre dans lequel les formulaires personnalisés apparaissent sur les objets.

   Pour plus d’informations sur la modification de l’ordre des formulaires, consultez [Réorganiser plusieurs formulaires personnalisés joints à un objet](#reorder-multiple-custom-forms-attached-to-an-object) dans cet article.

1. Cliquez sur **Supprimer le formulaire** pour supprimer un formulaire personnalisé des objets.

   Pour plus d’informations sur la suppression de formulaires personnalisés d’objets, consultez [Supprimer un formulaire personnalisé d’un objet](#remove-a-custom-form-from-an-object).

   Tenez compte des points suivants lors de la suppression de formulaires en masse de plusieurs objets :

   * Si vous avez apporté des modifications au formulaire, la suppression entraîne la perte de vos modifications et leur récupération est impossible.
   * Une fois que vous avez supprimé un formulaire, tous les champs de ce formulaire qui se trouvaient dans la section **Champs communs** sont supprimés de cette section et ne peuvent plus être modifiés ici.

1. Cliquez sur **Restaurer le formulaire** pour rétablir l’état dans lequel se trouvait le formulaire avant la modification des objets.
1. (Facultatif) Cliquez sur la flèche de réduction située en regard du nom du formulaire pour réduire un formulaire à la fois.

   Ou

   Cliquez sur **Réduire les formulaires** pour réduire tous les formulaires en même temps.

1. (Facultatif) Cliquez sur la flèche de développement située en regard du nom du formulaire pour développer un formulaire à la fois.

   Ou

   Cliquez sur **Développer les formulaires** pour développer tous les formulaires simultanément. 

1. Cliquez sur **Enregistrer les modifications**.
