---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Création d’un article Agile dans une itération
description: Cet article décrit comment créer un article agile lorsque vous êtes déjà dans l’itération.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 26%

---

# Créer une story agile dans une itération

Cet article décrit comment créer un article agile lorsque vous êtes déjà dans l’itération. Pour plus d’informations sur la création d’un article agile à partir d’une tâche, d’un problème ou d’une autre zone de [!DNL Adobe Workfront], voir [Ajout d’articles à une itération existante](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p> 
   ou
   <p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Accès en [!UICONTROL Manage] au projet contenant l’histoire </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une story agile dans une itération

1. Accédez à l&#39;itération agile où vous souhaitez créer l&#39;histoire :

   {{step1-to-team}}

   1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

   1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Itérations]**.
   1. Cliquez sur le nom de l’itération spécifique où vous souhaitez créer un article.
   1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Stories]**.

1.  Cliquez sur **[!UICONTROL New Story]**.
1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>Saisissez un nom pour l’histoire.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Saisissez une description pour l’article.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>Sélectionnez cette option si l’article est prêt à être ajouté à une itération. Lorsque cette option est sélectionnée, elle indique aux utilisateurs quels articles du journal sont prêts à être ajoutés à une itération.<br>Un article peut être ajouté à une itération, qu’il soit ou non marqué <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL (estimation)] (points)</strong></td>
      <td>Indiquez l’estimation de l’article. Si votre équipe agile est configurée pour estimer les articles en points, alors par défaut 1 point équivaut à 8 heures. Les estimations sont ajoutées sous la forme [!UICONTROL Heures planifiées] sur l’article.<br>Par exemple, si vous estimez un article à 3 points, le comportement par défaut consiste à ajouter 24 heures planifiées à l’article.<br>Si un article contient des sous-tâches, n’oubliez pas que les estimations combinées pour toutes les sous-tâches déterminent l’estimation de l’article parent. Pour plus d’informations, voir <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Ajout d’une sous-tâche à un article existant sur le panorama [!UICONTROL Scrum]</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Commencez à saisir le nom du projet auquel cet article sera associé.<br>Par défaut, la couleur de l’article s’affiche avec la même couleur que les autres articles de ce projet.<br>Le statut du projet doit être défini sur [!UICONTROL Current]. Si le statut du projet est autre que [!UICONTROL Current], il ne s’affiche pas dans le menu déroulant.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>Après avoir choisi un projet parent, vous avez la possibilité de choisir une tâche parent. Lorsque vous sélectionnez une tâche parente, l’article est créé en tant que sous-tâche de la tâche parente sur le projet que vous avez sélectionné.<br>Commencez à saisir le nom de la tâche parent pour l’article, puis cliquez dessus lorsqu’il apparaît dans la liste déroulante.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Sélectionnez les formulaires personnalisés à ajouter à l’article.</td>
     </tr>
    </tbody>
   </table>

1. Cliquez sur **[!UICONTROL Enregistrer l’histoire]**.
