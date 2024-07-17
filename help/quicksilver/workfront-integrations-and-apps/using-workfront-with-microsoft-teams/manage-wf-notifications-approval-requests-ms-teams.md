---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Gérer les  [!DNL Adobe Workfront] notifications dans les  [!DNL Microsoft] équipes
description: Vous pouvez recevoir des notifications de  [!DNL Adobe Workfront]  sur les éléments à approuver, les affectations qui vous ont été données ou les commentaires et modifications des éléments auxquels vous êtes associé.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 1f2655c0e88a5cc918501e2a0ef830758111ded8
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 7%

---

# Gérer [!DNL Adobe Workfront] notifications dans [!DNL Microsoft Teams]

>[!NOTE]
>
>L’intégration d’Adobe Workfront for Microsoft Teams n’est actuellement prise en charge que pour l’expérience de Microsofts Teams classiques.

Vous pouvez recevoir des notifications de [!DNL Adobe Workfront] sur les éléments à approuver, les affectations qui vous ont été données ou les commentaires et modifications des éléments auxquels vous êtes associé.

Ces notifications contiennent des actions [!DNL Workfront] que vous pouvez effectuer dans [!DNL Microsoft Teams] sans quitter [!DNL Microsoft Teams] pour les accomplir.

>[!NOTE]
>
>[!DNL Microsoft Teams] ne prend plus en charge [!DNL Internet Explorer]. Pour utiliser le [!DNL Adobe Workfront for Microsoft Teams integration], vous devez utiliser un navigateur web autre que [!DNL Internet Explorer].


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

## Conditions préalables pour la réception de notifications [!DNL Workfront] dans [!DNL Microsoft Teams]

Vous pouvez recevoir [!DNL Workfront] notifications dans [!DNL Microsoft Teams] si les conditions suivantes sont remplies :

* Un propriétaire d’équipe a installé et configuré [!DNL Workfront for Microsoft Teams] pour votre équipe.
* Vous êtes connecté à [!DNL Workfront] à partir de [!DNL Microsoft Teams].
* Vous avez activé les notifications instantanées dans [!DNL Workfront]. Pour plus d’informations sur l’activation des notifications instantanées, voir [Modification de vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Pour plus d&#39;informations sur l&#39;installation de [!DNL Workfront for Microsoft Teams] et la connexion à [!DNL Workfront from Microsoft Teams], voir [Installation [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Gestion des notifications [!DNL Workfront] dans [!DNL Microsoft Teams]

Lorsque l’application [!DNL Workfront for Microsoft Teams] est installée, un canal de conversation [!DNL Workfront] est créé dans [!DNL Microsoft Teams] pour chaque membre de l’équipe. Lorsqu&#39;une action spécifique est effectuée dans [!DNL Workfront], vous pouvez configurer les paramètres de [!DNL Workfront for Microsoft Teams] pour recevoir des notifications sur cette action dans le canal de conversation [!DNL Workfront] de [!DNL Microsoft Teams].

Tenez compte des points suivants lorsque vous utilisez des notifications [!DNL Workfront] de [!DNL Microsoft Teams] :

* Vous ne pouvez pas recevoir tous les messages, mais seulement un nombre restreint de [!DNL Workfront] notifications dans [!DNL Microsoft Teams].
* Toutes les notifications que vous recevez de [!DNL Workfront] apparaissent dans le canal de conversation de robot [!DNL Workfront].

  Pour plus d’informations sur l’installation du canal de robot [!DNL Workfront], reportez-vous à la section [Connexion à [!DNL Workfront] à partir de [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) dans l’article [Installation [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) .

* Un délai de 5 minutes peut s’écouler entre le moment où une mise à jour est effectuée dans [!DNL Workfront] et celui où vous recevez la notification à son sujet dans [!DNL Microsoft Teams].
* Pour chaque notification [!DNL Microsoft Teams], vous recevez également une notification électronique.

Pour gérer les notifications [!DNL Workfront] que vous pouvez recevoir dans [!DNL Microsoft Teams] :

1. Cliquez sur l’icône des applications **[!UICONTROL Plus ajouté]** (à trois points) dans la barre de navigation de gauche de [!DNL Microsoft Teams].

1. Cliquez sur [!DNL Workfront] dans la liste qui s’affiche.
1. Sélectionnez l’onglet **[!UICONTROL Paramètres]**.

   ![](assets/ms-teams-settings-tab-350x552.png)

1. Désactivez toutes les notifications que vous ne souhaitez pas recevoir. Vous pouvez activer ou désactiver des groupes de notifications, tels que des informations ou des notifications d’approbation, ou vous pouvez gérer les notifications individuellement.

   Toutes les notifications sont activées par défaut.

   Les paramètres de notification pour les équipes [!DNL Workfront for Microsoft] sont enregistrés automatiquement.

   >[!NOTE]
   >
   >Vous ne pouvez pas ajouter d’autres notifications à celles disponibles par défaut.

## Réponse à [!DNL Workfront] notifications et demandes d’approbation dans [!DNL Microsoft Teams]

1. Connectez-vous à [!DNL Workfront] depuis [!DNL Microsoft Teams].\
   Pour plus d&#39;informations sur la connexion à [!DNL Workfront], voir [Installation [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Accédez à la zone **[!UICONTROL Chat]** et cliquez sur le canal de robot **[!DNL Workfront]**.\
   Ce canal est destiné à votre conversation personnelle avec le robot [!DNL Workfront]. Toutes les notifications [!DNL Workfront] s&#39;affichent ici.
1. Selon le type de notification que vous recevez, passez à la section correspondante :

   * [Notifications de validation](#approval-notifications-approval-notifications)
   * [Notifications d’affectation](#assignment-notifications-assignment-notifications)
   * [Notifications de commentaires](#comment-notifications-comment-notifications)
   * [Mettre à jour les notifications](#update-notifications-update-notifications)
   * [Notifications de changement de date](#date-change-notifications-date-change-notifications)

### Notifications de validation {#approval-notifications}

Vous recevez des notifications de validation lorsque vous êtes invité à valider un objet, tel qu’une tâche, une feuille de temps ou un BAT. Vous pouvez toutefois toujours commenter la notification. Depuis la notification de validation, vous pouvez effectuer les actions suivantes :

* **[!UICONTROL Approve]** : cliquez pour approuver l’élément.
* **[!UICONTROL Modifier]** : cliquez pour approuver l’élément avec des modifications.
* **[!UICONTROL Rejeter]** : cliquez pour rejeter l’élément.
* **[!UICONTROL Commentaire]** : cliquez pour faire un commentaire. Votre commentaire apparaît également dans [!DNL Workfront] comme une mise à jour de l’objet sur lequel porte la notification.
* **[!UICONTROL Accéder au BAT]** : cliquez pour ouvrir le BAT. Vous pouvez ensuite prendre une décision directement dans le BAT. Pour plus d’informations, voir [Prise d’une décision sur un BAT dans la visionneuse de correctifs](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>Une fois que vous avez pris une décision de validation, vous ne pouvez pas la modifier à partir de la notification.

#### Actions disponibles sur les notifications de validation spécifiques :

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
   <th>[!UICONTROL Approuver]</th> 
   <th>[!UICONTROL Rejeter]</th> 
   <th> <p>[!UICONTROL Change]</p> </th> 
   <th> <p>[!UICONTROL Aller à la preuve] </p> </th> 
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
   <td role="rowheader">Quelqu'un veut que vous approuviez ce BAT</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Votre feuille de temps est rejetée</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Votre feuille de temps est rouverte</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une demande d’approbation de document que vous avez demandée est approuvée</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une demande d’approbation de document que vous avez demandée est approuvée avec les modifications</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une demande d’approbation de document que vous avez demandée est rejetée</td> 
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

### Notifications d’affectation {#assignment-notifications}

Vous recevez des notifications d’affectation lorsque vous, ou une équipe que vous utilisez, êtes affecté à une tâche ou à un problème dans Workfront. Dans la notification d’affectation, vous pouvez effectuer les actions suivantes :

* **[!UICONTROL Travailler dessus]** : sélectionnez cette option pour valider le travail sur l’élément. Une notification s’affiche brièvement pour confirmer qu’un nouvel élément a été ajouté à votre liste de travail.
* **[!UICONTROL Afficher dans[!DNL Workfront]]** : sélectionnez cette option pour afficher le problème ou la tâche assigné dans Workfront, ce qui ouvre un nouvel onglet.
* **[!UICONTROL Démarrer]** : cliquez pour commencer à travailler sur l’élément. Une notification s’affiche brièvement pour confirmer qu’un nouvel élément a été ajouté à votre liste de travail.
* **[!UICONTROL Commentaire]** : cliquez pour faire un commentaire sur l’élément. Votre commentaire apparaît également dans le flux de mise à jour de l’élément dans Workfront.
* **[!UICONTROL Status]** : cliquez sur, puis sélectionnez le nouvel état de l’élément de travail dans le menu déroulant.

#### Actions disponibles sur les notifications d’affectation spécifiques :

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
   <td role="rowheader">Vous êtes affecté à une tâche</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vous êtes affecté à un problème.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une équipe à laquelle vous êtes affecté reçoit une demande de travail pour une tâche.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Une équipe à laquelle vous êtes affecté reçoit une demande de travail pour un problème.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Notifications de commentaires {#comment-notifications}

Vous recevez une notification de communication lorsqu’une personne commente un élément auquel vous êtes associé ou vous inclut dans une mise à jour. A partir de la notification de communication, vous pouvez effectuer les actions suivantes :

* **Reply** : cliquez pour répondre au commentaire ou [!UICONTROL update]. Votre réponse apparaît également dans le flux de mise à jour où le commentaire apparaît dans Workfront.
* **[!UICONTROL Afficher dans Workfront]** : sélectionnez cette option pour afficher le commentaire et l’élément dans Workfront, qui est ouvert dans un nouvel onglet.
* **[!UICONTROL Status]** : cliquez sur, puis sélectionnez un nouvel état pour l’élément de travail sur lequel porte le commentaire ou la mise à jour.

#### Actions disponibles sur les notifications de communication spécifiques :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>[!UICONTROL Réponse]</th> 
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
   <td role="rowheader">Quelqu'un commente un fil dans lequel vous vous trouvez</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quelqu’un commente l’une de vos tâches</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quelqu’un commente une feuille de temps que vous approuvez</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un commentaire est ajouté à votre page de profil utilisateur ou en modifiant en masse plusieurs utilisateurs</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un commentaire est ajouté à l’une de vos mises à jour</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un commentaire est ajouté à votre feuille de temps.</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Mettre à jour les notifications {#update-notifications}

Vous recevez une notification d’informations en cas de mise à jour d’un élément auquel vous êtes associé, mais il n’est pas nécessaire d’effectuer une action sur l’élément. A partir de la notification d&#39;information, vous pouvez effectuer les actions suivantes :

* **[!UICONTROL Répondre]** : cliquez pour répondre à la [!UICONTROL mise à jour]. Votre réponse apparaît également dans le flux de mise à jour de l’élément dans Workfront.
* **Afficher dans Workfront** : sélectionnez cette option pour afficher le commentaire et l’élément dans Workfront, qui est ouvert dans un nouvel onglet.
* **[!UICONTROL Status]** : cliquez sur , puis sélectionnez le nouvel état de l’élément dans le menu déroulant.

#### Actions disponibles sur les notifications d’informations spécifiques :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>[!UICONTROL Réponse]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Une mise à jour est apportée à une tâche, un problème ou un projet auquel vous êtes abonné.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quelqu’un vous inclut à une mise à jour dirigée</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quelqu’un inclut votre équipe sur une [!UICONTROL mise à jour dirigée]</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Notifications de changement de date {#date-change-notifications}

Vous recevez une notification de changement de date lorsque la date change sur un élément de travail auquel vous êtes affecté. À partir de la notification de changement de date, vous pouvez effectuer les actions suivantes.

* **[!UICONTROL Commentaire]** : cliquez pour faire un commentaire sur l’élément. Votre commentaire apparaît également dans le flux de mise à jour de l’élément dans Workfront.
* **[!UICONTROL Status]** : cliquez sur, puis sélectionnez le nouvel état de l’élément de travail dans le menu déroulant.

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
   <td role="rowheader">La date d’échéance change pour une tâche à laquelle vous êtes affecté</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
