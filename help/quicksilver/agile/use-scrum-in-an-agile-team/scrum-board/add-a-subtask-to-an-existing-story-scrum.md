---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Ajout d’une sous-tâche à un article existant sur le panorama Scrum
description: Lors de la création de sous-tâches pour les articles existants, gardez à l’esprit le paramètre Mode d’exécution du projet, car cela affecte la manière dont les articles sont mis à jour.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Ajoutez une sous-tâche à un article existant sur la [!UICONTROL Scrum] board

Lors de la création de sous-tâches pour des articles existants, tenez compte des points suivants :

**Lorsque la variable [!UICONTROL Mode d’achèvement] le paramètre du projet est défini sur [!UICONTROL Manuel]:**

* Déplacement d’un article parent avec des sous-tâches vers [!UICONTROL Terminer] met à jour l’article parent à 100 % et la variable [!UICONTROL État] to [!UICONTROL Terminer]. Les sous-tâches ne sont pas mises à jour.
* Pour mettre à jour la variable [!UICONTROL Pourcentage terminé] pour l’article, vous devez le mettre à jour à partir du [!UICONTROL Histoires] ou depuis l’ [!UICONTROL Détails] de l’objet.

**Lorsque la variable [!UICONTROL Mode d’achèvement] le paramètre du projet est défini sur [!UICONTROL Automatique]**:

* Déplacement d’un article parent avec des sous-tâches vers [!UICONTROL Terminer] met à jour l’article parent à 100 % et la variable [!UICONTROL État] to [!UICONTROL Terminer]. Les sous-tâches sont également mises à jour à 100 % et la variable [!UICONTROL État] est mis à jour vers [!UICONTROL Terminer].
* Pour mettre à jour la variable [!UICONTROL Pourcentage terminé] pour l’article, vous devez mettre à jour la variable [!UICONTROL Pourcentage terminé] pour toutes les sous-tâches. Le [!UICONTROL Pourcentage terminé] pour que l’article soit calculé en fonction de la variable [!UICONTROL Pourcentage terminé] de toutes les sous-tâches.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou version ultérieure</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Contribute] ou [!UICONTROL Gérer] l’accès à la tâche sur laquelle se trouve la sous-tâche.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Ajout d’une sous-tâche à un article existant sur le panorama Scrum

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. (Facultatif) Cliquez sur le **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Accédez à l’itération agile ou au projet contenant l’article dans lequel vous souhaitez ajouter une sous-tâche. Pour plus d’informations sur la navigation vers une itération, voir [Afficher une itération](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Accédez à la mosaïque de l’article dans le tableau de bord où vous souhaitez ajouter une sous-tâche.
1. Cliquez sur **[!UICONTROL Ajouter une sous-tâche]** sur la carte principale de l’article pour créer une sous-tâche à l’article.

   ![Ajouter une sous-tâche](assets/agile-story-addsubtask-NWE.png)

   Ou

   Cliquez sur **[!UICONTROL Ajouter une sous-tâche]** sur une mosaïque de sous-tâche pour créer une sous-tâche à la sous-tâche.

   [!DNL Workfront] prend en charge des niveaux infinis de sous-tâches, mais seuls deux niveaux (sous-tâches de sous-tâches) s’affichent sur le tableau de bord agile.

   ![Ajouter une sous-tâche](assets/agile-story-addsubtask2-NWE.png)

   Lors de l’ajout d’une sous-tâche à un article qui n’a actuellement pas de couloir, la tâche parent est convertie en [!UICONTROL Histoire parente] et la sous-tâche se déplace à l’intérieur du couloir.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtask Name]</strong></td>
      <td> Spécifiez un nom pour la sous-tâche.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Spécifiez une description pour la sous-tâche.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td>Indiquez l’estimation de la sous-tâche.<br><p>Gardez à l’esprit les points suivants lors de la création d’estimations :</p>
       <ul>
        <li>Si votre équipe agile est configurée pour estimer les articles en points, alors par défaut 1 point équivaut à 8 heures. Les estimations sont ajoutées sous la forme [!UICONTROL Heures planifiées] sur l’article.</li>
        <li>Les estimations combinées pour toutes les sous-tâches déterminent l’estimation de l’article parent. Pour plus d’informations, voir <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Mettre à jour l’état des articles et des sous-tâches sur le panorama Scrum</a>.</li>
        <li>Lorsque vous créez une sous-tâche, le champ [!UICONTROL Estimation] est déjà défini. Si vous réinitialisez l’estimation sur la sous-tâche, vous réinitialisez l’estimation sur l’article parent (car l’article parent est la somme de toutes ses sous-tâches).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Heures planifiées]</strong></td>
      <td> (Disponible uniquement dans les projets) Indiquez le nombre d’heures planifiées pour la tâche.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignation]</strong></td>
      <td>Commencez à saisir le nom de l’équipe à laquelle vous souhaitez affecter la sous-tâche, puis cliquez dessus lorsqu’il apparaît dans la liste déroulante.</td>
     </tr>
    </tbody>
   </table>

1. Cliquez sur **[!UICONTROL Créer]**.
