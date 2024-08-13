---
title: Personnalisation des en-têtes d’objet à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En tant qu’administrateur Adobe Workfront ou administrateur de groupe , vous pouvez utiliser un modèle de mise en page pour configurer les champs que les utilisateurs voient dans l’en-tête de l’objet lorsqu’ils ouvrent la page d’un objet.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 27%

---

# Personnaliser les en-têtes d’objet avec un modèle de disposition

En tant qu’administrateur Adobe Workfront ou administrateur de groupe, vous pouvez utiliser un modèle de mise en page pour configurer les champs que les utilisateurs voient dans l’en-tête de l’objet lorsqu’ils ouvrent la page d’un objet.

>[!IMPORTANT]
>
>La personnalisation des en-têtes d’objet est actuellement disponible pour les projets, les tâches et les problèmes.

![](assets/object-header-fields.png)

Pour plus d’informations sur la création de modèles de disposition, voir [Créer et gérer des modèles de disposition](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de disposition pour les groupes, voir [Créer et modifier des modèles de disposition d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de disposition, vous devez l’attribuer à des utilisateurs et utilisatricess pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de disposition à des utilisateurs et utilisatrices, voir [Attribuer un modèle de disposition à des utilisateurs et utilisatrices](../use-layout-templates/assign-users-to-layout-template.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :


<table>
  <tr>
   <td><strong>Formule Adobe Workfront</strong>
   </td>
   <td>N’importe quelle
   </td>
  </tr>
  <tr>
   <td><strong>Licence Adobe Workfront</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong> Configurations de niveau d’accès</strong>
   </td>
   <td>Vous devez être un administrateur Workfront ou un administrateur de groupe.
<p>
   </td>
  </tr>
</table>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir [Créer ou modifier les niveaux d’accès personnalisés](../../add-users/configure-and-grant-access/create-modify-access-levels.md).

+++

## Personnalisation des en-têtes d’objet

1. Commencez à travailler sur un modèle de disposition, comme décrit dans la section [Créer et gérer des modèles de disposition](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Dans le menu déroulant **Personnaliser ce que les utilisateurs voient**, sélectionnez **Projets**, **Tâches** ou **Problèmes**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. Dans la section [!UICONTROL Champs d’en-tête] , placez le pointeur de la souris sur les champs affichés et effectuez l’une des opérations suivantes :
   * Cliquez sur l’icône **x** pour supprimer un champ.

     Ou

   * Cliquez sur l’icône **grab** et maintenez-la enfoncée pour faire glisser le champ vers un nouvel emplacement.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. L’en-tête d’un objet peut contenir jusqu’à cinq champs.
Si cinq champs sont déjà sélectionnés, vous devez en supprimer un avant d’en ajouter un nouveau.
1. Dans la zone **Ajouter un champ**, commencez à saisir le nom d’un champ Workfront non modifiable que vous souhaitez ajouter, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Le champ est ajouté à droite de la zone Ajouter un champ et s’affiche comme premier champ dans le coin supérieur gauche de l’en-tête de l’objet.

   >[!TIP]
   >
   >* Vous pouvez uniquement ajouter des champs qui s’affichent dans la zone Aperçu de la section Détails de l’objet et qui ne sont pas modifiables. Les champs non modifiables sont des champs que les utilisateurs ne peuvent pas modifier manuellement. Elles sont automatiquement calculées par Workfront.
   >
   >* Vous pouvez ajouter des champs modifiables qui font déjà partie des en-têtes par défaut (par exemple, Propriétaire du projet, État, Pourcentage terminé, Affectations).
   >
   >* Lorsque vous ajoutez le champ &quot;Résolu par&quot; à l’en-tête d’un problème, le champ devient &quot;Résoudre un problème, une tâche ou un projet&quot;, lorsqu’un objet de résolution est associé au problème.


   ![](assets/add-field-to-header-in-lt-list.png)


1. (Facultatif) Faites glisser et déposez les champs ajoutés dans un autre ordre.

1. Poursuivez la personnalisation du modèle de disposition.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Vous pouvez cliquer à tout moment sur Enregistrer pour enregistrer votre progression, puis continuer à modifier le modèle ultérieurement.
