---
product-area: workfront-integrations;projects
keywords: google,doc,document,feuille,diapositive
navigation-topic: workfront-for-g-suite
title: Mettre à jour un  [!DNL Adobe Workfront]  à partir de Google Workspace à l’aide du contenu d’un e-mail
description: Vous pouvez mettre à jour un projet, une tâche ou un problème existant à l’aide d’informations provenant d’un e-mail non lié à Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 68%

---

# Mettre à jour un élément [!DNL Adobe Workfront] de [!DNL Google Workspace] à l’aide du contenu des e-mails

>[!IMPORTANT]
>
>Pour offrir des intégrations plus stables et plus évolutives, nous passons à une approche d’intégration moderne et flexible à l’aide de Workfront Automation and Integration (Fusion). Dans le cadre de ce processus de transition, la fonctionnalité Workfront for Google Workspace suivante ne sera plus disponible après le **28 février 2026** :
>
>* Accès à la fonctionnalité Google Workspace depuis Workfront
>
>* Affichage et gestion des tâches Workfront à partir de Gmail ou du panneau du site Calendrier Google
>
>Nous vous recommandons d’utiliser l’automatisation et l’intégration de Workfront pour les besoins d’intégration de votre entreprise avec Google Workspace.
>
>Pour une présentation de l’automatisation et de l’intégration de Workfront, consultez [Présentation d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Pour plus d’informations sur les fonctionnalités spécifiques des modules d’automatisation et d’intégration de Workfront pour Google Workspace, voir [Modules Gmail](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) et [Modules de calendrier Google](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Vous pouvez mettre à jour un projet, une tâche ou un problème existant à l’aide d’informations provenant d’un e-mail non lié à [!DNL Adobe Workfront].

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p><p>Travail ou supérieur</p>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de pouvoir mettre à jour un élément [!DNL Workfront] à l’aide du contenu d’un e-mail provenant de [!DNL Google Workspace], vous devez

* installer [!DNL Workfront for Google Workspace]\
   Pour plus d’informations, voir [Installer  [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Mettre à jour un élément [!DNL Workfront] à l’aide du contenu d’e-mail provenant de [!DNL Google Workspace]

1. Si le panneau [!UICONTROL Workfront for Google Workspace] n’est pas affiché, cliquez sur l’icône Workfront ![Workfront](assets/wf-lion-icon.png) dans la barre latérale [!DNL Google Workspace] modules complémentaires située à l’extrême droite de la page.
1. Avec le message de l’e-mail ouvert dans [!DNL Google Workspace], cliquez sur **[!UICONTROL Publier comme nouvelle mise à jour]** dans le panneau [!DNL Google Workspace].
1. Sous **[!UICONTROL Type]**, cliquez sur la flèche déroulante, puis sur le type d’objet dans lequel vous souhaitez ajouter la mise à jour.
1. Cliquez sur l’option **[!UICONTROL Rechercher]**, commencez à saisir le nom de l’objet auquel vous souhaitez ajouter la mise à jour, puis sélectionnez l’élément lorsqu’il apparaît dans la liste ci-dessous.

   Cette option varie en fonction de ce que vous avez sélectionné à l’étape 3. Cela peut être **[!UICONTROL Rechercher un projet]**, **[!UICONTROL Rechercher une tâche]**, ou **[!UICONTROL Rechercher un problème]**.

   >[!NOTE]
   >
   >Lorsque vous saisissez le nom d’une tâche, les tâches personnelles ad hoc sont exclues de la liste de noms qui s’affiche ci-dessous.

1. Effectuez l’une de ces modifications facultatives :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Update]</td> 
      <td>Modifiez toute partie de ce texte, qui provient de la ligne d’objet et du corps de texte de l’e-mail.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td><p>(Disponible uniquement si l’e-mail contient au moins une pièce jointe.) Cliquez sur cette option pour enregistrer les pièces jointes dans l'onglet [!UICONTROL Documents] pour la tâche ou l'événement. </p><p>Si vous ne souhaitez pas enregistrer une pièce jointe, cliquez sur le X situé à droite de son nom. </p><p>Si l’e-mail contient des liens vers des documents dans [!DNL Google Drive], les liens sont enregistrés dans l’onglet [!UICONTROL Overview] de la tâche ou du problème que vous créez. </p><p>Important : <span style="color: #ff1493;"><span style="color: #000000;">pour que cela fonctionne, votre adminstrateur ou administratrice </span></span>[!DNL Workfront]<span style="color: #ff1493;"><span style="color: #000000;"> doit autoriser [!DNL Google Drive] à travailler avec [!DNL Workfront]</span></span>.</p>
      <p>Si vous activez cette option, elle reste activée pour les autres e-mails que vous convertissez en tâches, problèmes et mises à jour.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notifier </td> 
      <td>Cliquez sur <strong>[!UICONTROL Notify]</strong>, cliquez sur l’option <strong>[!UICONTROL Search for a user or team]</strong> qui s’affiche, puis commencez à saisir le nom de la personne ou de l’équipe et cliquez dessus lorsqu’il apparaît dans la liste ci-dessous. Répétez cette opération pour chaque personne et équipe à ajouter, puis cliquez sur <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Mettre à jour]**.

   Lorsque vous actualisez votre navigateur, un message contenant un lien au bas du panneau [!DNL Workfront for Google Workspace] confirme que vous avez converti l’e-mail en une mise à jour :

   Vous pouvez cliquer sur le lien pour accéder à l’onglet [!UICONTROL Mises à jour] dans [!DNL Workfront] pour l’objet spécifié à l’étape 4.

   Vous pouvez répéter ces étapes pour convertir le même e-mail en mises à jour, tâches et problèmes (voir [Création d’un problème Adobe Workfront dans [!DNL Google Workspace] à l’aide du contenu de l’e-mail](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Lorsque vous actualisez votre navigateur ou revenez à l’e-mail à un autre moment, tous les liens que vous avez créés pour l’e-mail sont répertoriés au bas du panneau [!UICONTROL Workfront pour Google Workspace].

1. (Facultatif) Continuez à utiliser la mise à jour dans le panneau du module complémentaire [!DNL Workfront] en effectuant l’une des opérations suivantes :

   * Pour ajouter une autre mise à jour sur l’onglet **[!UICONTROL Mises à jour]**, cliquez sur **[!UICONTROL Démarrer une nouvelle mise à jour]** et saisissez les informations.

   * Pour répondre à une mise à jour sur l’onglet **[!UICONTROL Mises à jour]**, cliquez sur **[!UICONTROL Répondre]** et saisissez votre réponse.

     Pour les deux options ci-dessus, vous pouvez cliquer sur **[!UICONTROL Notifier]** pour indiquer les destinataires de la réponse, comme à l’étape 5. Une fois cette étape effectuée, cliquez sur **[!UICONTROL Publier]** pour ajouter la mise à jour ou la réponse.

   * Cliquez sur l’onglet **[!UICONTROL Détails]** pour afficher les détails du nouveau projet, de la nouvelle tâche ou du nouveau problème.
