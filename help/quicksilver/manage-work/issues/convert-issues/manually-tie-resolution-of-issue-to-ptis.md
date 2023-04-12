---
product-area: projects
navigation-topic: convert-issues
title: Lier manuellement la résolution d’un problème à d’autres problèmes, tâches ou projets
description: Vous pouvez lier manuellement la résolution d’un problème à la résolution d’un projet, d’une tâche ou d’un problème sans le convertir. Le problème devient l’un des objets résolvables du projet, de la tâche ou du problème que vous sélectionnez. Lorsque vous procédez de la sorte, une modification de l’état du projet, de la tâche ou du problème déclenche une modification de l’état du problème d’origine.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: ea430157da539507c11a559a4dce6b24aca9e5a6
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Lier manuellement la résolution d’un problème à d’autres problèmes, tâches ou projets

Vous pouvez lier manuellement la résolution d’un problème à la résolution d’un projet, d’une tâche ou d’un problème sans le convertir. Le problème devient l’un des objets résolvables du projet, de la tâche ou du problème que vous sélectionnez. Lorsque vous procédez de la sorte, une modification de l’état du projet, de la tâche ou du problème déclenche une modification de l’état du problème d’origine.

>[!TIP]
>
>Lorsque vous liez la résolution d’un problème à la résolution d’un autre objet, vous ne pouvez plus modifier manuellement l’état du problème d’origine.

Pour plus d’informations sur la résolution et la résolution d’objets, voir [Présentation de la résolution et des objets résolvables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux problèmes, tâches et projets</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’accès au problème lié à un autre problème, tâche ou projet</p> <p>Afficher ou des autorisations supérieures au problème, à la tâche ou au projet que vous ajoutez au problème existant</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de commencer, vous devez :

* Posséder un problème dont vous souhaitez lier la résolution à un autre problème, tâche ou projet

* Posséder un problème, une tâche ou un projet supplémentaire

## Lier la résolution d’un problème à la résolution d’un autre problème, d’une autre tâche ou d’un autre projet

1. Accédez à un problème dont vous souhaitez lier la résolution à un autre problème ou à une tâche ou à un projet.
1. Cliquez sur le bouton **Détails du problème** > **Présentation** zone.

   ![](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Accédez au **Présentation** dans la zone **Détails du problème** .
1. Cliquez sur le bouton **Résolu par** et effectuez une sélection parmi les types d’objets de résolution suivants :

   * **Projet**
   * **Tâche**
   * **Problème**

   Selon l’objet sélectionné, les champs suivants s’affichent :

   * **Résolution du projet**
   * **Résolution de la tâche**
   * **Résolution de l&#39;événement**


1. Commencez à saisir le nom d’un projet, d’une tâche ou d’un problème spécifique dans la variable **Résolution du projet**, **Tâche** ou **Problème** puis cliquez dessus lorsqu’il apparaît dans la liste.

   >[!NOTE]
   >
   >Vous ne pouvez pas lier la résolution d’un problème à la tâche ou au projet dans lequel le problème se trouve. La tâche ou le projet du problème ne s’affiche pas dans les champs Résoudre une tâche ou Résoudre une tâche .


1. Cliquez sur **Enregistrer les modifications**.

   Le problème d’origine devient l’objet résolvable pour le projet, la tâche ou le problème que vous avez sélectionné aux étapes 4 et 5. Cela signifie que le problème d’origine se termine lorsque l’objet de résolution (le projet, la tâche ou le problème auquel vous l’avez lié) est terminé.

   >[!NOTE]
   >
   >Un projet, une tâche ou un problème peut présenter plusieurs problèmes comme des objets résolvables.
