---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,diapositive
navigation-topic: workfront-for-g-suite
title: Créez un [!DNL Adobe Workfront] Problème dans G Suite lors de l’utilisation du contenu des emails
description: Vous pouvez convertir un email externe (non généré par [!DNL Adobe Workfront)] à [!DNL Workfront] problème.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%

---

# Créez un [!DNL Adobe Workfront] Problème dans [!DNL G Suite] utilisation du contenu des emails

>[!NOTE]
>
>Il existe une [problème connu](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) avec la version actuelle de [!DNL Workfront for G Suite] ne fonctionne pas comme prévu. Nous travaillons sur une nouvelle version et nous espérons qu’elle sera publiée sur le [!DNL Google Marketplace] dans un avenir proche.

Vous pouvez convertir un email externe (non généré par [!DNL Adobe Workfront]) en [!DNL Workfront] problème.

Vous pouvez également convertir un email externe en une mise à jour sur un problème existant. Pour plus d’informations, voir [Mettre à jour une [!DNL Adobe Workfront] élément de [!DNL G Suite] à l’aide du contenu d’un email](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Pour plus d’informations sur l’utilisation de [!DNL G Suite] pour travailler avec les emails de notification envoyés par [!DNL Workfront], voir [Gérer [!DNL Adobe Workfront] Détails des notifications de [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

Avant de créer un problème à partir de [!DNL G Suite], vous devez

* Installer [!DNL Workfront for G suite]\
   Pour obtenir des instructions, voir [Installer [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Créez un [!DNL Adobe Workfront] Problème dans [!DNL G Suite] utilisation du contenu des emails

1. Si la variable [!UICONTROL Workfront for G Suite] ne s’affiche pas, cliquez sur le bouton [!DNL Workfront] icon ![](assets/wf-lion-icon.png) dans le [!DNL G Suite] la barre latérale des modules complémentaires située à l’extrémité droite de la page.
1. Avec le message électronique ouvert dans [!DNL G Suite], cliquez sur une option dans [!DNL Workfront for G Suite] pour convertir le courrier électronique en un nouveau [!DNL Workfront] problème.

   ![](assets/convert-email-task-issue-update.png)

1. Si vous souhaitez joindre le problème à un projet parent, cliquez sur **[!UICONTROL Nom du projet]**, commencez à saisir le nom du projet dans lequel vous souhaitez obtenir le problème, puis cliquez sur le nom du projet lorsqu’il apparaît dans la liste ci-dessous.
1. Apportez l’une des modifications suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nom du problème]</td> 
      <td>Modifiez toute partie de ce texte qui provient de l’objet de l’email.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Modifiez toute partie de ce texte qui provient du corps de l'email.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Affecter À]</td> 
      <td>Cliquez sur <strong>[!UICONTROL Affecter À]</strong>, cliquez sur le bouton <strong>[!UICONTROL Attribuer à]</strong> qui s’affiche, puis commencez à saisir le nom de la personne et cliquez dessus lorsqu’il apparaît dans la liste ci-dessous. Répétez cette opération pour chaque personne à ajouter, puis cliquez sur <strong>[!UICONTROL Enregistrer]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Cliquez sur la flèche de liste déroulante, puis sur la priorité que vous souhaitez obtenir pour le problème.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Inclure les pièces jointes aux emails]</td> 
      <td> <p>(Disponible uniquement si l’email contient au moins une pièce jointe.) Cliquez sur cette option pour enregistrer les pièces jointes dans le courrier électronique de la zone [!UICONTROL Documents] du problème. </p> <p>Si vous ne souhaitez pas enregistrer une pièce jointe, cliquez sur le X situé à droite de son nom. </p> <p>Si le courrier électronique contient des liens vers des documents dans [!DNL Google Drive], ils sont enregistrés dans l’onglet [!UICONTROL Aperçu] du problème que vous créez. </p> <p>Important : Pour que cela fonctionne, votre [!DNL Workfront] L’administrateur doit autoriser [!DNL Google Drive] pour utiliser des documents dans [!DNL Workfront], comme décrit dans la section <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configuration des intégrations pour gérer les documents</a> dans l’article <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configuration des intégrations de documents</a>.</p> <p>Si vous activez cette option, elle reste activée pour les autres emails que vous convertissez en tâches, problèmes et mises à jour.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Inclure le fichier de courrier électronique</td> 
      <td> <p>Cliquez sur cette option pour enregistrer l’email d’origine en tant que fichier Email (EML) (Email). <span>dans la zone [!UICONTROL Documents].</span> du problème. À partir de là, vous pouvez double-cliquer sur le fichier pour ouvrir l’email dans votre application de messagerie.</p> <p>Si vous activez cette option, elle reste activée pour les autres emails que vous convertissez en tâches, problèmes et mises à jour.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Créer un problème]**.

   Le **[!UICONTROL Détails]** s’affiche dans l’onglet correspondant au nouveau problème. [!DNL Workfront for G Suite] du panneau. Vous pouvez cliquer sur **[!UICONTROL Mises à jour]** et commencer à communiquer avec les collaborateurs immédiatement sans laisser votre boîte.

   Au bas de la **[!UICONTROL Détails]** vous pouvez également cliquer sur **[!UICONTROL Afficher dans Workfront]** pour accéder au nouveau problème dans Workfront.

   Lorsque vous actualisez votre navigateur, un message contenant un lien au bas de la page [!UICONTROL Workfront for G Suite] confirme que vous avez converti le courrier électronique en un problème :

   Vous pouvez cliquer sur le lien pour accéder à la vue Détails, au sein du [!DNL Workfront for G Suite] pour le problème que vous avez créé.

   Vous pouvez répéter ces étapes pour convertir le même email en plusieurs problèmes. Lorsque vous actualisez votre navigateur ou revenez à l’email à un autre moment, tous les liens que vous avez créés pour l’email sont répertoriés au bas de la page [!UICONTROL Workfront for G Suite] du panneau.

1. (Facultatif) Continuez à travailler sur le problème dans le [!DNL Workfront for G Suite] en effectuant l’une des opérations suivantes :

   * Pour ajouter une mise à jour au **[!UICONTROL Mises à jour]** , cliquez sur **[!UICONTROL Démarrer une nouvelle mise à jour]** et saisissez la mise à jour.

   * Pour répondre à une mise à jour de la variable **[!UICONTROL Mises à jour]** , cliquez sur **[!UICONTROL Répondre]** et tapez votre réponse.

      Pour les deux actions ci-dessus, vous pouvez informer des utilisateurs spécifiques de votre commentaire. Cliquez sur **[!UICONTROL Notifier]**, commencez à saisir le nom d’un utilisateur, puis cliquez sur celui-ci lorsqu’il apparaît dans la liste déroulante. Répétez cette procédure pour les autres utilisateurs que vous souhaitez avertir, puis cliquez sur **[!UICONTROL Post]**.

   * Cliquez sur le bouton **[!UICONTROL Documents]** pour afficher tous les documents enregistrés avec le problème.
