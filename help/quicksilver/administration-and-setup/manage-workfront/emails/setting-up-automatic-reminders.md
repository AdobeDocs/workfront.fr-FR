---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Configuration de rappels automatiques
description: Configuration de rappels automatiques
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 1%

---

# Configuration de rappels automatiques

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

En tant qu’administrateur d’Adobe Workfront, vous pouvez configurer des rappels automatiques pour déclencher des notifications par e-mail lorsque toutes les tâches ou tous les problèmes sont dus, en retard ou près de la date d’achèvement prévue. Une fois ces paramètres configurés, les utilisateurs ne peuvent pas désactiver les rappels automatiques.

Pour les notifications en retard, l’email est envoyé de nuit jusqu’à ce que la tâche ou le problème soit terminé.

Un rappel automatique peut être envoyé à un ou plusieurs des éléments suivants :

* Utilisateurs affectés à une tâche ou à un problème
* Gestionnaire immédiat de l’utilisateur
* Le responsable du responsable immédiat

>[!NOTE]
>
>Vous ne pouvez pas modifier le contenu ou l’objet de l’email déclenché par un rappel automatique.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Administrateur système</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configuration de rappels automatiques

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Email** >**Reminders automatiques**.

1. Dans le **Envoyer une notification tardive à** sélectionnez l’une des options suivantes :

   <table>
    <tr>
        <td>L’utilisateur "Affecté à"</td>
        <td>Sélectionnez cette option si vous souhaitez que l’utilisateur affecté à une tâche ou à un problème reçoive une notification de retard sur son élément de travail.</td>
        <td></td>
    </tr>
    <tr>
        <td>Le gestionnaire de l'utilisateur</td>
        <td>Sélectionnez cette option si vous souhaitez que le responsable de l’utilisateur reçoive une notification tardive indiquant que l’élément de travail de son rapport direct est en retard.</td>
        <td></td>
    </tr>
    <tr>
        <td>Le gestionnaire du gestionnaire</td>
        <td>Sélectionnez cette option si vous souhaitez que le responsable de l’environnement immédiat reçoive une notification tardive concernant un élément de travail de l’un des utilisateurs de son rapport direct étant en retard.</td>
        <td></td>
    </tr>
    <tr>
        <td>L’utilisateur "Affecté à"</td>
        <td>(Dans la variable <b>Envoyer un rappel d’échéance à</b> zone.) Sélectionnez cette option si vous souhaitez que l’utilisateur affecté à une tâche ou à un problème reçoive une notification sur son élément de travail approchant la date d’échéance.</td>
        <td></td>
    </tr>
</table>

1. Sélectionnez l’heure d’envoi du rappel automatique en sélectionnant la durée avant ou après la date d’échéance de l’élément de travail.

   L’heure est calculée à partir de la date d’achèvement planifiée de la tâche ou de la publication.

   Indiquez le nombre de minutes, heures, jours, semaines ou mois à ajouter à la date d’achèvement planifiée des tâches ou des problèmes. Sélectionner **Minutes écoulées**, **Heures écoulées**, **Jours écoulés** ou **Semaines terminées** pour ajouter une heure incluant les week-ends, jours fériés et heures non ouvrées, comme indiqué dans votre planning.

   Par exemple, si une tâche est affectée le vendredi et a une durée de 3 jours écoulés, la date d’achèvement de la tâche est définie pour le lundi (en supposant que le samedi et le dimanche soient un week-end). Si la tâche a une durée de 3 jours (non écoulée), la date de fin de la tâche est définie pour le mercredi.

   ![](assets/time-increments-for-automatic-reminder.png)

1. Cliquer sur **Enregistrer**.

## Recevoir des rappels automatiques

Si vous êtes l’entité désignée dans une notification de rappel automatique, vous recevez un courrier électronique lorsque la date limite spécifiée est atteinte. Pour les notifications en retard, l’email est envoyé de nuit jusqu’à ce que la tâche ou le problème soit terminé.

Les tâches avec certains types de dépendances peuvent être diffusées après la date de début spécifiée, même si elles sont en retard. Par exemple, si une tâche possède un prédécesseur avec une dépendance Finish-Start (fs), elle ne sera pas incluse dans l&#39;email, même si elle a dépassé la date de début spécifiée, car vous ne pouvez pas démarrer la tâche tant que le prédécesseur n&#39;est pas terminé.

Pour plus d’informations sur la réception d’emails de remise automatique, voir [Rappels automatiques](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) dans [Notifications Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Envoi de rappels automatiques

Les rappels automatiques sont envoyés dès que l’heure sélectionnée par l’administrateur Workfront est atteinte.

Si vous souhaitez déclencher manuellement l’envoi automatique des emails de rappel, vous pouvez le faire à l’aide de l’option Diagnostics. Pour plus d’informations sur l’accès et l’utilisation des diagnostics dans Workfront, voir [Utiliser les diagnostics pour déclencher des processus automatisés](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
