---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,diapositive
navigation-topic: workfront-for-g-suite
title: Création d’une tâche  [!DNL Adobe Workfront] dans Google Workspace à l’aide du contenu d’email
description: Vous pouvez convertir un email externe (non généré par Adobe [!DNL Workfront]) en tâche Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 3%

---

# Créez une tâche [!DNL Adobe Workfront] dans [!DNL Google Workspace] à l’aide du contenu d’email

>[!NOTE]
>
>La dernière version du module externe Adobe Workfront pour Google a été publiée le 26 juin 2023.

Vous pouvez convertir un email externe (non généré par [!DNL Adobe Workfront]) en tâche [!DNL Workfront].

Vous pouvez également convertir un email externe en une mise à jour sur une tâche existante. Pour plus d&#39;informations, voir [Mise à jour d&#39;un  [!DNL Adobe Workfront] élément à partir de [!DNL Google Workspace] à l&#39;aide du contenu d&#39;email](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Pour plus d&#39;informations sur l&#39;utilisation de [!DNL Google Workspace] pour utiliser les e-mails de notification envoyés par [!DNL Workfront], voir [Gérer [!DNL Adobe Workfront] les détails des notifications de [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
   </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Avant de pouvoir créer une tâche [!DNL Workfront] dans [!DNL Google Workspace], vous devez :

* Installer [!DNL Workfront for Google Workspace]\
   Pour obtenir des instructions, voir [Installation [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Créez une tâche [!DNL Adobe Workfront] dans [!DNL Google Workspace] à l’aide du contenu d’un email

1. Si le panneau [!UICONTROL  Workfront for Google Workspace] n’est pas affiché, cliquez sur l’icône [!DNL Workfront] ![](assets/wf-lion-icon.png) dans la barre latérale des modules complémentaires [!DNL Google Workspace] située à l’extrémité droite de la page.
1. Une fois le message électronique ouvert dans [!DNL Google Workspace], cliquez sur une option de [!DNL Workfront for Google Workspace] pour convertir le message électronique en une nouvelle tâche [!DNL Workfront].

1. Sélectionnez une option **[!UICONTROL Créer]** pour indiquer si la tâche va faire partie d’un projet ou d’une tâche personnelle indépendante d’un projet.
1. Si vous souhaitez joindre la tâche à un projet parent, cliquez sur **[!UICONTROL Nom du projet]**, commencez à saisir le nom du projet dans lequel vous souhaitez la tâche, puis cliquez sur le nom du projet lorsqu’il apparaît dans la liste ci-dessous.
1. Apportez l’une des modifications suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Task name]</td> 
      <td>Modifiez toute partie de ce texte qui provient de l’objet de l’email.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Modifiez toute partie de ce texte qui provient du corps de l'email.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Affecter À]</td> 
      <td>Cliquez sur <strong>[!UICONTROL Attribuer à]</strong>, cliquez sur l’option <strong>[!UICONTROL Attribuer à]</strong> qui s’affiche, puis commencez à saisir le nom de la personne et cliquez dessus lorsqu’il apparaît dans la liste ci-dessous. Répétez cette opération pour chaque personne à ajouter, puis cliquez sur <strong>[!UICONTROL Enregistrer]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Durée planifiée]</td> 
      <td> <p>Cliquez sur <strong>[!UICONTROL Durée planifiée]</strong>, puis saisissez le nombre de jours que vous souhaitez que la tâche prenne. </p> <p>Remarque : Cette option peut être configurée pour votre organisation de différentes manières. Par exemple, pour votre entreprise, vous devrez peut-être saisir un nombre d’heures au lieu de jours. Si vous avez besoin d’informations supplémentaires, consultez votre administrateur [!DNL Workfront]. Si vous souhaitez spécifier une période autre que la période par défaut configurée, saisissez <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong> ou <strong>mo</strong> après le nombre pour indiquer minutes, heures, jours, semaines ou mois.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>Cliquez sur la flèche de liste déroulante, puis sur la priorité de la tâche.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Inclure les pièces jointes aux emails]</td> 
      <td> <p>(Disponible uniquement si l’email contient au moins une pièce jointe.) Cliquez sur cette option pour enregistrer les pièces jointes dans le courrier électronique de la zone [!UICONTROL Documents] de la tâche. </p> <p>Si vous ne souhaitez pas enregistrer une pièce jointe, cliquez sur le X situé à droite de son nom. </p> <p>Si l’email contient des liens vers des documents dans [!DNL Google Drive], ils sont enregistrés dans l’onglet [!UICONTROL Aperçu] de la tâche que vous créez. </p> <p>Important : Pour que cela fonctionne, votre administrateur [!DNL Workfront] doit autoriser [!DNL Google Drive] à travailler avec des documents dans [!DNL Workfront], comme décrit dans la section <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configuration des intégrations pour gérer les documents</a> de l’article <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">}Configurer les intégrations de documents</a>.</p> <p>Si vous activez cette option, elle reste activée pour les autres emails que vous convertissez en tâches, problèmes et mises à jour.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Inclure le fichier de messagerie]</td> 
      <td> <p>Cliquez sur cette option pour enregistrer l'email d'origine sous forme de fichier d'email <span> dans la zone [!UICONTROL Documents]</span> de la tâche. À partir de là, vous pouvez double-cliquer sur le fichier pour ouvrir l’email dans votre application de messagerie.</p> <p>Si vous activez cette option, elle reste activée pour les autres emails que vous convertissez en tâches, problèmes et mises à jour.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Créer une tâche]**.

   L’onglet **[!UICONTROL Détails]** de la nouvelle tâche s’affiche dans le panneau [!DNL Workfront for Google Workspace]. Vous pouvez cliquer sur **[!UICONTROL Mises à jour]** et commencer immédiatement à communiquer avec les collaborateurs sans laisser votre compte dans la boîte.

   Au bas de l&#39;onglet **[!UICONTROL Détails]**, vous pouvez également cliquer sur **[!UICONTROL Afficher dans[!DNL Workfront]]** pour accéder à la nouvelle tâche dans Workfront.

   Lorsque vous actualisez votre navigateur, un message contenant un lien au bas du panneau [!DNL Workfront for Google Workspace] confirme que vous avez converti l’email en une tâche :

   Vous pouvez cliquer sur le lien pour accéder à la vue Détails, dans le panneau [!DNL Workfront for Google Workspace], de la tâche que vous avez créée.

   Vous pouvez répéter ces étapes pour convertir le même email en plusieurs tâches. Lorsque vous actualisez votre navigateur ou revenez à l’e-mail à un autre moment, tous les liens que vous avez créés pour l’e-mail sont répertoriés au bas du panneau [!UICONTROL Workfront for Google Workspace].

1. (Facultatif) Continuez à travailler sur la tâche dans le panneau [!DNL Workfront for Google Workspace] en effectuant l’une des opérations suivantes :

   * Pour ajouter une mise à jour sur l’onglet **[!UICONTROL Mises à jour]**, cliquez sur **[!UICONTROL Démarrer une nouvelle mise à jour]** et saisissez la mise à jour.

   * Pour répondre à une mise à jour sur l’onglet **[!UICONTROL Mises à jour]**, cliquez sur **[!UICONTROL Répondre]** et saisissez votre réponse.

     Pour les deux actions ci-dessus, vous pouvez informer des utilisateurs spécifiques de votre commentaire. Cliquez sur **[!UICONTROL Notifier]**, commencez à saisir le nom d’un utilisateur, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante. Répétez cette procédure pour les autres utilisateurs que vous souhaitez avertir, puis cliquez sur **[!UICONTROL Post]**.

   * Cliquez sur l’onglet **[!UICONTROL Documents]** pour afficher tous les documents enregistrés avec la tâche.

Vous pouvez répéter ces étapes pour convertir le même email en plusieurs tâches. Lorsque vous actualisez votre navigateur ou revenez à l’email à un autre moment, tous les liens que vous avez créés pour l’email sont répertoriés au bas du panneau [!DNL Workfront for Google Workspace].
