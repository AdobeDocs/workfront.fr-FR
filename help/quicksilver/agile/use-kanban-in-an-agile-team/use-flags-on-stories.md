---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Utiliser des drapeaux sur les articles sur le panorama de Kanban
description: Sur le [!DNL Kanban] panorama, les indicateurs fournissent une indication visuelle du moment où un article est prêt à passer à l’état suivant. Cela permet aux équipes de Kanban d’utiliser une approche "pull" plutôt qu’une approche "push" lors du déplacement d’articles entre états.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Utilisez des indicateurs sur les articles de la [!UICONTROL Kanban] board

Sur le [!DNL Kanban] panorama, les indicateurs fournissent une indication visuelle du moment où un article est prêt à passer à l’état suivant. Cette option active [!UICONTROL Kanban] Les équipes utilisent une approche &quot;pull&quot; plutôt qu’une approche &quot;push&quot; lors du déplacement d’articles entre états.

**Exemple :** Prenons l’exemple suivant d’une équipe utilisant une approche de &quot;tirage&quot; : Olivia, la graphiste de l&#39;équipe, termine son travail, puis définit le drapeau de l&#39;histoire comme &quot;[!UICONTROL Prêt à tirer].&quot; Ce drapeau indique visuellement à Tony, le rédacteur en chef de l&#39;équipe, que l&#39;histoire est prête à passer au statut suivant. Tony passe alors l&#39;histoire au statut suivant lorsqu&#39;il est prêt à commencer à y travailler.

Tenez compte des points suivants lorsque vous utilisez des indicateurs sur des articles :

* Les drapeaux ne sont pas un statut, mais plutôt une indication visuelle que l&#39;histoire est prête à être déplacée vers le statut suivant par un autre membre de l&#39;équipe.
* Les indicateurs n’apparaissent sur aucune fiche d’article qui se trouve dans la variable [!UICONTROL Backlog] ou dans la variable [!UICONTROL Terminer] ou dans toute colonne dont l’état de la colonne correspond à [!UICONTROL Terminer]).

   Pour plus d’informations sur les états d’un article, voir [Utiliser des drapeaux sur les articles sur le panorama de Kanban](#updating-the-status-of-stories-and-subtasks)

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
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Utilisez des indicateurs sur les articles de la [!UICONTROL Kanban] board

Pour changer un drapeau sur une histoire :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. (Facultatif) Cliquez sur le **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle [!UICONTROL Kanban] dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Accédez au [!UICONTROL Kanban] tableau où vous souhaitez changer un drapeau sur une histoire.
1. Développez la mosaïque de l’article pour afficher l’indicateur.\
   L’indicateur est défini sur **[!UICONTROL Sur le suivi]** pour chaque article par défaut.\
   ![Carte Kanban](assets/agile-storycard-kanban-2021-350x308.png)

1. Cliquez sur l’indicateur actuel, puis sélectionnez l’une des options d’indicateur suivantes :

   * **[!UICONTROL Sur le suivi]:** L’histoire est dans le bon état et aucune action ne doit être entreprise pour le moment.\

      Il s’agit de l’indicateur par défaut pour chaque article sur le panorama Kanban.\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Est bloqué]:** L’histoire ne peut pas passer au statut suivant. Lorsque cet indicateur est défini sur un article, l’article ne compte pas dans la limite du travail en cours. (Pour plus d’informations sur les limites de travaux en cours, voir l’article [Configurer Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

      ![kanban_flag_block.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Prêt à tirer]:** L&#39;histoire est prête à être déplacée vers le statut suivant par un autre membre de l&#39;équipe.\

      ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
