---
content-type: reference
navigation-topic: notifications
title: "Notifications : informations de validation"
description: Les notifications suivantes vous alertent sur les activités d’approbation qui se produisent sur un élément de travail auquel vous êtes impliqué. Pour plus d’informations sur la configuration des notifications que vous recevez, voir Modification de vos propres notifications par e-mail.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 3%

---

# Notifications : informations sur l’approbation

Les notifications suivantes vous alertent sur les activités d’approbation qui se produisent sur un élément de travail auquel vous êtes impliqué. Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Modification de vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Voir aussi [Notifications d’événements](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th> <p>Champs inclus </p> <p> *Champs de résumé quotidien uniquement</p> </th> 
   <th>État par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Une demande d’approbation de problème déléguée est terminée</strong> </p> <p>Une approbation de problème que vous avez déléguée à un autre utilisateur a été approuvée ou rejetée par cet utilisateur.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Problème Approbation/Rejet effectué en votre nom par] &lt;Nom d’utilisateur&gt;</em></p> <p>Le sujet de la notification de résumé quotidien est :<em> [!UICONTROL Digest of Approval Information] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a approuvé/rejeté le problème en votre nom<br>Décision d’approbation<br>État du problème<br>Nom de l’utilisateur qui a demandé l’approbation<br><strong>[!UICONTROL Voir plus de détails]</strong><br>*Numéro de référence du projet<br>*Nom du projet<br>}*Nombre total d’approbation des problèmes <br>}}}}}}*Nombre total d’approbation des problèmes délégués<br>*Nom de l’approbateur<br>*Date du résumé quotidien<br><br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d’approbation de projet déléguée est terminée</strong> </p> <p>Une approbation de projet que vous avez déléguée à un autre utilisateur a été approuvée ou rejetée par cet utilisateur.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Approbation/Rejet du projet effectué en votre nom] &lt;Nom d’utilisateur&gt;</em></p> <p><em>Le sujet de la notification de résumé quotidien est : [!UICONTROL Digest of Approval Information] &lt;Date of daily digest&gt;</em> </p> </td> 
   <td> Nom du projet<br>[!UICONTROL Nom du Portfolio]<br>[!UICONTROL Numéro de référence du projet]<br>Nom de l’utilisateur qui a approuvé/rejeté le projet en votre nom<br>[!UICONTROL Décision d’approbation]<br>[!UICONTROL État du projet]<br>Nom de l’utilisateur qui a demandé l’approbation<br><strong>[!UICONTROL Voir plus de détails]</strong>}}<br> Numéro de référence du projet<br>*Nom du projet<br>*Nom de l’approbateur<br>[!UICONTROL *Date du résumé quotidien]<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d’approbation de tâche déléguée est terminée</strong> </p> <p>Une approbation de tâche que vous avez déléguée à un autre utilisateur a été approuvée ou rejetée par cet utilisateur.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Validation/Rejet de la tâche effectué en votre nom] &lt;Nom d’utilisateur&gt;</em></p> <p>Le sujet de la notification de résumé quotidien est :<em> [!UICONTROL Digest of Approval Information] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a approuvé/rejeté la tâche en votre nom<br>Décision d’approbation<br>État de la tâche<br>Nom de l’utilisateur qui a demandé l’approbation<br><strong>Voir plus de détails</strong>}*Numéro de référence du projet<br>*Nom du projet<br>*Nombre total d’approbations de la tâche déléguée<br>*Nom de la tâche<br>*Nom de la tâche ver Name<br>*Date du résumé quotidien<br><br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d'approbation de document est annulée</strong> </p> <p>L’approbateur ou l’approbatrice du document reçoit une notification par e-mail lorsque la demande d’approbation du document est annulée.</p> <p>L’objet de l’email de notification instantanée est : <em>&lt;Nom d’utilisateur&gt; [!UICONTROL a annulé la demande d’approbation de document]</em></p> <p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </p> </td> 
   <td> Nom de l’utilisateur qui a annulé la demande d’approbation<br>[!UICONTROL Nom du document] </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Je suis délégué en tant qu’approbateur</strong> </p> <p>Si une personne vous a délégué une approbation, vous recevez une notification par e-mail. </p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Délégué] &lt;Type d’objet&gt; [!UICONTROL Approbation - Veuillez consulter] &lt;Nom de l’objet&gt;</em></p> <p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </p> </td> 
   <td> <p>[!UICONTROL Object Name]<br>[!UICONTROL Parent Object Name]<br>[!UICONTROL Object Reference Number]<br>Nom de l’utilisateur qui a soumis l’objet pour approbation<br>Nom de l’utilisateur au nom duquel vous approuvez l’objet<br>Object Status<br>Date et heure auxquelles l’approbation a été demandée<br>Object Priority<br>Approval Name<br>[!UICONTROL L Date d’achèvement planifiée] du bouton Object<br><strong>[!UICONTROL Make Approval Decision]</strong></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ma feuille de temps est approuvée</strong> </p> <p>Une fois votre feuille de temps validée, vous recevez une notification par e-mail.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Frise chronologique approuvée] : &lt;Date de début de la feuille de temps&gt; - &lt;Date de fin de la feuille de temps&gt;</em></p> <p> <p>Remarque : vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </p> </td> 
   <td> Nom de l’utilisateur qui a approuvé votre feuille de temps<br>Date et heure d’approbation de la feuille de temps<br>État de la feuille de temps ([!UICONTROL Approuvé])<br>Date de début et date de fin de la feuille de temps<br>Nombre total d’heures consignées dans la feuille de temps<br>Heures d’ouverture connectées dans la feuille de temps </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
 </tbody> 
</table>
