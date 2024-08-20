---
navigation-topic: notifications
title: Personnalisation des objets de courrier électronique pour les notifications d’événement
description: Vous pouvez personnaliser la ligne d’objet des e-mails déclenchés par les notifications d’événement.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 97%

---

# Personnaliser les objets des e-mails pour les notifications d’événement

Vous pouvez personnaliser la ligne d’objet des e-mails déclenchés par les notifications d’événement :

La modification des lignes d’objet affecte tous les utilisateurs et utilisatrices du système, quel que soit le niveau d’accès de la personne destinataire. Les utilisateurs et utilisatrices voient tous les objets et champs inclus dans l’objet de l’e-mail.

Certaines notifications d’événement ont plusieurs lignes d’objet, ce qui signifie que ces notifications d’événement peuvent comporter plusieurs objets d’e-mail en fonction de leurs fonctionnalités.

>[!IMPORTANT]
>
>Faites preuve de prudence lorsque vous supprimez des champs par défaut si les lignes d’objet font référence à plusieurs objets. Vous trouverez ci-dessous la liste des notifications d’événement contenant ces lignes d’objet :
>
>* Quelqu&#39;un m&#39;a inclus dans une mise à jour dirigée.
>* Quelqu&#39;un inclut mon équipe dans une mise à jour dirigée
>* Commentaire d&#39;élément de travail pour les participants du thread
>* Commentaire d&#39;élément de travail pour le cessionnaire de l&#39;élément de travail
>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Planificateur ou version ultérieure, avec accès administratif aux notifications de rappel</p> <p>Pour plus d’informations sur l’octroi d’un accès administratif à un utilisateur ou une utilisatrice de plan, voir la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroyer un accès administratif à certaines zones</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Personnaliser les lignes d’objet des e-mails pour les notifications d’événement {#customize-email-subject-lines-for-event-notifications}

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **E-mail** > **Notifications**.

1. Cliquez sur l’onglet **Notifications d’événement**.
1. Cliquez sur le nom de la notification d’événement à personnaliser pour ouvrir la zone **Notification d’événement**.
1. Dans le **Objet du courrier électronique** , modifiez le texte et les champs, y compris les champs personnalisés, dans l’objet de l’email.

   Les noms des champs ajoutés doivent correspondre à la syntaxe « camel case » de notre structure de base de données. <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. Cliquez sur **Mettre à jour** pour enregistrer les nouvelles lignes d’objet de vos e-mails.

## Personnaliser les lignes d’objet des e-mails contenant plusieurs objets

Certaines notifications d’événement comportent plusieurs lignes d’objet, selon les objets qu’elles déclenchent.

Par exemple, « Quelqu’un m’a inclus dans une mise à jour dirigée » comporte deux lignes d’objet différentes : d’abord pour les tâches, les problèmes, les tâches de modèle et les documents (également appelée « referenceObject »), puis pour les objets qui permettent aux utilisateurs et utilisatrices de faire des commentaires, comme un portfolio, un programme, etc. (également appelée « topReferenceObject »).

![](assets/Ev-not-mult-subj-lines.png)

Si une personne est incluse dans une conversation sur la tâche, le problème, la tâche de modèle ou le document, un e-mail est généré avec la première ligne d’objet. La ligne d’objet contient « referenceObject:name » et le système définit l’objet et affiche le nom approprié dans le champ d’objet. La ligne d’objet de l’e-mail ressemblerait à ceci : « Commentaire sur la tâche 123 sur le projet ABC ».

Si elle est ajoutée à une conversation de projet, un e-mail contenant le second objet est généré. Ici, la ligne d’objet contient « topReferenceObject:name » et de nouveau Workfront identifie l’objet référencé et renvoie ce nom d’objet au lieu de « topReferenceObject:name » dans l’objet. La ligne d’objet de l’e-mail ressemble à ceci : « Commentaire sur le projet ABC ».

Pour modifier les lignes d’objet de l’e-mail et ajouter des champs supplémentaires à l’une des lignes d’objet, voir la section [Personnaliser les lignes d’objet des e-mails pour les notifications d’événement](#customize-email-subject-lines-for-event-notifications) dans cet article.

## Personnaliser les lignes d’objet des e-mails à actions multiples

Certaines notifications d’événement comportent également plusieurs objets d’e-mail pour décrire les différentes actions effectuées sur les objets.

Par exemple, la demande d’ajout d’un document à un problème peut déclencher deux e-mails différents : un pour le moment où le document est ajouté et un autre pour le moment où le document est modifié.

![](assets/ev-not-mult-subj-lines-diff-actions.png)

Pour modifier les lignes d’objet de l’e-mail et ajouter des champs supplémentaires à l’une des lignes d’objet, voir la section [Personnaliser les lignes d’objet des e-mails pour les notifications d’événement](#customize-email-subject-lines-for-event-notifications) dans cet article.
