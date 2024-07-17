---
product-area: projects
navigation-topic: use-the-home-area
title: Marquer un élément comme terminé dans la zone d’accueil
description: Vous pouvez marquer une tâche ou un problème comme Terminé si vous êtes la tâche ou la personne désignée pour le problème. Lorsque vous marquez une tâche ou un problème comme Terminé, l’état de la tâche ou du problème passe à Terminé.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 11%

---

# Marquez un élément comme [!UICONTROL Terminé] dans la zone [!UICONTROL Accueil]

Vous pouvez marquer une tâche ou un problème comme Terminé si vous êtes la tâche ou la personne désignée pour le problème. Lorsque vous marquez une tâche ou un problème comme [!UICONTROL Terminé], l’état de la tâche ou du problème est remplacé par [!UICONTROL Terminé].

>[!NOTE]
>
>Vous ne voyez pas le bouton [!UICONTROL Terminé] à moins que vous ne soyez l’une des ressources affectées à la tâche ou au problème.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>Accès [!UICONTROL Edit] aux tâches et aux problèmes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations de contribution ou niveau supérieur pour les tâches et les problèmes sur lesquels vous devez travailler</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Marquer une tâche ou un problème comme [!UICONTROL Terminé]

Seul l’utilisateur affecté à la tâche ou au problème peut le marquer comme [!UICONTROL Terminé].

1. Cliquez sur le **[!UICONTROL menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis sur **[!UICONTROL Accueil]**.
1. Dans la **[!UICONTROL liste de travail]**, recherchez l’un des éléments en attente de traitement.
1. Effectuez l’une des opérations suivantes :

* Cliquez sur **[!UICONTROL Terminé]** sur l’élément de travail.\
   Pour plus d’informations sur l’affichage de ce bouton, voir [Comprendre les options du bouton [!UICONTROL Terminé]](#understand-the-options-of-the-done-button) .

* Sélectionnez l’élément que vous souhaitez marquer comme terminé, puis, dans le panneau de droite, cliquez sur **[!UICONTROL Mettre à jour l’état]**, puis remplacez l’état de l’élément par un état correspondant à [!UICONTROL Complet] ou [!UICONTROL Fermé].

## Comprendre les options du bouton [!UICONTROL Terminé]

Par défaut, lorsque vous cliquez sur le bouton [!UICONTROL Terminé] sur un élément de travail, l’état de cet élément devient [!UICONTROL Terminé] (pour les tâches) ou [!UICONTROL Résolu] (pour les problèmes).

Votre administrateur [!DNL Adobe Workfront] peut personnaliser les états associés au bouton [!UICONTROL Terminé] et appliquer ces personnalisations à votre équipe d’accueil.

Selon le nombre d’états associés au bouton [!UICONTROL Terminé] ou le nombre de ressources affectées à la tâche ou au problème, l’aspect du bouton [!UICONTROL Terminé] peut changer.

* [Bouton [!UICONTROL Terminé] associé à un état](#done-button-associated-with-one-status)
* [Bouton [!UICONTROL Terminé] associé à plusieurs états](#done-button-associated-with-multiple-statuses)
* [Bouton [!UICONTROL Terminé] pour les éléments affectés à plusieurs ressources](#done-button-for-items-assigned-to-multiple-resources)

### Bouton [!UICONTROL Terminé] associé à un état

Lorsque le bouton [!UICONTROL Terminé] est associé à un état et que l’élément de travail vous est attribué uniquement, le bouton indique **[!UICONTROL Terminé]**. Lorsque vous cliquez dessus, l’état de la tâche ou du problème est modifié en état associé au bouton [!UICONTROL Terminé].

![Bouton Terminé](assets/Done.png)

Pour comprendre quel état est associé au bouton [!UICONTROL Terminé], vérifiez les [!UICONTROL Paramètres de l’équipe] de votre équipe d’accueil pour la section [!UICONTROL Bouton Terminé], comme décrit dans la section [Modifier les paramètres de l’équipe](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

Si vous n’êtes pas affecté à une équipe d’accueil, l’état par défaut est sélectionné lorsque vous cliquez sur [!UICONTROL Terminé], comme décrit ci-dessus dans la section [Comprendre les options du bouton [!UICONTROL Terminé]](#understand-the-options-of-the-done-button).

### Bouton [!UICONTROL Terminé] associé à plusieurs états

Lorsque le bouton [!UICONTROL Terminé] est associé à plusieurs états, le bouton affiche le mot **[!UICONTROL Terminé]** suivi d’un menu déroulant. Dans ce scénario, vous ne pouvez pas simplement cliquer sur [!UICONTROL Terminé]. Vous devez sélectionner un état dans le menu déroulant. Sélectionnez l’état qui correspond le mieux à la fin de l’élément de travail. Ce faisant, vous modifiez l’état de l’élément de travail.

Pour comprendre comment vous pouvez associer plusieurs états au bouton [!UICONTROL Terminé], voir [Configuration du bouton [!UICONTROL Terminé] pour les tâches](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) et [Configuration du bouton [!UICONTROL Terminé] pour les problèmes](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### Bouton [!UICONTROL Terminé] pour les éléments affectés à plusieurs ressources

Lorsque la tâche ou le problème est assigné à plusieurs ressources, le bouton affiche le mot **[!UICONTROL Terminé]** suivi d’un menu déroulant. Dans le menu déroulant, vous avez la possibilité de choisir entre **[!UICONTROL Terminé avec ma partie]** (qui indique aux membres de l’équipe que vous avez terminé avec votre partie de la tâche) ou l’état associé au bouton [!UICONTROL Terminé] (qui termine l’élément). Une fois que vous avez sélectionné **[!UICONTROL Terminé avec ma partie]**, l’élément de travail est supprimé de votre liste de tâches, mais reste dans la liste de tâches des tâches toujours affectées à l’élément de travail.\
Si le bouton Terminé est associé à plusieurs états, ils sont répertoriés sous **Terminé avec ma partie**.

>[!NOTE]
>
>Sur une tâche ou un problème avec plusieurs personnes désignées, chaque utilisateur est responsable d’indiquer que sa propre affectation à la tâche ou au problème a été effectivement terminée. Pour cette raison, chaque personne désignée doit cliquer sur [!UICONTROL Terminé] pour afficher qu’elle a terminé le travail qui lui est affecté sur l’élément.

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
