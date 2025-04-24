---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Création et gérer des champs personnalisés dans [!DNL Workfront Proof]
description: Un plan  [!DNL Workfront]  Select ou Premium est requis pour utiliser cette fonctionnalité. Pour plus d’informations sur les différentes formules disponibles, voir Formules Workfront.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 50%

---

# Créer et gérer des champs personnalisés dans [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Un plan [!DNL Workfront] Select ou Premium est requis pour utiliser cette fonctionnalité. Pour plus d’informations sur les différents plans disponibles, voir [Plans Workfront](https://www.workfront.com/plans?lang=fr).

Les champs personnalisés vous permettent de capturer des données supplémentaires lors de la création d’une nouvelle épreuve, d’un nouvel utilisateur ou d’un nouvel invité. Par exemple, les utilisateurs et utilisatrices qui créent une épreuve peuvent inclure une section supplémentaire qui leur permettra de capturer un numéro de traitement, un code de service ou une référence du fournisseur.

>[!NOTE]
>
>* La capture de ce type d’informations sur la page Nouvelle épreuve via des champs personnalisés vous permet également de réduire la longueur du nom de votre épreuve, car ces détails n’auront pas à être inclus dans le nom.
>
>* Une fois qu’un champ personnalisé a été utilisé pour une épreuve, un utilisateur ou un contact, vous ne pouvez plus le supprimer ni modifier le type de champ. Cependant, vous pourrez le masquer via la page Paramètres des champs personnalisés afin qu’il ne soit pas utilisé pour de nouveaux éléments.
>
>* Si vous masquez une section de champ personnalisé, tous les champs de la section sont également masqués, même si les champs individuels sont définis comme visibles.

## Créer des champs personnalisés

{{step1-to-proofing}}

1. Dans le coin supérieur droit de la page, cliquez sur **Paramètres du compte**.

1. Sur la page **Paramètres du compte** sélectionnez l’onglet **Champs personnalisés**.

1. Cliquez sur **[!UICONTROL Ajouter une section de champ personnalisé]** sur le côté droit du module (**Épreuve**, **Utilisateurs** ou **Contacts**) auquel vous souhaitez ajouter le champ personnalisé. L’onglet **Détails de la section** s’ouvre.

1. Saisissez un **Nom** pour la section de champ personnalisé, puis cliquez sur **[!UICONTROL Enregistrer]**.

1. Cliquez sur l’onglet **[!UICONTROL Paramètres des champs personnalisés]** pour actualiser la page. La nouvelle section de champ personnalisé s’affiche sous son module affecté.

   ![Onglet Paramètres des champs personnalisés](assets/custom-field-settings-tab.png)

1. Cliquez sur le nom de votre nouvelle section de champ personnalisé pour ouvrir l’onglet **Section de champs personnalisés**.

1. Dans le coin supérieur droit de la page, cliquez sur le bouton **[!UICONTROL Nouveau champ personnalisé]**. La page **Nouveau champ personnalisé** s’affiche.

1. Spécifiez le **Détails du champ** :

   * **Nom** : saisissez le nom du champ personnalisé.
   * **Aide** : saisissez le texte de l’aide qui s’affichera dans une info-bulle.
   * **Obligatoire** : cochez cette case pour que l’utilisateur ou l’utilisatrice remplisse le champ.
   * **Recherchable** (conditionnel) : cochez cette case pour que le champ personnalisé puisse faire l’objet d’une recherche.
   * **Masqué** : cochez cette case pour masquer le champ personnalisé sur les pages **Nouvelle épreuve**, **Nouvel invité** et **Nouvel utilisateur**.

1. Spécifiez le **Type de champ** ainsi que les détails :

   * **Type** : sélectionnez le type de champ personnalisé.
   * **Éléments de liste** : (conditionnel) ajoutez les éléments de liste qui apparaîtront dans le champ personnalisé.
   * **Valeur par défaut** : sélectionnez la valeur par défaut de ce champ personnalisé. Cette option varie en fonction du type de champ personnalisé sélectionné.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

1. Apportez d’autres modifications aux paramètres du champ :

   * Masquez ou affichez la section de champ personnalisé en cliquant sur le menu **Plus** ![Plus](assets/more-button-small.png) à droite du nom de la section de champ personnalisé, puis en cliquant sur **[!UICONTROL Masquer la section]** ou **[!UICONTROL Afficher la section]**.
   * Masquez ou affichez le champ personnalisé en cliquant sur le menu **Plus** ![Plus](assets/more-button-small.png) à droite du nom de la section des champs personnalisés, puis en cliquant sur **[!UICONTROL Masquer le champ personnalisé]** ou **[!UICONTROL Afficher le champ personnalisé]**.
   * Modifiez l’ordre des champs à l’aide des flèches haut/bas qui s’affichent à droite de leur nom (si vous avez ajouté plusieurs champs dans une section).

1. Cliquez sur l’onglet **[!UICONTROL Règles de visibilité]**.

   Les règles de visibilité vous permettent de dicter quels champs supplémentaires sont affichés en fonction de l’achèvement du champ personnalisé initial. Par exemple, si le champ dépendant est A et que le champ de contrôle est X, cela signifie que le champ A ne sera visible que si le champ X est renseigné.

   Vous pouvez utiliser des valeurs de contrôle pour déterminer les valeurs du champ de contrôle qui, si elles sont sélectionnées, rendront le champ dépendant visible. Par exemple, imaginez que le champ dépendant est A et que le champ de contrôle est X et que vous définissez les valeurs de contrôle dans X sur les options 1 et 2 uniquement. Cela signifie que le champ A ne sera visible que si l’option 1 ou 2 du champ X est sélectionnée. En outre, si les options 3 ou 4 du champ X sont sélectionnées, le champ A ne s’affiche pas.

   >[!NOTE]
   >
   >Seuls les types de champs personnalisés Liste et Cases d’option peuvent être utilisés pour le champ de contrôle dans une règle de visibilité, tandis que le champ dépendant peut être n’importe quel type de champ.

   Pour ajouter une règle de visibilité, procédez comme suit :

   1. Cliquez sur **[!UICONTROL Nouvelle règle de visibilité]** pour le module auquel vous souhaitez ajouter la règle.

   1. Sélectionnez les paramètres de la règle, puis cliquez sur **[!UICONTROL Enregistrer]**.

1. Ouvrez l’onglet **[!UICONTROL Règles de dépendance]**.

   Les règles de dépendance vous permettent de déterminer les options disponibles dans le champ dépendant lorsque certaines options sont sélectionnées dans le champ de contrôle. Par exemple, si le champ dépendant est « B » et que le champ de contrôle est « Y », vous pouvez le configurer comme suit :

   * Si l’option 1 du champ Y est sélectionnée, seules les options 1 et 2 du champ B s’affichent.

   * Si l’option 2 du champ Y est sélectionnée, seules les options 3 et 4 du champ B s’affichent.

   >[!NOTE]
   >
   >Seuls les types de champs personnalisés Liste et Radio peuvent être utilisés pour les champs dépendants et de contrôle dans une règle de dépendance.

   Pour ajouter une règle de dépendance, procédez comme suit :

   1. Cliquez sur **[!UICONTROL Nouvelle règle de dépendance]** pour le module auquel vous souhaitez ajouter la règle.

   1. Sélectionnez les paramètres de la dépendance, puis cliquez sur **[!UICONTROL Enregistrer]**.

## Gérer les champs personnalisés

Vous pouvez afficher et modifier les détails de votre section Champ personnalisé ou de vos champs personnalisés individuels.

{{step1-to-proofing}}

1. Dans le coin supérieur droit de la page, cliquez sur **Paramètres du compte**.

1. Sur la page **Paramètres du compte** sélectionnez l’onglet **Champs personnalisés**.

1. Cliquez sur le nom de la section de champ personnalisé ou du champ personnalisé spécifique.

1. (Le cas échéant) Si vous gérez une section de champ personnalisé, apportez l’une des modifications suivantes sur la page **[!UICONTROL Section de champ personnalisé]** :

   * Modifiez le nom de la section.
   * Déplacez-la vers un autre module.
   * Masquez/affichez la section.

1. (Le cas échéant) Si vous gérez un champ personnalisé, apportez l’une des modifications suivantes sur la page **[!UICONTROL Champ personnalisé]** :

   * Déplacez le champ vers une autre section.
   * Modifiez le nom du champ.
   * Modifier le texte d’aide.
   * Activez/désactivez le paramètre **[!UICONTROL Obligatoire]** du champ.
   * (Conditionnel) Activez/désactivez le paramètre **[!UICONTROL pouvant faire l’objet d’une recherche]** dans le champ.
   * Masquez/affichez le champ.
   * Modifiez le type de champ.
   * Définissez/modifiez une valeur par défaut pour le champ.
   * Configurez les règles de visibilité et de dépendance.
