---
content-type: reference
navigation-topic: notifications
title: 'Notifications : validations unifiées'
description: Les notifications suivantes vous avertissent des activités d’approbation relatives à l’expérience Approbations unifiées . Pour plus d’informations sur la configuration des notifications que vous recevez, voir Modifier vos propres notifications par e-mail.
author: Courtney
feature: Get Started with Workfront
exl-id: 6e60a9ec-4fe0-4f3d-a4dd-8dc09d11b834
last-update: 2026-10-20T00:00:00.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 7957c410d4a0e39b23b4f5a3d29a794e5deec72a
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 3%
---
# Notifications : validations unifiées

{{highlighted-preview}}

Utilisez les notifications suivantes pour rester informé des activités relatives à la Révision et aux approbations unifiées. Pour plus d’informations sur la configuration des notifications par e-mail que vous recevez, voir [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Ces notifications sont disponibles uniquement en tant que notifications instantanées et ne sont pas disponibles dans un résumé quotidien.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notification</th> 
   <th>Champs inclus</th> 
   <th>Statut par défaut</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Approbation terminée - Approuvée</strong> </p> <p>Une approbation de document se termine par une décision finale d’Approuvé.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>La décision finale : (document) est approuvée</em></p> </td> 
   <td> <p>Décision finale<br>Document<br>Approbation demandée date<br>Échéance<br> bouton « Aller à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Message personnalisé<br>Étape<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Approbation terminée - Approuvé avec des modifications</strong> </p> <p>Une approbation de document se termine par une décision finale d’Approuvé avec des modifications.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>La décision finale : (document) est approuvée avec des modifications</em></p> </td> 
   <td> <p>Décision finale<br>Document<br>Approbation demandée date<br>Échéance<br> bouton « Aller à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Message personnalisé<br>Étape<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Approbation terminée - Travail nécessaire</strong> </p> <p>L’approbation du document se termine par une décision finale indiquant que le travail doit être effectué.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Décision finale : (document) nécessite un travail</em></p> </td> 
   <td> <p>Décision finale<br>Document<br>Approbation demandée date<br>Échéance<br> bouton « Aller à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Message personnalisé<br>Étape<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La date limite approche</strong> </p> <p>L’échéance d’une approbation de document à laquelle vous participez approche.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Date limite d’approbation approchant pour (Document)</em></p> </td> 
   <td> <p>Demandeur<br>Votre rôle<br>Équipe<br>Approbation date demandée<br>Date d’échéance<br> bouton « Accéder à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Aperçu du document<br>Message personnalisé<br>Étape<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Échéance passée</strong> </p> <p>L’approbation de document à laquelle vous participez dépasse son délai sans décision finale.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Délai d’approbation dépassé pour (Document)</em></p> </td> 
   <td> <p>Titre fixe<br>Date de demande d’approbation<br>Date d’échéance<br> Bouton « Accéder à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Phase</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Révision terminée</strong> </p> <p>Un réviseur termine sa révision lors de l’approbation d’un document.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>(Document) a été révisé</em></p> </td> 
   <td> <p>Réviseur<br>Document<br> bouton « Accéder à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Aperçu du document<br>Phase<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>La limite de validation de la vidéo approche (80 %)</strong> </p> <p>Une approbation vidéo atteint 80 % de la limite d’approbation vidéo de son plan.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Vous êtes proche de la limite de votre demande annuelle d’approbation vidéo dans Workfront</em></p> </td> 
   <td> Titre et corps du texte<br>Validations vidéo demandées (utilisation actuelle)<br>Plafond total (limite)<br>Autres destinataires<br>Bouton « Afficher dans Workfront » <br>« Mettre à niveau vers FIO Grands comptes » </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Limite d’approbation vidéo atteinte</strong> </p> <p>Une approbation vidéo atteint la limite d’approbation vidéo de son plan.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Vous avez atteint la limite de votre demande annuelle d’approbation vidéo dans Workfront</em></p> </td> 
   <td> Titre et corps du texte<br>Validations vidéo demandées (utilisation actuelle)<br>Plafond total (limite)<br>Autres destinataires<br>Bouton « Afficher dans Workfront » <br>« Mettre à niveau vers FIO Grands comptes » </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Décision prise - Approuvée</strong> </p> <p>Un approbateur prend une décision Approuvé pour l’approbation d’un document.</p> <p>L'objet de l'e-mail de notification instantanée est : <em>(Document) approuvé par (Nom)</em></p> </td> 
   <td> <p>Décideur<br>Décision<br>Document et version<br> Bouton « Accéder à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Aperçu du document<br>Message personnalisé<br>Étape<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Décision prise - Approuvée avec des modifications</strong> </p> <p>Un approbateur prend une décision Approuvée avec des modifications pour l’approbation d’un document.</p> <p>L'objet de l'e-mail de notification instantanée est : <em>(Document) approuvé avec des modifications par (Nom)</em></p> </td> 
   <td> <p>Décideur<br>Décision<br>Document et version<br> Bouton « Accéder à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Aperçu du document<br>Message personnalisé<br>Étape<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Décision prise - Travail nécessaire</strong> </p> <p>Un approbateur ou une approbatrice prend une décision indiquant que l’approbation d’un document nécessite un travail.</p> <p>L'objet de l'e-mail de notification instantanée est : <em>(Document) nécessite un travail de (Nom)</em></p> </td> 
   <td> <p>Décideur<br>Décision<br>Document et version<br> Bouton « Accéder à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Aperçu du document<br>Message personnalisé<br>Étape<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Documents ajoutés ou supprimés lors d'une validation groupée</strong> </p> <p>Les documents sont ajoutés ou supprimés lors de l’approbation d’un document groupé dont vous faites partie.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Un document a été ajouté à une approbation à laquelle vous faites partie ou en a été supprimé</em></p> </td> 
   <td> <p><strong>Ajouté :</strong><br>Demandeur<br>Nom du groupe<br>Aperçu de la miniature<br>Dates<br> bouton « Accéder à la révision »<br>Bloc de détails : Nom du groupe, Nombre de ressources, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Message personnalisé<br>Projet</p> <p><strong>Supprimé :</strong><br>Demandeur<br>Nom du groupe<br>Aperçu de la miniature (pas de bouton ni de bloc Détails)</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Toutes les révisions sont terminées</strong> </p> <p>Chaque réviseur termine sa révision lors de l’approbation d’un document.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Toutes les révisions sont terminées le (document)</em></p> </td> 
   <td> <p>Document<br>Approbation demandée date<br>Date d’échéance<br> bouton « Aller à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Message personnalisé<br>Étape<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Rappel - 24 heures</strong> </p> <p>Il vous reste 24 heures pour examiner et approuver le document.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Rappel : votre approbation est nécessaire le (document)</em></p> </td> 
   <td> <p>Demandeur<br>Votre rôle<br>Équipe<br>Approbation date demandée<br>Date d’échéance<br> bouton « Accéder à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Aperçu du document<br>Message personnalisé<br>Étape<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Rappel - 72 heures</strong> </p> <p>Il vous reste 72 heures pour examiner et approuver le document.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Rappel : votre approbation est nécessaire le (document)</em></p> </td> 
   <td> <p>Demandeur<br>Votre rôle<br>Équipe<br>Approbation date demandée<br>Date d’échéance<br> bouton « Accéder à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Aperçu du document<br>Message personnalisé<br>Étape<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ajouté en tant qu’approbateur ou réviseur</strong> </p> <p>Vous êtes ajouté en tant qu’approbateur ou réviseur à une approbation de document.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Votre approbation est nécessaire le (document)</em></p> </td> 
   <td> <p>Demandeur<br>Votre rôle<br>Équipe<br>Approbation date demandée<br>Date d’échéance<br> bouton « Accéder à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Aperçu du document<br>Message personnalisé<br>Étape<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Supprimé en tant qu'approbateur ou réviseur</strong> </p> <p>Vous êtes supprimé(e) en tant qu’approbateur ou réviseur d’une approbation de document.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Votre approbation n’est plus nécessaire le (document)</em></p> </td> 
   <td> <p>Demandeur<br>document et version<br>Rôle<br>Équipe (pas de bouton ni de bloc Détails)</p> <p><em>Inclus lors de la validation :</em><br>Prévisualisation du document<br>Message personnalisé</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Rôle modifié</strong> </p> <p>Votre rôle d’approbateur ou de réviseur change lors de l’approbation d’un document.</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>Votre rôle sur (document) a changé</em></p> </td> 
   <td> <p>Demandeur<br>document et version<br>sens du changement de rôle<br> bouton « Aller à la révision »<br>Bloc de détails : Nom du document, Détails du document, Tous les destinataires</p> <p><em>Inclus lors de la validation :</em><br>Aperçu du document<br>Phase<br>Projet</p> </td> 
   <td><strong>Instantané</strong> </td> 
  </tr> 
 </tbody> 
</table>
