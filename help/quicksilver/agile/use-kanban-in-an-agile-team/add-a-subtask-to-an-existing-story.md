---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Ajouter une sous-tâche à un article existant sur le panorama Kanban
description: Consultez cet article pour savoir comment créer des sous-tâches pour les articles existants sur le panorama Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Ajouter une sous-tâche à un article existant sur le panorama Kanban

Lors de la création de sous-tâches pour des articles existants, tenez compte des points suivants :

**Lorsque la variable [!UICONTROL Mode d’achèvement du résumé] le paramètre du projet est défini sur [!UICONTROL Manuel]:**

* Vous pouvez déplacer un article parent avec des sous-tâches vers [!UICONTROL Terminer], qui met à jour l’article parent à 100 % et l’ [!UICONTROL État] to [!UICONTROL Terminer]. Les sous-tâches ne sont pas mises à jour.
* Pour mettre à jour la variable [!UICONTROL Pourcentage terminé] pour l’article, vous devez le mettre à jour à partir du [!UICONTROL Histoires] ou depuis l’ [!UICONTROL Détails] de l’objet.

**Lorsque la variable [!UICONTROL Mode d’achèvement du résumé] le paramètre du projet est défini sur [!UICONTROL Automatique]:**

* Vous ne pouvez pas déplacer l’histoire parente dans son ensemble. Pour mettre à jour la variable [!UICONTROL Pourcentage terminé] pour l’article, vous devez mettre à jour la variable [!UICONTROL Pourcentage terminé] pour toutes les sous-tâches. Le [!UICONTROL Pourcentage terminé] pour que l’article soit calculé en fonction de la variable [!UICONTROL Pourcentage terminé] de toutes les sous-tâches.
* Déplacement d’un article parent avec des sous-tâches vers [!UICONTROL Terminer] met à jour l’article parent à 100 % et la variable [!UICONTROL État] to [!UICONTROL Terminer]. Les sous-tâches sont également mises à jour à 100 % et la variable [!UICONTROL État] est mis à jour vers [!UICONTROL Terminer].

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[!UICONTROL Worker] ou version ultérieure</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>[!UICONTROL Contribute] ou [!UICONTROL Gérer] l’accès à la tâche sur laquelle se trouve la sous-tâche.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Ajoutez une sous-tâche à un article existant sur la [!UICONTROL Kanban] board

1. Accédez au [!UICONTROL Kanban] tableau contenant l’article dans lequel vous souhaitez ajouter une sous-tâche.
1. Cliquez sur le nom de la tâche sur la mosaïque de l’article dans la [!UICONTROL Kanban] panorama.
1. Ajoutez une sous-tâche à la tâche comme vous le feriez dans toute autre liste de tâches dans [!DNL Workfront], comme décrit dans [Création de sous-tâches](../../manage-work/tasks/create-tasks/create-subtasks.md).
