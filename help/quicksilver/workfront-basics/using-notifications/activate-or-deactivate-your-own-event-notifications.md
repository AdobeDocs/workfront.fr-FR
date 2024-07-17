---
product-area: setup
navigation-topic: notifications
keywords: modify,email,notification,settings
title: Modifier vos propres notifications par e-mail
description: Cet article décrit comment gérer vos notifications électroniques dans votre profil utilisateur.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: f9afe7c8f04777dd547ea1e202e7844bdfd3518e
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 22%

---

# Modifier vos propres notifications par e-mail

<!-- Audited: 1/2024 -->

Votre administrateur [!DNL Workfront] de l&#39;Adobe configure les notifications électroniques que reçoivent les utilisateurs lorsqu&#39;un événement se produit dans Workfront (comme décrit dans la section [[!UICONTROL Configurer les notifications d&#39;événement] pour tous les utilisateurs du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

L’administrateur de votre groupe peut également configurer les notifications qui sont activées pour vous et les utilisateurs de votre [!UICONTROL groupe d’accueil]. Si votre [!UICONTROL groupe d’accueil] est un sous-groupe, vous recevez les notifications activées pour le groupe de niveau supérieur au-dessus de votre groupe.

Vous pouvez personnaliser davantage cela en configurant les notifications que vous recevez. Vous pouvez également choisir de recevoir des notifications au fur et à mesure des événements ou dans un email quotidien de résumé.

Pour plus d’informations sur les notifications par e-mail, voir [[!DNL Adobe Workfront] notifications](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Si vous activez un type de notification puis constatez que vous ne recevez pas de notifications de ce type, c’est peut-être parce que ce type ne s’applique pas à votre rôle.
>* L&#39;administrateur [!DNL Workfront] ou un administrateur de groupe ne peut pas configurer de notifications pour [!DNL Workfront Goals]. Pour plus d&#39;informations sur les notifications que l&#39;administrateur [!DNL Workfront] peut configurer, voir [Configuration des notifications d&#39;événement pour tous les membres du système](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Pour plus d’informations sur la configuration des notifications individuelles pour [!DNL Workfront Goals], consultez cet article.
>

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence</strong></td> 
   <td>  <p>Nouveau :</p> 
   <ul><li>Contributeur ou version ultérieure</li></ul>
   <p>Actuel :</p>
   <ul><li>Requête ou supérieure</li></ul>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher et modifier vos paramètres de notification électronique

{{step1-click-profile-pic}}

1. Cliquez sur l’icône **[!UICONTROL Plus]** ![](assets/more-icon.png) en regard de votre nom, puis cliquez sur **[!UICONTROL Modifier]**.

1. Dans la zone **[!UICONTROL Modifier la personne]** qui s’affiche, accédez à la section **[!UICONTROL Notifications]** .

1. Cliquez sur une catégorie pour afficher les paramètres de notification associés à cette catégorie.

   ![](assets/my-profile-notifications.png)

1. Cochez ou décochez les cases à droite pour indiquer si vous souhaitez recevoir ou non des notifications quotidiennement, instantanément ou les deux.

   Vous pouvez également cocher les cases d’une catégorie pour activer ou désactiver toutes les notifications de cette catégorie.

   >[!NOTE]
   >
   >Si vous êtes membre de l’équipe d’un projet, vous continuez à recevoir des notifications par courrier électronique jusqu’à ce que vous soyez supprimé de l’équipe, même si vous n’avez plus accès au projet. Pour obtenir des instructions sur la suppression des utilisateurs d’une équipe, voir [Suppression des utilisateurs des projets](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   Pour la catégorie **[!UICONTROL Communication]**, vous pouvez sélectionner des notifications individuelles pour une diffusion instantanée uniquement. Pour que les notifications soient diffusées dans un résumé quotidien, vous devez tous les sélectionner.

   Si toutes les notifications électroniques d’une catégorie donnée sont activées, la case du titre de la catégorie apparaît comme étant sélectionnée. Si toutes les notifications électroniques d’une catégorie donnée sont désactivées, la case est désélectionnée. Si certaines notifications sont activées et que d’autres sont désactivées, la case à cocher de catégorie s’affiche en ligne droite.\
   Lorsque vous modifiez un paramètre de notification, le libellé **[!UICONTROL Modifié]** s’affiche pour ce paramètre de notification afin de vous informer que ce paramètre de notification a été modifié.

1. Si vous avez sélectionné des notifications à envoyer sous forme de résumé quotidien, sélectionnez l’heure de la journée à laquelle vous souhaitez la recevoir en haut de la section **[!UICONTROL Notifications]** dans le menu **[!UICONTROL Email Daily Digest after]** .

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   La synthèse quotidienne comprend les événements qui répondent aux critères des notifications 24 heures avant l’heure sélectionnée. Vous recevez un courrier électronique condensé quotidien pour chaque type de notification.\
   La synthèse quotidienne peut arriver après l’heure sélectionnée, selon le nombre d’e-mails placés en file d’attente pour diffusion dans le système. L’heure indiquée correspond à l’heure locale spécifiée dans les paramètres du navigateur.

1. (Conditionnel et facultatif) Lors de la modification des paramètres des notifications électroniques dans l’environnement Aperçu, activez le paramètre **[!UICONTROL Recevoir les emails de cet environnement de test]** pour recevoir des emails. Les emails ne sont pas générés automatiquement à partir de l&#39;environnement Aperçu .

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
