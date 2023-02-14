---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,diapositive
navigation-topic: workfront-for-g-suite
title: Mettre à jour une [!DNL Adobe Workfront] élément de la suite G à l’aide du contenu des emails
description: Vous pouvez mettre à jour un projet, une tâche ou un problème existant à l’aide d’informations provenant d’un courrier électronique non Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 0934ae23a8e80dd18872efef7d274bd57d227647
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Mettre à jour une [!DNL Adobe Workfront] item from [!DNL G Suite] utilisation du contenu des emails

>[!NOTE]
>
>Il existe une [problème connu](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) avec la version actuelle de [!DNL Workfront for G Suite] ne fonctionne pas comme prévu. Nous travaillons sur une nouvelle version et nous espérons qu’elle sera publiée sur le [!DNL Google Marketplace] dans un avenir proche.

Vous pouvez mettre à jour un projet, une tâche ou un problème existant à l’aide d’informations provenant d’une[!DNL Adobe Workfront] e-mail.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Avant de pouvoir mettre à jour une [!DNL Workfront] élément à l’aide du contenu d’email provenant de [!DNL G Suite], vous devez

* Installer [!DNL Workfront for G suite]\
   Pour obtenir des instructions, voir [Installer [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Mettre à jour une [!DNL Workfront] élément à l’aide du contenu d’email provenant de [!DNL G Suite]

1. Si la variable [!UICONTROL Workfront for G Suite] ne s’affiche pas, cliquez sur l’icône Workfront ![](assets/wf-lion-icon.png) dans le [!DNL G Suite] la barre latérale des modules complémentaires située à l’extrémité droite de la page.
1. Avec le message électronique ouvert dans [!DNL G Suite], cliquez sur **[!UICONTROL Publier comme nouvelle mise à jour]** dans le [!DNL G Suite] du panneau.
1. Sous **[!UICONTROL Type]**, cliquez sur la flèche déroulante, puis sur le type d’objet dans lequel vous souhaitez ajouter la mise à jour.
1. Cliquez sur le bouton **[!UICONTROL Rechercher]** , commencez à saisir le nom de l’objet auquel vous souhaitez ajouter la mise à jour, puis sélectionnez l’élément lorsqu’il apparaît dans la liste ci-dessous.

   ![](assets/click-search-for-task-issue.png)

   Cette option varie en fonction de ce que vous avez sélectionné à l’étape 3. Il se peut que **[!UICONTROL Recherche d’un projet]**, **[!UICONTROL Recherche d’une tâche]** ou **[!UICONTROL Recherche d’un problème]**.

   >[!NOTE]
   >
   >Lorsque vous saisissez le nom d’une tâche, les tâches personnelles ad hoc sont exclues de la liste de noms qui s’affiche ci-dessous.

1. Effectuez l’une de ces modifications facultatives :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Update]</td> 
      <td>Modifiez toute partie de ce texte, qui provient de l’objet et du corps du message.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Inclure les pièces jointes aux emails]</td> 
      <td><p>(Disponible uniquement si l’email contient au moins une pièce jointe.) Cliquez sur cette option pour enregistrer les pièces jointes dans l’onglet [!UICONTROL Documents] de la tâche ou du problème. </p><p>Si vous ne souhaitez pas enregistrer une pièce jointe, cliquez sur le X situé à droite de son nom. </p><p>Si le courrier électronique contient des liens vers des documents dans [!DNL Google Drive], les liens sont enregistrés dans l’onglet [!UICONTROL Aperçu] de la tâche ou du problème que vous créez. </p><p>Important : <span style="color: #ff1493;"><span style="color: #000000;">Pour que cela fonctionne, votre</span></span>[!DNL Workfront] administrator<span style="color: #ff1493;"><span style="color: #000000;"> must [!DNL Google Drive] pour utiliser [!DNL Workfront]</span></span></p>
      <p>Si vous activez cette option, elle reste activée pour les autres emails que vous convertissez en tâches, problèmes et mises à jour.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notifier </td> 
      <td>Cliquez sur <strong>[!UICONTROL Notifier]</strong>, cliquez sur le bouton <strong>[!UICONTROL Recherche d’un utilisateur ou d’une équipe]</strong> qui s’affiche, puis commencez à saisir le nom de la personne ou de l’équipe et cliquez dessus lorsqu’il apparaît dans la liste ci-dessous. Répétez cette opération pour chaque personne et équipe à ajouter, puis cliquez sur <strong>[!UICONTROL Enregistrer]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Mettre à jour]**.

   Lorsque vous actualisez votre navigateur, un message contenant un lien au bas de la page [!DNL Workfront for G Suite] confirme que vous avez converti l&#39;email en une mise à jour :

   ![](assets/email-was-converted-as-update.png)

   Vous pouvez cliquer sur le lien pour accéder au [!UICONTROL Mises à jour] dans [!DNL Workfront] pour l’objet que vous avez spécifié à l’étape 4.

   Vous pouvez répéter ces étapes pour convertir le même email en mises à jour, tâches et problèmes (voir [Création d’un problème Adobe Workfront dans [!DNL G Suite] à l’aide du contenu d’un email](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Lorsque vous actualisez votre navigateur ou revenez à l’email à un autre moment, tous les liens que vous avez créés pour l’email sont répertoriés au bas de la page [!UICONTROL Workfront for G Suite] du panneau.

1. (Facultatif) Continuez à utiliser la mise à jour dans la variable [!DNL Workfront] pour ajouter un composant en effectuant l’une des opérations suivantes :

   * Pour ajouter une autre mise à jour au **[!UICONTROL Mises à jour]** , cliquez sur **[!UICONTROL Démarrer une nouvelle mise à jour]** et saisissez les informations.

   * Pour répondre à une mise à jour de la variable **[!UICONTROL Mises à jour]** , cliquez sur **[!UICONTROL Répondre]** et tapez votre réponse.

      Pour les deux options ci-dessus, vous pouvez cliquer sur **[!UICONTROL Notifier]** pour indiquer les destinataires de la réponse, comme à l&#39;étape 5. Lorsque vous êtes prêt, cliquez sur **[!UICONTROL Post]** pour ajouter la mise à jour ou la réponse.

   * Cliquez sur le bouton **[!UICONTROL Détails]** pour afficher les détails du nouveau projet, de la nouvelle tâche ou du nouveau problème.
