---
product-area: projects
navigation-topic: use-the-home-area
title: Marquer un élément comme Terminé dans la zone Accueil
description: Vous pouvez marquer une tâche ou un problème comme Terminé si vous êtes le ou la cessionnaire de la tâche ou du problème. Lorsque vous marquez une tâche ou un problème comme étant terminé, le statut de la tâche ou du problème passe à Terminé.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 100%

---

# Marquer un élément comme [!UICONTROL Terminé] dans la zone [!UICONTROL Accueil].

Vous pouvez marquer une tâche ou un problème comme Terminé si vous êtes le ou la cessionnaire de la tâche ou du problème. Lorsque vous marquez une tâche ou un problème comme [!UICONTROL Terminé], le statut de la tâche ou du problème passe à [!UICONTROL Terminé].

>[!NOTE]
>
>Vous ne voyez pas le bouton [!UICONTROL Terminé] si vous n’êtes pas l’une des ressources affectées à la tâche ou au problème.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Work] ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>[!UICONTROL Edit] l’accès aux tâches et aux problèmes</p> <p>Note : si vous n’avez toujours pas d’accès, demandez à votre administrateur ou administratrice [!DNL Workfront] si des restrictions supplémentaires ont été définies dans votre niveau d’accès. Pour plus d’informations sur la manière dont l’administration [!DNL Workfront] peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations de contribution ou niveau supérieur pour les tâches et les problèmes sur lesquels vous devez travailler</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander un accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice de [!DNL Workfront].

## Marquer une tâche ou un problème comme [!UICONTROL Terminé]

Seule la personne affectée à la tâche ou au problème peut les marquer comme [!UICONTROL Terminé].

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Dans la **[!UICONTROL liste de travail]**, localisez l’un des éléments en attente de travail.
1. Utilisez l’une des méthodes suivantes :

* Cliquez sur **[!UICONTROL Terminé]** sur l’élément de travail.\
   Voir [Comprendre les options du bouton [!UICONTROL Terminé]](#understand-the-options-of-the-done-button) pour des informations plus détaillées sur la façon dont ce bouton peut apparaître.

* Sélectionnez lélément que vous souhaitez marquer comme terminé, puis dans le panneau de droite, cliquez sur **[!UICONTROL Mettre à jour le statut]**, et modifiez le statut de l’élément en un statut équivalent à [!UICONTROL Terminé] ou [!UICONTROL Clôturé].

## Comprendre les options du bouton [!UICONTROL Terminé]

Par défaut, le fait de cliquer sur le bouton [!UICONTROL Terminé] sur un élément de travail fait passer le statut de cet élément à [!UICONTROL Terminé] (pour les tâches) ou [!UICONTROL Résolu] (pour les problèmes).

Votre administrateur ou administratrice [!DNL Adobe Workfront] peut personnaliser les statuts associés au bouton [!UICONTROL Terminé] et appliquer ces personnalisations à votre équipe interne.

Selon le nombre de statuts associés au bouton [!UICONTROL Terminé] ou le nombre de ressources affectées à la tâche ou au problème, l’aspect du bouton [!UICONTROL Terminé] peut changer.

* [Bouton [!UICONTROL Terminé] associé à un statut](#done-button-associated-with-one-status)
* [Bouton [!UICONTROL Terminé] associé à plusieurs statuts](#done-button-associated-with-multiple-statuses)
* [Bouton [!UICONTROL Terminé] pour les éléments affectés à plusieurs ressources](#done-button-for-items-assigned-to-multiple-resources)

### Bouton [!UICONTROL Terminé] associé à un statut

Lorsque le bouton [!UICONTROL Terminé] est associé à un statut et que l’élément de travail ne vous est affecté qu’à vous, le bouton indique **[!UICONTROL Terminé]**. Lorsque vous cliquez sur ce bouton, le statut de la tâche ou du problème passe au statut associé au bouton [!UICONTROL Terminé].

![Bouton Terminé](assets/Done.png)

Pour savoir quel statut est associé au bouton [!UICONTROL Terminé], vérifiez les [!UICONTROL Paramètres d’équipe] de votre équipe interne pour la section [!UICONTROL Bouton Terminé], comme décrit dans [Modifier les paramètres d’équipe](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

Si vous n’avez pas d’affectation à une équipe interne, le statut par défaut est choisi lorsque vous cliquez sur [!UICONTROL Terminé], comme décrit ci-dessus dans [Comprendre les options du bouton [!UICONTROL Terminé]](#understand-the-options-of-the-done-button).

### Bouton [!UICONTROL Terminé] associé à plusieurs statuts

Lorsque le bouton [!UICONTROL Terminé] est associé à plusieurs statuts, le bouton affiche le mot **[!UICONTROL Terminé]** qui est suivi d’un menu déroulant. Dans ce cas, vous ne pouvez pas simplement cliquer sur [!UICONTROL Terminé]. Vous devez sélectionner un statut dans le menu déroulant. Sélectionnez le statut qui correspond le mieux à l’achèvement de l’élément de travail. Ce faisant, vous modifiez le statut de l’élément de travail.

Pour comprendre comment vous pouvez associer plusieurs statuts au bouton [!UICONTROL Terminé], voir [Configurer le bouton [!UICONTROL Terminé] pour les tâches](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) et [Configurer le bouton [!UICONTROL Terminé] pour les problèmes](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### Bouton [!UICONTROL Terminé] pour les éléments affectés à plusieurs ressources

Lorsque la tâche ou le problème est affecté à plus d’une ressource, le bouton affiche le mot **[!UICONTROL Terminé]** suivi d’un menu déroulant. Dans le menu déroulant, vous pouvez choisir entre **[!UICONTROL J’ai fait ma part]** (qui indique aux personnes membres de l’équipe que vous avez terminé votre partie de la tâche) ou le statut associé au bouton [!UICONTROL Terminé] (qui termine l’élément). Lorsque vous avez sélectionné **[!UICONTROL J’ai fait ma part]**, l’élément de travail est supprimé de votre liste de travail, mais reste dans celle des personnes encore affectées à l’élément de travail.\
Si le bouton Terminé est associé à plusieurs statuts, ceux-ci sont répertoriés sous **J’ai fait ma part**.

>[!NOTE]
>
>Dans le cas d’une tâche ou d’un problème comportant plusieurs personnes cessionnaires, chaque personne est tenue d’indiquer que sa propre affectation sur la tâche ou le problème est effectivement terminée. C’est la raison pour laquelle chaque personne cessionnaire doit cliquer sur [!UICONTROL Terminé] pour montrer qu’elle a terminé le travail qui lui a été assigné sur l’élément.

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
