---
content-type: reference
navigation-topic: notifications
title: "Notifications : communication"
description: Les notifications suivantes vous alertent sur la communication, par exemple un commentaire de mise à jour, qui se produit sur un élément de travail auquel vous êtes impliqué. Pour plus d’informations sur la configuration des notifications que vous recevez, voir Modification de vos propres notifications par e-mail.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 18%

---

# Notifications : communication

Les notifications suivantes vous alertent sur la communication, par exemple un commentaire de mise à jour, qui se produit sur un élément de travail auquel vous êtes impliqué. Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Modification de vos propres notifications électroniques](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Ces notifications vous avertissent de tous les commentaires qui ont été publiés sur un élément spécifique. Pour cette raison, vous devez sélectionner ou désélectionner toutes les notifications en même temps pour les diffuser dans un email de résumé quotidien. Si vous souhaitez être averti de certains commentaires uniquement au fur et à mesure qu’ils se produisent, vous pouvez spécifier que les notifications individuelles doivent être envoyées instantanément.

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
   <td> <p><strong>Quelqu'un m'a inclus dans une mise à jour dirigée.</strong> </p> <p>Une mise à jour dirigée est lorsqu’un utilisateur inclut spécifiquement un autre utilisateur dans une mise à jour, comme décrit dans <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Baliser les autres sur] mises à jour</a>.</p> <p>Dans ce cas, l’utilisateur ou l’utilisatrice qui est inclus dans la mise à jour dirigée reçoit une notification par e-mail concernant la mise à jour.</p> <p>La notification électronique n’est envoyée que si l’utilisateur dispose des droits d’accès à l’objet .</p> <p>Le sujet de l'email de notification instantanée est : <em>&lt;Nom de l'utilisateur qui vous a inclus dans la mise à jour&gt; [!UICONTROL voulait que vous connaissiez]</em></p> <p>Le sujet de la notification quotidiennement de résumé est : <em>[!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> Nom d’objet où la mise à jour a été effectuée <br>Nom d’objet parent<br>Numéro de référence d’objet<br>Noms de tous les utilisateurs et équipes inclus dans la mise à jour dirigée<br>Date et heure auxquelles la mise à jour a été effectuée<br>Texte de la mise à jour dirigée<br><strong>[!UICONTROL Comment]</strong><br>*Nombre total de commentaires reçus<br>*Nombre pour chaque objet<br>}}*<strong>* CONTROL Voir toutes les notifications]</strong> button<br>*Date du résumé quotidien<br></td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un répond à ma demande</strong> </p> <p>Une fois qu’un utilisateur a envoyé une demande de travail et qu’un autre utilisateur a répondu à cette demande, l’utilisateur qui l’a envoyée reçoit une notification par courrier électronique.</p> <p>Une notification par e-mail n’est pas envoyée si :</p> 
    <ul> 
     <li> <p>L’utilisateur ou l’utilisatrice qui envoie la réponse est la même personne que celle qui a effectué la demande.</p> </li> 
     <li> <p>L’utilisateur ou l’utilisatrice n’a pas accès en affichage à la note.</p> </li> 
    </ul><strong>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Commentaire sur] &lt;Nom de la demande&gt; sur &lt;Nom du projet&gt; (réf. &lt;Numéro de référence de la demande&gt;)</em></strong> L’objet de la notification de résumé quotidienne est :<em> [!UICONTROL Résumé de la communication] &lt;Date du résumé quotidien&gt;</em></td> 
   <td> Nom de la demande<br>Nom du projet<br>Numéro de référence<br>Nom de l’utilisateur qui a répondu à votre demande<br>Date et heure auxquelles le commentaire a été fait<br>Texte de commentaire effectué sur votre demande<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque demande<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong>}<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un commentaire est publié sur ma requête</strong> </p> <p>Le contact principal pour un problème reçoit une notification par courrier électronique lorsqu’un commentaire est publié sur une demande du [!UICONTROL Help Desk], sauf si l’utilisateur qui a publié le commentaire est également le contact principal pour le problème.</p> <p>Tous les utilisateurs et toutes les utilisatrices qui sont directement inclus dans le commentaire reçoivent également une notification par e-mail.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Commentaire sur] &lt;Nom de la demande&gt; sur &lt;Nom du projet&gt; (réf. &lt;Numéro de référence de la demande&gt;)</em></p> <p>Le sujet de la notification quotidiennement de résumé est :<em> [!UICONTROL Digest of Communication] &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> Nom de la demande<br>Nom du projet<br>Numéro de référence<br>Nom de l’utilisateur qui a répondu à votre demande<br>Date et heure auxquelles le commentaire a été fait<br>Texte de commentaire effectué sur votre demande<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque demande<br>*Nom du projet<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong>}}} *Date du résumé quotidien<br><br></td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un commentaire est ajouté sur mon document</strong> </p> <p>Le propriétaire d’un document dans [!DNL Adobe Workfront] reçoit une notification par courrier électronique lorsqu’un commentaire est publié sur le document, sauf si l’utilisateur qui a publié le commentaire est également le propriétaire du document.</p> <p>Tous les utilisateurs et toutes les utilisatrices qui sont directement inclus dans le commentaire reçoivent également une notification par e-mail.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel]. </p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Commentaire sur] &lt;Nom de la demande&gt; sur &lt;Nom du projet&gt; (réf. &lt;Numéro de référence de la demande&gt;)</em></p> <p> Le sujet de la notification quotidiennement de résumé est :<em> [!UICONTROL Digest of Communication] &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td>Nom du document<br>Nom du projet, de la tâche ou du problème<br>Numéro de référence<br>Nom de l’utilisateur qui a répondu à votre demande<br>Date et heure auxquelles le commentaire a été fait<br>Texte de commentaire fait sur le document</td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un commente un thread dans lequel je suis </strong> </p> <p>Les participantes et participants au thread et les utilisateurs et utilisatrices inclus dans un message direct reçoivent une notification par e-mail lorsqu’une personne fait un commentaire dans le thread.</p> <p>Les utilisateurs doivent disposer d’un accès [!UICONTROL View] pour recevoir une notification.</p> <p>Les utilisateurs et utilisatrices suivants ne reçoivent pas de notification :</p> 
    <ul> 
     <li>Équipes incluses dans un message direct</li> 
     <li>Personne propriétaire de la note</li> 
     <li>Contact principal</li> 
    </ul> <p><strong>L’objet de l’email de notification instantanée est : <em>[!UICONTROL RE : Commentaire sur] &lt;Nom de l’objet&gt;&lt;Type d’objet&gt; sur &lt;Nom du projet&gt;(ref# &lt;Numéro de référence de l’objet&gt;</em>)</strong> </p> <p><strong> Le sujet de la notification quotidiennement de résumé est :<em> [!UICONTROL Digest of Communication] &lt;Date du résumé quotidien&gt;</em></strong> </p> </td> 
   <td> Nom de l’objet<br>Nom de l’objet parent<br>Nom de l’utilisateur ayant commenté le thread<br>Texte du commentaire effectué sur le thread<br>Date et heure auxquelles le commentaire a été fait<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*Nom du projet<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong>} bouton 10}* Date de digitale est<br> </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un commente l'une de mes tâches</strong> </p> <p>La personne cessionnaire de l’élément de travail reçoit une notification par e-mail chaque fois qu’une personne ajoute une mise à jour à un élément de travail, sauf si la personne qui ajoute la mise à jour est également la personne cessionnaire. </p> <p>Lorsqu’un commentaire est publié sur une demande, envoyez un e-mail au contact principal du problème.</p> <p>Le contact principal d’un problème reçoit une notification par e-mail lorsqu’un commentaire est publié sur une demande, sauf si l’utilisateur ou l’utilisatrice qui a publié le commentaire est également le contact principal du problème.</p> <p>Tous les utilisateurs et toutes les utilisatrices qui sont directement inclus dans le commentaire reçoivent également une notification par e-mail.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Commentaire sur] &lt;Nom de l’élément de travail&gt; sur &lt;Nom du projet (réf. &lt;Numéro de référence de l’élément de travail&gt;)</em></p> <p> Le sujet de la notification quotidiennement de résumé est :<em> [!UICONTROL Digest of Communication] &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> Nom de l’élément de travail<br>Nom du projet<br>Numéro de référence de l’élément de travail<br>Nom de l’utilisateur qui a commenté l’élément de travail<br>Texte du commentaire effectué sur l’élément de travail<br>Date et heure de création du commentaire<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*Nom du projet<br>*<strong>}[!UICONTROL Voir toutes les notifications]</strong>}}}} button<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un inclut mon équipe à une mise à jour dirigée</strong> </p> <p>Une mise à jour dirigée réside dans le fait qu’une personne inclut spécifiquement un autre utilisateur ou une autre utilisatrice dans une mise à jour, comme décrit dans <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Taguer d’autres personnes sur les mises à jour</a>.</p> <p>Dans ce cas, tout membre de l’équipe inclus dans la mise à jour ciblée reçoit une notification par courrier électronique à propos de la mise à jour.</p> <p>La notification électronique est envoyée uniquement aux utilisateurs disposant de droits d’accès à l’objet .</p> <p>Si la personne qui envoie la mise à jour dirigée est un membre de l’équipe en cours d’inclusion, la personne qui envoie la mise à jour ne reçoit pas de notification par e-mail.</p> <p>L’objet de l’email de notification instantanée est : [!UICONTROL Commentaire sur] &lt;Nom de l’objet&gt; sur &lt;Nom de l’objet parent&gt; (réf. &lt;Numéro de référence de l’objet&gt;)</p> <p> Le sujet de la notification quotidiennement de résumé est :<em> [!UICONTROL Digest of Communication] &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> <p>Nom de l’objet <br>Nom de l’objet parent<br>Numéro de référence de l’objet<br>Nom de l’utilisateur qui a effectué la mise à jour dirigée<br>Nom de toutes les équipes et tous les utilisateurs inclus dans la mise à jour dirigée<br>Date et heure de la mise à jour dirigée<br>Texte de la mise à jour dirigée<br><strong>[!UICONTROL Comment]</strong>}*Nombre total de commentaires reçus<br>}}*Nombre total<br>}}}}*Nombre total de commentaires reçus<br>}}}}}}}*9}*Nombre total de commentaires reçus}}}} 0}*Nom du projet<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong> bouton<br>*Date du résumé quotidien </p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque un commentaire est ajouté sur l’utilisateur</strong> </p> <p>Vous pouvez faire un commentaire sur un utilisateur dans l’onglet [!UICONTROL Mises à jour] de l’objet utilisateur. Vous pouvez également ajouter un commentaire à un utilisateur lorsque vous modifiez les paramètres de ce dernier. L’utilisateur contre lequel le commentaire est fait reçoit un e-mail l’informant de ce commentaire. </p> <p>Vous devez disposer d’autorisations pour au moins [!UICONTROL Afficher] l’utilisateur afin de saisir une mise à jour dans l’onglet [!UICONTROL Mises à jour] de l’utilisateur. Pour pouvoir modifier les paramètres de l’utilisateur, vous devez disposer des autorisations [!UICONTROL Modifier] sur l’utilisateur. </p> <p>Pour plus d’informations sur l’ajout de commentaires aux utilisateurs dans l’onglet Mises à jour, voir <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mise à jour du travail</a>.</p> <p>Pour plus d’informations sur la saisie d’un commentaire sur un utilisateur lorsque vous modifiez les paramètres de l’utilisateur, voir <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configuration de mes paramètres</a>.</p> <p>Le sujet de l'email de notification instantanée est : <em>&lt;Nom d'utilisateur&gt; [!UICONTROL voulait que vous sachiez]</em></p> <p>Le sujet de la notification quotidiennement de résumé est :<em> [!UICONTROL Digest of Communication] &lt;Date du résumé quotidien&gt;</em></p> </td> 
   <td> Votre nom d’utilisateur<br>Nom de l’utilisateur ayant ajouté le commentaire<br>Texte du commentaire<br>Date et heure auxquelles le commentaire a été fait<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong> bouton<br>*Date de résumé quotidien </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>et Daily</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
