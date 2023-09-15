---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Recevoir [!DNL Adobe Workfront] notifications dans [!DNL Slack]
description: Recevoir [!DNL Adobe Workfront] notifications dans [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 6%

---

# Recevoir [!DNL Adobe Workfront] notifications dans [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Après avoir installé [!DNL Adobe Workfront for Slack], vous pouvez recevoir [!DNL Workfront] notifications dans [!DNL Slack].\
Pour plus d’informations sur l’installation [!DNL Workfront for Slack], voir [Configurer [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Vous pouvez activer un nombre sélectionné de [!UICONTROL notifications] qui apparaissent dans la bulle de notifications de la variable [!DNL Workfront] , à diffuser également dans [!DNL Slack].

Les notifications électroniques fonctionnent indépendamment de [!DNL Workfront] notifications d’interface. Vous ou votre [!DNL Workfront] l’administrateur peut désactiver les notifications par courrier électronique, tandis que les notifications de l’interface ne peuvent pas être désactivées dans [!DNL Workfront].\
Vous pouvez toutefois désactiver [!DNL Workfront] notifications que vous pourriez recevoir [!DNL Slack], si vous souhaitez vous concentrer uniquement sur ces notifications dans la variable [!DNL Workfront] .

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrator.\

## Conditions préalables

Avant de recevoir [!DNL Workfront] notifications dans [!DNL Slack], vous devez

* Configurer [!DNL Workfront for Slack]\
   Pour obtenir des instructions sur la configuration [!DNL Workfront for Slack], voir [Configurer [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configurer [!DNL Workfront] notifications pour [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Conditionnel) Après [!DNL Workfront] a été ajouté à votre [!DNL Slack] instance, se connecter [!DNL Workfront] de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] de [!DNL Slack], voir [Accès [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir l&#39;une des commandes suivantes dans le champ de message :

   `/workfront settings`

   Ou

   `/wf settings`

1. Par défaut, toutes les notifications sont activées.\
   Désactivez l’une des notifications suivantes :

   * [!UICONTROL Je suis affecté à une nouvelle tâche ou à un nouveau problème.]
   * [!UICONTROL Mon équipe est affectée à une nouvelle tâche ou à un nouveau problème.]
   * [!UICONTROL Je reçois une nouvelle demande d’approbation ou d’accès]
   * [!UICONTROL Quelqu&#39;un m&#39;a inclus dans une mise à jour dirigée.]
   * [!UICONTROL Lorsque quelqu&#39;un fait un commentaire sur un élément de travail, envoyer un e-mail à tous ceux qui ont également fait un commentaire sur cet élément de travail]
   * [!UICONTROL Une mise à jour est apportée à la tâche, à l&#39;événement ou au projet auquel/à laquelle je suis abonné]
   * [!UICONTROL Lorsque quelqu&#39;un fait un commentaire sur un élément de travail, envoyer un e-mail au cessionnaire]
   * [!UICONTROL Quelqu&#39;un commente ma demande d&#39;aide]

   Les modifications que vous apportez à la variable [!UICONTROL notifications] les options prennent effet immédiatement.\
   Les notifications que vous avez activées sont diffusées dans la [!DNL Workfront] [!DNL Slack] canal. Lorsque vous désactivez les notifications ici, elles ne sont désactivées que pour [!DNL Slack], et non pour le [!DNL Workfront] . Vous continuez à les recevoir dans la variable [!DNL Workfront] bulle de notifications dans le coin supérieur droit de l’interface.

## Gérer [!DNL Workfront] notifications de [!DNL Slack]

Vous pouvez recevoir et répondre à [!DNL Workfront] notifications de [!DNL Slack].

Vous pouvez désactiver les notifications électroniques pour les notifications que vous activez dans [!DNL Slack], afin de vous assurer que vous ne recevez pas de notifications en double.\
Pour plus d’informations sur la configuration de vos notifications électroniques, voir [Modifier vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Activer ou désactiver [!DNL Workfront] notifications dans [!DNL Slack] n’affecte pas les notifications que vous recevez dans la variable [!DNL Workfront] .\
Notifications à l’intérieur du [!DNL Workfront] ne peut pas être désactivée.

Pour gérer vos [!DNL Workfront] notifications pour [!DNL Slack]:

1. Connexion à [!UICONTROL Slack].
1. Connexion à [!DNL Workfront] de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] de [!DNL Slack], voir &quot;Connexion à [!DNL Workfront] de [!DNL Slack]&quot; dans [Accès [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Assurez-vous que la variable [!DNL Workfront] notifications pour [!DNL Slack] sont activées.\
   Pour plus d’informations sur [!DNL Workfront] les notifications peuvent également être configurées pour être envoyées à [!DNL Slack], voir [Configurer [!DNL Workfront] notifications pour [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Accédez au **[!DNL Workfront]** canal pour trouver votre [!DNL Workfront] notifications.
1. (Conditionnel et facultatif) Effectuez l’une des opérations suivantes :

   * Cliquez sur **[!UICONTROL Travailler dessus]** accepter de travailler sur une tâche.

   * (Conditionnel et facultatif) Cliquez sur **[!UICONTROL Répondre à[!DNL Workfront]]** pour répondre à un commentaire, tapez votre réponse, puis cliquez sur **[!UICONTROL Répondre]**.

   * (Conditionnel et facultatif) Cliquez sur **[!UICONTROL Approuver]** ou **[!UICONTROL Rejeter]** pour approuver ou rejeter une tâche, une émission ou un projet en attente de votre approbation.

   * (Conditionnel et facultatif) Cliquez sur **[!UICONTROL Approuver]**, **[!UICONTROL Modifications]**, ou **[!UICONTROL Rejeter]**, pour approuver, approuver avec des modifications ou rejeter un document.

     Vous pouvez également positionner la souris sur la miniature du document et cliquer sur l’icône en forme de loupe pour afficher un aperçu plus grand du document avant de l’approuver.\
      Seul le Slack approuvé [types de fichiers](https://api.slack.com/types/file) peut être prévisualisé.

   * (Conditionnel et facultatif) Cliquez sur **[!UICONTROL Subvention]** ou **[!UICONTROL Ignorer]** pour accorder ou ignorer la demande d’accès supplémentaire d’un autre utilisateur.\

     Vous recevez la confirmation que votre action a été effectuée dans [!DNL Workfront], pour chaque décision que vous prenez dans vos notifications.
