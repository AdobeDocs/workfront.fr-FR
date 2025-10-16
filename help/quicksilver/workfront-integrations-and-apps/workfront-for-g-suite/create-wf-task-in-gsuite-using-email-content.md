---
product-area: workfront-integrations;projects
keywords: google,doc,document,feuille,diapositive
navigation-topic: workfront-for-g-suite
title: Création d [!DNL Adobe Workfront] une tâche dans Google Workspace à l’aide du contenu d’un e-mail
description: Vous pouvez convertir un e-mail externe (non généré par Adobe) [!DNL Workfront]) en une tâche Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 76%

---

# Créer une tâche [!DNL Adobe Workfront] dans [!DNL Google Workspace] à l’aide du contenu d’un e-mail

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
>Pour plus d’informations sur les fonctionnalités spécifiques des modules d’automatisation et d’intégration de Workfront pour Google Workspace, voir [Modules Gmail](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) et [Modules de calendrier Google](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Vous pouvez convertir un e-mail externe (non généré par [!DNL Adobe Workfront]) en tâche [!DNL Workfront].

Vous pouvez également convertir un e-mail externe en une mise à jour sur une tâche existante. Pour plus d’informations, voir [&#x200B; [!DNL Adobe Workfront]  Mettre à jour un élément à partir de [!DNL Google Workspace] utiliser le contenu de l’e-mail](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Pour plus d’informations sur l’utilisation de [!DNL Google Workspace] pour travailler avec les e-mails de notification envoyés par [!DNL Workfront], voir [Gérer [!DNL Adobe Workfront] les détails des notifications depuis [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

Avant de pouvoir créer une tâche [!DNL Workfront] dans [!DNL Google Workspace], vous devez :

* Installez [!DNL Workfront for Google Workspace].\
   Pour obtenir des instructions, voir [Installer  [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Créer une tâche [!DNL Adobe Workfront] dans [!DNL Google Workspace] à l’aide du contenu d’un e-mails

1. Si le panneau [!UICONTROL Workfront for Google Workspace] n’est pas affiché, cliquez sur l’icône [!DNL Workfront] ![Workfront](assets/wf-lion-icon.png) dans la barre latérale [!DNL Google Workspace] modules complémentaires située à l’extrême droite de la page.
1. Avec l’e-mail ouvert dans [!DNL Google Workspace], cliquez sur une option dans [!DNL Workfront for Google Workspace] pour convertir l’e-mail en une nouvelle tâche [!DNL Workfront].

1. Sélectionnez une option **[!UICONTROL Créer]** pour indiquer si la tâche va faire partie d’un projet ou d’une tâche personnelle indépendante d’un projet.
1. Si vous souhaitez joindre la tâche à un projet parent, cliquez sur **[!UICONTROL Nom du projet]**, commencez à saisir le nom du projet dans lequel vous souhaitez que la tâche soit effectuée, puis cliquez sur le nom du projet lorsqu’il apparaît dans la liste ci-dessous.
1. Apportez l’une des modifications suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Task name]</td> 
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
      <td role="rowheader">[!UICONTROL Planned duration]</td> 
      <td> <p>Cliquez sur <strong>[!UICONTROL Planned duration]</strong>, puis saisissez le nombre de jours que vous souhaitez que la tâche prenne. </p> <p>Remarque : cette option peut être configurée pour votre organisation de différentes manières. Par exemple, pour votre organisation, vous devrez peut-être saisir un nombre d’heures au lieu de jours. Si vous avez besoin d’informations supplémentaires, contactez votre administrateur ou administratrice [!DNL Workfront]. Si vous souhaitez spécifier une période autre que la valeur par défaut configurée, saisissez <strong>m</strong>, <strong>h</strong>, <strong>j</strong>, <strong>s</strong>, ou <strong>mo</strong> après le nombre pour désigner les minutes, heures, jours, semaines ou mois.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Cliquez sur la flèche de liste déroulante, puis sur la priorité à donner à la tâche.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td> <p>(Disponible uniquement si l’e-mail contient au moins une pièce jointe.) Cliquez sur cette option pour enregistrer les pièces jointes de l'e-mail dans la zone [!UICONTROL Documents] de la tâche. </p> <p>Si vous ne souhaitez pas enregistrer une pièce jointe, cliquez sur le X situé à droite de son nom. </p> <p>Si l’e-mail contient des liens vers des documents dans [!DNL Google Drive], ils sont enregistrés dans l’onglet [!UICONTROL Overview] de la tâche que vous créez. </p> <p>Important : pour que cela fonctionne, votre administrateur ou administratrice [!DNL Workfront] doit autoriser [!DNL Google Drive] à utiliser des documents dans [!DNL Workfront], comme décrit dans la section <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurer les intégrations pour gérer des documents</a> dans l’article <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurer des intégrations de documents</a>.</p> <p>Si vous activez cette option, elle reste activée pour les autres e-mails que vous convertissez en tâches, problèmes et mises à jour.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email file]</td> 
      <td> <p>Cliquez sur cette option pour enregistrer l’e-mail d’origine en tant que fichier d’e-mail (EML) <span>dans la zone [!UICONTROL Documents]</span> de la tâche. À partir de là, vous pouvez double-cliquer sur le fichier pour ouvrir l’e-mail dans votre application de messagerie.</p> <p>Si vous activez cette option, elle reste activée pour les autres e-mails que vous convertissez en tâches, problèmes et mises à jour.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Créer une tâche]**.

   L’onglet **[!UICONTROL Détails]** de la nouvelle tâche s’affiche dans le panneau [!DNL Workfront for Google Workspace]. Vous pouvez cliquer sur **[!UICONTROL Mises à jour]** et commencer à communiquer avec les collaborateurs et collaboratrices immédiatement sans quitter votre boîte de réception.

   Au bas de l’onglet **[!UICONTROL Détails]**, vous pouvez également cliquer sur **[!UICONTROL Afficher dans[!DNL Workfront]]** pour accéder à la nouvelle tâche dans Workfront.

   Lorsque vous actualisez votre navigateur, un message contenant un lien au bas du panneau [!DNL Workfront for Google Workspace] confirme que vous avez converti l’email en une tâche :

   Vous pouvez cliquer sur le lien pour accéder à la vue Détails, au sein du panneau [!DNL Workfront for Google Workspace] pour la tâche que vous avez créée.

   Vous pouvez répéter ces étapes pour convertir le même e-mail en plusieurs tâches. Lorsque vous actualisez votre navigateur ou revenez à l’e-mail à un autre moment, tous les liens que vous avez créés pour l’e-mail sont répertoriés au bas du panneau [!UICONTROL Workfront pour Google Workspace].

1. (Facultatif) Continuez à travailler sur la tâche dans le panneau [!DNL Workfront for Google Workspace] en effectuant l’une des opérations suivantes :

   * Pour ajouter une mise à jour à l’onglet **[!UICONTROL Mises à jour]**, cliquez sur **[!UICONTROL Démarrer une nouvelle mise à jour]** et saisissez la mise à jour.

   * Pour répondre à une mise à jour de l’onglet **[!UICONTROL Mises à jour]**, cliquez sur **[!UICONTROL Répondre]** et saisissez votre réponse.

     Pour les deux actions ci-dessus, vous pouvez informer des personnes spécifiques de votre commentaire. Cliquez sur **[!UICONTROL Notifier]**, commencez à saisir le nom d’un utilisateur ou d’utilisatrice, puis cliquez sur celui-ci lorsqu’il apparaît dans la liste déroulante. Répétez cette procédure pour les autres personnes que vous souhaitez notifier, puis cliquez sur **[!UICONTROL Publier]**.

   * Cliquez sur l’onglet **[!UICONTROL Documents]** pour afficher tous les documents enregistrés avec la tâche.

Vous pouvez répéter ces étapes pour convertir le même e-mail en plusieurs tâches. Lorsque vous actualisez votre navigateur ou revenez à l’e-mail à un autre moment, tous les liens que vous avez créés pour l’e-mail sont répertoriés au bas du panneau [!DNL Workfront for Google Workspace].
