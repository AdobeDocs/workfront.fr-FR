---
content-type: reference
navigation-topic: notifications
title: 'Notifications : Communication'''
description: Les notifications suivantes vous alertent sur la communication, par exemple un commentaire de mise à jour, qui se produit sur un élément de travail auquel vous êtes impliqué. Pour plus d’informations sur la configuration des notifications que vous recevez, voir Activation ou désactivation de vos propres notifications d’événement.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: 2af2a1f7d1a4d0b06cf4e7bfd2b9997ff8b9a6bf
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 4%

---

# Notifications : Communication

Les notifications suivantes vous alertent sur la communication, par exemple un commentaire de mise à jour, qui se produit sur un élément de travail auquel vous êtes impliqué. Pour plus d’informations sur la configuration des notifications que vous recevez, voir [Activation ou désactivation de vos propres notifications d’événement](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Quelqu'un m'a inclus dans une mise à jour dirigée.</strong> </p> <p>Une mise à jour ciblée est effectuée lorsqu’un utilisateur inclut spécifiquement un autre utilisateur dans une mise à jour, comme décrit dans la section <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Balisage des autres sur] mises à jour</a>.</p> <p>Dans ce cas, l’utilisateur inclus dans la mise à jour redirigée reçoit une notification par courrier électronique concernant la mise à jour.</p> <p>La notification électronique n’est envoyée que si l’utilisateur dispose des droits d’accès à l’objet .</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>&lt;name of="" the="" user="" who="" included="" you="" in="" the="" update=""&gt; [!UICONTROL voulait que vous sachiez]</em></p> <p>L’objet de la notification quotidiennement Digest est : <em>[!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom de l’objet où la mise à jour a été effectuée<br>Nom de l’objet parent<br>Numéro de référence de l’objet<br>Noms de tous les utilisateurs et équipes inclus dans la mise à jour dirigée<br>Date et heure de la mise à jour<br>Texte de la mise à jour ciblée<br><strong>[!UICONTROL Comment]</strong> button<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong> button<br>*Date du résumé quotidien<br></td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un répond à ma demande</strong> </p> <p>Une fois qu’un utilisateur a envoyé une demande de travail et qu’un autre utilisateur a répondu à cette demande, l’utilisateur qui l’a envoyée reçoit une notification par courrier électronique.</p> <p>Une notification électronique n’est pas envoyée si :</p> 
    <ul> 
     <li> <p>L’utilisateur qui envoie la réponse est le même utilisateur qui a effectué la demande.</p> </li> 
     <li> <p>L’utilisateur n’a pas accès à l’affichage de la note.</p> </li> 
    </ul><strong>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Commentaire sur] &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></strong> L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></td> 
   <td> Nom de la requête<br>Nom du projet<br>Numéro de référence<br>Nom de l’utilisateur qui a répondu à votre demande<br>Date et heure auxquelles le commentaire a été fait<br>Texte du commentaire sur votre requête<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque demande<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong> button<br>*Date du résumé quotidien<br></td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un commentaire a été publié au sujet de ma demande</strong> </p> <p>Le Principal contact pour un problème reçoit une notification par courrier électronique lorsqu’un commentaire est publié sur une demande du [!UICONTROL Help Desk], sauf si l’utilisateur qui a publié le commentaire est également le Principal contact pour le problème.</p> <p>Tous les utilisateurs qui sont directement inclus dans le commentaire reçoivent également une notification par courrier électronique.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel].</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Commentaire sur] &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom de la requête<br>Nom du projet<br>Numéro de référence<br>Nom de l’utilisateur qui a répondu à votre demande<br>Date et heure auxquelles le commentaire a été fait<br>Texte du commentaire sur votre requête<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque demande<br>*Nom du projet<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong> button<br>*Date du résumé quotidien<br></td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Un commentaire a été ajouté sur mon document</strong> </p> <p>Le propriétaire d’un document dans [!DNL Adobe Workfront] reçoit une notification par courrier électronique lorsqu’un commentaire est publié sur le document, sauf si l’utilisateur qui a publié le commentaire est également le propriétaire du document.</p> <p>Tous les utilisateurs qui sont directement inclus dans le commentaire reçoivent également une notification par courrier électronique.</p> <p>Une notification est envoyée uniquement si l’état du projet est [!UICONTROL Actuel]. </p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Commentaire sur] &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td>Document Name<br>Nom du projet, de la tâche ou du problème<br>Numéro de référence<br>Nom de l’utilisateur qui a répondu à votre demande<br>Date et heure auxquelles le commentaire a été fait<br>Texte de commentaire sur le document</td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque quelqu'un fait un commentaire sur un élément de travail, envoyer un e-mail à tous ceux qui ont également fait un commentaire sur cet élément de travail</strong> </p> <p>Les participants au thread et les utilisateurs inclus dans un message direct reçoivent une notification par email lorsqu’un utilisateur fait un commentaire dans le thread.</p> <p>Les utilisateurs doivent disposer d’un accès [!UICONTROL View] pour recevoir une notification.</p> <p>Les utilisateurs suivants ne reçoivent pas de notification :</p> 
    <ul> 
     <li>Équipes incluses dans un message direct</li> 
     <li>Propriétaire de la note</li> 
     <li>Contact Principal</li> 
    </ul> <p><strong>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL RE : Commentaire sur] &lt;object name=""&gt;&lt;object type=""&gt; on &lt;project name=""&gt;(ref# &lt;object reference="" number=""&gt;</em>)</strong> </p> <p><strong> L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></strong> </p> </td> 
   <td> Nom de l’objet<br>Nom de l’objet parent<br>Nom de l’utilisateur qui a commenté le fil<br>Texte de commentaire sur le fil<br>Date et heure auxquelles le commentaire a été fait<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*Nom du projet<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong> button<br>*Date du résumé quotidien </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsque quelqu'un fait un commentaire sur un élément de travail, envoyer un e-mail au cessionnaire</strong> </p> <p>La personne désignée de l’élément de travail reçoit une notification par courrier électronique chaque fois qu’un utilisateur ajoute une mise à jour à un élément de travail, sauf si l’utilisateur qui ajoute la mise à jour est également la personne désignée. </p> <p>Lorsqu’un commentaire est publié sur une demande, envoyez un email Principal au problème.</p> <p>Le Principal contact pour un problème reçoit une notification par courrier électronique lorsqu’un commentaire est publié sur une demande, sauf si l’utilisateur qui a publié le commentaire est également le Principal contact pour le problème.</p> <p>Tous les utilisateurs qui sont directement inclus dans le commentaire reçoivent également une notification par courrier électronique.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>[!UICONTROL Commentaire sur] &lt;work item="" name=""&gt; on &lt;project name="" ref="" work="" item="" reference="" number=""&gt;)</em></p> <p> L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Nom de l’élément de travail<br>Nom du projet<br>Numéro de référence de l’élément de travail<br>Nom de l’utilisateur qui a commenté l’élément de travail<br>Texte du commentaire sur l’élément de travail<br>Date et heure auxquelles le commentaire a été fait<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*Nom du projet<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong> button<br>*Date du résumé quotidien </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Quelqu'un inclut mon équipe dans une mise à jour dirigée</strong> </p> <p>Une mise à jour ciblée est effectuée lorsqu’un utilisateur inclut spécifiquement un autre utilisateur dans une mise à jour, comme décrit dans la section <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Balisage des autres sur les mises à jour</a>.</p> <p>Dans ce cas, tout membre de l’équipe inclus dans la mise à jour ciblée reçoit une notification par courrier électronique à propos de la mise à jour.</p> <p>La notification électronique est envoyée uniquement aux utilisateurs disposant de droits d’accès à l’objet .</p> <p>Si l’utilisateur qui envoie la mise à jour redirigée est membre de l’équipe en cours d’inclusion, l’utilisateur qui envoie la mise à jour ne reçoit pas de notification par courrier électronique.</p> <p>L'objet de l'email de notification instantanée est le suivant : [!UICONTROL Commentaire sur] &lt;object name=""&gt; on &lt;parent object="" name=""&gt; (ref# &lt;object reference="" number=""&gt;)</p> <p> L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Nom de l’objet<br>Nom de l’objet parent<br>Numéro de référence de l’objet<br>Nom de l’utilisateur qui a effectué la mise à jour dirigée<br>Nom de toutes les équipes et tous les utilisateurs inclus dans la mise à jour dirigée<br>Date et heure auxquelles la mise à jour ciblée a été effectuée<br>Texte de la mise à jour dirigée<br><strong>[!UICONTROL Comment]</strong> button<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*Nom du projet<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong> button<br>*Date du résumé quotidien </p> </td> 
   <td><strong>Chaque jour</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lorsqu'un commentaire est ajouté à propos d'un utilisateur</strong> </p> <p>Vous pouvez faire un commentaire sur un utilisateur dans l’onglet [!UICONTROL Mises à jour] de l’objet utilisateur. Vous pouvez également ajouter un commentaire à un utilisateur lorsque vous modifiez les paramètres de ce dernier. L’utilisateur contre lequel le commentaire est fait reçoit un e-mail l’informant de ce commentaire. </p> <p>Vous devez disposer d’autorisations pour au moins [!UICONTROL Afficher] l’utilisateur afin de saisir une mise à jour dans l’onglet [!UICONTROL Mises à jour] de l’utilisateur. Pour pouvoir modifier les paramètres de l’utilisateur, vous devez disposer des autorisations [!UICONTROL Modifier] sur l’utilisateur. </p> <p>Pour plus d’informations sur l’ajout de commentaires aux utilisateurs dans l’onglet Mises à jour, voir <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mise à jour du travail</a>.</p> <p>Pour plus d’informations sur la saisie d’un commentaire sur un utilisateur lors de la modification des paramètres de l’utilisateur, voir <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configurer mes paramètres</a>.</p> <p>L'objet de l'email de notification instantanée est le suivant : <em>&lt;user name=""&gt; [!UICONTROL voulait que vous sachiez]</em></p> <p>L’objet de la notification quotidiennement Digest est :<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Votre nom d’utilisateur<br>Nom de l’utilisateur qui a ajouté le commentaire<br>Texte du commentaire<br>Date et heure auxquelles le commentaire a été fait<br>*Nombre total de commentaires reçus<br>*Nombre de commentaires reçus pour chaque objet<br>*<strong>[!UICONTROL Voir toutes les notifications]</strong> button<br>*Date du résumé quotidien </td> 
   <td> <p><strong>Instantané</strong> </p> <p><strong>et Quotidien</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
