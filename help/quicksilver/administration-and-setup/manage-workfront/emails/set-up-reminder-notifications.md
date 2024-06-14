---
title: Configurer des notifications de rappel
description: Les notifications de rappel génèrent des emails envoyés aux utilisateurs selon des critères spécifiés. Les notifications de rappel rappellent aux utilisateurs qu’une action doit être effectuée pour une tâche, un problème, un projet ou une feuille de temps.
author: Alina, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 4%

---

# Configurer des notifications de rappel

<!-- Audited: 1/2024 -->

En tant qu’administrateur Workfront, vous pouvez créer des notifications de rappel pour les utilisateurs et les associer à des objets auxquels vous souhaitez que vos utilisateurs accordent une attention particulière.

Les notifications de rappel génèrent des emails envoyés aux utilisateurs selon des critères spécifiés. Les notifications de rappel rappellent aux utilisateurs qu’une action doit être effectuée pour une tâche, un problème, un projet ou une feuille de temps.

Après avoir créé les notifications de rappel, les utilisateurs peuvent les associer manuellement aux tâches, telles que les projets, les tâches, les problèmes et les feuilles de temps. Pour plus d’informations, voir [Joindre une notification de rappel à un objet](/help/quicksilver/workfront-basics/using-notifications/attach-reminder-notification-object.md).

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard </p>
 <p>ou</p> 
<p>Actuel : formule</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Planificateur ou version ultérieure, avec accès administratif aux notifications de rappel</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personnalisation de l’email de rappel

Vous pouvez personnaliser l’objet, le corps et le HTML dans l’email de notification de rappel.

Vous pouvez également utiliser l&#39;email par défaut inclus dans la notification de rappel. L’e-mail par défaut utilise le nom de la notification de rappel comme objet de l’e-mail et le nom de l’objet dans le corps de l’e-mail, y compris l’événement qui a déclenché la notification.

Si vous souhaitez personnaliser l&#39;email de rappel, vous devez créer un modèle d&#39;email et le joindre à la notification de rappel.

Pour plus d’informations sur la création d’un modèle de courrier électronique, voir [Configurer des modèles de courrier électronique](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Créer une notification de rappel

{{step-1-to-setup}}

1. Cliquez sur **Email** > **Notifications** > **Notifications de rappel**.

   ![](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. Cliquez sur **Nouvelle notification de rappel**.

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
      <td> <p>Spécifiez le nombre d’heures, de jours de travail, de jours (jours calendaires), de semaines ou de mois avant ou après la date dans la variable <strong>Minutage</strong> champ .</p> <p><b>REMARQUE</b>:  
        <ul> 
         <li> <p>Les notifications de rappel démarrent 24 heures après la date spécifiée et une fois tous les critères satisfaits.</p> </li> 
         <li> <p>Les notifications de rappel pour les projets, les tâches et les problèmes se déclenchent toutes les nuits à minuit, heure des Rocheuses. Tous les objets qui remplissent les critères d’une notification de rappel à partir de cette journée déclenchent une notification aux utilisateurs désignés peu de temps après cette date.</p> </li> 
         <li> <p>Les notifications de rappel pour les feuilles de temps sont envoyées à l’heure spécifiée en fonction du fuseau horaire et de la date de fin, de la date de début ou de la date de dernière mise à jour de la feuille de temps.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planning</td> 
      <td> <p>Sélectionnez l'événement qui déclenche la planification de la notification de rappel.</p> <p>Si la notification de rappel est destinée aux projets, tâches ou problèmes, les options disponibles sont liées à la date de fin ou à la date de début. La notification de rappel prend en compte l’horodatage des dates de fin et de début des projets, tâches et problèmes.</p>

   <p>Si la notification de rappel est destinée aux feuilles de calcul, les options disponibles sont liées à la date de fin, à la date de début ou à la date de dernière mise à jour. La notification de rappel pour les feuilles horaires prend en compte l’horodatage de fin de la feuille de temps, de début et de date de dernière mise à jour. La feuille de calcul commence à minuit le jour de la date de début (12h00) et se termine juste avant minuit la date de fin (23h59).</p>

   <p><b>NOTE</b></p>
      <p>Les notifications de rappel de la feuille de temps ne sont distribuées qu’une fois toutes les 24 heures.</p> <p>Lorsque vous configurez plusieurs notifications de rappel dans une période de 24 heures, Workfront envoie un email de notification avec tous les rappels inclus dans cette notification.</p>
      <p>Par exemple, si vous configurez trois notifications de rappel pour qu’elles se déclenchent 10 heures avant, 2 heures avant et 1 heure avant une date d’échéance, les trois rappels seront tous combinés dans la même notification s’ils se produisent le même jour.</p> <p>Cependant, si vous définissez une notification de rappel pour 26 heures avant et une autre pour 1 heure avant l’échéance, les utilisateurs recevront deux notifications distinctes. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Critères</td> 
      <td> <p>Sélectionnez les critères pour qualifier la notification de rappel à programmer. Les notifications de rappel ne sont pas planifiées, sauf si la sélection de critères est respectée.</p> <p>Les options de critères suivantes sont disponibles, selon le type d’objet sélectionné à l’étape 4 :</p> 
       <ul> 
        <li><strong>Incomplète dans les projets en cours :</strong> <i>(Disponible pour les rappels de tâche et de problème)</i> L’envoi de la notification de rappel est programmé uniquement lorsque l’état de l’objet auquel la notification de rappel est associée n’est pas Terminé et que l’état du projet est Actuel.</li> 
        <li><strong>Tous dans les projets en cours :</strong> <i>(Disponible pour les rappels de tâche et de problème)</i> L’envoi de la notification de rappel est planifié quel que soit l’état de l’objet. Cette notification doit être envoyée uniquement lorsque l’état du projet auquel la notification de rappel est associée est Actuel.</li> 
        <li><strong>Projets incomplets :</strong> <i>(Disponible pour les rappels de projet)</i> L’envoi de la notification de rappel est programmé lorsque l’état du projet est autre que Terminé.</li> 
        <li><strong>Tous les projets :</strong> <i>(Disponible pour les rappels de projet)</i> L’envoi de la notification de rappel est programmé quel que soit l’état du projet.</li> 
        <li><strong>Ouvrir les feuilles de temps :</strong> <i>(Disponible pour les rappels de feuille de temps)</i> L'envoi de la notification de rappel est programmé lorsque l'état de la feuille de temps est Ouverture.</li> 
        <li><strong>Feuilles de temps envoyées :</strong> <i>(Disponible pour les rappels de feuille de temps)</i> L'envoi de la notification de rappel est programmé lorsque l'état de la feuille de temps est Envoyé.</li> 
        <li><strong>Ouvrez la feuille de temps ou moins de 40 heures par semaine :</strong> <i>(Disponible pour les rappels de feuille de temps)</i> L'envoi de la notification de rappel est programmé lorsque l'état de la feuille de temps est Ouverture ou lorsque la feuille de temps est enregistrée depuis moins de 40 heures.</li> 
        <li><strong>Modèle de courrier électronique :</strong> Dans la liste déroulante, sélectionnez un modèle d'email à joindre à votre rappel.<br>Pour plus d’informations sur la création d’un modèle d’email, reportez-vous à la section <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Configurer des modèles de courrier électronique</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Destinataires</td> 
      <td><p>En fonction de l’objet pour lequel la notification de rappel est envoyée, sélectionnez l’un des types d’utilisateurs suivants auxquels vous souhaitez envoyer la notification :</p>
      <ul>
      <li>Affecté à</li>
      <li>Entré par</li>
      <li>Équipe de projet (tous les utilisateurs de l’équipe de projet reçoivent un rappel)</li>
      <li>Affectations de tâches dépendantes (les utilisateurs affectés à des tâches dépendantes reçoivent le rappel)</li>
      <li>Propriétaire du projet</li>
      <li>Affecté à (les utilisateurs affectés à une tâche ou à un problème reçoivent le rappel)</li>
      <li>Propriétaire de feuille de temps</li>
      <li>Approbateur de feuilles de temps</li>
      <li>Gestionnaire du propriétaire de feuille de temps</li></ul>
      </td> 
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

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Diagnostics** dans le coin inférieur gauche de Workfront.

1. Cliquez sur **Envoyer des notifications de rappel** et attendez la confirmation en haut de l’écran qu’ils ont été envoyés.

   Les utilisateurs désignés dans la notification de rappel reçoivent un email.

![](assets/reminder-test.png)