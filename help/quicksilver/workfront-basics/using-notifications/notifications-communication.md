---
content-type: reference
navigation-topic: notifications
title: 'Notifications : communication'
description: Les notifications suivantes vous avertissent des communications, telles qu’un commentaire de mise à jour, qui ont lieu sur un élément de travail auquel vous participez. Pour plus d’informations sur la configuration des notifications que vous recevez, voir Modifier vos propres notifications par e-mail.
author: Courtney
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 100%

---

# Notifications : communication

Les notifications suivantes vous avertissent des communications, telles qu’un commentaire de mise à jour, qui ont lieu sur un élément de travail auquel vous participez. Pour plus d’informations sur la configuration des notifications que vous recevez, consultez la section [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Ces notifications vous informent de tous les commentaires qui ont été publiés sur un article spécifique. C’est pourquoi vous devez sélectionner ou désélectionner toutes les notifications en même temps pour qu’elles vous soient envoyées dans un e-mail de synthèse quotidienne. Si vous souhaitez être informé de certains commentaires au fur et à mesure qu’ils se produisent, vous pouvez spécifier que les notifications individuelles doivent être envoyées instantanément.

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
   <td> <p><strong>Quelqu'un m'a inclus dans une mise à jour dirigée.</strong> </p> <p>On parle de mise à jour dirigée lorsqu’un utilisateur ou une utilisatrice inclut spécifiquement une autre personne dans une mise à jour, comme décrit dans <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Tag others on] mises à jour</a>.</p> <p>Dans ce cas, l’utilisateur ou utilisatrice qui est inclus dans la mise à jour dirigée reçoit une notification par e-mail concernant la mise à jour.</p> <p>La notification par e-mail n’est envoyée que si la personne dispose de droits d’accès à l’objet.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>&lt;Name of the user who included you in the update&gt; [!UICONTROL wanted you to know].</em></p> <p>L’objet de la notification du résumé quotidien est : <em>[!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;.</em></p> </td> 
   <td> Nom de l’objet où la mise à jour a été effectuée<br>Nom de l’objet parent<br>Numéro de référence de l’objet<br>Noms de tous les utilisateurs, utilisatrices et équipes inclus dans la mise à jour dirigée<br>Date et heure de la mise à jour<br>Texte de la mise à jour dirigée<br><strong>Bouton [!UICONTROL Comment]</strong><br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*<strong>Bouton [!UICONTROL See All Notifications]</strong><br>*Date de la synthèse quotidienne<br></td> 
   <td> <p><strong>Instantanée</strong> </p> <p><strong>et quotidienne</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu’un répond à ma demande</strong> </p> <p>Lorsqu’une personne soumet une demande de travail et qu’une autre personne y répond, l’utilisateur ou utilisatrice qui a soumis la demande reçoit une notification par e-mail.</p> <p>Une notification par e-mail n’est pas envoyée si :</p> 
    <ul> 
     <li> <p>L’utilisateur ou utilisatrice qui répond est celui qui a fait la demande.</p> </li> 
     <li> <p>L’utilisateur ou utilisatrice n’a pas accès à la note</p> </li> 
    </ul><strong>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Comment on] &lt;Request Name&gt; sur &lt;Project Name&gt; (réf n° &lt;Request Reference Number&gt;)</em></strong> L’objet de la notification quotidienne est :<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;.</em></td> 
   <td> Nom de la demande<br>Nom du projet<br>Numéro de référence<br>Nom de l’utilisateur ou utilisatrice qui a répondu à votre demande<br>Date et heure du commentaire<br>Texte du commentaire sur votre demande<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque demande<br>*<strong>Bouton [!UICONTROL See All Notifications]</strong><br>*Date de la synthèse quotidienne<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un commentaire a été publié au sujet de ma demande</strong> </p> <p>La personne ayant créé un problème reçoit une notification par e-mail lorsqu’un commentaire est posté sur une demande [!UICONTROL Help Desk], sauf si l’utilisateur ou utilisatrice qui a posté le commentaire est également la personne ayant créé le problème.</p> <p>Tous les utilisateurs et utilisatrices directement concernés par le commentaire reçoivent également une notification par e-mail.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current].</p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Comment on] &lt;Request Name&gt; sur &lt;Project Name&gt; (réf n°  &lt;Request Reference Number&gt;)</em></p> <p>L’objet de la notification de la synthèse quotidienne est le suivant :<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;.</em></p> </td> 
   <td> Nom de la demande<br>Nom du projet<br>Numéro de référence<br>Nom de l’utilisateur ou utilisatrice qui a répondu à votre demande<br>Date et heure du commentaire<br>Texte du commentaire sur votre demande<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque demande<br>*Nom du projet<br>*<strong>Bouton [!UICONTROL See All Notifications]</strong><br>*Date de la synthèse quotidienne<br></td> 
   <td> <p><strong>Instantanée</strong> </p> <p><strong>et quotidienne</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un commentaire a été ajouté sur mon document</strong> </p> <p>La personne propriétaire d’un document dans [!DNL Adobe Workfront] reçoit une notification par e-mail lorsqu’un commentaire est publié sur le document, sauf si l’utilisateur ou utilisatrice qui a publié le commentaire est également la personne propriétaire du document.</p> <p>Tous les utilisateurs et utilisatrices directement concernés par le commentaire reçoivent également une notification par e-mail.</p> <p>Une notification est envoyée uniquement si le statut du projet est [!UICONTROL Current]. </p> <p>L’objet de l’e-mail de notification instantanée est le suivant : <em>[!UICONTROL Comment on] &lt;Request Name&gt; sur &lt;Project Name&gt; (n° réf. &lt;Request Reference Number&gt;)</em></p> <p> L’objet de la notification de la synthèse quotidienne est le suivant :<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;.</em></p> </td> 
   <td>Nom du document<br>Nom du projet, de la tâche ou du problème<br>Numéro de référence<br>Nom de l’utilisateur ou utilisatrice qui a répondu à votre demande<br>Date et heure auxquelles le commentaire a été fait<br>Texte du commentaire fait sur le document</td> 
   <td> <p><strong>Instantanée</strong> </p> <p><strong>et quotidienne</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu’un fait un commentaire sur un thread sur lequel je travaille</strong> </p> <p>Les personnes participant au thread et les utilisateurs et utilisatrices inclus dans un message direct reçoivent une notification par e-mail lorsque quelqu’un fait un commentaire dans le thread.</p> <p>Les utilisateurs et utilisatrices doivent avoir accès à [!UICONTROL View] pour recevoir une notification.</p> <p>Les utilisateurs et utilisatrices suivants ne reçoivent pas de notification :</p> 
    <ul> 
     <li>Les équipes incluses dans un message direct</li> 
     <li>La personne propriétaire de la note</li> 
     <li>Le contact principal</li> 
    </ul> <p><strong>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL RE: Comment on] &lt;Object Name&gt;&lt;Object Type&gt; on &lt;Project Name&gt;(ref# &lt;Object Reference Number&gt;</em>)</strong>. </p> <p><strong> L’objet de la notification de synthèse quotidienne est : <em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></strong>. </p> </td> 
   <td> Nom de l’objet<br>Nom de l’objet parent<br>Nom de l’utilisateur ou de l’utilisatrice qui a commenté le thread<br>Texte du commentaire sur le thread<br>Date et heure du commentaire<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*Nom du projet<br>*Bouton <strong>[!UICONTROL See All Notifications]</strong><br>*Date de la synthèse quotidienne </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu’un fait un commentaire sur l’un de mes éléments de travail</strong> </p> <p>La personne assignée de l’élément de travail reçoit une notification par e-mail chaque fois qu’une personne ajoute une mise à jour à un élément de travail, sauf si la personne qui ajoute la mise à jour est également la personne assignée. </p> <p>Lorsqu’un commentaire est publié sur une requête, envoyez un e-mail au contact principal du problème.</p> <p>Le contact principal d’un problème reçoit une notification par e-mail lorsqu’un commentaire est publié sur une requête, sauf si la personne qui a publié le commentaire est également le contact principal du problème.</p> <p>Tous les utilisateurs et utilisatrices directement concernés par le commentaire reçoivent également une notification par e-mail.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>[!UICONTROL Comment on] &lt;Work Item Name&gt; sur &lt;Project Name (ref# &lt;Work Item Reference Number&gt;)</em>.</p> <p> L’objet de la notification de synthèse quotidienne est :<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em>.</p> </td> 
   <td> Nom de l’élément de travail<br>Nom du projet<br>Numéro de référence de l’élément de travail<br>Nom de l’utilisateur ou de l’utilisatrice qui a commenté l’élément de travail<br>Texte du commentaire sur l’élément de travail<br>Date et heure du commentaire<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*Nom du projet<br>*Bouton <strong>[!UICONTROL See All Notifications]</strong><br>*Date de la synthèse quotidienne </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu’un inclut mon équipe dans une mise à jour dirigée</strong> </p> <p>On parle de mise à jour dirigée lorsqu’un utilisateur ou une utilisatrice inclut spécifiquement une autre personne dans une mise à jour, tel que décrit dans <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Taguer d’autres personnes sur les mises à jour</a>.</p> <p>Dans ce cas, tous les membres de l’équipe concernés par la mise à jour reçoivent une notification par e-mail à ce sujet.</p> <p>La notification par e-mail n’est envoyée qu’aux personnes qui ont des droits d’accès à l’objet.</p> <p>Si la personne qui envoie la mise à jour dirigée est membre de l’équipe incluse, la personne qui envoie la mise à jour ne reçoit pas de notification par e-mail.</p> <p>L’objet de l’e-mail de notification instantanée est : [!UICONTROL Comment on] &lt;Object name&gt; sur &lt;Parent Object Name&gt; (ref# &lt;Object Reference Number&gt;).</p> <p> L’objet de la notification de synthèse quotidienne est :<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em>.</p> </td> 
   <td> <p>Nom de l’objet<br>Nom de l’objet parent<br>Numéro de référence de l’objet<br>Nom de l’utilisateur ou de l’utilisatrice qui a effectué la mise à jour dirigée<br>Nom de toutes les équipes et de tous les utilisateurs et utilisatrices inclus dans la mise à jour dirigée<br>Date et heure de la mise à jour dirigée<br>Texte de la mise à jour dirigée<br><strong>Bouton [!UICONTROL Comment]</strong><br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*Nom du projet<br>*Bouton <strong>[!UICONTROL See All Notifications]</strong><br>*Date de la synthèse quotidienne </p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu’un commentaire est ajouté à propos d’un utilisateur ou d’une utilisatrice</strong> </p> <p>Vous pouvez faire un commentaire sur un utilisateur ou une utilisatrice dans l’onglet [!UICONTROL Updates] de l’objet utilisateur. Vous pouvez également faire un commentaire sur un utilisateur ou une utilisatrice lorsque vous modifiez ses paramètres. L’utilisateur ou l’utilisatrice qui a fait l’objet du commentaire reçoit un e-mail l’informant de ce commentaire. </p> <p>Vous devez avoir au moins l’autorisation [!UICONTROL View] l’utilisateur ou l’utilisatrice pour pouvoir saisir une mise à jour dans l’onglet [!UICONTROL Updates] de l’utilisateur ou de l’utilisatrice. Vous devez disposer des autorisations [!UICONTROL Edit] sur l’utilisateur ou l’utilisatrice pour pouvoir modifier les paramètres de l’utilisateur ou de l’utilisatrice. </p> <p>Pour plus d’informations sur la formulation de commentaires sur les utilisateurs et utilisatrices dans l’onglet Mises à jour, voir <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mettre à jour le travail</a>.</p> <p>Pour plus d’informations sur la saisie d’un commentaire sur un utilisateur ou une utilisatrice lorsque vous modifiez les paramètres de l’utilisateur ou de l’utilisatrice, voir <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurer Mes paramètres</a>.</p> <p>L’objet de l’e-mail de notification instantanée est : <em>&lt;User Name&gt; [!UICONTROL wanted you to know]</em>.</p> <p>L’objet de la notification de synthèse quotidienne est :<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em>.</p> </td> 
   <td> Votre nom d’utilisateur ou d’utilisatrice<br>Nom de l’utilisateur ou de l’utilisatrice qui a ajouté le commentaire<br>Texte du commentaire<br>Date et heure du commentaire<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*Bouton <strong>[!UICONTROL See All Notifications]</strong><br>*Date de la synthèse quotidienne </td> 
   <td> <p><strong>Instantanée</strong> </p> <p><strong>et quotidienne</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
