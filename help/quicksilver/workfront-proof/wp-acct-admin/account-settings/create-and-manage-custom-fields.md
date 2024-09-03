---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Création et gérer des champs personnalisés dans [!DNL Workfront Proof]
description: Un plan  [!DNL Workfront]  Select ou Premium est requis pour utiliser cette fonctionnalité. Pour plus d’informations sur les différentes formules disponibles, voir Formules Workfront.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: 6e6cc1db8f89b76d9903905e6ee4cf9014727ba1
workflow-type: tm+mt
source-wordcount: '1040'
ht-degree: 100%

---

# Créer et gérer des champs personnalisés dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence aux fonctionnalités du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Un plan [!DNL Workfront] Select ou Premium est requis pour utiliser cette fonctionnalité. Pour plus d’informations sur les différents plans disponibles, voir [Plans Workfront](https://www.workfront.com/plans?lang=fr).

Les champs personnalisés vous permettent de capturer des données supplémentaires lors de la création d’une épreuve, d’un utilisateur ou utilisatrice ou d’une personne invitée.

Par exemple, les utilisateurs et utilisatrices qui créent une épreuve peuvent inclure une section supplémentaire qui leur permettra de capturer un numéro de traitement, un code de service ou une référence du fournisseur.

>[!NOTE]
>
>* La capture de ce type d&#39;informations sur la page Nouvelle épreuve via des champs personnalisés vous permet également de réduire la longueur de votre nom d’épreuve, car ces détails n’auront pas à être inclus dans le nom. Pour plus d’informations sur la page Nouvelle épreuve, voir « Créer des épreuves dans [!DNL Workfront Proof] ».
>
>Une fois qu’un champ personnalisé a été utilisé sur une épreuve, une personne ou un contact, vous ne pourrez plus le supprimer ni modifier le type de champ. Vous pourrez toutefois le masquer (via l’option [!UICONTROL Paramètres des champs personnalisés]) afin qu’il ne soit pas utilisé pour les nouveaux éléments.
>
>Si vous masquez une section de champ personnalisé , tous les champs de la section seront également masqués même si les champs individuels sont définis comme visibles.

Cet article explique comment effectuer les opérations suivantes :

## Créer des champs personnalisés

Tout d’abord, vous devez configurer la section Champ personnalisé à laquelle vous allez ajouter des champs personnalisés.

1. Cliquez sur **[!UICONTROL Paramètres]** >**[!UICONTROL Paramètres du compte]**, puis ouvrez l’onglet **[!UICONTROL Champs personnalisés]**.

1. Cliquez sur **[!UICONTROL Ajouter une section de champ personnalisé]** dans le module correspondant (Épreuve, Personnes ou Contacts).
1. Saisissez un **Nom** pour la section de champ personnalisé, puis cliquez sur **[!UICONTROL Enregistrer]**.

   Vous pouvez maintenant configurer des champs personnalisés dans la section :

1. Cliquez sur l’onglet **[!UICONTROL Paramètres des champs personnalisés]** pour actualiser la page.
1. Cliquez sur le nom de votre nouvelle section de champ personnalisé pour ouvrir la section **[!UICONTROL Champ personnalisé] de la page** pour la nouvelle section.
1. Cliquez sur le **[!UICONTROL Nouveau champ personnalisé]** près du coin supérieur droit.
1. Dans la page **[!UICONTROL Nouveau champ personnalisé]** qui s’affiche, spécifiez les détails du champ personnalisé :

   | **Obligatoire** | Workfront exige que les utilisateurs et urilisatrices remplissent le champ. |
   |---|---|
   | **Recherche** | Permet aux personnes de trouver des éléments en effectuant une recherche sur les données de champ personnalisé. |
   | **Masqué** | Masque le champ personnalisé sur les pages [!UICONTROL Nouvelle épreuve], Nouvelle personne invitée et [!UICONTROL Nouvel utilisateur ou utilisatrice]. |

   {style="table-layout:auto"}

1. Cliquer sur **[!UICONTROL Enregistrer]**.
1. Dans la page **Champ personnalisé** qui s’affiche, cliquez sur **[!UICONTROL Paramètres des champs personnalisés]** pour actualiser la page.

1. Apportez d’autres modifications aux paramètres du champ :

   * Pour masquer ou afficher la section de champ personnalisé, cliquez sur le menu **[!UICONTROL Plus]** (trois points) à droite du nom de la section de champ personnalisé, puis sur **[!UICONTROL Masquer la section]** ou **[!UICONTROL Afficher la section]**.

   * Pour masquer ou afficher le champ personnalisé, cliquez sur le menu **[!UICONTROL Plus]** (trois points) à droite du nom de la section de champ personnalisé, puis sur **[!UICONTROL Masquer le champ personnalisé]** ou **[!UICONTROL Afficher le champ personnalisé]**.

   * Modifiez l’ordre des champs à l’aide des flèches haut/bas qui s’affichent à droite de leur nom (si vous avez ajouté plusieurs champs dans une section).

1. Ouvrez l’onglet **[!UICONTROL Règles de visibilité]**.\
   Les règles de visibilité vous permettent de déterminer les champs supplémentaires qui s’affichent en fonction de la fin du champ personnalisé initial. Par exemple, si le champ dépendant est A et que le champ de contrôle est X, cela signifie que le champ A ne sera visible que si le champ X est renseigné.

   Vous pouvez utiliser des valeurs de contrôle pour déterminer les valeurs du champ de contrôle qui, si elles sont sélectionnées, rendront le champ dépendant visible. Par exemple, imaginez que le champ dépendant est A et que le champ de contrôle est X et que vous définissez les valeurs de contrôle dans X sur les options 1 et 2 uniquement. Cela signifie que le champ A ne sera visible que si l’option 1 ou 2 du champ X est sélectionnée. Cela signifie que si les options 3 ou 4 du champ X sont sélectionnées, le champ A ne s’affiche pas. Ouvrez l’onglet **[!UICONTROL Règles de visibilité]**.

   >[!NOTE]
   >
   >Seuls les types de champs personnalisés Liste et Cases d’option peuvent être utilisés pour le champ de contrôle dans une règle de visibilité, tandis que le champ dépendant peut être n’importe quel type de champ.

   Pour ajouter une règle de visibilité, procédez comme suit :

   1. Cliquez sur **[!UICONTROL Nouvelle règle de visibilité]** pour le module dans lequel vous souhaitez ajouter la règle.
   1. Sélectionnez les paramètres de la règle, puis cliquez sur **[!UICONTROL Enregistrer]**.

1. Ouvrez l’onglet **[!UICONTROL Règles de dépendance]**.

   Les règles de dépendance vous permettent de déterminer les options disponibles dans le champ dépendant lorsque certaines options sont sélectionnées dans le champ de contrôle. Par exemple, si le champ dépendant est « B » et que le champ de contrôle est « Y », vous pouvez le configurer comme suit :

   Si l’option 1 du champ Y est sélectionnée, seules les options 1 et 2 du champ B s’affichent.

   Si l’option 2 du champ Y est sélectionnée, seules les options 3 et 4 du champ B s’affichent.

   >[!NOTE]
   >
   >Seuls les types de champs personnalisés Liste et Radio peuvent être utilisés pour les champs dépendants et de contrôle dans une règle de dépendance.

   Pour ajouter une règle de dépendance, procédez comme suit :

   1. Cliquez sur **[!UICONTROL Nouvelle règle de dépendance]** pour le module auquel vous souhaitez ajouter la règle.
   1. Sélectionnez les paramètres de la dépendance, puis cliquez sur **[!UICONTROL Enregistrer]**.

## Gérer les champs personnalisés

Vous pouvez afficher et modifier les détails de votre section de champ personnalisé ou de champs personnalisés spécifiques.

1. Cliquez sur **[!UICONTROL Paramètres]** >**[!UICONTROL Paramètres du compte]**, puis ouvrez l’onglet **[!UICONTROL Champs personnalisés]**.

1. Cliquez sur le nom de la section de champ personnalisé ou du champ personnalisé spécifique.
1. (Le cas échéant) Si vous gérez une section de champ personnalisé, apportez l’une des modifications suivantes sur la page **[!UICONTROL Section de champ personnalisé]** :

   * Modifiez le nom de la section.
   * Déplacez-la vers un autre module.
   * Masquez/affichez la section.

1. (Le cas échéant) Si vous gérez un champ personnalisé, apportez l’une des modifications suivantes sur la page **[!UICONTROL Champ personnalisé]** :

   * Déplacez le champ vers une autre section.
   * Modifiez le nom du champ.
   * Texte d’aide de saisie (une icône de point d’interrogation s’affiche en regard de la section du champ et le texte s’affiche lorsque vous pointez dessus).
   * Activez/désactivez le paramètre **[!UICONTROL Obligatoire]** du champ.
   * Activez/désactivez le paramètre **[!UICONTROL Consultable]** du champ.
   * Masquez/affichez le champ.
   * Modifiez le type de champ.
   * Définissez/modifiez une valeur par défaut pour le champ.
   * Configurez les règles de visibilité et de dépendance (comme décrit ci-dessus aux étapes 11 et 12).
