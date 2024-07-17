---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Mettre en place des rappels automatiques
description: Mettre en place des rappels automatiques
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 100%

---

# Mettre en place des rappels automatiques

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

En tant qu’administrateur ou administratice Adobe Workfront, vous pouvez configurer des rappels automatiques pour déclencher des notifications par e-mail lorsque toutes les tâches ou tous les problèmes sont dus, en retard ou approchant de la date d’achèvement prévue. Une fois ces paramètres configurés, les utilisateurs et utilisatrices ne peuvent pas désactiver les rappels automatiques.

Pour les notifications en retard, l’e-mail est envoyé de nuit jusqu’à ce que la tâche ou le problème soit terminé(e).

Un rappel automatique peut être envoyé à une ou plusieurs des personnes destinataires suivantes :

* La personne affectée à une tâche ou à un problème.
* La personne responsable directe de cette personne.
* La personne responsable de la personne responsable directe.

>[!NOTE]
>
>Vous ne pouvez pas modifier le contenu ou l’objet de l’e-mail déclenché par un rappel automatique.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Administrateur ou administratrice système</p> </td> 
  </tr> 
 </tbody> 
</table>

## Mettre en place des rappels automatiques

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **E-mail** > **Rappels automatiques**.

1. Dans la zone **Envoyer une notification tardive à**, sélectionnez l’une des options suivantes :

   <table>
    <tr>
        <td>La personne « Affectée à »</td>
        <td>Sélectionnez cette option si vous souhaitez que la personne affectée à une tâche ou à un problème reçoive une notification tardive concernant son élément de travail en retard.</td>
        <td></td>
    </tr>
    <tr>
        <td>Le gestionnaire de l'utilisateur</td>
        <td>Sélectionnez cette option si vous souhaitez que la personne responsable de la personne reçoive une notification tardive indiquant que l’élément de travail de son rapport direct a du retard.</td>
        <td></td>
    </tr>
    <tr>
        <td>Le gestionnaire du gestionnaire</td>
        <td>Sélectionnez cette option si vous souhaitez que la personne responsable de la personne responsable directe reçoive une notification tardive concernant un élément de travail de l’un des utilisateurs ou de l’une des utilisatrices sous son rapport direct ayant du retard.</td>
        <td></td>
    </tr>
    <tr>
        <td>La personne « Affectée à »</td>
        <td>(Dans la zone <b>Envoyer un rappel d’échéance à</b>.) Sélectionnez cette option si vous souhaitez que la personne affectée à une tâche ou à un problème reçoive une notification sur son élément de travail approchant la date d’échéance.</td>
        <td></td>
    </tr>
</table>

1. Sélectionnez l’heure d’envoi du rappel automatique en sélectionnant la durée avant ou après la date d’échéance de l’élément de travail.

   L’heure est calculée à partir de la date d’achèvement prévue de la tâche ou du problème.

   Indiquez le nombre de minutes, heures, jours, semaines ou mois à ajouter à la date d’achèvement prévue des tâches ou des problèmes. Sélectionnez **Minutes écoulées**, **Heures écoulées**, **Jours écoulés**, ou **Semaines écoulées** pour ajouter une heure incluant les week-ends, jours fériés et heures non ouvrées, comme indiqué dans votre planning.

   Par exemple, si une tâche est affectée le vendredi et a une durée de 3 jours écoulés, la date d’achèvement de la tâche est définie pour le lundi (en supposant que le samedi et le dimanche soient un week-end). Si la tâche a une durée de 3 jours (non écoulés), la date d’achèvement de la tâche est définie pour le mercredi.

   ![](assets/time-increments-for-automatic-reminder.png)

1. Cliquez sur **Enregistrer**.

## Recevoir des rappels automatiques

Si vous êtes l’entité désignée dans une notification de rappel automatique, vous recevez un e-mail lorsque la date d’échéance spécifiée est atteinte. Pour les notifications en retard, l’e-mail est envoyé de nuit jusqu’à ce que la tâche ou le problème soit terminé(e).

Les tâches avec certains types de dépendances peuvent être diffusées après la date de début spécifiée, même si elles sont en retard. Par exemple, si une tâche possède une tâche antérieure avec une dépendance Finish-Start (fs), elle ne sera pas incluse dans l’e-mail, même si elle a dépassé la date de début spécifiée, car vous ne pouvez pas démarrer la tâche tant que la tâche antérieure n’est pas terminée.

Pour plus d’informations sur la réception d’e-mails de rappel automatique, voir la section [Rappels automatiques](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) dans [Notifications Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Envoyer des rappels automatiques

Les rappels automatiques sont envoyés dès que l’heure sélectionnée par l’équipe d’administration Workfront est atteinte.

Si vous souhaitez déclencher manuellement l’envoi des e-mails de rappel automatique, vous pouvez le faire à l’aide des diagnostics. Pour plus d’informations sur l’accès et l’utilisation des diagnostics dans Workfront, voir [Utiliser les diagnostics pour déclencher des processus automatisés](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
