---
product-area: workfront-integrations;projects
keywords: google,doc,document,feuille,diapositive
navigation-topic: workfront-for-g-suite
title: Créer un  [!DNL Adobe Workfront]  dans Google Workspace à l’aide du contenu d’un e-mail
description: Vous pouvez convertir un e-mail externe (non généré par  [!DNL Adobe Workfront)]  en problème  [!DNL Workfront] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 80%

---

# Créer un problème [!DNL Adobe Workfront] dans [!DNL Google Workspace] à l’aide du contenu d’un e-mail

>[!NOTE]
>
>La dernière version en date du plug-in Adobe Workfront pour Google a été publiée le 26 juin 2023.

Vous pouvez convertir un e-mail externe (non généré par [!DNL Adobe Workfront]) en problème [!DNL Workfront].

Vous pouvez également convertir un e-mail externe en une mise à jour sur un problème existant. Pour plus d’informations, voir [ [!DNL Adobe Workfront]  Mettre à jour un élément à partir de [!DNL Google Workspace] utiliser le contenu de l’e-mail](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Pour plus d’informations sur l’utilisation de [!DNL Google Workspace] pour travailler avec les e-mails de notification envoyés par [!DNL Workfront], voir [Gérer [!DNL Adobe Workfront] les détails des notifications depuis [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
   </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Avant de créer un problème à partir de [!DNL Google Workspace], vous devez

* installer [!DNL Workfront for Google Workspace].\
   Pour obtenir des instructions, voir [Installer  [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Créer un problème [!DNL Adobe Workfront] dans [!DNL Google Workspace] à l’aide du contenu d’un e-mail

1. Si le panneau [!UICONTROL Workfront for Google Workspace] n’est pas affiché, cliquez sur l’icône [!DNL Workfront] ![Workfront](assets/wf-lion-icon.png) dans la barre latérale [!DNL Google Workspace] modules complémentaires située à l’extrême droite de la page.
1. Avec le message de l’e-mail ouvert dans [!DNL Google Workspace], cliquez sur une option dans [!DNL Workfront for Google Workspace] pour convertir l’e-mail en un nouveau problème [!DNL Workfront].

   ![Convertir l’e-mail](assets/convert-email-task-issue-update.png)

1. Si vous souhaitez joindre le problème à un projet parent, cliquez sur **[!UICONTROL Nom du projet]**, commencez à saisir le nom du projet dans lequel vous souhaitez obtenir le problème, puis cliquez sur le nom du projet lorsqu’il apparaît dans la liste ci-dessous.
1. Apportez l’une des modifications suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Issue Name]</td> 
      <td>Modifiez n’importe quelle partie de ce texte qui provient de l’objet de l’e-mail.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Modifiez n’importe quelle partie de ce texte qui provient du corps de l’e-mail.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Assign To]</td> 
      <td>Cliquez sur <strong>[!UICONTROL Assign To]</strong>, cliquez sur l’option <strong>[!UICONTROL Assign this to]</strong> qui s’affiche, puis commencez à saisir le nom de la personne et cliquez dessus lorsqu’il apparaît dans la liste ci-dessous. Répétez cette opération pour chaque personne à ajouter, puis cliquez sur <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Cliquez sur la flèche déroulante, puis sur la priorité que vous souhaitez obtenir pour le problème.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td> <p>(Disponible uniquement si l’e-mail contient au moins une pièce jointe.) Cliquez sur cette option pour enregistrer les pièces jointes de l’e-mail dans la zone [!UICONTROL Documents] du problème. </p> <p>Si vous ne souhaitez pas enregistrer une pièce jointe, cliquez sur le X situé à droite de son nom. </p> <p>Si l’e-mail contient des liens vers des documents dans [!DNL Google Drive], ils sont enregistrés dans l’onglet [!UICONTROL Overview] du problème que vous créez. </p> <p>Important : pour que cela fonctionne, votre administrateur ou administratrice [!DNL Workfront] doit autoriser [!DNL Google Drive] à utiliser des documents dans [!DNL Workfront], tel que décrit dans la section <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurer des intégrations pour gérer des documents</a> dans l’article <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurer des intégrations de documents</a>.</p> <p>Si vous activez cette option, elle reste activée pour les autres e-mails que vous convertissez en tâches, problèmes et mises à jour.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Inclure le fichier e-mail</td> 
      <td> <p>Cliquez sur cette option pour enregistrer l’e-mail d’origine comme fichier e-mail (EML) (Email) <span>dans la zone [!UICONTROL Documents]</span> du problème. À partir de là, vous pouvez double-cliquer sur le fichier pour ouvrir l’e-mail dans votre application de messagerie.</p> <p>Si vous activez cette option, elle reste activée pour les autres e-mails que vous convertissez en tâches, problèmes et mises à jour.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Créer un problème]**.

   L’onglet **[!UICONTROL Détails]** du nouveau problème s’affiche dans le panneau [!DNL Workfront for Google Workspace]. Cliquez sur **[!UICONTROL Mises à jour]** et commencer à communiquer immédiatement avec les collaborateurs et collaboratrices sans quitter votre zone.

   Au bas de l’onglet **[!UICONTROL Détails]**, vous pouvez également cliquer sur **[!UICONTROL Afficher dans Workfront]** pour accéder au nouveau problème dans Workfront.

   Lorsque vous actualisez votre navigateur, un message contenant un lien en bas du panneau [!UICONTROL Workfront for Google Workspace] confirme que vous avez converti l’e-mail en problème :

   Vous pouvez cliquer sur le lien afin d’accéder à la vue Détails, dans le panneau [!DNL Workfront for Google Workspace], pour le problème que vous avez créé.

   Vous pouvez répéter ces étapes pour convertir le même e-mail en plusieurs problèmes. Lorsque vous actualisez votre navigateur ou revenez à l’e-mail à un autre moment, tous les liens que vous avez créés pour l’e-mail sont répertoriés au bas du panneau [!UICONTROL Workfront pour Google Workspace].

1. (Facultatif) Continuez à travailler sur le problème dans le panneau [!DNL Workfront for Google Workspace] en effectuant l’une des opérations suivantes :

   * Pour ajouter une mise à jour à l’onglet **[!UICONTROL Mises à jour]**, cliquez sur **[!UICONTROL Démarrer une nouvelle mise à jour]** et saisissez la mise à jour.

   * Pour répondre à une mise à jour de l’onglet **[!UICONTROL Mises à jour]**, cliquez sur **[!UICONTROL Répondre]** et saisissez votre réponse.

     Pour les deux actions ci-dessus, vous pouvez informer des personnes spécifiques de votre commentaire. Cliquez sur **[!UICONTROL Notifier]**, commencez à saisir le nom d’un utilisateur ou d’utilisatrice, puis cliquez sur celui-ci lorsqu’il apparaît dans la liste déroulante. Répétez cette procédure pour les autres utilisateurs et utilisatrices que vous souhaitez notifier, puis cliquez sur **[!UICONTROL Publier]**.

   * Cliquez sur l’onglet **[!UICONTROL Documents]** pour afficher tous les documents enregistrés avec le problème.
