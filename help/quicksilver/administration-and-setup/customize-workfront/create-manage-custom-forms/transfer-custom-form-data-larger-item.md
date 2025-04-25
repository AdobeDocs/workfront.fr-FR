---
title: Transfert de données de formulaire personnalisé lors de la conversion d’un objet
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Lorsque le travail défini dans un élément de travail devient trop volumineux, vous pouvez le convertir en élément de travail plus volumineux.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 98%

---

# Transférer des données de formulaire personnalisé lors de la conversion d’un objet

Selon les besoins de votre entreprise, le travail défini dans une tâche ou un problème peut devenir trop volumineux pour être géré dans la tâche ou le problème. Dans ce cas, vous pouvez convertir l’élément en un élément de travail plus volumineux :

* Vous pouvez convertir des problèmes en tâches ou en projets.
* Vous pouvez convertir des tâches en projets.

Pour transférer des données de formulaire personnalisé d’un problème vers une tâche ou un projet, vous devez effectuer les deux tâches de cet article, dans l’ordre ci-dessous.

Pour plus d’informations, voir [Vue d’ensemble des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) ou [Vue d’ensemble des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Premièrement : ajouter des objets supplémentaires au formulaire personnalisé

{{step-1-to-setup}}

1. Cliquez sur **Formulaires personnalisés**.
1. Recherchez le formulaire dont vous avez besoin, puis cliquez sur l’![icône Modifier](assets/edit-icon.png).
1. Dans la partie supérieure du formulaire, ajoutez l’objet dans lequel vous envisagez de convertir la tâche ou le problème.

   >[!INFO]
   >
   >**Exemple** : si vous souhaitez transférer les données de formulaire personnalisé vers un projet, sélectionnez Projet.

1. Cliquez sur **Appliquer** au bas du formulaire.

1. Passez à [Deuxièmement : convertir le problème ou la tâche et transférer les données du formulaire personnalisé](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Deuxièmement : convertir le problème ou la tâche et transférer les données du formulaire personnalisé {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Ajoutez des objets supplémentaires au formulaire personnalisé sur le problème ou la tâche que vous convertissez, comme expliqué dans la section [Premièrement : ajouter des objets supplémentaires au formulaire personnalisé](#first-add-additonal-objects-to-the-custom-form) dans cet article.
1. Convertissez le problème ou la tâche à l’aide de l’option **Formulaires personnalisés** dans la zone qui s’affiche pour sélectionner le formulaire personnalisé dont vous avez besoin. Pour obtenir des instructions, reportez-vous aux articles suivants :

   * [Convertir un problème en projet dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Convertir un problème en tâche dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Convertir une tâche en projet](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. Dans la boîte de dialogue **Convertir en (type d’objet)** qui s’affiche, cliquez sur le menu déroulant **Ajouter des formulaires** et sélectionnez le formulaire que vous avez copié dans la section précédente.

   Les informations capturées dans les champs personnalisés du problème sont maintenant transférées vers le formulaire personnalisé sur la tâche.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->
