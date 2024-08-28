---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Ajout d’une sous-tâche à un article existant sur le panorama Kanban
description: Consultez cet article pour savoir comment créer des sous-tâches pour les articles existants sur le panorama Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 20%

---

# Ajouter une sous-tâche à une story existante sur le panorama Kanban

Lors de la création de sous-tâches pour des articles existants, tenez compte des points suivants :

**Lorsque le paramètre [!UICONTROL Mode d’achèvement de résumé] pour le projet est défini sur [!UICONTROL Manuel]:**

* Vous pouvez déplacer un article parent avec des sous-tâches vers [!UICONTROL Complete], ce qui met à jour l’article parent à 100 % et [!UICONTROL Status] vers [!UICONTROL Complete]. Les sous-tâches ne sont pas mises à jour.
* Pour mettre à jour le [!UICONTROL pourcentage terminé] de l’article, vous devez le mettre à jour à partir de l’onglet [!UICONTROL Articles] ou de la page [!UICONTROL Détails] de l’objet.

**Lorsque le paramètre [!UICONTROL Mode d’achèvement récapitulatif] pour le projet est défini sur [!UICONTROL Automatique] :**

* Vous ne pouvez pas déplacer l’histoire parente dans son ensemble. Pour mettre à jour le [!UICONTROL pourcentage terminé] de l’article, vous devez mettre à jour le [!UICONTROL pourcentage terminé] pour toutes les sous-tâches. Le [!UICONTROL pourcentage terminé] pour l’article est calculé en fonction du [!UICONTROL pourcentage terminé] de toutes les sous-tâches.
* Le déplacement d’un article parent avec des sous-tâches vers [!UICONTROL Complete] met à jour l’article parent à 100 % et le [!UICONTROL Status] à [!UICONTROL Complete]. Les sous-tâches sont également mises à jour à 100 % et le [!UICONTROL statut] est mis à jour à [!UICONTROL Terminé].

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td>Accès à [!UICONTROL Contribute] ou [!UICONTROL Gérer] à la tâche sur laquelle se trouve la sous-tâche</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajoutez une sous-tâche à un article existant sur le panorama [!UICONTROL Kanban]

1. Accédez au panorama [!UICONTROL Kanban] qui contient l’article dans lequel vous souhaitez ajouter une sous-tâche.
1. Cliquez sur le nom de la tâche sur la mosaïque de l’article sur le panorama [!UICONTROL Kanban].
1. Ajoutez une sous-tâche à la tâche comme vous le feriez dans toute autre liste de tâches dans [!DNL Workfront], comme décrit dans la section [Créer des sous-tâches](../../manage-work/tasks/create-tasks/create-subtasks.md).
