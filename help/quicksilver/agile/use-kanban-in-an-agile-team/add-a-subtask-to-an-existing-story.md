---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Ajouter une sous-tâche à une story existante sur le panorama Kanban
description: Consultez cet article pour savoir comment créer des sous-tâches pour les articles existants sur le panorama Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 24%

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

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[!UICONTROL Worker] ou version ultérieure</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la manière dont l’équipe d’administration [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Accès à [!UICONTROL Contribute] ou [!UICONTROL Gérer] à la tâche sur laquelle se trouve la sous-tâche</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Ajoutez une sous-tâche à un article existant sur le panorama [!UICONTROL Kanban]

1. Accédez au panorama [!UICONTROL Kanban] qui contient l’article dans lequel vous souhaitez ajouter une sous-tâche.
1. Cliquez sur le nom de la tâche sur la mosaïque de l’article sur le panorama [!UICONTROL Kanban].
1. Ajoutez une sous-tâche à la tâche comme vous le feriez dans toute autre liste de tâches dans [!DNL Workfront], comme décrit dans la section [Créer des sous-tâches](../../manage-work/tasks/create-tasks/create-subtasks.md).
