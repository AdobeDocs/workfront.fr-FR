---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Recevoir les notifications  [!DNL Adobe Workfront]  dans  [!DNL Slack]
description: Recevoir les notifications  [!DNL Adobe Workfront]  dans  [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 99%

---

# Recevoir des notifications [!DNL Adobe Workfront] dans [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Après avoir installé [!DNL Adobe Workfront for Slack], vous pouvez recevoir les notifications [!DNL Workfront] dans [!DNL Slack].\
Pour plus d’informations sur l’installation de [!DNL Workfront for Slack], voir [Configurer  [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Vous pouvez activer un nombre sélectionné de [!UICONTROL notifications] qui apparaissent dans la bulle de notifications de l’interface [!DNL Workfront], à diffuser également dans [!DNL Slack].

Les notifications par e-mail fonctionnent indépendamment des notifications de l’interface [!DNL Workfront]. Vous, votre administrateur ou administratrice [!DNL Workfront] peut désactiver les notifications par e-mail, tandis que les notifications de l’interface ne peuvent pas être désactivées dans [!DNL Workfront].\
Vous pouvez toutefois désactiver les notifications [!DNL Workfront] que vous pourriez recevoir dans [!DNL Slack], si vous souhaitez vous concentrer uniquement sur ces notifications dans l’interface [!DNL Workfront].

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
   <td> <p>Tous</p>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de recevoir les notifications [!DNL Workfront] dans [!DNL Slack], vous devez :

* Configurer [!DNL Workfront for Slack]\
   Pour obtenir des instructions sur la configuration de [!DNL Workfront for Slack], voir [Configurer  [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configurer les notifications [!DNL Workfront] pour [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Le cas échéant) Après que [!DNL Workfront] a été ajouté à votre instance [!DNL Slack], connectez-vous à [!DNL Workfront] à partir de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], voir [Accèder à  [!DNL Adobe Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n’importe quel canal, commencez à saisir l’une des commandes suivantes dans le champ de message :

   `/workfront settings`

   Ou

   `/wf settings`

1. Par défaut, toutes les notifications sont activées.\
   Désactivez l’une des notifications suivantes :

   * [!UICONTROL Je suis affecté à une nouvelle tâche ou à un nouveau problème.]
   * [!UICONTROL Mon équipe est affectée à une nouvelle tâche ou à un nouveau problème.]
   * [!UICONTROL Je reçois une nouvelle demande d’approbation ou d’accès.]
   * [!UICONTROL Quelqu&#39;un m&#39;a inclus dans une mise à jour dirigée.]
   * [!UICONTROL Quelqu’un fait un commentaire sur un thread où je suis.]
   * [!UICONTROL Une mise à jour est apportée à la tâche, au problème ou au projet auquel/à laquelle je suis abonné.]
   * [!UICONTROL Lorsque quelqu’un fait un commentaire sur un de mes éléments de travail.]
   * [!UICONTROL Quelqu’un fait un commentaire sur ma demande d’aide.]

   Les modifications que vous apportez aux options des [!UICONTROL notifications] prennent effet immédiatement.\
   Les notifications que vous avez activées sont diffusées dans le canal [!DNL Workfront] [!DNL Slack]. Lorsque vous désactivez les notifications ici, elles ne sont désactivées que pour [!DNL Slack], et non pour l’interface [!DNL Workfront]. Vous continuez à les recevoir dans la bulle des notifications [!DNL Workfront] dans le coin supérieur droit de l’interface.

## Gérer les notifications [!DNL Workfront] à partir de [!DNL Slack]

Vous pouvez recevoir et répondre aux notifications [!DNL Workfront] à partir de [!DNL Slack].

Vous pouvez désactiver les notifications par e-mail pour les notifications que vous activez dans [!DNL Slack], afin de vous assurer que vous ne recevez pas de notifications en double.\
Pour plus d’informations sur la configuration de vos notifications par e-mail, voir [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Activer ou désactiver les notifications [!DNL Workfront] dans [!DNL Slack] n’affecte pas les notifications que vous recevez dans l’interface [!DNL Workfront].\
Les notifications au sein de l’interface [!DNL Workfront] ne peuvent pas être désactivées.

Pour gérer vos notifications [!DNL Workfront] pour [!DNL Slack] :

1. Connectez-vous à [!UICONTROL Slack].
1. Connectez-vous à [!DNL Workfront] dans [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section « Se connecter à [!DNL Workfront] à partir de [!DNL Slack] » sur la page [Accéder à  [!DNL Adobe Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Assurez-vous que les notifications [!DNL Workfront] pour [!DNL Slack] sont activées.\
   Pour plus d’informations sur les notifications [!DNL Workfront] pouvant être configurées pour être également envoyées à [!DNL Slack], consultez [Configurer les notifications  [!DNL Workfront]  pour  [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Accédez au canal **[!DNL Workfront]** pour rechercher vos notifications [!DNL Workfront].
1. (Le cas échéant et facultatif) Effectuez l’une des opérations suivantes :

   * Cliquez sur **[!UICONTROL Travailler sur cette tâche]** pour accepter de travailler sur une tâche.

   * (Le cas échéant et facultatif) Cliquez sur **[!UICONTROL Répondre dans[!DNL Workfront]]** pour répondre à un commentaire, saisissez votre réponse, puis cliquez sur **[!UICONTROL Répondre]**.

   * (Le cas échéant et facultatif) Cliquez sur **[!UICONTROL Approuver]** ou sur **[!UICONTROL Rejeter]** pour approuver ou rejeter une tâche, un problème ou un projet en attente de votre approbation.

   * (Le cas échéant et facultatif) Cliquez sur **[!UICONTROL Approuver]**, sur **[!UICONTROL Modifications]** ou sur **[!UICONTROL Rejeter]** pour approuver, approuver avec des modifications ou rejeter un document.

     Vous pouvez également positionner la souris sur la miniature du document et cliquer sur l’icône en forme de loupe pour afficher une plus grande prévisualisation du document avant de l’approuver.\
      Seuls les [types de fichiers](https://api.slack.com/types/file) approuvés par Slack peut être prévisualisés.

   * (Le cas échéant et facultatif) Cliquez sur **[!UICONTROL Accorder]** ou sur **[!UICONTROL Ignorer]** pour accorder ou ignorer la demande d’accès supplémentaire d’un autre utilisateur ou d’une autre utilisatrice.

     Vous recevez la confirmation que votre action a été effectuée dans [!DNL Workfront] pour chaque décision que vous prenez dans vos notifications.
