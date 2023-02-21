---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Création de tâches et de problèmes à partir de Slack
description: Une fois que vous avez installé et configuré [!DNL Adobe Workfront] pour Slack, vous pouvez créer des tâches et des problèmes à partir de Slack et les associer à des projets dans Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Création de tâches et de problèmes à partir de [!DNL Slack]

Une fois que vous avez installé et configuré [!DNL Adobe Workfront for Slack], vous pouvez créer des tâches et des problèmes à partir de [!DNL Slack] et les associer à des projets dans [!DNL Workfront].

Pour plus d’informations sur la configuration [!DNL Workfront] avec [!DNL Slack], voir [Configurer [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Vous devez avoir accès à la création de tâches et de problèmes dans votre niveau d’accès et vous devez disposer des [!UICONTROL Contribution] autorisations sur le projet auquel vous les associez.

Pour plus d’informations sur les niveaux d’accès, voir [Présentation des niveaux d’accès](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Pour plus d’informations sur les autorisations d’objets, voir [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

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

Avant de pouvoir créer des tâches et des problèmes à partir de [!DNL Slack], vous devez

* Configurer [!DNL Workfront] pour le Slack\
   Pour obtenir des instructions sur la configuration [!DNL Workfront for Slack], voir [Configurer [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Création de tâches à partir de [!DNL Slack]

1. Connectez-vous à [!DNL Slack] et connectez-vous à [!DNL Workfront] de [!DNL Slack].\
   Pour plus d’informations sur la connexion à Workfront à partir de [!DNL Slack], voir &quot;Connexion à [!DNL Workfront] de [!DNL Slack]&quot; dans la section [Accès [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir la commande suivante dans le champ de message :

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Les commandes sont sensibles à la casse. Vous pouvez lancer votre commande avec `/wf` au lieu de `/workfront`.
   >  
   >Le Nom de la tâche doit être saisi tel qu’il apparaîtra dans la [!DNL Workfront] sans crochets ni guillemets.

1. (Facultatif) Commencez à saisir le nom d’un projet auquel vous souhaitez associer la nouvelle tâche et sélectionnez-le lorsqu’il apparaît dans la liste.\
   Vous recevez une confirmation indiquant que la tâche a été ajoutée au projet sélectionné.
1. (Facultatif) Cliquez sur le nom de la tâche dans le message de confirmation pour l’ouvrir dans [!DNL Workfront], dans un nouvel onglet du navigateur.

## Création de problèmes à partir de [!DNL Slack]

1. Connectez-vous à [!DNL Slack] et connectez-vous à [!DNL Workfront] de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] de [!DNL Slack], voir &quot;Connexion à [!DNL Workfront] de [!DNL Slack]&quot; dans la section [Accès [!DNL Adobe Workfront] de [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Depuis n&#39;importe quel canal, commencez à saisir la commande suivante dans le champ de message :

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Les commandes sont sensibles à la casse. Vous pouvez démarrer votre commande avec &quot;/wf&quot; au lieu de &quot;/workfront.&quot; \
   >Le nom du problème doit être saisi tel qu’il apparaîtra dans la [!DNL Workfront] sans crochets ni guillemets.

1. (Facultatif) Commencez à saisir le nom d’un projet auquel vous souhaitez associer le nouveau problème et sélectionnez-le lorsqu’il apparaît dans la liste.\
   Vous recevez une confirmation indiquant que le problème a été ajouté au projet sélectionné.
1. (Facultatif) Cliquez sur le nom du problème dans le message de confirmation pour l’ouvrir dans [!DNL Workfront], dans un nouvel onglet du navigateur.
