---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Ajout d’une sous-tâche à un article existant sur le panorama Kanban
description: Consultez cet article pour savoir comment créer des sous-tâches pour les histoires existantes sur le tableau Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 96%

---

# Ajouter une sous-tâche à une histoire existante sur le tableau Kanban

Lors de la création de sous-tâches pour des histoires existantes, tenez compte des points suivants :

**Lorsque le paramètre [!UICONTROL Résumé du mode d’achèvement] du projet est défini sur [!UICONTROL Manuel] :**

* Vous pouvez déplacer une histoire parent avec des sous-tâches vers [!UICONTROL Terminé], qui met à jour l’histoire parent sur 100 % et le [!UICONTROL statut] sur [!UICONTROL Terminé]. Les sous-tâches ne sont pas mises à jour.
* Pour mettre à jour la variable [!UICONTROL Pourcentage terminé] pour l’histoire, vous devez la mettre à jour à partir de l’onglet [!UICONTROL Histoires] ou depuis la page [!UICONTROL Détails] de l’objet.

**Lorsque le paramètre[!UICONTROL Résumé du mode d’achèvement] du projet est défini sur [!UICONTROL Automatique] :**

* vous ne pouvez pas déplacer l’histoire parent dans le panorama. Pour mettre à jour la variable [!UICONTROL Pourcentage terminé] pour l’histoire, vous devez mettre à jour [!UICONTROL Pourcentage terminé] pour toutes les sous-tâches. La variable [!UICONTROL Pourcentage terminé] pour l’histoire est calculée en fonction du [!UICONTROL Pourcentage terminé] de toutes les sous-tâches.
* Le déplacement d’une histoire parent avec des sous-tâches vers [!UICONTROL Terminé] met à jour l’histoire parent sur 100 % et le [!UICONTROL statut] sur [!UICONTROL Terminé]. Les sous-tâches sont également mises à jour sur 100 % et le [!UICONTROL statut] est mis à jour vers [!UICONTROL Terminé].

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
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p> 
   ou
   <p>Actuelle : [!UICONTROL Work] ou niveau supérieur</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Accès [!UICONTROL Contribute] ou [!UICONTROL Manage] à la tâche sur laquelle se trouve la sous-tâche</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter une sous-tâche à une histoire existante sur le tableau [!UICONTROL Kanban]

1. Accédez au tableau [!UICONTROL Kanban] contenant l’histoire dans laquelle vous souhaitez ajouter une sous-tâche.
1. Cliquez sur le nom de la tâche sur la vignette de l’histoire dans le tableau [!UICONTROL Kanban].
1. Ajoutez une sous-tâche à la tâche comme vous le feriez dans toute autre liste de tâches dans [!DNL Workfront], comme décrit dans [Créer des sous-tâches](../../manage-work/tasks/create-tasks/create-subtasks.md).
