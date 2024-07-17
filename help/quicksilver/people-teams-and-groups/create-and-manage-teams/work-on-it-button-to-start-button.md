---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Remplacer le bouton Travailler sur ce projet par un bouton Démarrer
description: La configuration par défaut d’Adobe Workfront comprend un bouton Travailler dessus pour les tâches et les problèmes qui s’affichent pour les éléments auxquels vous avez été affecté.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 13%

---

# Remplacez le bouton [!UICONTROL Work On It] par un bouton [!UICONTROL Start]

La configuration par défaut de [!DNL Adobe Workfront] comprend un bouton [!UICONTROL Travailler dessus] pour les tâches et les problèmes qui s’affichent pour les éléments auxquels vous avez été affecté. Lorsque vous cliquez sur [!UICONTROL Travailler dessus] sur les éléments qui vous sont affectés, vous signalez aux autres utilisateurs que vous avez reçu le travail et que vous reconnaissez que vous y travaillerez. Cependant, le bouton [!DNL Work On It] ne met pas à jour l’état de la tâche ou du problème pour signaler que le travail a réellement commencé.

Vous pouvez remplacer le bouton [!DNL Work On It] par un bouton [!UICONTROL Démarrer] pour une équipe à laquelle vous appartenez. Dans ce cas, vous cliquez sur le bouton [!UICONTROL Démarrer] au lieu de [!UICONTROL Travailler dessus], ce qui met automatiquement à jour l’état et la [!UICONTROL Date de début réelle] de l’élément de travail, indiquant que vous avez commencé le travail. Pour plus d’informations sur la définition de l’équipe susceptible d’affecter vos modifications dans le bouton [!UICONTROL Travailler dessus], voir la section [Configuration du bouton [!UICONTROL Démarrer]](#configure-the-uicontrol-start-button) de cet article.

>[!IMPORTANT]
>
>Cliquer sur le bouton [!UICONTROL Démarrer] modifie l’état de l’élément et la [!UICONTROL Date de début réelle]. Si quelqu’un d’autre a commencé à travailler sur une tâche ou un problème (qui a changé l’état de [!UICONTROL En cours] et renseigné la [!UICONTROL Date de début réelle]), le bouton de l’élément s’affiche sous la forme [!UICONTROL Travail sur cette tâche] même lorsqu’une équipe à laquelle vous appartenez a fait remplacer le bouton par un bouton [!UICONTROL Démarrer].

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir quel plan ou type de licence vous avez, contactez votre administrateur [!DNL Workfront].

## Configuration du bouton [!UICONTROL Démarrer]

Si vous disposez d’une licence [!UICONTROL Plan], vous pouvez configurer le bouton [!UICONTROL Démarrer] pour une équipe dans la fenêtre [!UICONTROL Modifier] de l’équipe. Voici comment fonctionne le bouton après son activation pour une équipe :

* **L’équipe est affectée à un élément de travail** : si une équipe est affectée à l’élément de travail, les membres de cette équipe voient le bouton [!UICONTROL Démarrer] et les états configurés pour cette équipe.
* **L’utilisateur appartient à une équipe d’accueil** : si aucune équipe n’est affectée à l’élément de travail, mais que l’utilisateur est affecté à une équipe d’accueil dans son profil, l’utilisateur voit le bouton [!UICONTROL Démarrer] et les états configurés pour cette équipe. Il s’agit du scénario que nous vous recommandons si vous souhaitez que les utilisateurs utilisent fréquemment le bouton [!UICONTROL Démarrer] .
* **L’utilisateur est affecté à un élément de travail** : si aucune équipe n’est affectée à l’élément de travail et qu’aucune équipe d’accueil n’est affectée à l’utilisateur, mais que l’utilisateur est affecté à l’élément de travail, l’utilisateur voit le bouton [!UICONTROL Démarrer] et les états combinés configurés pour que toutes les équipes auxquelles il est affecté.
* **L’utilisateur n’est assigné à aucune équipe :** Si aucune équipe n’est affectée à l’élément de travail et qu’aucune équipe n’est affectée à l’utilisateur, y compris l’équipe d’accueil, et que l’élément est attribué à l’utilisateur, l’utilisateur affiche le bouton [!UICONTROL Travailler dessus].

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible dans
>
>* L&#39;application mobile [!DNL Workfront]
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] notifications électroniques
>

Pour configurer le bouton Démarrer , procédez comme suit :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Equipes]**.

1. Dans le menu déroulant **[!UICONTROL Équipes]**, sélectionnez une équipe.\
   ou\
   Cliquez sur **[!UICONTROL Créer une équipe]**.

1. Cliquez sur l&#39;icône **[!UICONTROL Plus]** ![](assets/more-icon.png), puis sur **[!UICONTROL Modifier]**.

1. Recherchez la section de bouton **[!UICONTROL Travailler dessus]** près du bas de la page [!UICONTROL Modifier les équipes].
1. Sélectionnez le bouton **[!UICONTROL Remplacer le travail dessus par un bouton Démarrer pour mettre automatiquement à jour l&#39;état d&#39;un élément]** .
1. Sélectionnez un ou plusieurs états pour chaque type d’élément de travail. Si vous sélectionnez plusieurs états, un menu déroulant s’affiche lorsque vous cliquez sur [!UICONTROL Démarrer] pour sélectionner l’état de votre choix.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**. Les utilisateurs voient désormais un bouton [!UICONTROL Démarrer la tâche] ou [!UICONTROL Démarrer le problème] au lieu du bouton [!UICONTROL Travailler dessus] lorsqu’un élément de travail leur est attribué.

   >[!NOTE]
   >
   >Nous vous recommandons de définir l’équipe en tant qu’équipe d’accueil d’un utilisateur afin que le bouton de démarrage s’affiche sur toutes les tâches qui lui sont affectées. Voir [Associer les utilisateurs à une équipe d’accueil](#associate-users-with-a-home-team) ci-dessous.

## Associer des utilisateurs et utilisatrices à une équipe d’accueil

Pour associer des utilisateurs et des utilisatrices à une équipe d’accueil :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront].

1. Cliquez sur **[!UICONTROL Utilisateurs et utilisatrices]**, puis sélectionnez la ou les personnes que vous souhaitez associer à une équipe d’accueil.
1. Cliquez sur le menu **[!UICONTROL Plus]**, puis sélectionnez **[!UICONTROL Modifier]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Dans la section **[!UICONTROL Organisation]**, sélectionnez le champ **[!UICONTROL Équipe d’accueil]**. Commencez à saisir le nom de l’équipe dont vous souhaitez associer les paramètres aux utilisateurs et utilisatrices. Cliquez sur le nom de l’équipe lorsque vous le voyez dans la liste.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.\
   Les utilisateurs que vous avez sélectionnés sont désormais associés à une équipe d’accueil.

   Tous les paramètres de l’équipe, y compris les états associés au bouton [!UICONTROL Terminé], sont désormais visibles par ces utilisateurs.

