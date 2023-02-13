---
title: Transfert de données de formulaire personnalisées lors de la conversion d’un objet
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Lorsque la tâche définie dans une tâche devient trop volumineuse, vous pouvez la convertir en tâche plus volumineuse.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Transfert de données de formulaire personnalisées lors de la conversion d’un objet

Selon les besoins de votre entreprise, le travail défini dans une tâche ou un problème peut devenir trop volumineux pour être géré dans la tâche ou le problème. Dans ce cas, vous pouvez les convertir en élément de travail plus volumineux :

* Vous pouvez convertir des problèmes en tâches ou en projets.
* Vous pouvez convertir des tâches en projets.

Pour transférer des données de formulaire personnalisées d’un problème vers une tâche ou un projet, vous devez effectuer les deux tâches de cet article, dans l’ordre ci-dessous.

Pour plus d’informations, voir [Présentation des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) ou [Présentation des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> <p>Pour plus d’informations sur la manière dont les administrateurs de Workfront accordent cet accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur Workfront.

## Premier : Copier le formulaire personnalisé {#first-copy-the-custom-form}

Tout d’abord, vous devez vous assurer de conserver toutes les données de formulaire personnalisées pour une tâche ou un problème que vous souhaitez convertir. Comme les données de formulaire personnalisées doivent correspondre exactement à l’élément converti, il est recommandé de dupliquer le formulaire pour le joindre au nouvel objet.

>[!TIP]
>
>Dans ce cas, une autre méthode consiste à ajouter le type d’objet le plus grand au formulaire personnalisé. Pour obtenir des instructions, reportez-vous à la section [Commencer à modifier un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) dans l’article [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Forms personnalisée**.
1. Sélectionnez le formulaire personnalisé de type tâche ou problème, puis cliquez sur **Copier**.
1. Dans le **Formulaire personnalisé** , indiquez le nom du nouveau formulaire.

1. Dans la **Type de formulaire** , sélectionnez le type d’objet pour lequel vous souhaitez créer un formulaire personnalisé.

   **Exemple :** Si vous souhaitez transférer les données de formulaire personnalisées vers un projet, sélectionnez Projet.

1. Cliquez sur **Copier le formulaire**.

   Ce formulaire personnalisé copié peut désormais être joint à une tâche ou à un projet.

1. Passez à la [Deuxièmement : Convertir le problème ou la tâche et transférer les données de formulaire personnalisées](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Deuxièmement : Convertir le problème ou la tâche et transférer les données de formulaire personnalisées {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Copiez le formulaire personnalisé sur le problème ou la tâche que vous convertissez, comme expliqué dans la section . [Premier : Copier le formulaire personnalisé](#first-copy-the-custom-form) dans cet article.
1. Convertissez le problème ou la tâche à l’aide de la fonction **Forms personnalisée** dans la zone qui s’affiche pour sélectionner le formulaire personnalisé que vous avez copié. Pour obtenir des instructions, reportez-vous aux articles suivants :

   * [Convertir un problème en projet dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Convertir un problème en tâche dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Convertir une tâche en projet](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. Dans le **Convertir en (type d’objet)** , cliquez sur la boîte de dialogue qui s’affiche. **Ajouter Forms** et sélectionnez le formulaire que vous avez copié dans la section précédente.

   Les informations capturées dans les champs personnalisés du problème sont maintenant transférées vers le formulaire personnalisé sur la tâche.

