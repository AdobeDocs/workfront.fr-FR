---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Recevez  [!DNL Adobe Workfront]  notifications dans [!DNL Slack]
description: Recevez  [!DNL Adobe Workfront]  notifications dans [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 3%

---

# Recevez [!DNL Adobe Workfront] notifications dans [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Après avoir installé [!DNL Adobe Workfront for Slack], vous pouvez recevoir [!DNL Workfront] notifications dans [!DNL Slack].\
Pour plus d&#39;informations sur l&#39;installation de [!DNL Workfront for Slack], voir [Configuration [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Vous pouvez activer un nombre restreint de [!UICONTROL notifications] qui apparaissent dans la bulle de notifications de l’interface [!DNL Workfront], qui seront également diffusées dans [!DNL Slack].

Les notifications électroniques fonctionnent indépendamment des notifications de l’interface [!DNL Workfront]. Votre administrateur [!DNL Workfront] ou vous-même pouvez désactiver les notifications par e-mail, alors que les notifications de l&#39;interface ne peuvent pas être désactivées dans [!DNL Workfront].\
Vous pouvez toutefois désactiver les [!DNL Workfront] notifications que vous pourriez recevoir dans [!DNL Slack] si vous souhaitez vous concentrer uniquement sur ces notifications dans l&#39;interface [!DNL Workfront].

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans?lang=fr" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur [!DNL Workfront].\

## Conditions préalables

Avant de pouvoir recevoir [!DNL Workfront] notifications dans [!DNL Slack], vous devez :

* Configurer [!DNL Workfront for Slack]\
   Pour obtenir des instructions sur la configuration de [!DNL Workfront for Slack], voir [Configuration [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configurer des notifications [!DNL Workfront] pour [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Conditionnel) Une fois [!DNL Workfront] ajouté à votre instance [!DNL Slack], connectez-vous à [!DNL Workfront] à partir de [!DNL Slack].\
   Pour plus d&#39;informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], voir [Accès [!DNL Adobe Workfront] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir l&#39;une des commandes suivantes dans le champ de message :

   `/workfront settings`

   Ou

   `/wf settings`

1. Par défaut, toutes les notifications sont activées.\
   Désactivez l’une des notifications suivantes :

   * [!UICONTROL Je suis assigné à une nouvelle tâche ou à un nouveau problème]
   * [!UICONTROL Mon équipe est affectée à une nouvelle tâche ou à un nouveau problème]
   * [!UICONTROL Je reçois une nouvelle demande d’approbation ou d’accès]
   * [!UICONTROL Quelqu&#39;un m&#39;a inclus dans une mise à jour dirigée.]
   * [!UICONTROL Quelqu&#39;un commente un thread dans lequel je suis ]
   * [!UICONTROL Une mise à jour est effectuée sur une tâche, un problème ou un projet auquel je suis abonné ]
   * [!UICONTROL Quelqu&#39;un commente l&#39;une de mes tâches]
   * [!UICONTROL Quelqu&#39;un commente ma demande d&#39;aide]

   Les modifications que vous apportez aux options [!UICONTROL notifications] prennent effet immédiatement.\
   Les notifications que vous avez activées sont diffusées dans le canal [!DNL Workfront] [!DNL Slack] . Lorsque vous désactivez les notifications ici, elles ne sont désactivées que pour [!DNL Slack], et non pour l’interface [!DNL Workfront]. Vous continuez à les recevoir dans la bulle de notifications [!DNL Workfront] en haut à droite de l’interface.

## Gérer [!DNL Workfront] notifications de [!DNL Slack]

Vous pouvez recevoir des [!DNL Workfront] notifications de [!DNL Slack] et y répondre.

Vous pouvez désactiver les notifications électroniques pour les notifications que vous activez dans [!DNL Slack], afin de vous assurer que vous ne recevez pas de notifications en double.\
Pour plus d’informations sur la configuration de vos notifications par e-mail, voir [Modification de vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

L&#39;activation ou la désactivation de [!DNL Workfront] notifications dans [!DNL Slack] n&#39;affecte pas les notifications que vous recevez dans l&#39;interface [!DNL Workfront].\
Les notifications dans l’interface [!DNL Workfront] ne peuvent pas être désactivées.

Pour gérer vos notifications [!DNL Workfront] pour [!DNL Slack] :

1. Connectez-vous à [!UICONTROL Slack].
1. Connectez-vous à [!DNL Workfront] depuis [!DNL Slack].\
   Pour plus d&#39;informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section &quot;Connexion à [!DNL Workfront] à partir de [!DNL Slack]&quot; dans [Accès [!DNL Adobe Workfront] à partir de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Assurez-vous que vos [!DNL Workfront] notifications pour [!DNL Slack] sont activées.\
   Pour plus d&#39;informations sur les [!DNL Workfront] notifications qui peuvent également être configurées pour être envoyées à [!DNL Slack], voir [Configurer [!DNL Workfront] les notifications pour [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Accédez au canal **[!DNL Workfront]** pour trouver vos notifications [!DNL Workfront].
1. (Conditionnel et facultatif) Effectuez l’une des opérations suivantes :

   * Cliquez sur **[!UICONTROL Travailler dessus]** pour accepter de travailler sur une tâche.

   * (Conditionnel et facultatif) Cliquez sur **[!UICONTROL Répondre dans[!DNL Workfront]]** pour répondre à un commentaire, entrez votre réponse, puis cliquez sur **[!UICONTROL Répondre]**.

   * (Conditionnel et facultatif) Cliquez sur **[!UICONTROL Approve]** ou **[!UICONTROL Reject]** pour approuver ou rejeter une tâche, un problème ou un projet en attente de votre approbation.

   * (Conditionnel et facultatif) Cliquez sur **[!UICONTROL Approve]**, **[!UICONTROL Changes]** ou **[!UICONTROL Reject]** pour approuver, approuver avec des modifications ou rejeter un document.

     Vous pouvez également positionner la souris sur la miniature du document et cliquer sur l’icône en forme de loupe pour afficher un aperçu plus grand du document avant de l’approuver.\
      Seuls les [types de fichiers](https://api.slack.com/types/file) du Slack approuvé peuvent être prévisualisés.

   * (Conditionnel et facultatif) Cliquez sur **[!UICONTROL Accorder]** ou **[!UICONTROL Ignorer]** pour accorder ou ignorer la demande d’accès supplémentaire d’un autre utilisateur.\

     Vous recevez une confirmation que votre action a été terminée dans [!DNL Workfront], pour chaque décision que vous prenez dans vos notifications.
