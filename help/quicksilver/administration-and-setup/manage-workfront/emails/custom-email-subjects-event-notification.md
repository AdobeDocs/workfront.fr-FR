---
navigation-topic: notifications
title: Personnalisation des sujets des emails pour les notifications d’événement
description: Vous pouvez personnaliser l’objet des emails déclenchés par les notifications d’événement.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 4%

---

# Personnalisation des sujets des emails pour les notifications d’événement

Vous pouvez personnaliser l’objet des emails déclenchés par les notifications d’événement :

La modification des lignes d&#39;objet affecte tous les utilisateurs du système, quel que soit le niveau d&#39;accès du destinataire. Les utilisateurs voient tous les objets et champs inclus dans l’objet du courrier électronique.

Certaines notifications d’événement ont plusieurs objets, ce qui signifie que ces notifications d’événement peuvent comporter plusieurs sujets d’email en fonction de leurs fonctionnalités.

>[!IMPORTANT]
>
>Soyez prudent lorsque vous supprimez des champs par défaut lorsque les lignes d’objet font référence à plusieurs objets. Vous trouverez ci-dessous la liste des notifications d’événement contenant ces objets :
>
>* Quelqu&#39;un m&#39;a inclus dans une mise à jour dirigée.
>* Quelqu&#39;un inclut mon équipe dans une mise à jour dirigée
>* Commentaire d&#39;élément de travail pour les participants du thread
>* Commentaire d&#39;élément de travail pour le cessionnaire de l&#39;élément de travail
>

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>Quelconque</td> 
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

## Personnalisation de l’objet des emails pour les notifications d’événement {#customize-email-subject-lines-for-event-notifications}

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Email** > **Notifications**.

1. Cliquez sur le bouton **Notifications d’événement** .
1. Cliquez sur le nom de la notification d’événement à personnaliser pour ouvrir la **Notification d’événement** de la boîte.
1. Dans le **Objet du courrier électronique** , modifiez le texte et les champs, y compris les champs personnalisés, dans l’objet de l’email.

   Les noms des champs ajoutés doivent correspondre à la syntaxe de la casse des chameaux de notre structure de base de données. <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. Cliquez sur **Mettre à jour** pour enregistrer les nouveaux objets de vos emails.

## Personnalisation de l’objet des emails contenant plusieurs objets

Certaines notifications d’événement comportent plusieurs lignes d’objet, selon les objets qu’elles déclenchent.

Par exemple, &quot;Quelqu’un m’inclut sur une mise à jour dirigée&quot; comporte deux lignes de sujets différents : d’abord pour les tâches, les problèmes, les tâches de modèle et les documents (également appelé &quot;referenceObject&quot;), et ensuite pour les objets qui permettent aux utilisateurs de faire des commentaires, comme un portfolio, un programme, etc. (également appelé &quot;topReferenceObject&quot;).

![](assets/Ev-not-mult-subj-lines.png)

Si un utilisateur est inclus dans une conversation sur la tâche, le problème, la tâche de modèle ou le document, un courrier électronique est généré avec le premier objet. La ligne d’objet contient &quot;referenceObject:name&quot; et le système définit l’objet et affiche le nom approprié dans le champ d’objet. L’objet du courrier électronique ressemblerait à ceci : &quot;Commentaire sur la tâche 123 sur le projet ABC&quot;.

S’il est ajouté à une conversation de projet, un courrier électronique contenant le deuxième objet est généré. Ici, la ligne d’objet contient &quot;topReferenceObject:name&quot; et de nouveau Workfront identifie l’objet référencé et renvoie ce nom d’objet au lieu de &quot;topReferenceObject:name&quot; dans l’objet. L’objet de l’email ressemble à ceci : &quot;Commentaire sur le projet ABC&quot;.

Pour modifier l’objet du courrier électronique et ajouter des champs supplémentaires à l’une des lignes d’objet, reportez-vous à la section [Personnalisation de l’objet des emails pour les notifications d’événement](#customize-email-subject-lines-for-event-notifications) dans cet article.

## Personnalisation de l’objet des emails à actions multiples

Certaines notifications d’événement comportent également plusieurs sujets de courrier électronique pour décrire les différentes actions effectuées sur les objets.

Par exemple, la demande d’ajout d’un document à un problème peut déclencher deux emails différents : un pour lorsque le document est ajouté et un autre pour lorsque le document est modifié.

![](assets/ev-not-mult-subj-lines-diff-actions.png)

Pour modifier l’objet du courrier électronique et ajouter des champs supplémentaires à l’une des lignes d’objet, reportez-vous à la section [Personnalisation de l’objet des emails pour les notifications d’événement](#customize-email-subject-lines-for-event-notifications) dans cet article.
