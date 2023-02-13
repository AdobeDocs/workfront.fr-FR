---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Mettre à jour les éléments liés entre [!DNL Jira] et [!DNL Adobe Workfront]
description: Lorsque vous liez [!DNL Jira] problèmes à [!DNL Adobe Workfront] tâches ou problèmes, vos utilisateurs peuvent mettre à jour des éléments dans une application et la contrepartie de cet élément est également mise à jour pour les utilisateurs travaillant dans la deuxième application.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: f533c9000c14d5692c87987973eb0b1d6665229d
workflow-type: tm+mt
source-wordcount: '1723'
ht-degree: 0%

---

# Mettre à jour les éléments liés entre [!DNL Jira] et [!DNL Adobe Workfront]

Lorsque vous liez [!DNL Jira] problèmes à [!DNL Adobe Workfront] tâches ou problèmes, vos utilisateurs peuvent mettre à jour des éléments dans une application et la contrepartie de cet élément est également mise à jour pour les utilisateurs travaillant dans la deuxième application.

Pour plus d’informations sur la liaison d’éléments entre [!DNL Workfront] et [!DNL Jira], voir [Lier des éléments entre Adobe Workfront et Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

En cours de configuration [!DNL Workfront] pour [!DNL Jira], as a [!DNL Jira] administrateur système, vous pouvez configurer certains champs d’une application pour les synchroniser avec les champs des éléments liés de l’autre application.

Pour plus d’informations sur la synchronisation de champs entre les champs liés [!DNL Jira] et [!DNL Workfront] éléments, voir [Configurer [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] Présentation des licences</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] accès</td> 
   <td> <p>Accès administrateur système</p> <p>Important : Nous vous recommandons de créer des comptes d’administrateur système distincts dans [!DNL Jira] et [!DNL Workfront] pour dédier à cette intégration, plutôt que d’utiliser des qui peuvent être associés à des utilisateurs existants.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Avant de pouvoir lier des éléments entre [!DNL Workfront] et [!DNL Jira], vous devez

* Installer [!DNL Workfront for Jira].

   Pour obtenir des instructions sur l’installation [!DNL Workfront for Jira], voir [Installer [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurer [!DNL Workfront for Jira].

   Pour obtenir des instructions sur la configuration [!DNL Workfront for Jira], voir [Configurer [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Lier des éléments entre [!DNL Workfront] et [!DNL Jira].

   Pour obtenir des instructions, voir [Lier des éléments entre [!DNL Adobe Workfront] et [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Mise à jour des éléments liés dans [!DNL Workfront]

Si vous travaillez principalement dans [!DNL Workfront], vous pouvez mettre à jour vos tâches dans [!DNL Workfront] et leurs homologues dans les [!DNL Jira] également mettre à jour. Cette mise à jour se fait par l’intégration de [!DNL Workfront] pour [!DNL Jira] qui ne nécessite pas que vous ayez une [!DNL Jira] licence.

Tant que votre [!DNL Workfront] l’administrateur a configuré [!DNL Workfront for Jira] pour synchroniser les champs entre les éléments liés, certains champs que vous mettez à jour dans [!DNL Workfront] également mettre à jour pour le lien [!DNL Jira] problème. Pour plus d’informations sur la mise à jour des éléments dans [!DNL Workfront], voir [Modification des problèmes](../../manage-work/issues/manage-issues/edit-issues.md) et [Modifier les tâches](../../manage-work/tasks/manage-tasks/edit-tasks.md).

La liste suivante indique laquelle [!DNL Workfront] synchroniser les champs avec [!DNL Jira] champs sur les éléments liés :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Mise à jour [!DNL Workfront] field</strong> </th> 
   <th><strong>Synchronisé [!DNL Jira] champ/mise à jour</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problème ou nom de la tâche]</td> 
   <td> <p>[!UICONTROL Nom du problème]</p> <p>Un commentaire sur le changement de nom est ajouté à la variable <strong>[!DNL Workfront]</strong> de l’onglet [!DNL Jira] problème. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problème ou description de la tâche]</td> 
   <td> <p> [!UICONTROL Description du problème]</p> <p>Un commentaire sur la Description mise à jour est ajouté à la variable <strong>[!DNL Workfront]</strong> de l’onglet [!DNL Jira] problème.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Documents téléchargés]</p> <p>Remarque : Documents liés [!DNL Workfront] les éléments d’un serveur externe ne sont pas transférés vers [!DNL Jira] problèmes. Seuls les documents téléchargés directement vers [!DNL Workfront] Les éléments sont également mis à jour vers le lien [!DNL Jira] problèmes. </p> </td> 
   <td> <p>[!UICONTROL Pièces jointes]</p> <p>Un commentaire sur les pièces jointes chargées est ajouté à la variable <strong>[!DNL Workfront]</strong> de l’onglet [!DNL Jira] problème.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date d’achèvement prévue]</td> 
   <td> <p>[!UICONTROL Échéance]</p> <p>Un commentaire sur la modification de la [!UICONTROL Échéance] est ajouté à la variable [!DNL Workfront] de l’onglet [!DNL Jira] problème. </p> <p>Remarque : Vous devez activer <strong>[!UICONTROL Échéance]</strong> pour votre [!DNL Jira] problèmes pour pouvoir voir ce champ mis à jour dans [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Forms et champs personnalisés</td> 
   <td> <p> Afficher dans le [!DNL Workfront] panneau droit de [!DNL Jira] problème. <br>Seuls les champs personnalisés ayant une valeur réelle s’affichent dans le panneau.<br><img src="assets/new-custom-form-in-workfront-side-panel-1012x1314.png" alt="custom_form_in_workfront_side_panel.png" style="width: 1012;height: 1014;"></p> <p>Remarque : Les sections Formulaire personnalisé s’affichent avec le niveau d’accès de la [!DNL Workfront] administrateur. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problème ou priorité de la tâche]</td> 
   <td>S’affiche dans la variable [!DNL Workfront] panneau droit de [!DNL Jira] problème. <br>Il ne met pas à jour le problème <strong>[!UICONTROL Priority]</strong> champ dans [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Temps journal] </td> 
   <td> <p>Un commentaire sur l’heure consignée est ajouté dans la variable <strong>[!DNL Workfront]</strong> de l’onglet [!DNL Jira] problème. Cela inclut le nom de l’utilisateur qui consigne l’heure, ainsi que l’utilisateur pour lequel l’heure est enregistrée, en cas de différence. Aucune heure n’est connectée à <strong>[!UICONTROL Journal de travail]</strong> dans [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>Le commentaire est ajouté à la variable <strong>[!DNL Workfront]</strong> de l’onglet [!DNL Jira] problème. Il n’est pas ajouté à la variable <strong>[!UICONTROL Comments]</strong> de l’onglet [!DNL Jira] issue</p> <p>Remarque : Lorsque vous liez manuellement deux éléments existants, les commentaires ajoutés au [!DNL Workfront] élément avant de l’associer à [!DNL Jira] ne pas effectuer de synchronisation avec le [!DNL Jira] problème. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Mise à jour des éléments liés dans [!DNL Jira]

Si vous travaillez principalement dans [!DNL Jira], vous pouvez mettre à jour vos tâches dans [!DNL Jira] et leurs homologues dans les [!DNL Workfront] également mettre à jour. Vous n’avez pas besoin d’avoir une [!DNL Workfront] de la licence [!DNL Workfront] éléments liés à votre [!DNL Jira] problèmes pour recevoir les mises à jour que vous effectuez dans [!DNL Jira].

À condition que la variable [!DNL Workfront] l’administrateur a configuré [!DNL Workfront] pour [!DNL Jira] pour synchroniser les champs entre les éléments liés, certains champs que vous mettez à jour dans [!DNL Jira] également mettre à jour pour le lien [!DNL Workfront] élément .

La liste suivante indique laquelle [!DNL Jira] synchroniser les champs avec [!DNL Workfront] champs sur les éléments liés :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Mise à jour [!DNL Jira] Champ</strong> </th> 
   <th><strong>Synchronisé [!DNL Workfront] Champ/Mise à jour</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL État du problème]</td> 
   <td> <p> [!UICONTROL Problème ou état de la tâche]</p> <p>Etat du problème dans [!DNL Jira] synchronise avec les états suivants, ou qui correspondent aux états suivants, dans Workfront :</p> 
    <ul> 
     <li> <p>[!UICONTROL Nouveau] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL En Cours] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Fermé]/[!UICONTROL Terminé] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Remarque : Le [!DNL Jira] synchronise l’état avec la première [!DNL Workfront] qui correspond au statut approprié.</p> <p>Pour plus d’informations sur les états des éléments dans [!DNL Workfront], voir <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Création ou modification d’un état</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue Assignee]</td> 
   <td> <p> [!UICONTROL Problème ou cessionnaire de tâche]</p> <p>Important : Lorsque vous affectez un élément dans [!DNL Jira] à un utilisateur qui n’a pas de [!DNL Workfront] , l’intégration crée un utilisateur principal dans [!DNL Workfront] uniquement lorsque l’option "[!UICONTROL Créer automatiquement un utilisateur dans [!DNL Workfront] si la variable [!DNL Jira] L’utilisateur n’a pas de [!DNL Workfront] account]" est défini sur [!UICONTROL Always]. Cet utilisateur n’occupe pas un [!DNL Workfront] licence. Les utilisateurs principaux peuvent être affectés à des tâches dans [!DNL Workfront], mais ne peuvent pas être inclus dans les mises à jour. Pour plus d’informations sur la configuration de la création automatique de [!DNL Workfront] utilisateurs de [!DNL Jira], voir <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuration [!DNL Workfront for Jira]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problèmes en pièce jointe]</td> 
   <td> [!UICONTROL Problème ou documents de tâche]<br>Commentaire sur le téléchargement d’un nouveau document dans [!DNL Jira] est ajouté à l’onglet [!UICONTROL Mises à jour] de la variable [!DNL Workfront] problème ou tâche.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Échéance]</td> 
   <td> <p> Commentaire sur le changement de la date d’échéance [!UICONTROL] dans [!DNL Jira] est ajouté à l’onglet [!UICONTROL Mises à jour] de la variable [!DNL Workfront] problème ou tâche. </p> <p>Remarque : Aucune date ne change sur le [!DNL Workfront] problème ou tâche. </p> </td> 
  </tr> 
  <tr> 
   <td> Temps de connexion dans le [!DNL Workfront] panneau droit ou à partir du menu [!UICONTROL Plus] sur la [!DNL Jira] issue<br></td> 
   <td> <p>Heures<br>Outre l’ajout des heures de connexion à Jira au lien [!DNL Workfront] , un commentaire sur l’heure de connexion est ajouté à l’onglet [!UICONTROL Mises à jour] de l’élément [!DNL Workfront] élément .</p> <p>Pour plus d’informations sur le temps de connexion sur les liens [!DNL Jira] problèmes, notamment la mise à jour de la variable [!DNL Jira] utilisateur qui se connecte [!DNL Workfront], voir <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Temps de connexion pour les liens [!DNL Jira] et [!DNL Workfront] items</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Commentaires <br><br></td> 
   <td> <p>Des commentaires sont ajoutés à l’onglet [!UICONTROL Mises à jour] de la variable [!DNL Workfront] Problème ou tâche si la variable <strong>[!UICONTROL Comments]</strong> dans la section [!UICONTROL SYNCHRONISER DE JIRA À WORKFRONT] de l’onglet [!UICONTROL Configuration] sur <strong>[!UICONTROL Toujours]</strong>.</p> <p>Pour plus d’informations sur la configuration des paramètres Workfront dans [!DNL Jira], voir <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuration [!DNL Workfront for Jira]</a>.</p> <p>Pour plus d’informations sur les commentaires sur les éléments issus de liens [!DNL Jira] problèmes, voir <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Commentaire d’un lien [!DNL Jira] issue</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Temps de connexion depuis le lien [!DNL Jira] Problèmes

L’heure à laquelle vous enregistrez pour un [!DNL Jira] élément dans [!DNL Jira] sera également transféré au lien [!DNL Workfront] élément, où que dans [!DNL Jira] vous enregistrez l&#39;heure.\
Lorsque vous vous connectez à Jira dans la variable [!DNL Workfront] , la durée n’est enregistrée que dans [!DNL Workfront].\
L’heure à laquelle vous enregistrez [!DNL Workfront] n’a aucune incidence sur le moment où le problème lié se produit dans [!DNL Jira].

>[!NOTE]
>
>Si l’heure est ajoutée à une [!DNL Jira] élément lié à un [!DNL Workfront] la tâche, [!UICONTROL Type d’heure] pour l’heure en [!DNL Workfront] is [!UICONTROL Heure de la tâche]. Si l’heure est ajoutée à une [!DNL Jira] élément lié à un [!DNL Workfront] le problème, [!UICONTROL Type d’heure] pour l’heure en [!DNL Workfront] is [!UICONTROL Heure de publication].

Un commentaire est ajouté à la variable **[!DNL Workfront]** dans [!DNL Jira] et au **[!UICONTROL Mises à jour]** de l’élément dans [!DNL Workfront] pour enregistrer la journalisation de l’heure.\
L’heure est également affichée dans la variable **[!UICONTROL Heures]** de l’onglet [!DNL Workfront] élément .

* [Temps de connexion pour les liens [!DNL Jira] et [!DNL Workfront] items](#log-time-for-linked-jira-and-workfront-items)
* [Temps de connexion à partir de [!DNL Jira] à [!DNL Workfront] item](#log-time-from-jira-to-a-workfront-item)

### Temps de connexion pour les liens [!DNL Jira] et [!DNL Workfront] items

Vous pouvez consigner l’heure à partir d’un [!DNL Jira] lié à un problème [!DNL Workfront] et l’heure est enregistrée à la fois sur la variable [!DNL Jira] ainsi que le problème [!DNL Workfront] élément .

>[!IMPORTANT]
>
>Si l’utilisateur se connecte [!DNL Jira] n’existe pas dans [!DNL Workfront], l’intégration crée un utilisateur principal dans Workfront si la variable **[!UICONTROL Création automatique d’un utilisateur dans [!DNL Workfront]&#x200B; si la variable [!DNL Jira] L’utilisateur n’a pas de *[!DNL Workfront]Compte &#x200B;]** est défini sur**[!UICONTROL  Toujours ]**. Cet utilisateur n’occupe pas un [!DNL Workfront] licence. Vous pouvez affecter des utilisateurs principaux à des tâches dans [!DNL Workfront], mais vous ne pouvez pas les inclure dans les mises à jour. Pour plus d’informations sur la configuration de la création automatique de [!DNL Workfront] utilisateurs de [!DNL Jira], voir [Configuration [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Pour consigner l’heure d’un élément dans [!DNL Jira] et le faire enregistrer à la fois dans [!DNL Jira] et [!DNL Workfront]:

1. Se connecter [!DNL Jira].
1. Accédez au [!DNL Jira] qui est liée au [!DNL Workfront] élément .
1. Développez l’objet **[!UICONTROL Plus]** et cliquez sur **[!UICONTROL Journal]**.\
   ![log_time_from_More_menu_in_Jira.png](assets/new-log-time-from-more-menu-in-jira-994x594.png)

1. Dans le **[!UICONTROL Durée]** , indiquez le temps passé à travailler sur ce problème. Vous devez spécifier l’heure à l’aide des périodes suivantes :

   * [!UICONTROL Semaines] (w)
   * [!UICONTROL Days] (d)
   * [!UICONTROL Heures] (h)

1. Continuez à ajouter des informations à votre saisie horaire, y compris une **[!UICONTROL Description du travail]**, puis cliquez sur **[!UICONTROL Journal]**.\
   L’heure est ajoutée à la variable **[!UICONTROL Journal de travail]** de l’onglet [!DNL Jira] , ainsi qu’au [!DNL Workfront] élément qui lui est lié.\
   La description de travail de la saisie temporelle est enregistrée en tant que note sur l’entrée d’heure dans [!DNL Workfront].

### Temps de connexion à partir de [!DNL Jira] à [!DNL Workfront] item

Vous pouvez consigner l’heure uniquement sur le lien [!DNL Workfront] de l’élément [!DNL Jira] problème sans enregistrer cette fois-ci au [!DNL Jira] problème.

1. Se connecter [!DNL Jira].
1. Accédez à un [!DNL Jira] problème lié à un [!DNL Workfront] élément .

   Les détails de la variable [!DNL Workfront] doit s’afficher dans le [!DNL Workfront] panneau droit du problème.

1. Cliquez sur le bouton **[!UICONTROL Temps journal]** icône .

   ![Log_time_in_Jira.png](assets/log-time-in-jira.png)

1. Indiquez le nombre de **[!UICONTROL Heures]** et **[!UICONTROL Minutes]** vous souhaitez vous connecter pour le problème.

1. Cliquez sur **[!UICONTROL Temps journal]**.

   L’heure est ajoutée à la variable [!DNL Workfront] élément .

   Cette fois-ci, la fonction [!UICONTROL Journal de travail] de l’onglet [!DNL Jira] problème.

## Commentaire d’un lien [!DNL Jira] issue {#comment-from-a-linked-jira-issue}

Lorsque vous commentez une [!DNL Jira] de l’élément [!DNL Workfront] panneau droit [!DNL Jira], le commentaire est également ajouté à la variable [!UICONTROL Mises à jour] de l’élément lié dans Workfront.

Pour commenter depuis [!DNL Jira] à [!DNL Workfront] item:

1. Se connecter [!DNL Jira].
1. Accédez à un [!DNL Jira] problème lié à un [!DNL Workfront] élément .

   Les détails de la variable [!DNL Workfront] doit s’afficher dans le [!DNL Workfront] panneau droit du problème.

1. Cliquez sur le bouton **[!UICONTROL Commentaires]** dans le [!DNL Workfront] ou dans le panneau **[!UICONTROL Commentaires]** . ![Jira_comments_icon.png](assets/jira-comments-icon.png)

1. Commencez à saisir un commentaire, puis cliquez sur **[!UICONTROL Envoyer]**.

   Le commentaire est ajouté à ce qui suit :

   * Le **[!DNL Workfront]** de l’onglet [!DNL Jira] problème.
   * Le **[!UICONTROL Commentaires]** de l’onglet [!DNL Jira] problème.
   * Le **[!UICONTROL Mises à jour]** de l’élément lié dans Workfront.
