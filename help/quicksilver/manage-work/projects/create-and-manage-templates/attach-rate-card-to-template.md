---
content-type: overview
product-area: templates
navigation-topic: financials
title: Joindre une carte tarifaire à un modèle
description: Lorsque vous affectez une carte tarifaire à un modèle, celle-ci est ensuite associée à tous les projets créés à partir du modèle.
author: Lisa
feature: Work Management
source-git-commit: ace9a01e852e6d99ddc6f150c0ac34bd4ef44817
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 10%

---

# Joindre une carte tarifaire à un modèle

Lorsque vous affectez une carte tarifaire à un modèle, celle-ci est ensuite associée à tous les projets créés à partir du modèle. La carte tarifaire devient la carte par défaut du projet, mais elle peut être remplacée si nécessaire.

Pour plus d’informations sur les cartes tarifaires, voir [&#x200B; Gérer les cartes tarifaires &#x200B;](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Pour plus d’informations sur les modèles de projet, voir [Présentation des modèles de projet](/help/quicksilver/manage-work/projects/create-and-manage-templates/project-template-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Modifier l’accès aux modèles</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Gérez les autorisations de la carte tarifaire avec les autorisations de Modifier les taux de facturation</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

La carte tarifaire que vous souhaitez affecter au modèle doit être créée dans Workfront. Pour plus d’informations, voir [Gérer les cartes tarifaires](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Le champ **Carte tarifaire** doit être activé pour les modèles de votre modèle de mise en page.

1. Dans le modèle de mise en page, cliquez sur la flèche vers le bas sous **Personnaliser ce que voient les utilisateurs**, puis cliquez sur **Modèle**.
1. Dans la section **Détails**, sélectionnez le champ **Carte tarifaire** dans la zone **Aperçu**.

   Pour plus d’informations, voir [Personnaliser la vue Détails à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

## Joindre une carte tarifaire à un modèle

{{step1-to-templates}}

1. Créez un modèle ou modifiez un modèle existant.
1. Dans la section Détails du modèle > Aperçu > Association des modèles , sélectionnez une carte tarifaire dans le champ **Carte tarifaire**.

   Seules les cartes tarifaires pour lesquelles vous disposez d’autorisations peuvent être sélectionnées.
Vous pouvez commencer à saisir le nom d’une carte tarifaire pour affiner la liste des résultats.

   ![Sélectionnez une carte tarifaire sur le modèle](assets/select-rate-card-on-template.png)

1. Enregistrez le modèle lorsque vous avez terminé de le modifier.

   Pour plus d’informations sur la création d’un modèle, voir [Créer un modèle de projet](/help/quicksilver/manage-work/projects/create-and-manage-templates/create-template.md).

   Pour plus d’informations sur la modification d’un modèle, voir [Modifier les modèles de projet](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

## Application du modèle à un projet

1. Créez un projet à l’aide du modèle.

   Il existe plusieurs façons de créer un projet à partir d’un modèle. Pour plus d’informations, consultez les articles suivants :

   * [Créer un projet à partir d’un modèle](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)
   * [Convertir une tâche en projet](/help/quicksilver/manage-work/tasks/manage-tasks/convert-task-to-project.md)
   * [Convertir un problème en projet](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md)

   La carte tarifaire est automatiquement enregistrée dans le projet. Dans la section Aperçu > Association de projets de la zone Nouveau projet, vous pouvez supprimer la carte tarifaire ou en sélectionner une autre dans le champ **Carte tarifaire**.

   ![La carte tarifaire du modèle apparaît dans les détails du projet](assets/create-project-from-template-rate-card.png)

   La carte tarifaire et ses taux associés apparaissent dans la zone Taux du projet .

   Vous pouvez également supprimer la carte tarifaire du projet ou joindre une autre carte tarifaire dans la zone Taux . Pour plus d’informations, voir [Joindre une carte tarifaire à un projet](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

   ![Carte tarifaire du modèle pour le projet](assets/template-rates-on-project.png)

   >[!NOTE]
   >
   >Si un taux individuel figure sur le modèle et qu’une carte tarifaire est également associée au modèle, lorsque vous créez un projet à partir du modèle, le taux individuel et la carte tarifaire apparaissent tous deux dans la liste des taux.

1. (Facultatif) Pour appliquer la carte tarifaire à un projet existant, joignez le modèle au projet.

   Lorsque vous utilisez l’option **Personnaliser et joindre** dans l’aperçu du modèle, vous pouvez sélectionner l’élément **Carte tarifaire** dans la section Joindre un modèle > Options pour ajouter la carte tarifaire au projet. Décochez la case pour exclure la carte tarifaire du transfert vers le projet.

   Pour plus d’informations, voir [Joindre un modèle à un projet](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. (Facultatif) Pour enregistrer la carte tarifaire d’un projet spécifique dans un modèle, enregistrez le projet en tant que modèle.

   Dans la section Options de la zone Enregistrer en tant que modèle, vous pouvez sélectionner l’élément **Carte tarifaire** pour ajouter la carte tarifaire au modèle. Décochez la case pour exclure la carte tarifaire du transfert vers le modèle.

   Pour plus d’informations, voir [Enregistrer un projet en tant que modèle](/help/quicksilver/manage-work/projects/manage-projects/save-project-as-template.md).


