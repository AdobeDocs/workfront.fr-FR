---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Utiliser des indicateurs sur les histoires sur le tableau kanban
description: Sur le panorama  [!DNL Kanban] , les indicateurs fournissent une indication visuelle du moment où une histoire est prête à passer au statut suivant. Cela permet aux équipes Kanban d’utiliser une approche « pull » plutôt qu’une approche « push » lors du déplacement des histoires d’un statut à l’autre.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 85%

---

# Utiliser des indicateurs sur les histoires du panorama [!UICONTROL Kanban]

Sur le panorama [!DNL Kanban], les indicateurs fournissent une indication visuelle du moment où une histoire est prête à passer au statut suivant. Ceci permet aux équipes [!UICONTROL Kanban] d’utiliser une approche « pull » plutôt qu’une approche « push » lors du déplacement des histoires d’un statut à l’autre.

**Exemple :** prenons l’exemple suivant d’une équipe utilisant une approche « pull » : Olivia, la designer de l’équipe, termine son travail, puis définit l’indicateur de l’histoire sur « [!UICONTROL Prête pour la stratégie pull] ». Cet indicateur indique visuellement à Tony, le rédacteur en chef de l’équipe, que l’histoire est prête à passer au statut suivant. Tony déplace alors l’histoire vers le statut suivant lorsqu’il est prêt à travailler dessus.

Tenez compte des points suivants lorsque vous utilisez des indicateurs sur des histoires :

* Les indicateurs ne sont pas un statut, mais plutôt une indication visuelle que l’histoire est prête à être déplacée vers le statut suivant par un ou une autre membre de l’équipe.
* Les indicateurs n’apparaissent sur aucune carte d’histoire qui se trouve dans la colonne [!UICONTROL Liste d’attente] ou dans la colonne [!UICONTROL Terminer] (ou dans toute colonne dont le statut de la colonne correspond à [!UICONTROL Terminer]).

  Pour plus d’informations sur les statuts des histoires, voir [Utiliser des indicateurs pour des histoires sur le panorama Kanban](#updating-the-status-of-stories-and-subtasks).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Travail ou supérieur</p> </td> 
  </tr>
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utiliser des indicateurs pour des histoires du panorama [!UICONTROL Kanban]

Pour modifier un indicateur sur une histoire :

{{step1-to-team}}

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe [!UICONTROL Kanban] dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Accédez au panorama [!UICONTROL Kanban] sur lequel vous souhaitez modifier un indicateur sur une histoire.
1. Développez la mosaïque Histoire pour afficher l’indicateur .
L’indicateur est défini par défaut sur **[!UICONTROL Dans les temps]** pour chaque histoire.
   ![Carte Kanban](assets/agile-storycard-kanban-2021-350x308.png)

1. Cliquez sur l’indicateur actuel, puis sélectionnez l’une des options d’indicateur suivantes :

   * **[!UICONTROL En bonne voie] :** le statut de l’histoire est correct et aucune action ne doit être entreprise pour le moment.

     Il s’agit de l’indicateur par défaut pour chaque histoire du panorama Kanban.
     ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Est bloquée] :** l’histoire ne peut pas passer au statut suivant. Lorsque cet indicateur est défini sur une histoire, l’histoire ne compte pas dans la limite du travail en cours. (Pour plus d’informations sur les limites WIP, voir l’article [Configurer Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).)

     ![kanban_flag_block.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Prêt pour l’extraction] :** l’histoire est prête à être déplacée vers le statut suivant par un autre membre de l’équipe.

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
