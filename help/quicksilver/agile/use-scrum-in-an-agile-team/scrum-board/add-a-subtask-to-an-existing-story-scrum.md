---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Ajout d’une sous-tâche à un article existant sur le panorama de défilement
description: Lors de la création de sous-tâches pour les articles existants, gardez à l’esprit le paramètre Mode d’exécution du projet, car cela affecte la manière dont les articles sont mis à jour.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 13%

---

# Ajoutez une sous-tâche à un article existant sur le panorama [!UICONTROL Scrum]

Lors de la création de sous-tâches pour des articles existants, tenez compte des points suivants :

**Lorsque le paramètre [!UICONTROL Mode d’achèvement] du projet est défini sur [!UICONTROL Manuel]:**

* Le déplacement d’un article parent avec des sous-tâches vers [!UICONTROL Complete] met à jour l’article parent à 100 % et le [!UICONTROL Status] à [!UICONTROL Complete]. Les sous-tâches ne sont pas mises à jour.
* Pour mettre à jour le [!UICONTROL pourcentage terminé] de l’article, vous devez le mettre à jour à partir de l’onglet [!UICONTROL Articles] ou de la page [!UICONTROL Détails] de l’objet.

**Lorsque le paramètre [!UICONTROL Mode d’achèvement] du projet est défini sur [!UICONTROL Automatique]** :

* Le déplacement d’un article parent avec des sous-tâches vers [!UICONTROL Complete] met à jour l’article parent à 100 % et le [!UICONTROL Status] à [!UICONTROL Complete]. Les sous-tâches sont également mises à jour à 100 % et le [!UICONTROL statut] est mis à jour à [!UICONTROL Terminé].
* Pour mettre à jour le [!UICONTROL pourcentage terminé] de l’article, vous devez mettre à jour le [!UICONTROL pourcentage terminé] pour toutes les sous-tâches. Le [!UICONTROL pourcentage terminé] pour l’article est calculé en fonction du [!UICONTROL pourcentage terminé] de toutes les sous-tâches.

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
   <td>Accès à [!UICONTROL Contribute] ou [!UICONTROL Gérer] à la tâche sur laquelle se trouve la sous-tâche </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter une sous-tâche à une story existante sur le panorama Scrum

{{step1-to-team}}

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Accédez à l’itération agile ou au projet contenant l’article dans lequel vous souhaitez ajouter une sous-tâche. Pour plus d’informations sur la navigation vers une itération, voir [Affichage d’une itération](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Accédez à la mosaïque de l’article dans le tableau de bord où vous souhaitez ajouter une sous-tâche.
1. Cliquez sur **[!UICONTROL Ajouter une sous-tâche]** sur la carte de l’article principal pour créer une sous-tâche à l’article.

   ![Ajouter une sous-tâche](assets/agile-story-addsubtask-NWE.png)

   Ou

   Cliquez sur **[!UICONTROL Ajouter une sous-tâche]** sur une mosaïque de sous-tâche pour créer une sous-tâche à la sous-tâche.

   [!DNL Workfront] prend en charge des niveaux infinis de sous-tâches, mais seuls deux niveaux (sous-tâches de sous-tâches) s’affichent sur le tableau de bord agile.

   ![Ajouter une sous-tâche](assets/agile-story-addsubtask2-NWE.png)

   Lors de l’ajout d’une sous-tâche à un article qui n’a actuellement pas de couloir, la tâche parent est promue dans la colonne [!UICONTROL Parent Story] et la sous-tâche se déplace dans le couloir.

1. Indiquez les informations suivantes :

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
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>Indiquez l’estimation de la sous-tâche.<br><p>Gardez à l’esprit les points suivants lors de la création d’estimations :</p>
       <ul>
        <li>Si votre équipe agile est configurée pour estimer les articles en points, alors par défaut 1 point équivaut à 8 heures. Les estimations sont ajoutées sous la forme [!UICONTROL Heures planifiées] sur l’article.</li>
        <li>Les estimations combinées pour toutes les sous-tâches déterminent l’estimation de l’article parent. Pour plus d’informations, voir <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Mise à jour de l’état des articles et des sous-tâches sur le Scrum board</a>.</li>
        <li>Lorsque vous créez une sous-tâche, le champ [!UICONTROL Estimation] est déjà défini. Si vous réinitialisez l’estimation sur la sous-tâche, vous réinitialisez l’estimation sur l’article parent (car l’article parent est la somme de toutes ses sous-tâches).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Planned Hours]</strong></td>
      <td> (Disponible uniquement dans les projets) Indiquez le nombre d’heures planifiées pour la tâche.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignment]</strong></td>
      <td>Commencez à saisir le nom de l’équipe à laquelle vous souhaitez affecter la sous-tâche, puis cliquez dessus lorsqu’il apparaît dans la liste déroulante.</td>
     </tr>
    </tbody>
   </table>

1. Cliquez sur **[!UICONTROL Créer]**.
