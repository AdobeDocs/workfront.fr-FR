---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Remplacez le bouton Travailler dessus par un bouton Démarrer
description: La configuration par défaut d’Adobe Workfront comprend un bouton Travailler dessus pour les tâches et les problèmes qui s’affichent pour les éléments auxquels vous avez été affecté.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Remplacez la variable [!UICONTROL Travailler dessus] avec un bouton [!UICONTROL Début] button

[!DNL Adobe Workfront]La configuration par défaut d’ comprend une [!UICONTROL Travailler dessus] pour les tâches et les problèmes qui s’affichent pour les éléments auxquels vous avez été affecté. Lorsque vous cliquez sur [!UICONTROL Travailler dessus] sur les éléments qui vous sont assignés, vous signalez à d’autres utilisateurs que vous avez reçu le travail et que vous l’aurez réalisé. Toutefois, la variable [!DNL Work On It] ne met pas à jour l’état de la tâche ou du problème pour signaler que le travail a réellement commencé.

Vous pouvez remplacer la variable [!DNL Work On It] avec un bouton [!UICONTROL Début] pour une équipe à laquelle vous appartenez. Dans ce cas, vous pouvez cliquer sur le bouton [!UICONTROL Début] au lieu de [!UICONTROL Travailler dessus], qui met automatiquement à jour l’état et la variable [!UICONTROL Date de début réelle] de l’élément de travail, signalant que vous avez commencé le travail. Pour plus d’informations sur la définition de l’équipe susceptible d’affecter vos modifications dans la variable [!UICONTROL Travailler dessus] , voir la section [Configurez la variable [!UICONTROL Début] button](#configure-the-uicontrol-start-button) dans cet article.

>[!IMPORTANT]
>
>Cliquez sur le bouton [!UICONTROL Début] modifie l’état de l’élément et [!UICONTROL Date de début réelle]. Si une autre personne a commencé à travailler sur une tâche ou un problème (qui a modifié l’état en [!UICONTROL En cours] et renseignait le [!UICONTROL Date de début réelle]), le bouton de l’élément s’affiche sous la forme [!UICONTROL Travailler dessus] même lorsqu’une équipe à laquelle vous appartenez a fait remplacer le bouton par un [!UICONTROL Début] bouton .

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan ou le type de licence dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Configurez la variable [!UICONTROL Début] button

Si vous avez une [!UICONTROL Plan] , vous pouvez configurer la variable [!UICONTROL Début] pour une équipe dans le [!UICONTROL Modifier] la fenêtre de l&#39;équipe. Voici comment fonctionne le bouton après son activation pour une équipe :

* **L’équipe est affectée à un élément de travail.**: Si une équipe est affectée à l’élément de travail, les membres de cette équipe voient le [!UICONTROL Début] et les états configurés pour cette équipe.
* **L’utilisateur appartient à une équipe d’accueil.**: Si aucune équipe n’est affectée à l’élément de travail, mais que l’utilisateur est affecté à une équipe d’accueil dans son profil, l’utilisateur voit l’événement [!UICONTROL Début] et les états configurés pour cette équipe. Il s’agit du scénario que nous vous recommandons si vous souhaitez que les utilisateurs utilisent la variable [!UICONTROL Début] fréquemment.
* **L’utilisateur est affecté à une tâche**: Si aucune équipe n’est affectée à l’élément de travail et qu’aucune équipe d’accueil n’est affectée à l’utilisateur, mais que l’utilisateur est affecté à l’élément de travail, l’utilisateur voit la variable [!UICONTROL Début] et les états combinés configurés pour que toutes les équipes auxquelles elles sont affectées soient affectées.
* **L’utilisateur n’est affecté à aucune équipe :** Si aucune équipe n’est affectée à l’élément de travail et qu’aucune équipe n’est affectée à l’utilisateur, y compris l’équipe d’accueil, et que l’élément est attribué à l’utilisateur, l’utilisateur semble avoir [!UICONTROL Travailler dessus] bouton .

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible dans
>
>* Le [!DNL Workfront] application mobile
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] notifications par e-mail
>


Pour configurer le bouton Démarrer , procédez comme suit :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Équipes]**.

1. Dans le **[!UICONTROL Équipes]** menu déroulant, sélectionnez une équipe.\
   ou\
   Cliquez sur **[!UICONTROL Créer une équipe]**.

1. Cliquez sur le bouton **[!UICONTROL Plus]** icon ![](assets/more-icon.png), puis cliquez sur **[!UICONTROL Modifier]**.

1. Recherchez le **[!UICONTROL Travailler dessus]** section de bouton près du bas de la [!UICONTROL Modifier les équipes] page.
1. Sélectionnez la **[!UICONTROL Remplacez le bouton Travailler dessus par un bouton Démarrer pour mettre automatiquement à jour l’état d’un élément.]** .
1. Sélectionnez un ou plusieurs états pour chaque type d’élément de travail. Si vous sélectionnez plusieurs états, un menu déroulant s’affiche lorsque vous cliquez sur [!UICONTROL Début] où vous pouvez choisir l’état souhaité.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**. Les utilisateurs affichent désormais une [!UICONTROL Tâche de début] ou [!UICONTROL Problème de début] au lieu du bouton [!UICONTROL Travailler dessus] lorsqu’une tâche leur est affectée.

   >[!NOTE]
   >
   >Nous vous recommandons de définir l’équipe en tant qu’équipe d’accueil d’un utilisateur afin que le bouton de démarrage s’affiche sur toutes les tâches qui lui sont affectées. Voir [Association d’utilisateurs à une équipe d’accueil](#associate-users-with-a-home-team) ci-dessous.

## Association d’utilisateurs à une équipe d’accueil

Pour associer des utilisateurs à une équipe d’accueil :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront].

1. Cliquez sur **[!UICONTROL Utilisateurs]**, puis sélectionnez le ou les utilisateurs que vous souhaitez associer à une équipe d’accueil.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Dans le **[!UICONTROL Organisation]** , sélectionnez **[!UICONTROL Équipe Accueil]** champ . Commencez à saisir le nom de l’équipe dont vous souhaitez associer les paramètres aux utilisateurs. Cliquez sur le nom de l’équipe lorsque vous le voyez dans la liste.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.\
   Les utilisateurs que vous avez sélectionnés sont désormais associés à une équipe d’accueil.

   Tous les paramètres de l’équipe, y compris les états associés à la variable [!UICONTROL Terminé] sont désormais visibles par ces utilisateurs.

