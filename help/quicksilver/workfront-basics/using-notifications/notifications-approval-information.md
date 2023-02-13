---
content-type: reference
navigation-topic: notifications
title: 'Notifications : Informations de validation"'
description: Les notifications suivantes vous alertent sur les activités d’approbation qui se produisent sur un élément de travail auquel vous êtes impliqué. Pour plus d’informations sur la configuration des notifications que vous recevez, voir Activation ou désactivation de vos propres notifications d’événement.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 6%

---

# Notifications : Informations de validation

Les notifications suivantes vous alertent sur les activités d’approbation qui se produisent sur un élément de travail auquel vous êtes impliqué. Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Activation ou désactivation de vos propres notifications d’événement](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Une demande d'approbation d'événement déléguée a été remplie</strong> </p> <p>Une approbation de problème que vous avez déléguée à un autre utilisateur a été approuvée ou rejetée par cet utilisateur.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Problème Approbation / Rejet effectué en votre nom par] &lt;user name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Digest of Approval Information] (Résumé des informations d’approbation) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nom du problème<br>Nom du projet<br>Numéro de référence du problème<br>Nom de l’utilisateur qui a approuvé/rejeté le problème en votre nom<br>Décision d’approbation<br>État du problème<br>Nom de l’utilisateur qui a demandé l’approbation<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Numéro de référence du projet<br>*Nom du projet<br>*Nombre total d’approbations de problèmes déléguées<br>*Nom du problème<br>*Nom de l’approbateur<br>*Date du résumé quotidien<br><br></p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d'approbation de projet déléguée a été remplie</strong> </p> <p>Une approbation de projet que vous avez déléguée à un autre utilisateur a été approuvée ou rejetée par cet utilisateur.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Approbation/Rejet du projet par votre nom] &lt;user name=""&gt;</em></p> <p><em>L’objet de la notification quotidiennement Digest est : [!UICONTROL Digest of Approval Information] (Résumé des informations d’approbation) &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> Nom du projet<br>[!UICONTROL Portfolio Name]<br>[!UICONTROL Numéro de référence du projet]<br>Nom de l’utilisateur qui a approuvé/rejeté le projet pour votre compte<br>[!UICONTROL Approval Decision]<br>[!UICONTROL État du projet]<br>Nom de l’utilisateur qui a demandé l’approbation<br><strong>[!UICONTROL Voir Plus De Détails]</strong> button<br>*Numéro de référence du projet<br>*Nom du projet<br>*Nom de l’approbateur<br>[!UICONTROL *Date du résumé quotidien]<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d'approbation de tâche déléguée a été remplie</strong> </p> <p>Une approbation de tâche que vous avez déléguée à un autre utilisateur a été approuvée ou rejetée par cet utilisateur.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Approbation/Rejet de tâche effectué en votre nom par] &lt;user name=""&gt;</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Digest of Approval Information] (Résumé des informations d’approbation) &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom de la tâche<br>Nom du projet<br>Numéro de référence de la tâche<br>Nom de l’utilisateur qui a approuvé/rejeté la tâche en votre nom<br>Décision d’approbation<br>État de la tâche<br>Nom de l’utilisateur qui a demandé l’approbation<br><strong>Voir Plus de détails</strong> button<br>*Numéro de référence du projet<br>*Nom du projet<br>*Nombre total d’approbations de tâches déléguées<br>*Nom de la tâche<br>*Nom de l’approbateur<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Une demande d'approbation du document est annulée</strong> </p> <p>L’approbateur du document reçoit une notification par courrier électronique lorsque la demande d’approbation du document est annulée.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>&lt;user name=""&gt; [!UICONTROL a annulé la demande d’approbation de document]</em></p> <p> <p>Remarque : Vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </p> </td> 
   <td> Nom de l’utilisateur qui a annulé la demande de validation<br>[!UICONTROL Document Name] </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Je suis délégué en tant qu'approbateur</strong> </p> <p>Si une personne vous a délégué une approbation, vous recevez une notification par e-mail. </p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Délégué] &lt;object type=""&gt; [!UICONTROL Approbation - Veuillez Réviser] &lt;object name=""&gt;</em></p> <p> <p>Remarque : Vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </p> </td> 
   <td> <p>[!UICONTROL Object Name]<br>[!UICONTROL Parent Object Name]<br>[!UICONTROL Object Reference Number]<br>Nom de l’utilisateur qui a soumis l’objet à approbation<br>Nom de l’utilisateur au nom duquel vous approuvez l’objet<br>Statut de l’objet<br>Date et heure auxquelles l’approbation a été demandée<br>Priorité de l’objet<br>Nom de l’étape de validation<br>[!UICONTROL Date d’achèvement planifiée] de l’objet<br><strong>[!UICONTROL Effectuer une décision d’approbation]</strong> button</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu'une feuille de temps est acceptée et fermée, envoyer un e-mail à l'utilisateur</strong> </p> <p>Une fois votre feuille de temps validée, vous recevez une notification par e-mail.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Frise chronologique approuvée] : &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>Remarque : Vous ne pouvez pas configurer cette notification pour un courrier électronique de résumé quotidien.</p> </p> </td> 
   <td> Nom de l’utilisateur qui a approuvé votre feuille de calcul<br>Date et heure d’approbation de la feuille de calcul<br>État de la feuille de calcul ([!UICONTROL Approuvé])<br>Date de début et date de fin de la feuille de temps<br>Nombre total d’heures consignées dans la feuille de calcul<br>Heures de dépassement de délai connectées à la feuille de calcul </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
 </tbody> 
</table>
