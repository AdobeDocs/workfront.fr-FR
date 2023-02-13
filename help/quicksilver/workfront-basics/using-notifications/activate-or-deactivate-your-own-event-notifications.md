---
product-area: setup
navigation-topic: notifications
title: Activation ou désactivation de vos propres notifications d’événement
description: Votre administrateur Adobe Workfront configure les notifications d’événement que les utilisateurs reçoivent lorsqu’un événement se produit dans Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: ea16b13b6ecb6ecea365c6c4d31ee23b7bb712c6
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# Activation ou désactivation de vos propres notifications d’événement

Votre Adobe [!DNL Workfront] L’administrateur configure les notifications d’événement que reçoivent les utilisateurs lorsqu’un événement se produit dans Workfront (comme décrit dans la section [[!UICONTROL Configurer un événement] notifications destinées à tous les utilisateurs du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

L’administrateur de votre groupe peut également configurer les notifications d’événement qui sont activées pour vous et les utilisateurs de votre groupe d’accueil. Si votre [!UICONTROL Groupe d’accueil] est un sous-groupe, vous recevez les notifications d’événement activées pour le groupe de niveau supérieur au-dessus de votre groupe.

Vous pouvez personnaliser davantage cela en configurant les notifications que vous recevez. Vous pouvez également choisir de recevoir des notifications au fur et à mesure des événements ou dans un email quotidien de résumé.

Pour plus d’informations sur les notifications électroniques, voir [[!DNL Adobe Workfront] notifications](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Si vous activez un type de notification puis constatez que vous ne recevez pas de notifications de ce type, c’est peut-être parce que ce type ne s’applique pas à votre rôle.
>* Le [!DNL Workfront] un administrateur ou un administrateur de groupe ne peut pas configurer de notifications pour [!DNL Workfront Goals]. Pour plus d’informations sur les notifications de la variable [!DNL Workfront] l’administrateur peut configurer, voir [Configuration des notifications d’événement pour tous les membres du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Pour plus d’informations sur la configuration de notifications individuelles pour [!DNL Workfront Goals] continuez à lire cet article.
>


## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan ou le type de licence dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Afficher et modifier vos paramètres de notification électronique

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur votre nom d’utilisateur en regard de votre image de profil.

1. Cliquez sur le bouton **[!UICONTROL Plus]** icon ![](assets/more-icon.png) , puis cliquez sur **[!UICONTROL Modifier]**.

1. Dans le **[!UICONTROL Modifier la personne]** qui s’affiche, accédez à la **[!UICONTROL Notifications]** .

1. Cliquez sur une catégorie pour afficher les paramètres de notification associés à cette catégorie.

   ![](assets/my-profile-notifications.png)

1. Cochez ou décochez les cases à droite pour indiquer si vous souhaitez recevoir ou non des notifications quotidiennement, instantanément ou les deux.

   Vous pouvez également utiliser les cases à cocher d’une catégorie pour activer ou désactiver toutes les notifications de cette catégorie.

   >[!NOTE]
   >
   >Si vous êtes membre de l’équipe d’un projet, vous continuez à recevoir des notifications par courrier électronique jusqu’à ce que vous soyez supprimé de l’équipe, même si vous n’avez plus accès au projet. Pour obtenir des instructions sur la suppression d’utilisateurs d’une équipe, voir [Suppression des utilisateurs des projets](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   Pour le **[!UICONTROL Communication]** vous pouvez sélectionner des notifications individuelles pour une diffusion instantanée uniquement. Pour que les notifications soient diffusées dans un résumé quotidien, vous devez tous les sélectionner.

   Si toutes les notifications électroniques d’une catégorie donnée sont activées, la case du titre de la catégorie apparaît comme étant sélectionnée. Si toutes les notifications électroniques d’une catégorie donnée sont désactivées, la case est désélectionnée. Si certaines notifications sont activées et que d’autres sont désactivées, la case à cocher de catégorie s’affiche en ligne droite.\
   Lorsque vous modifiez un paramètre de notification, le libellé **[!UICONTROL Modifié]** s’affiche pour ce paramètre de notification afin de vous informer que ce paramètre de notification a été modifié.

1. Si vous avez sélectionné des notifications à envoyer sous forme de résumé quotidien, sélectionnez l’heure de la journée à laquelle vous souhaitez la recevoir en haut de la page **[!UICONTROL Notifications]** dans la section **[!UICONTROL Email Daily Digest après]** .

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   Le résumé quotidien comprend les événements qui répondent aux critères des notifications 24 heures avant l’heure sélectionnée. Vous recevez un courrier électronique condensé quotidien pour chaque type de notification.\
   Le résumé quotidien peut arriver après la période sélectionnée, selon le nombre d&#39;emails placés en file d&#39;attente pour diffusion dans le système. L’heure indiquée correspond à l’heure locale spécifiée dans les paramètres du navigateur.

1. (Conditionnel et facultatif) Lors de la modification des paramètres des notifications électroniques dans l’environnement Aperçu, activez la variable **[!UICONTROL Réception d’emails à partir de cet environnement de test]** pour recevoir des emails. Les emails ne sont pas générés automatiquement à partir de l&#39;environnement Aperçu .

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
