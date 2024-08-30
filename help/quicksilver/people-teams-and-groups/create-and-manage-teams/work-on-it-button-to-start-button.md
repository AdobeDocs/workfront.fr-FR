---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Remplacement du bouton Travailler dessus par un bouton Démarrer
description: La configuration par défaut d’Adobe Workfront comprend un bouton Travailler sur ce projet pour les tâches et les problèmes qui s’affiche pour les éléments qui vous ont été attribués.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 97%

---

# Remplacer le bouton [!UICONTROL Travailler sur ce projet] par un bouton [!UICONTROL Démarrer] 

La configuration par défaut d’[!DNL Adobe Workfront] comprend un bouton [!UICONTROL Travailler sur ce projet] pour les tâches et les problèmes qui s’affichent pour les éléments qui vous ont été attribués. Lorsque vous cliquez sur [!UICONTROL Travailler sur ce projet] sur les éléments qui vous sont attribués, vous signalez aux autres utilisateurs et utilisatrices que vous avez reçu le travail et que vous vous engagez à travailler dessus. Cependant, le bouton [!DNL Work On It] ne met pas à jour le statut de la tâche ou du problème pour signaler que le travail a réellement commencé.

Vous pouvez remplacer le bouton [!DNL Work On It] par un bouton [!UICONTROL Démarrer] pour une équipe à laquelle vous appartenez. Dans ce cas, vous cliquez sur le bouton [!UICONTROL Démarrer] au lieu de [!UICONTROL Travailler sur ce projet], ce qui met automatiquement à jour le statut et la [!UICONTROL Date de début effective] de l’élément de travail, signalant que vous avez commencé à travailler. Pour plus d’informations sur les paramètres de l’équipe susceptible d’affecter vos modifications dans le bouton [!UICONTROL Travailler sur ce projet], voir la section [Configurer le bouton [!UICONTROL Démarrer]](#configure-the-uicontrol-start-button) de cet article.

>[!IMPORTANT]
>
>Un clic sur le bouton [!UICONTROL Démarrer] modifie le statut de l’élément et la [!UICONTROL Date de début effectif]. Si quelqu’un d’autre a commencé à travailler sur une tâche ou un problème (qui a changé le statut en [!UICONTROL En cours] et rempli la [!UICONTROL Date de début effectif]), le bouton de l’élément s’affiche comme [!UICONTROL Travailler sur ce projet] même si le bouton d’une équipe à laquelle vous appartenez a été remplacé par un bouton [!UICONTROL Démarrer].

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer le bouton [!UICONTROL Démarrer]

Si vous disposez d’une licence [!UICONTROL Forfait], vous pouvez configurer le bouton [!UICONTROL Démarrer] pour une équipe dans la fenêtre [!UICONTROL Modifier l’équipe]. Voici comment fonctionne le bouton une fois qu’il a été activé pour une équipe :

* **L’équipe est affectée à un élément de travail** : si une équipe est affectée à l’élément de travail, les membres de cette équipe voient le bouton [!UICONTROL Démarrer] et les statuts configurés pour cette équipe.
* **L’utilisateur ou l’utilisatrice fait partie d’une équipe d’accueil** : si aucune équipe n’est assignée à l’élément de travail mais que la personne est assignée à une équipe d’accueil dans son profil, celle-ci verra le bouton [!UICONTROL Démarrer] et les statuts configurés pour cette équipe. C’est le scénario que nous recommandons si vous voulez que les utilisateurs et utilisatrices utilisent fréquemment le bouton [!UICONTROL Démarrer].
* **L’utilisateur ou l’utilisatrice est affecté à un élément de travail** : si aucune équipe n’est affectée à l’élément de travail et aucune équipe d’acueil n’est affectée à l’utilisateur/utilisatrice, mais que la personne est affectée à l’élément de travail, celle-ci verra le bouton [!UICONTROL Démarrer] et les statuts combinés configurés pour toutes les équipes auxquelles elle est affectée.
* **L’utilisateur ou l’utilisatrice n’est affecté à aucune équipe :** s’il n’y a pas d’équipe affectée à l’élément de travail ni d’équipe pour l’utilisateur ou l’utilisatrice, y compris l’équipe d’accueil, et que l’élément est affecté à la personne, celle-ci verra le bouton [!UICONTROL Travailler sur ce projet].

>[!NOTE]
>
>Cette fonction est actuellement indisponible dans
>
>* l’application mobile [!DNL Workfront]
>* [!DNL Workfront for Office 365]
>* les notifications par e-mail [!DNL Workfront]
>

Pour configurer le bouton Démarrer :

{{step1-to-team}}

1. Dans le menu déroulant **[!UICONTROL Équipes]**, sélectionnez une équipe.\
   ou\
   Sélectionnez **[!UICONTROL Créer une équipe]**.

1. Cliquez sur l’icône **[!UICONTROL Plus]** ![](assets/more-icon.png), puis cliquez sur **[!UICONTROL Modifier]**.

1. Vous trouverez le bouton **[!UICONTROL Travailler sur ce projet]** au bas de la page [!UICONTROL Modifier les équipes].
1. Sélectionnez la case à cocher **[!UICONTROL Modifier le bouton « Travailler sur ce projet » en un bouton Démarrer pour mettre à jour automatiquement le statut d’un élément]**.
1. Sélectionnez un ou plusieurs statuts pour chaque type d’élément de travail. Si vous sélectionnez plus d’un statut, un menu déroulant s’affiche lorsque vous cliquez sur [!UICONTROL Démarrer], dans lequel vous pouvez choisir le statut souhaité.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**. Les utilisateurs et utilisatrices voient maintenant un bouton [!UICONTROL Démarrer la tâche] ou [!UICONTROL Démarrer le problème] au lieu du bouton [!UICONTROL Travailler sur ce projet] lorsqu’un élément de travail leur est attribué.

   >[!NOTE]
   >
   >Nous recommandons de définir l’équipe comme l’équipe d’accueil d’un utilisateur ou d’une utilisatrice afin que le bouton de démarrage apparaisse sur tous les éléments de travail qui lui sont attribués. Voir [Associer des utilisateurs et utilisatrices à une équipe d’accueil](#associate-users-with-a-home-team) ci-dessous.

## Associer les utilisateurs et utilisatrices à une équipe d’accueil

Pour associer des utilisateurs et des utilisatrices à une équipe d’accueil :

{{step-1-to-users}}

1. Sélectionnez le ou les utilisateurs que vous souhaitez associer à une équipe d’accueil.
1. Cliquez sur le menu **[!UICONTROL Plus]**, puis sélectionnez **[!UICONTROL Modifier]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Dans la section **[!UICONTROL Organisation]**, sélectionnez le champ **[!UICONTROL Équipe principale]**. Commencez à taper le nom de l’équipe dont vous souhaitez associer les paramètres aux utilisateurs et utilisatrices. Cliquez sur le nom de l’équipe lorsque vous le voyez dans la liste.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.\
   Les personnes que vous avez sélectionnées sont maintenant associées à une équipe interne.

   Tous les paramètres de l’équipe, y compris les statuts associés au bouton [!UICONTROL Terminé], sont désormais visibles pour ces utilisateurs et utilisatrices.

