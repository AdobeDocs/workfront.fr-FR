---
title: Personnalisation des en-têtes d’objet à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En tant qu’administrateur ou administratrice Adobe Workfront ou de groupes, vous pouvez utiliser un modèle de mise en page pour configurer les champs que les personnes voient dans l’en-tête de l’objet lorsqu’elles ouvrent la page de l’objet.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 96%

---

# Personnaliser les en-têtes d’objet avec un modèle de disposition

En tant qu’administrateur ou administratrice Adobe Workfront ou de groupes, vous pouvez utiliser un modèle de mise en page pour configurer les champs que les personnes voient dans l’en-tête de l’objet lorsqu’elles ouvrent la page d’un objet.

>[!IMPORTANT]
>
>La personnalisation des en-têtes d’objets est actuellement disponible pour les projets, les tâches et les problèmes.

![Champs d’en-tête d’objet](assets/object-header-fields.png)

Pour plus d’informations sur la création de modèles de disposition, voir [Créer et gérer des modèles de disposition](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de disposition pour les groupes, voir [Créer et modifier des modèles de disposition d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de mise en page, vous devez l’affecter aux utilisateurs et utilisatrices pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de disposition aux utilisateurs et utilisatrices, voir [Affecter des utilisateurs et utilisatrices à un modèle de disposition](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td><p>Nouveau : Standard</p>
  <p> Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.
Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personnaliser les en-têtes d’objets

1. Commencez à travailler sur un modèle de disposition, comme décrit dans la section [Créer et gérer des modèles de disposition](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Dans le menu déroulant **Personnaliser ce que les personnes voient**, sélectionnez **Projets**, **Tâches** ou **Problèmes**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. Dans la section [!UICONTROL Champs d’en-tête], pointez sur les champs affichés et effectuez l’une des opérations suivantes :
   * Cliquez sur l’icône **x** pour supprimer un champ.

     Ou

   * Cliquez sur l’icône **main** et maintenez-la enfoncée pour faire glisser et déposer le champ à un nouvel emplacement.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![Les champs d’en-tête d’objet masquent et déplacent les icônes](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. L’en-tête d’un objet peut comporter jusqu’à cinq champs.
Si vous avez déjà sélectionné cinq champs, vous devez supprimer un champ avant d’en ajouter un nouveau.
1. Dans la case **Ajouter un champ**, commencez à saisir le nom d’un champ Workfront non modifiable que vous souhaitez ajouter, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Le champ est ajouté immédiatement à droite de la zone Ajouter un champ et s’affiche comme le premier champ dans le coin supérieur gauche de l’en-tête de l’objet.

   >[!TIP]
   >
   >* Vous ne pouvez ajouter que des champs qui s’affichent dans la zone Vue d’ensemble de la section Détails de l’objet et qui ne sont pas modifiables. Les champs non modifiables sont des champs que les personnes ne peuvent pas modifier manuellement. Ils sont calculés automatiquement par Workfront.
   >
   >* Vous pouvez ajouter des champs modifiables qui font déjà partie des en-têtes par défaut (par exemple, Personne propriétaire du projet, Statut, Pourcentage terminé, Affectations).
   >
   >* Lorsque vous ajoutez le champ « Résolu par » à l’en-tête d’un problème, le champ devient « Résolution du problème, de la tâche ou du projet », lorsqu’un objet de résolution est associé au problème.


   ![Ajouter un champ à l’en-tête](assets/add-field-to-header-in-lt-list.png)


1. (Facultatif) Faites glisser et déposez les champs ajoutés dans un ordre différent.

1. Poursuivez la personnalisation du modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Vous pouvez cliquer à tout moment sur Enregistrer pour enregistrer votre progression, puis continuer à modifier le modèle ultérieurement.
