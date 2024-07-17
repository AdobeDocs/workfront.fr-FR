---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Créer une story agile dans une itération
description: Cet article décrit comment créer un article agile lorsque vous êtes déjà dans l’itération.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 16%

---

# Créer une story agile dans une itération

Cet article décrit comment créer un article agile lorsque vous êtes déjà dans l’itération. Pour plus d’informations sur la création d’un article agile à partir d’une tâche, d’un problème ou d’une autre zone de [!DNL Adobe Workfront], voir [Ajout d’articles à une itération existante](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou version ultérieure</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Gérer] Accès au projet sur lequel se trouve l’article</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Créer une story agile dans une itération

1. Accédez à l&#39;itération agile où vous souhaitez créer l&#39;histoire :

   1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe] Workfront, puis cliquez sur **[!UICONTROL Équipes]**.

   1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

   1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Itérations]**.
   1. Cliquez sur le nom de l’itération spécifique où vous souhaitez créer un article.
   1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Stories]**.

1.  Cliquez sur **[!UICONTROL New Story].**
1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>Saisissez le nom de l’article.</td>
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
      <td>Commencez à saisir le nom du projet auquel cet article sera associé.<br>Par défaut, la couleur de l’article s’affiche avec la même couleur que les autres articles de ce projet.<br>L’état du projet doit être défini sur [!UICONTROL Actuel]. Si l’état du projet est autre que [!UICONTROL Actuel], il ne s’affiche pas dans le menu déroulant.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tâche Parente]</strong></td>
      <td>Après avoir choisi un projet parent, vous avez la possibilité de choisir une tâche parent. Lorsque vous sélectionnez une tâche parente, l’article est créé en tant que sous-tâche de la tâche parente sur le projet que vous avez sélectionné.<br>Commencez à saisir le nom de la tâche parent pour l’article, puis cliquez dessus lorsqu’il apparaît dans la liste déroulante.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Sélectionnez les formulaires personnalisés à ajouter à l’article.</td>
     </tr>
    </tbody>
   </table>

1. Cliquez sur **[!UICONTROL Enregistrer l’article]**.
