---
product-area: templates
keywords: task,defaults,automate,creation
navigation-topic: templates-navigation-topic
title: Supprimer une tâche de modèle
description: Vous pouvez supprimer un modèle de tâches s’il n’est plus nécessaire. Les tâches de modèles supprimées ne peuvent pas être récupérées. Les tâches de projet créées à partir de la tâche de modèle ne sont ni supprimées ni modifiées.
author: Alina
feature: Work Management
exl-id: dd733e9f-8045-4b65-828b-fe6aa40d973f
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/G4OdOAGqiLA0PNUADG9ONsN9Dc2euNHQQGCYXK6ohvA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 285
ht-degree: 27%

---

# Supprimer une tâche de modèle

Vous pouvez supprimer un modèle de tâches s’il n’est plus nécessaire. Les tâches de projet créées à partir de la tâche de modèle ne sont ni supprimées ni modifiées.

>[!NOTE]
>
>Les tâches de modèles supprimées et leurs informations supplémentaires (affectations, documents, approbations) ne peuvent pas être récupérées. Vous pouvez récupérer un modèle qui récupère également toutes les tâches du modèle. Si vous supprimez des tâches de modèles (et non le modèle), vous ne pourrez jamais les récupérer.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Modifier l’accès aux modèles</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p> </td> 
   <td> <p>Autorisations de gestion pour un modèle.</p> <p>Vous ne pouvez pas partager une tâche de modèle.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Standard </p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level</p></td> 
   <td> <p>Edit access to Templates</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p> </td> 
   <td> <p>Manage permissions for a template.</p> <p>You cannot share a template task.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Supprimer une tâche de modèle

Vous pouvez supprimer une ou plusieurs tâches de modèles en bloc.

{{step1-to-templates}}

1. Cliquez sur le nom d’un modèle pour l’ouvrir.
1. Cliquez sur **Tâches de modèle** dans le panneau de gauche.
1. Utilisez l’une des méthodes suivantes :
   * Cliquez sur le nom d’une tâche de modèle dans la liste pour ouvrir la tâche de modèle > cliquez sur le menu **Plus** ![Menu Plus](assets/more-icon.png) > **Supprimer la tâche de modèle**.
   * Sélectionnez une ou plusieurs tâches de modèles dans la liste > **Icône Supprimer** ![Icône Supprimer](assets/delete.png).

   La boîte de dialogue **Supprimer la tâche de modèle** s&#39;ouvre.
1. Cliquez sur **Oui, supprimer** pour confirmer.

   Les tâches de modèles sont supprimées et ne peuvent pas être récupérées.

>[!TIP]
>
>Vous pouvez cliquer sur les sections Prédécesseurs ou Sous-tâches dans le panneau de gauche d’une tâche de modèle pour supprimer un prédécesseur ou une sous-tâche.
>
>Répétez les étapes ci-dessus pour supprimer les tâches antérieures ou les sous-tâches de modèles.
