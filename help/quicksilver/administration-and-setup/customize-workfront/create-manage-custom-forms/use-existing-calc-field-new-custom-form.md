---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Réutilisation d’un champ personnalisé calculé existant dans un formulaire personnalisé avec l’ancien créateur de formulaires
description: Vous pouvez utiliser le même champ personnalisé calculé sur les formulaires personnalisés appartenant à des objets différents. Par exemple, vous pouvez utiliser le champ calculé de profit que vous avez créé pour le formulaire personnalisé du projet sur un formulaire personnalisé de tâche.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 24482fca-94e4-406d-9d62-3db9f51481e6
source-git-commit: ac5b7e0237dbcaea14010eda658f7d5a6be089cc
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Réutilisation d’un champ personnalisé calculé existant dans un formulaire personnalisé avec l’ancien créateur de formulaires

Vous pouvez utiliser le même champ personnalisé calculé sur les formulaires personnalisés appartenant à des objets différents. Par exemple, vous pouvez utiliser le champ calculé de profit que vous avez créé pour le formulaire personnalisé du projet sur un formulaire personnalisé de tâche.

Pour plus d’informations sur l’ajout d’un champ personnalisé calculé à un formulaire personnalisé, voir [Ajout de données calculées à un formulaire personnalisé à l’aide de l’ancien créateur de formulaires](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Lors de l’utilisation d’un champ personnalisé calculé existant, le calcul n’est pas transféré vers le nouveau formulaire. Vous devez à nouveau ajouter le calcul, sur le même champ, sur le nouveau formulaire personnalisé.

>[!TIP]
>
>Cela se produit lors de l’utilisation du calcul stocké dans la variable **Instructions** du formulaire personnalisé.

Vous pouvez également avoir un calcul différent pour le même champ, sur le nouveau formulaire. Le fait de conserver le même nom pour le champ personnalisé calculé garantit la cohérence et la cohérence de votre convention d’affectation des noms.

>[!IMPORTANT]
>
>Les champs personnalisés calculés peuvent devenir obsolètes au fil du temps. Pour vérifier que vous affichez toujours les calculs à jour dans ces champs, effectuez l’une des opérations suivantes :
>
>* Après avoir enregistré un objet pour lequel vous avez modifié des données dans un formulaire personnalisé joint, cliquez sur l’icône Plus ![](assets/more-icon.png) sur la page principale de l’objet, puis Recalculer les expressions personnalisées.
>* Sélectionnez l’option Recalculer les expressions personnalisées lors de l’édition d’objets en bloc.
>* Sélectionnez l’option Mettre à jour les calculs précédents lors de la modification d’un champ personnalisé calculé sur un formulaire personnalisé.
>

