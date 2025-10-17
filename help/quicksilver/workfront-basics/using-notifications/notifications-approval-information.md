---
content-type: reference
navigation-topic: notifications
title: 'Notifications : informations d’approbation'
description: Les notifications suivantes vous alertent sur les activités d’approbation qui se produisent sur un élément de travail auquel vous participez. Pour plus d’informations sur la configuration des notifications que vous recevez, voir Modifier vos propres notifications par e-mail.
author: Courtney
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 100%

---

# Notifications : informations d’approbation

Les notifications suivantes vous alertent sur les activités d’approbation qui se produisent sur un élément de travail auquel vous participez. Pour plus d’informations sur la configuration des notifications que vous recevez, consultez la section [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consultez également la section [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th> <p>Champs inclus </p> <p> * Champs de résumé quotidien uniquement</p> </th> 
   <th>Statut par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Une demande d’approbation d’événement déléguée a été remplie.</strong> </p> <p>Une approbation de problème que vous avez déléguée à une autre personne a été approuvée ou rejetée par cette personne.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Issue Approval/ Rejection Made on Your Behalf by] &lt;User Name&gt;</em>.</p> <p>L’objet de la notification de synthèse quotidienne est : <em>[!UICONTROL Digest of Approval Information] &lt;Date of daily digest&gt;</em>.</p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de la personne qui a approuvé/rejeté le problème pour votre compte<br>Décision d’approbation<br>Statut du problème<br>Nom de la personne qui a demandé l’approbation<br><strong>Bouton [!UICONTROL See More Details]</strong><br>* Numéro de référence du projet<br>* Nom du projet<br>* Nombre total d’autorisations de publication déléguées<br>* Nom du problème<br>* Nom de la personne approbatrice<br>* Date de la synthèse quotidienne<br><br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d’approbation de projet déléguée a été remplie.</strong> </p> <p>Une approbation de projet que vous avez déléguée à une autre personne a été approuvée ou rejetée par cette personne.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Project Approval/ Rejection Made on Your Behalf by] &lt;User Name&gt;</em>.</p> <p><em>L’objet de la notification de synthèse quotidienne est : [!UICONTROL Digest of Approval Information] &lt;Date of daily digest&gt;</em>. </p> </td> 
   <td> Nom du projet<br>[!UICONTROL Portfolio Name]<br>[!UICONTROL Project Reference Number]<br>Nom de la personne qui a approuvé/rejeté le projet pour votre compte<br>[!UICONTROL Approval Decision]<br>[!UICONTROL Project Status]<br>Nom de la personne qui a demandé l’approbation<br><strong>Bouton [!UICONTROL See More Details]</strong><br>* Numéro de référence du projet<br>* Nom du projet<br>* Nom de la personne approbatrice<br>[!UICONTROL *Date of the daily digest]<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d’approbation de tâche déléguée a été remplie.</strong> </p> <p>Une approbation de tâche que vous avez déléguée à une autre personne a été approuvée ou rejetée par cette personne.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Task Approval/ Rejection Made on Your Behalf by] &lt;User Name&gt;</em>.</p> <p>L’objet de la notification de synthèse quotidienne est : <em>[!UICONTROL Digest of Approval Information] &lt;Date of daily digest&gt;</em>.</p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de la personne qui a approuvé/rejeté la tâche pour votre compte<br>Décision d’approbation<br>Statut de la tâche<br>Nom de la personne qui a demandé l’approbation<br><strong>Bouton Plus de détails</strong><br>* Numéro de référence du projet<br>* Nom du projet<br>* Nombre total d’autorisations de tâches déléguées<br>* Nom de la tâche<br>* Nom de la personne approbatrice<br>* Date de la synthèse quotidienne<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d’approbation de document a été annulée.</strong> </p> <p>L’approbateur ou l’approbatrice du document reçoit une notification par e-mail lorsque la demande d’approbation du document est annulée.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>&lt;User Name&gt; [!UICONTROL canceled the document approval request]</em>.</p> <p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un e-mail de synthèse quotidienne.</p> </p> </td> 
   <td> Nom de la personne qui a annulé la demande d’approbation <br>[!UICONTROL Document Name]. </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>J’ai reçu une délégation en tant que personne approbatrice.</strong> </p> <p>Si une approbation vous a été déléguée, vous recevez une notification par e-mail. </p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Delegated] &lt;Object Type&gt; [!UICONTROL Approval - Please Review] &lt;Object Name&gt;</em>.</p> <p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un e-mail de synthèse quotidienne.</p> </p> </td> 
   <td> <p>[!UICONTROL Object Name]<br>[!UICONTROL Parent Object Name]<br>[!UICONTROL Object Reference Number]<br>Nom de la personne qui a soumis l’objet à approbation<br>Nom de la personne au nom de laquelle vous approuvez l’objet<br>Statut de l’objet<br>Date et heure de la demande d’approbation<br>Priorité de l’objet<br>Nom de l’étape d’approbation<br>[!UICONTROL Planned Completion Date] de l’objet<br><strong>Bouton [!UICONTROL Make Approval Decision]</strong></p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu’une feuille de temps est acceptée et fermée, envoyer un e-mail à la personne.</strong> </p> <p>Une fois votre feuille de temps validée, vous recevez une notification par e-mail.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Timesheet Approved] : &lt;Timesheet Start Date&gt; - &lt;Timesheet End Date&gt;</em>.</p> <p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un e-mail de synthèse quotidienne.</p> </p> </td> 
   <td> Nom de la personne qui a approuvé votre feuille de temps<br>Date et heure de l’approbation de la feuille de temps<br>Statut de la feuille de temps ([!UICONTROL Approved])<br>Date de début et date de fin de la feuille de temps<br>Nombre total d’heures consignées dans la feuille de temps<br>Heures supplémentaires consignées dans la feuille de temps </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
 </tbody> 
</table>
