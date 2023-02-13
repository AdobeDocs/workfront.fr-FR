---
title: Configuration des notifications de rappel
description: Configuration des notifications de rappel
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 1%

---

# Configuration des notifications de rappel

Les notifications de rappel envoient des emails aux destinataires selon des critères spécifiés. En tant qu’administrateur Adobe Workfront ou utilisateur disposant d’un niveau d’accès Planificateur et d’un accès administratif aux notifications de rappel, vous pouvez associer manuellement les notifications de rappel à vos tâches, telles que les projets, les tâches, les problèmes et les feuilles de temps.

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Planificateur ou version ultérieure, avec accès administratif aux notifications de rappel</p> <p>Pour plus d’informations sur l’octroi d’un accès administratif à un utilisateur de formule, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Personnalisation de l’email de rappel

Vous pouvez personnaliser la notification de rappel à l’aide d’un courrier électronique personnalisé qui comprend un objet et un corps de courrier électronique personnalisés. Le corps du courrier électronique peut contenir un HTML personnalisé.

Vous pouvez également utiliser l&#39;email par défaut inclus dans la notification de rappel. L’e-mail par défaut utilise le nom de la notification de rappel comme objet de l’e-mail et le nom de l’objet dans le corps de l’e-mail, y compris l’événement qui a déclenché la notification.

Si vous souhaitez personnaliser l&#39;email de rappel, vous devez créer un modèle d&#39;email et le joindre à la notification de rappel.

Pour plus d’informations sur la création d’un modèle de courrier électronique, voir [Configurer des modèles de courrier électronique](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Créer une notification de rappel

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Email** > **Notifications**.

1. Cliquez sur le bouton **Notifications de rappel** , puis cliquez sur **Nouvelle notification de rappel**.

1. Dans la liste déroulante, cliquez sur le type d&#39;objet à associer à la notification de rappel.

   Par exemple, si vous souhaitez joindre une notification de rappel à une feuille de temps, cliquez sur **Feuille de calcul**.

1. Dans le **Nouvelle notification de rappel** qui s’affiche, indiquez les informations suivantes.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom de la notification de rappel</td> 
      <td>Indiquez le nom de la notification de rappel.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Période qualifiante</td> 
      <td> <p>Spécifiez le nombre d’heures, de jours de travail, de jours (jours calendaires), de semaines ou de mois avant ou après la date dans la variable <strong>Minutage</strong> champ .</p> <p><b>NOTE</b>:  
        <ul> 
         <li> <p>Les notifications de rappel démarrent 24 heures après la date spécifiée et une fois tous les critères satisfaits.</p> </li> 
         <li> <p>Les notifications de rappel pour les projets, les tâches et les problèmes se déclenchent toutes les nuits à minuit, heure des Rocheuses. Tous les objets qui remplissent les critères d’une notification de rappel à partir de cette journée déclenchent une notification aux utilisateurs désignés peu de temps après cette date.</p> </li> 
         <li> <p>Les notifications de rappel pour les feuilles de temps sont envoyées à l’heure spécifiée en fonction du fuseau horaire et de la date de fin, de la date de début ou de la date de dernière mise à jour de la feuille de temps.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planning</td> 
      <td> <p>Sélectionnez l'événement qui déclenche la planification de la notification de rappel.</p> <p>Si la notification de rappel est destinée aux projets, tâches ou problèmes, les options disponibles sont liées à la date de fin ou à la date de début. La notification de rappel prend en compte l’horodatage des dates de fin et de début des projets, tâches et problèmes.</p> <p>Si la notification de rappel est destinée aux feuilles de calcul, les options disponibles sont liées à la date de fin, à la date de début ou à la date de dernière mise à jour. La notification de rappel pour les feuilles horaires prend en compte l’horodatage de fin de la feuille de temps, de début et de date de dernière mise à jour. La feuille de calcul commence à minuit le jour de la date de début (12h00) et se termine juste avant minuit la date de fin (23h59).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Critères</td> 
      <td> <p>Sélectionnez les critères pour qualifier la notification de rappel à programmer. Les notifications de rappel ne sont pas planifiées, sauf si la sélection de critères est respectée.</p> <p>Les options de critères suivantes sont disponibles, selon le type d’objet sélectionné à l’étape 4 :</p> 
       <ul> 
        <li><strong>Incomplète dans les projets en cours :</strong> (Disponible pour les rappels de tâche et de problème) L’envoi de la notification de rappel est programmé uniquement lorsque l’état de l’objet auquel la notification de rappel est associée n’est pas Terminé et que l’état du projet est Actuel.</li> 
        <li><strong>Tous dans les projets en cours :</strong>(Disponible pour les rappels de tâche et de problème) L’envoi de la notification de rappel est programmé quel que soit l’état de l’objet et uniquement lorsque l’état du projet auquel la notification de rappel est associée est Actuel.</li> 
        <li><strong>Projets incomplets :</strong> (Disponible pour les rappels de projet) L’envoi de la notification de rappel est programmé lorsque le statut du projet est autre que Terminé.</li> 
        <li><strong>Projets complets :</strong> (Disponible pour les rappels de projet) L’envoi de la notification de rappel est programmé lorsque l’état du projet est Terminé.</li> 
        <li><strong>Ouvrir les feuilles de temps :</strong> (Disponible pour les rappels de feuille de temps) L’envoi de la notification de rappel est programmé lorsque l’état de la feuille de temps est Ouverture.</li> 
        <li><strong>Feuilles de temps envoyées :</strong> (Disponible pour les rappels de feuille de temps) L’envoi de la notification de rappel est programmé lorsque l’état de la feuille de temps est Envoyé.</li> 
        <li><strong>Ouvrez la feuille de temps ou moins de 40 heures par semaine :</strong> (Disponible pour les rappels de feuille de temps) L’envoi de la notification de rappel est programmé lorsque l’état de la feuille de temps est Ouverture ou lorsque la feuille de temps est enregistrée depuis moins de 40 heures.</li> 
        <li><strong>Modèle de courrier électronique :</strong> Dans la liste déroulante, sélectionnez un modèle d'email à joindre à votre rappel.<br>Pour plus d’informations sur la création d’un modèle d’email, reportez-vous à la section <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Configurer des modèles de courrier électronique</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Destinataires</td> 
      <td>Sélectionnez les types d'utilisateurs auxquels vous souhaitez envoyer la notification. Effectuez une sélection parmi les différents intervenants d’objet, tels que le propriétaire, l’approbateur ou la personne désignée.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.
1. Joindre la notification de rappel à un élément de travail, comme décrit dans [Joindre une notification de rappel à un objet](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Recevoir une notification de rappel

Lorsque la condition est remplie sur l’élément auquel est jointe la notification de rappel, une notification électronique est déclenchée à l’utilisateur défini dans la notification de rappel.

Pour plus d’informations sur la réception de notifications de rappel, voir [Notifications de rappel](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) dans [Notifications Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Tester la diffusion de la notification de rappel

Les notifications de rappel se déclenchent toutes les nuits à minuit, heure des Rocheuses. Tous les objets qui remplissent les critères d’une notification de rappel déclenchent une notification aux utilisateurs désignés peu de temps après.

Pour que les notifications de rappel se déclenchent manuellement, la condition du rappel doit d’abord être remplie.\
Par exemple, si un rappel est défini pour se déclencher une heure après la date d’achèvement planifiée d’un projet, ce délai doit s’être écoulé entre le moment où le rappel a été défini et maintenant. Les projets dont la date d’achèvement était antérieure à l’activation du rappel ne déclenchent pas de notification.

Pour déclencher manuellement une notification de rappel :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Diagnostics** dans le coin inférieur gauche de Workfront.

1. Cliquez sur **Envoyer des notifications de rappel** et attendez la confirmation en haut de l’écran qu’ils ont été envoyés.

   Les utilisateurs désignés dans la notification de rappel reçoivent un email.
