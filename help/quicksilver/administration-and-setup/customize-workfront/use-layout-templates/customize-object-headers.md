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
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 61%

---

# Personnaliser les en-têtes d’objet avec un modèle de mise en page

En tant qu’administrateur ou administratrice Adobe Workfront ou de groupes, vous pouvez utiliser un modèle de mise en page pour configurer les champs que les personnes voient dans l’en-tête de l’objet lorsqu’elles ouvrent la page d’un objet.

>[!IMPORTANT]
>
>La personnalisation des en-têtes d’objets est actuellement disponible pour les projets, les tâches et les problèmes.

![Champs d’en-tête d’objet](assets/object-header-fields.png)

Pour plus d’informations sur la création de modèles de mise en page, voir [Créer et gérer des modèles de mise en page](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de mise en page pour les groupes, voir [Créer et modifier des modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de mise en page, vous devez l’affecter aux utilisateurs et utilisatrices pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de mise en page à des utilisateurs et utilisatrices, voir [Attribuer un modèle de mise en page à des utilisateurs et utilisatrices](../use-layout-templates/assign-users-to-layout-template.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.</p>
        <p>Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personnaliser les en-têtes d’objets

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans la section [Créer et gérer des modèles de mise en page](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Dans le menu déroulant **Personnaliser ce que les personnes voient**, sélectionnez **Projets**, **Tâches** ou **Problèmes**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. Dans la section [!UICONTROL Champs d’en-tête], passez la souris sur les champs actifs et effectuez l’une des opérations suivantes :
   * Cliquez sur l’icône **x** pour supprimer un champ.

     Ou

   * Cliquez sur l’icône **main** et maintenez-la enfoncée pour faire glisser et déposer le champ à un nouvel emplacement.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![Les champs d’en-tête d’objet masquent et déplacent les icônes](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. L’en-tête d’un objet peut comporter jusqu’à cinq champs.
Si vous avez déjà sélectionné cinq champs, vous devez supprimer un champ avant d’en ajouter un nouveau.
1. Dans la zone **Ajouter un champ**, commencez à saisir le nom d’un champ personnalisé ou d’un champ Workfront natif que vous souhaitez ajouter, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Le champ est ajouté à droite immédiate de la zone Ajouter un champ et s’affiche comme le premier champ dans le coin supérieur droit de l’en-tête de l’objet .

   >[!TIP]
   >
   >* Vous pouvez ajouter n’importe quel champ personnalisé ou n’importe quel champ natif disponible dans la zone Aperçu de la section Détails d’un objet. Par exemple, seuls les problèmes comportent le champ Gravité et ce champ n’est pas disponible pour être ajouté aux projets ou aux tâches.
   >
   >* Lorsque l’utilisateur modifie un champ personnalisé dans l’en-tête qui est contenu dans un formulaire personnalisé non joint à l’objet , le formulaire personnalisé est automatiquement ajouté à l’objet .
   >
   >* Lorsque vous ajoutez le champ « Résolu par » à l’en-tête d’un problème, le champ devient « Résolution du problème, de la tâche ou du projet », lorsqu’un objet de résolution est associé au problème.

   ![Ajouter un champ à l’en-tête](assets/add-field-to-header-in-lt-list.png)

1. (Facultatif) Faites glisser et déposez les champs dans un ordre différent.

1. Continuez à personnaliser le modèle de mise en page. Vous pouvez cliquer sur **Appliquer** à tout moment pour enregistrer votre progression.

   Ou

   Si vous avez terminé la personnalisation, cliquez sur **Enregistrer et fermer**.

