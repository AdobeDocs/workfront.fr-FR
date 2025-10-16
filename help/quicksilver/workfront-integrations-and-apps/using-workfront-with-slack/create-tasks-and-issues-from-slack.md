---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Créer des tâches et des problèmes depuis Slack
description: Après avoir installé et configuré  [!DNL Adobe Workfront]  pour Slack, vous pouvez créer des tâches et des problèmes à partir de Slack et les associer à des projets dans Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 99%

---

# Créer des tâches et des problèmes à partir de [!DNL Slack]

Après avoir installé et configuré [!DNL Adobe Workfront for Slack], vous pouvez créer des tâches et des problèmes à partir de [!DNL Slack] et les associer à des projets dans [!DNL Workfront].

Pour plus d’informations sur la configuration de [!DNL Workfront] avec [!DNL Slack], voir [Configurer  [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Vous devez avoir accès à la création de tâches et de problèmes dans votre niveau d’accès et vous devez disposer des autorisations de [!UICONTROL Contribution] sur le projet auquel vous les associez.

Pour plus d’informations sur les niveaux d’accès, voir [Vue d’ensemble des niveaux d’accès](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Pour plus d’informations sur les autorisations d’objets, voir [Vue d’ensemble des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

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

Avant de pouvoir créer des tâches et des problèmes [!DNL Slack], vous devez effectuer les opérations suivantes :

* Configurer [!DNL Workfront] pour Slack\
   Pour obtenir des instructions sur la configuration de [!DNL Workfront for Slack], voir [Configurer  [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Créer des tâches à partir de [!DNL Slack]

1. Connectez-vous à votre instance [!DNL Slack] et connectez-vous à [!DNL Workfront] à partir de [!DNL Slack].\
   Pour plus d’informations sur la connexion à Workfront depuis [!DNL Slack], voir la section « Se connecter à [!DNL Workfront] à partir de [!DNL Slack] » dans [Accéder à  [!DNL Adobe Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Choisissez un canal au choix et commencez à saisir la commande suivante dans le champ de message :

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Les commandes respectent la casse. Vous pouvez démarrer votre commande avec `/wf` au lieu de `/workfront`.
   >  
   >Le Nom de la tâche doit être saisi tel qu’il apparaîtra dans l’interface [!DNL Workfront], sans crochets ni guillemets.

1. (Facultatif) Commencez à saisir le nom d’un projet auquel vous souhaitez associer la nouvelle tâche et sélectionnez-le lorsqu’il apparaît dans la liste.\
   Vous recevez une confirmation indiquant que la tâche a été ajoutée au projet sélectionné.
1. (Facultatif) Cliquez sur le nom de la tâche dans le message de confirmation pour l’ouvrir dans [!DNL Workfront], dans un nouvel onglet du navigateur.

## Créer des problèmes à partir de [!DNL Slack]

1. Connectez-vous à votre instance [!DNL Slack] et connectez-vous à [!DNL Workfront] à partir de [!DNL Slack].\
   Pour plus d’informations sur la connexion à [!DNL Workfront] à partir de [!DNL Slack], consultez la section « Se connecter à [!DNL Workfront] à partir de [!DNL Slack] » sur la page [Accéder à  [!DNL Adobe Workfront]  à partir de  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Choisissez un canal au choix et commencez à saisir la commande suivante dans le champ de message :

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Les commandes respectent la casse. Vous pouvez démarrer votre commande avec « /wf » au lieu de « /workfront ». \
   >Le nom du problème doit être saisi tel qu’il apparaîtra dans l’interface [!DNL Workfront], sans crochets ni guillemets.

1. (Facultatif) Commencez à saisir le nom d’un projet auquel vous souhaitez associer le nouveau problème et sélectionnez-le lorsqu’il apparaît dans la liste.\
   Vous recevez une confirmation indiquant que le problème a été ajouté au projet sélectionné.
1. (Facultatif) Cliquez sur le nom du problème dans le message de confirmation pour l’ouvrir dans [!DNL Workfront], dans un nouvel onglet du navigateur.
