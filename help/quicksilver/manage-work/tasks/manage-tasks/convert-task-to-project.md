---
product-area: projects
navigation-topic: manage-tasks
title: Convertir une tâche en projet
description: Lorsqu’une tâche d’un projet nécessite un effort plus important que celui initialement prévu, vous pouvez la convertir en projet.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Convertir une tâche en projet

Lorsqu’une tâche d’un projet nécessite un effort plus important que celui initialement prévu, vous pouvez la convertir en projet.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p>Affichage ou accès supérieur aux modèles lors de la conversion vers un projet à l’aide d’un modèle</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour une tâche</p> <p>Afficher les autorisations sur un modèle, en cas de conversion en projet à l’aide d’un modèle</p> <p>Après avoir créé le projet, vous disposez des autorisations de gestion pour le projet.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Observations relatives à la conversion de tâches en projets

* La tâche d’origine est supprimée.
* Les validations de tâche sont supprimées.
* Toutes les sous-tâches, les problèmes et les notes sont cumulés jusqu’au nouveau projet.
* Les documents, versions de document et BAT sont déplacés vers le nouveau projet.
* L’état et le pourcentage d’achèvement de toutes les sous-tâches et problèmes sont conservés.
* Les utilisateurs partagés de la tâche deviennent des utilisateurs partagés sur le projet.
* La date de début du projet est définie sur la date de début de la tâche.
* Si l’état de la tâche est &quot;Nouveau&quot;, l’état du projet est défini sur &quot;Planification&quot;.
* Si l’état de la tâche est &quot;En cours&quot;, l’état du projet est défini sur &quot;Actuel&quot;.
* Si l’état de la tâche est &quot;Terminé&quot;, l’état du projet est défini sur &quot;Terminé&quot;.

## Convertir une tâche en projet

1. Accédez à la tâche que vous souhaitez convertir en projet.
1. Cliquez sur le bouton **Plus** icon ![](assets/more-icon.png), puis **Convertir en projet**.
1. Choisissez l’une des options suivantes :

   * **Nouveau projet**
   * Un modèle dans le **Sélectionner parmi les modèles** section

      ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Cliquez sur **Continuer** sur la notification qui s’affiche.
1. Dans le **Convertir en projet** , spécifiez les éléments suivants :

   * **Nom**: Nommez votre projet. Le nom par défaut est le nom de la tâche.
   * (Facultatif) **Description**: Décrivez l’objectif de ce projet.
   * (Facultatif et conditionnel) Si vous avez choisi de créer un projet à partir d’un modèle, mettez à jour les champs disponibles dans la variable **Convertir en projet** de la boîte de dialogue

      Pour plus d’informations sur la modification des champs des projets, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >Pour mettre à jour les champs de la section Finance de la zone Convertir en projet , vous devez disposer de l’option Modifier l’accès aux données financières de votre niveau d’accès. Si vous disposez de l’option Afficher l’accès aux données financières dans votre niveau d’accès, toutes les informations financières du modèle sont transférées vers le nouveau projet et vous ne pouvez pas les modifier pendant que vous convertissez le problème. Pour plus d’informations, voir [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) et [Partage d’un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Facultatif) Ajoutez **Forms personnalisée** au nouveau projet.

      >[!TIP]
      Si un formulaire personnalisé contenant plusieurs objets associés à la tâche est configuré pour être utilisé avec les tâches et les projets, toutes les informations enregistrées dans le formulaire sont conservées lorsque vous effectuez la conversion.
      Si vous utilisez un modèle pour la conversion et qu’un formulaire personnalisé associé au modèle contient un champ personnalisé également trouvé dans un formulaire personnalisé associé à la tâche, la valeur du champ de la tâche est utilisée pour le nouveau projet. Cependant, si le champ personnalisé est vide sur la tâche, la valeur du modèle est utilisée.

1. Cliquez sur **Enregistrer les modifications**.
