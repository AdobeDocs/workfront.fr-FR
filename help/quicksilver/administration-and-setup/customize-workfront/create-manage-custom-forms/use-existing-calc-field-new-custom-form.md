---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Réutilisation d’un champ personnalisé calculé existant dans un formulaire personnalisé avec l’ancien créateur de formulaires
description: Vous pouvez utiliser le même champ personnalisé calculé sur les formulaires personnalisés appartenant à des objets différents. Par exemple, vous pouvez utiliser le champ calculé de profit que vous avez créé pour le formulaire personnalisé du projet sur un formulaire personnalisé de tâche.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 24482fca-94e4-406d-9d62-3db9f51481e6
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Réutilisation d’un champ personnalisé calculé existant dans un formulaire personnalisé avec l’ancien créateur de formulaires

{{form-designer-default}}

Vous pouvez utiliser le même champ personnalisé calculé sur les formulaires personnalisés appartenant à des objets différents. Par exemple, vous pouvez utiliser le champ calculé de profit que vous avez créé pour le formulaire personnalisé du projet sur un formulaire personnalisé de tâche.

Pour plus d’informations sur l’ajout d’un champ personnalisé calculé à un formulaire personnalisé, voir [Ajout de données calculées à un formulaire personnalisé avec l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Lors de l’utilisation d’un champ personnalisé calculé existant, le calcul n’est pas transféré vers le nouveau formulaire. Vous devez à nouveau ajouter le calcul, sur le même champ, sur le nouveau formulaire personnalisé.

>[!TIP]
>
>C’est le cas lorsque vous utilisez le calcul stocké dans le champ **Instructions** du formulaire personnalisé.

Vous pouvez également avoir un calcul différent pour le même champ, sur le nouveau formulaire. Le fait de conserver le même nom pour le champ personnalisé calculé garantit la cohérence et la cohérence de votre convention d’affectation des noms.

>[!IMPORTANT]
>
>Les champs personnalisés calculés peuvent devenir obsolètes au fil du temps. Pour vérifier que vous affichez toujours les calculs à jour dans ces champs, effectuez l’une des opérations suivantes :
>
>* Après avoir enregistré un objet pour lequel vous avez modifié des données dans un formulaire personnalisé joint, cliquez sur l’icône Plus ![](assets/more-icon.png) sur la page principale de l’objet, puis sur Recalculer les expressions personnalisées.
>* Sélectionnez l’option Recalculer les expressions personnalisées lors de l’édition d’objets en bloc.
>* Sélectionnez l’option Mettre à jour les calculs précédents lorsque vous modifiez un champ personnalisé calculé sur un formulaire personnalisé.
>
