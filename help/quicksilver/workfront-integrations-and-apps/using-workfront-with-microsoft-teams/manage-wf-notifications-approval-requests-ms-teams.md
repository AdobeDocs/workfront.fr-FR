---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Gérer les notifications  [!DNL Adobe Workfront]  dans  [!DNL Microsoft]  Teams
description: Vous pouvez recevoir des notifications d’ [!DNL Adobe Workfront]  concernant les éléments que vous devez approuver, les affectations que vous avez reçues ou les commentaires et modifications apportés aux éléments auxquels vous vous associez.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 7720d51864428e6d7cf493f88bbee13b5203774b
workflow-type: tm+mt
source-wordcount: '1466'
ht-degree: 87%

---

# Gérer les notifications [!DNL Adobe Workfront] dans [!DNL Microsoft Teams]

>[!IMPORTANT]
>
>Comme [Microsoft passe au client Nouvelles équipes](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability), le client Équipes classiques ne sera plus disponible après le 1er juillet 2025. Pour continuer à utiliser Microsoft Teams et les applications intégrées telles que Workfront, les clients doivent passer au client New Teams avant cette date.
>
>L’intégration Workfront mise à jour est désormais disponible et entièrement compatible avec la nouvelle expérience Équipes . Dans la plupart des cas, Workfront s’affiche automatiquement une fois la transition effectuée. Si ce n’est pas le cas, l’intégration peut être installée manuellement à partir de Microsoft Teams App Store. Pour installer ou vérifier l’intégration de Workfront dans le client New Teams, voir [Installer [!DNL Adobe Workfront] pour Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

Vous pouvez recevoir des notifications d’[!DNL Adobe Workfront] concernant les éléments que vous devez approuver, les affectations que vous avez reçues ou les commentaires et modifications apportés aux éléments auxquels vous vous associez.

Ces notifications incluent les actions [!DNL Workfront] que vous pouvez effectuer dans [!DNL Microsoft Teams], sans devoir quitter [!DNL Microsoft Teams] pour les accomplir.

>[!NOTE]
>
>[!DNL Microsoft Teams] ne prend plus en charge [!DNL Internet Explorer]. Pour utiliser [!DNL Adobe Workfront for Microsoft Teams integration], vous devez utiliser un navigateur web autre qu’[!DNL Internet Explorer].




## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Travail ou supérieur</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables à la réception de notifications [!DNL Workfront] dans [!DNL Microsoft Teams]

Pour recevoir des notifications [!DNL Workfront] dans [!DNL Microsoft Teams], vous devez remplir les conditions suivantes :

* Une personne propriétaire d’équipe a installé et configuré [!DNL Workfront for Microsoft Teams] pour votre équipe.
* Votre équipe est connectée à [!DNL Workfront] dans [!DNL Microsoft Teams].
* Vous avez activé les notifications instantanées dans [!DNL Workfront]. Pour plus d’informations sur l’activation des notifications instantanées, consultez la section [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Pour plus d’informations sur l’installation de [!DNL Workfront for Microsoft Teams] et la connexion à [!DNL Workfront from Microsoft Teams], consultez la section [Installer [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Gérer les notifications [!DNL Workfront] dans [!DNL Microsoft Teams]

Lorsque l’application [!DNL Workfront for Microsoft Teams] est installée, un canal de conversation [!DNL Workfront] est créé dans [!DNL Microsoft Teams] pour chaque personne membre de cette équipe. Lorsqu’une certaine action est effectuée dans [!DNL Workfront], vous pouvez configurer les paramètres permettant aux [!DNL Workfront for Microsoft Teams] de recevoir des notifications sur cette action dans le canal de conversation [!DNL Workfront] d’[!DNL Microsoft Teams].

Tenez compte des points suivants lorsque vous activez les notifications [!DNL Workfront] dans [!DNL Microsoft Teams] :

* Vous ne pouvez recevoir qu’un nombre restreint de notifications [!DNL Workfront] dans [!DNL Microsoft Teams].
* Les notifications que vous recevez de [!DNL Workfront] s’affichent dans le canal de conversation avec le robot [!DNL Workfront].

  Pour plus d’informations sur l’installation du canal avec le robot [!DNL Workfront], consultez la section [Se connecter à  [!DNL Workfront]  dans  [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) de l’article [Installer  [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

* Un délai de 5 minutes peut s’écouler entre le moment où une mise à jour est effectuée dans [!DNL Workfront] et la réception de la notification dans [!DNL Microsoft Teams].
* Toute notification dans [!DNL Microsoft Teams] génère également une notification par e-mail.

Pour gérer les notifications [!DNL Workfront] que vous pouvez recevoir dans [!DNL Microsoft Teams], procédez comme suit :

1. Cliquez sur l’icône d’applications **[!UICONTROL Afficher d’autres applications]** (à trois points) dans la barre de navigation de gauche de [!DNL Microsoft Teams].

1. Cliquez sur [!DNL Workfront] dans la liste qui s’affiche.
1. Sélectionnez l’onglet **[!UICONTROL Paramètres]**.

   ![Onglet Paramètres de MS Teams](assets/ms-teams-settings-tab-350x552.png)

1. Désactivez toutes les notifications que vous ne souhaitez pas recevoir. Vous pouvez activer ou désactiver des groupes de notifications, tels que des informations ou des notifications d’approbation, ou vous pouvez gérer les notifications individuellement.

   L’option « Toutes les notifications » est activée par défaut.

   Les paramètres de notification pour [!DNL Workfront for Microsoft] Teams sont enregistrés automatiquement.

   >[!NOTE]
   >
   >Vous ne pouvez pas ajouter d’autres notifications à celles disponibles par défaut.

## Répondre aux notifications [!DNL Workfront] et aux demandes d’approbation dans [!DNL Microsoft Teams]

1. Connectez-vous à [!DNL Workfront] dans [!DNL Microsoft Teams].\
   Pour plus d’informations sur la connexion à [!DNL Workfront], consultez la section [Installer  [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Accédez à la zone **[!UICONTROL Conversation]** et cliquez sur le canal du robot **[!DNL Workfront]**.\
   Ce canal constitue votre conversation privée avec le robot [!DNL Workfront]. Toutes les notifications [!DNL Workfront] s’affichent ici.
1. Selon le type de notification que vous recevez, passez à la section correspondante :

   * [Notifications d’approbation](#approval-notifications-approval-notifications)
   * [Notifications d’affectation](#assignment-notifications-assignment-notifications)
   * [Notifications de commentaires](#comment-notifications-comment-notifications)
   * [Notifications de mise à jour](#update-notifications-update-notifications)
   * [Notifications de changement de date](#date-change-notifications-date-change-notifications)

### Notifications d’approbation {#approval-notifications}

Vous recevez des notifications d’approbation lorsque vous recevez une invitation à approuver un objet, tel qu’une tâche, une feuille de temps ou une épreuve. Toutefois, vous pouvez toujours commenter la notification. Dans la notification d’approbation, vous pouvez effectuer les actions suivantes :

* **[!UICONTROL Approuver]** : cliquez pour approuver l’élément.
* **[!UICONTROL Modifier]** : cliquez pour approuver l’élément avec les modifications.
* **[!UICONTROL Rejeter]** : cliquez pour rejeter l’élément.
* **[!UICONTROL Commenter]** : cliquez pour faire un commentaire. Votre commentaire apparaît également dans [!DNL Workfront] en tant que mise à jour de l’objet sur lequel porte la notification.
* **[!UICONTROL Accéder à l’épreuve]** : cliquez pour ouvrir l’épreuve. Vous pouvez ensuite prendre une décision directement dans l’épreuve. Pour plus d’informations, voir [Prendre une décision sur une épreuve dans la visionneuse de relecture](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>Une fois que vous avez pris une décision d’approbation, vous ne pouvez pas la modifier à partir de la notification.

#### Actions disponibles sur des notifications d’approbation spécifiques :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>[!UICONTROL Approve]</th> 
   <th>[!UICONTROL Reject]</th> 
   <th> <p>[!UICONTROL Change]</p> </th> 
   <th> <p>[!UICONTROL Go to Proof] </p> </th> 
   <th>[!UICONTROL Comment]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Vous devez approuver un projet.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vous devez approuver une tâche.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vous devez approuver un problème.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vous devez approuver un document.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vous devez approuver l’accès à un objet.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vous devez approuver une feuille de temps.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quelqu’un souhaite que vous approuviez cette épreuve.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Votre feuille de temps est rejetée.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Votre feuille de temps est rouverte.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une demande d'approbation de document que vous avez demandée est approuvée*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une demande d'approbation de document que vous avez demandée est approuvée avec des modifications*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une demande d'approbation de document que vous avez demandée est rejetée*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Votre feuille de temps est approuvée.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Ces notifications se rapportent aux approbations de documents hérités. Les notifications d’approbation de documents unifiés ne sont actuellement pas prises en charge dans [!DNL Microsoft Teams]. Pour plus d’informations sur les différents systèmes d’approbation dans Workfront, voir [Fonctionnalité disponible pour les approbations de documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md).

### Notifications d’affectation {#assignment-notifications}

Vous recevez des notifications d’affectation lorsque vous, ou une équipe dont vous êtes membre, faites l’objet d’une affectation à une tâche ou à un problème dans Workfront. Dans la notification d’affectation, vous pouvez effectuer les actions suivantes :

* **[!UICONTROL Travailler sur ce projet]** : sélectionnez cette option pour vous engager à travailler sur l’élément. Une notification s’affiche brièvement pour confirmer qu’un nouvel élément a été ajouté à votre liste de travail.
* **[!UICONTROL Afficher dans[!DNL Workfront]]** : sélectionnez cette option pour afficher le problème ou la tâche affecté(e) dans Workfront, ce qui ouvre un nouvel onglet.
* **[!UICONTROL Démarrer]** : cliquez pour commencer à travailler sur l’élément. Une notification s’affiche brièvement pour confirmer qu’un nouvel élément a été ajouté à votre liste de travail.
* **[!UICONTROL Commenter]** : cliquez pour ajouter un commentaire à l’élément. Votre commentaire apparaît également dans le flux de mise à jour de l’élément dans Workfront.
* **[!UICONTROL Statut]** : cliquez, puis sélectionnez le nouveau statut de l’élément de travail dans le menu déroulant.

#### Actions disponibles sur des notifications d’affectation spécifiques :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>[!UICONTROL Start]</th> 
   <th>[!UICONTROL Comment]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Une tâche vous est affectée.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un problème vous est affecté.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une équipe qui vous est affectée reçoit une demande de travail pour une tâche.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une équipe qui vous est affectée reçoit une demande de travail pour un problème.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Notifications de commentaires {#comment-notifications}

Vous recevez une notification de communication lorsqu’une personne commente un élément associé à vous ou vous inclut dans une mise à jour. Dans la notification de communication, vous pouvez effectuer les actions suivantes :

* **Répondre** : cliquez pour répondre au commentaire ou à la [!UICONTROL mise à jour]. Votre réponse apparaît également dans le flux de mise à jour où le commentaire apparaît dans Workfront.
* **[!UICONTROL Afficher dans Workfront]** : sélectionnez cette option pour afficher le commentaire et l’élément dans Workfront, qui est ouvert dans un nouvel onglet.
* **[!UICONTROL Statut]** : cliquez, puis sélectionnez un nouveau statut pour l’élément de travail sur lequel porte le commentaire ou la mise à jour.

#### Actions disponibles sur des notifications de communication spécifiques :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Un commentaire est publié sur votre demande.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une réponse est publiée sur votre demande de travail.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quelqu’un commente un flux auquel vous participez.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une personne apporte des commentaires sur l’un de vos éléments de travail.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une personne apporte des commentaires sur une feuille de temps que vous approuvez.</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un commentaire est ajouté à votre page de profil d’utilisateur ou d’utilisatrice ou lors de la modification en bloc de plusieurs utilisateurs et utilisatrices.</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un commentaire est ajouté à l’une de vos mises à jour.</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un commentaire a été ajouté sur votre feuille de temps.</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Notifications de mise à jour {#update-notifications}

Vous recevez une notification d’informations en cas de mise à jour d’un élément associé à vous, mais il n’est pas nécessaire d’effectuer une action sur l’élément. À partir de la notification d’information, vous pouvez effectuer les actions suivantes :

* **[!UICONTROL Répondre]** : cliquez pour répondre à la [!UICONTROL mise à jour]. Votre réponse apparaît également dans le flux de mise à jour de l’élément dans Workfront.
* **Afficher dans Workfront** : sélectionnez cette option pour afficher le commentaire et l’élément dans Workfront (ouverture dans un nouvel onglet).
* **[!UICONTROL Statut]** : cliquez et sélectionnez le nouveau statut de l’élément dans le menu déroulant.

#### Actions disponibles pour des notifications d’informations spécifiques :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Une mise à jour est apportée à une tâche, à un problème ou à un projet et j’ai un abonnement à cet élément.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une personne m’inclut dans une mise à jour dirigée.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une personne inclut mon équipe dans une [!UICONTROL directed update].</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Notifications de changement de date {#date-change-notifications}

Vous recevez une notification de modification de date en cas de modification de la date d’un élément de travail qui vous est affecté. À partir de la notification de modification de date, vous pouvez effectuer les actions suivantes.

* **[!UICONTROL Commentaire]** : cliquez dessus pour ajouter un commentaire à l’élément. Votre commentaire apparaît également dans le flux de mise à jour de l’élément dans Workfront.
* **[!UICONTROL Statut]** : cliquez et sélectionnez le nouveau statut de l’élément de travail dans le menu déroulant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th> <p>[!UICONTROL Comment]</p> </th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">La date d’échéance d’une tâche qui vous est affectée est modifiée.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
