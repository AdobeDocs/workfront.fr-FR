---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Mise à jour des éléments liés entre [!DNL Jira] et [!DNL Adobe Workfront]
description: Lorsque vous liez des problèmes  [!DNL Jira] à des tâches ou des problèmes  [!DNL Adobe Workfront] , vos utilisateurs peuvent mettre à jour des éléments dans une application et la contrepartie de cet élément est également mise à jour pour les utilisateurs travaillant dans la deuxième application.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e01f5eaf3133fa1bdaedf4dad56e9a8175b70667
workflow-type: tm+mt
source-wordcount: '1570'
ht-degree: 3%

---

# Mise à jour des éléments liés entre [!DNL Jira] et [!DNL Adobe Workfront]

Lorsque vous liez des problèmes [!DNL Jira] à des tâches ou des problèmes [!DNL Adobe Workfront], vos utilisateurs peuvent mettre à jour des éléments dans une application et la contrepartie de cet élément est également mise à jour pour les utilisateurs travaillant dans la deuxième application.

Pour plus d’informations sur la liaison d’éléments entre [!DNL Workfront] et [!DNL Jira], voir [Lier des éléments entre Adobe Workfront et Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Pendant que vous configurez [!DNL Workfront] pour [!DNL Jira], en tant qu&#39;administrateur système [!DNL Jira], vous pouvez configurer certains champs d&#39;une application pour les synchroniser avec les champs des éléments liés de l&#39;autre application.

Pour plus d&#39;informations sur la synchronisation des champs entre les éléments [!DNL Jira] et [!DNL Workfront] liés, voir [Configurer [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td><p>Nouveau : Tous</p>
       <p>ou</p>
       <p>Actuel : [!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
       <p>ou</p>
       <p>Actuelle : [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Accès administrateur système</p> <p>Important : Nous vous recommandons de créer des comptes d’administrateur système distincts dans [!DNL Jira] et [!DNL Workfront] afin de vous consacrer à cette intégration, plutôt que d’utiliser des comptes existants pouvant être joints aux utilisateurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Avant de pouvoir lier des éléments entre [!DNL Workfront] et [!DNL Jira], vous devez :

* Installez [!DNL Workfront for Jira].

  Pour plus d&#39;informations sur l&#39;installation de [!DNL Workfront for Jira], voir [Installation [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurez [!DNL Workfront for Jira].

  Pour obtenir des instructions sur la configuration de [!DNL Workfront for Jira], voir [Configuration [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Liez des éléments entre [!DNL Workfront] et [!DNL Jira].

  Pour obtenir des instructions, reportez-vous à la section [Lier des éléments entre [!DNL Adobe Workfront] et [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Mise à jour des éléments liés dans [!DNL Workfront]

Si vous travaillez principalement dans [!DNL Workfront], vous pouvez mettre à jour vos tâches dans [!DNL Workfront] et leurs homologues dans [!DNL Jira]. Cette mise à jour se fait par l’intégration de [!DNL Workfront] pour [!DNL Jira] qui ne nécessite pas que vous disposiez d’une licence [!DNL Jira].

Tant que votre administrateur [!DNL Workfront] a configuré [!DNL Workfront for Jira] pour synchroniser les champs entre les éléments liés, certains champs que vous mettez à jour dans [!DNL Workfront] sont également mis à jour pour le problème [!DNL Jira] lié. Pour plus d’informations sur la mise à jour des éléments dans [!DNL Workfront], voir [Modification des problèmes](../../manage-work/issues/manage-issues/edit-issues.md) et [Modification des tâches](../../manage-work/tasks/manage-tasks/edit-tasks.md).

La liste suivante indique les [!DNL Workfront] champs synchronisés avec les [!DNL Jira] champs sur les éléments liés :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Champ [!DNL Workfront] mis à jour</strong> </th> 
   <th><strong> [!DNL Jira] champ/mise à jour synchronisée</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Problème ou nom de la tâche]</td> 
   <td> <p>[!UICONTROL Nom du problème]</p> <p>Un commentaire sur le changement de nom est ajouté à l’onglet <strong>[!DNL Workfront]</strong> du problème [!DNL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problème ou description de la tâche]</td> 
   <td> <p> [!UICONTROL Description du problème]</p> <p>Un commentaire sur la description mise à jour est ajouté à l’onglet <strong>[!DNL Workfront]</strong> du problème [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Documents téléchargés]</p> <p>Remarque : Les documents liés à des éléments [!DNL Workfront] d’un serveur externe ne sont pas transférés vers des problèmes [!DNL Jira]. Seuls les documents chargés directement sur les éléments [!DNL Workfront] sont également mis à jour vers les problèmes [!DNL Jira] liés. </p> </td> 
   <td> <p>[!UICONTROL Pièces jointes]</p> <p>Un commentaire sur les pièces jointes chargées est ajouté à l’onglet <strong>[!DNL Workfront]</strong> du problème [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date d’achèvement prévue]</td> 
   <td> <p>[!UICONTROL Échéance]</p> <p>Un commentaire sur l’[!UICONTROL Échéance] modifiée est ajouté à l’onglet [!DNL Workfront] du problème [!DNL Jira]. </p> <p>Remarque : Vous devez activer <strong>[!UICONTROL Échéance]</strong> pour que vos problèmes [!DNL Jira] puissent voir ce champ mis à jour dans [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Forms et champs personnalisés</td> 
   <td> <p> Affichage dans le panneau de droite [!DNL Workfront] du problème [!DNL Jira]. <br>Seuls les champs personnalisés ayant une valeur réelle s’affichent dans le panneau.<br></p> <p>Remarque : les sections Formulaire personnalisé s’affichent avec le niveau d’accès de l’administrateur [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problème ou priorité de la tâche]</td> 
   <td>S’affiche dans le panneau de droite [!DNL Workfront] du problème [!DNL Jira]. <br>Il ne met pas à jour le problème <strong>[!UICONTROL Priority]</strong> dans [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Temps journal] </td> 
   <td> <p>Un commentaire sur l’heure consignée est ajouté dans l’onglet <strong>[!DNL Workfront]</strong> du problème [!DNL Jira]. Cela inclut le nom de l’utilisateur qui consigne l’heure, ainsi que l’utilisateur pour lequel l’heure est enregistrée, en cas de différence. Aucune heure n’est enregistrée dans l’onglet <strong>[!UICONTROL Work log]</strong> dans [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>Le commentaire est ajouté à l’onglet <strong>[!DNL Workfront]</strong> du problème [!DNL Jira]. Elle n’est pas ajoutée à l’onglet <strong>[!UICONTROL Comments]</strong> du problème [!DNL Jira]</p> <p>Remarque : lorsque vous liez manuellement deux éléments existants, les commentaires ajoutés à l’élément [!DNL Workfront] avant de le lier à [!DNL Jira] ne se synchronisent pas avec le problème [!DNL Jira]. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Mise à jour des éléments liés dans [!DNL Jira]

Si vous travaillez principalement dans [!DNL Jira], vous pouvez mettre à jour vos tâches dans [!DNL Jira] et leurs homologues dans [!DNL Workfront]. Vous n’avez pas besoin d’avoir une licence [!DNL Workfront] pour les éléments [!DNL Workfront] liés à vos problèmes [!DNL Jira] afin de recevoir les mises à jour que vous effectuez dans [!DNL Jira].

À condition que votre administrateur [!DNL Workfront] ait configuré [!DNL Workfront] pour [!DNL Jira] pour synchroniser les champs entre les éléments liés, certains champs que vous mettez à jour dans [!DNL Jira] sont également mis à jour pour l’élément [!DNL Workfront] lié.

La liste suivante indique les [!DNL Jira] champs synchronisés avec les [!DNL Workfront] champs sur les éléments liés :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Champ [!DNL Jira] mis à jour</strong> </th> 
   <th><strong>Synchronisé [!DNL Workfront] Field/ Update</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL État du problème]</td> 
   <td> <p> [!UICONTROL Problème ou état de la tâche]</p> <p>L’état du problème dans [!DNL Jira] se synchronise avec les états suivants, ou les états correspondant aux états suivants, dans Workfront :</p> 
    <ul> 
     <li> <p>[!UICONTROL Nouveau] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL En Cours] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Fermé]/[!UICONTROL Terminé] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Remarque : l’état [!DNL Jira] se synchronise avec le premier état [!DNL Workfront] correspondant à l’état approprié.</p> <p>Pour plus d’informations sur les états des éléments dans [!DNL Workfront], voir <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Création ou modification d’un état</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Problèmes en pièce jointe]</td> 
   <td> [!UICONTROL Problème ou documents de tâche]<br>Un commentaire sur le téléchargement d’un nouveau document dans [!DNL Jira] est ajouté à l’onglet [!UICONTROL Mises à jour] du problème ou de la tâche [!DNL Workfront].  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Échéance]</td> 
   <td> <p> Un commentaire sur le changement de la [!UICONTROL Échéance] dans [!DNL Jira] est ajouté à l’onglet [!UICONTROL Mises à jour] du problème ou de la tâche [!DNL Workfront]. </p> <p>Remarque : Aucune date ne change pour le problème ou la tâche [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td> Connectez-vous au panneau de droite [!DNL Workfront] ou à partir du menu [!UICONTROL Plus] sur le problème [!DNL Jira].<br></td> 
   <td> <p>Hours<br>Outre l’ajout des heures de connexion à Jira à l’élément [!DNL Workfront] lié, un commentaire sur l’heure de connexion est ajouté à l’onglet [!UICONTROL Mises à jour] de l’élément [!DNL Workfront].</p> <p>Pour plus d’informations sur le temps de connexion pour les problèmes [!DNL Jira] liés, y compris la mise à jour de l’utilisateur [!DNL Jira] qui consigne l’heure dans [!DNL Workfront], voir <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Temps de connexion pour les éléments [!DNL Jira] et [!DNL Workfront] liés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Commentaires <br><br></td> 
   <td> <p>Des commentaires sont ajoutés à l’onglet [!UICONTROL Mises à jour] du problème ou de la tâche [!DNL Workfront] si le paramètre <strong>[!UICONTROL Commentaires]</strong> de la section [!UICONTROL SYNCHRONISER DE JIRA À WORKFRONT] de l’onglet [!UICONTROL Configuration] vers <strong>[!UICONTROL Toujours]</strong>.</p> <p>Pour plus d'informations sur la configuration des paramètres Workfront dans [!DNL Jira], voir <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuration de [!DNL Workfront for Jira]</a>.</p> <p>Pour plus d'informations sur les commentaires sur les éléments provenant de problèmes [!DNL Jira] liés, voir <a href="#comment-from-a-linked-jira-issue" class="MCXref xref"> Commentaire provenant d'un problème [!DNL Jira] lié </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Temps de connexion des problèmes [!DNL Jira] liés

L’heure que vous enregistrez pour un élément [!DNL Jira] dans [!DNL Jira] sera également transférée à l’élément [!DNL Workfront] lié, indépendamment de l’emplacement dans [!DNL Jira] où vous enregistrez l’heure.\
Lorsque vous connectez l’heure dans Jira dans le panneau [!DNL Workfront], l’heure n’est enregistrée que dans [!DNL Workfront].\
L’heure que vous enregistrez dans [!DNL Workfront] n’affecte pas l’heure du problème lié dans [!DNL Jira].

>[!NOTE]
>
>Si l’heure est ajoutée à un élément [!DNL Jira] lié à une tâche [!DNL Workfront], le [!UICONTROL type d’heure] associé à l’heure dans [!DNL Workfront] est [!UICONTROL temps de la tâche]. Si l’heure est ajoutée à un élément [!DNL Jira] lié à un problème [!DNL Workfront], le [!UICONTROL type d’heure] correspondant à l’heure dans [!DNL Workfront] est [!UICONTROL heure de la publication].

Un commentaire est ajouté à l’onglet **[!DNL Workfront]** dans [!DNL Jira] et à l’onglet **[!UICONTROL Mises à jour]** de l’élément dans [!DNL Workfront] pour enregistrer la journalisation de l’heure.\
L’heure est également affichée dans l’onglet **[!UICONTROL Heures]** de l’élément [!DNL Workfront] .

* [Temps de connexion pour Linked [!DNL Jira] et [!DNL Workfront] items](#log-time-for-linked-jira-and-workfront-items)
* [Temps de connexion de [!DNL Jira]  à un élément  [!DNL Workfront] ](#log-time-from-jira-to-a-workfront-item)

### Temps de connexion pour les éléments [!DNL Jira] et [!DNL Workfront] liés

Vous pouvez consigner l’heure à partir d’un problème [!DNL Jira] lié à un élément [!DNL Workfront] et l’heure est enregistrée sur le problème [!DNL Jira] ainsi que sur l’élément [!DNL Workfront].

>[!IMPORTANT]
>
>Si l’utilisateur qui consigne l’heure dans [!DNL Jira] n’existe pas dans [!DNL Workfront], l’intégration crée un nouvel utilisateur actif dans Workfront si l’option **[!UICONTROL Créer automatiquement un utilisateur dans [!DNL Workfront] &#x200B; si l’utilisateur [!DNL Jira] n’a pas de compte *[!DNL Workfront] &#x200B;]** est définie sur**[!UICONTROL  Toujours ]**. Cet utilisateur n’utilise pas de licence [!DNL Workfront]. Vous pouvez affecter des utilisateurs actifs à des tâches dans [!DNL Workfront], mais vous ne pouvez pas les inclure dans les mises à jour. Pour plus d&#39;informations sur la configuration de la création automatique d&#39;utilisateurs [!DNL Workfront] à partir de [!DNL Jira], voir [Configuration [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Pour consigner la durée de connexion d’un élément dans [!DNL Jira] et l’enregistrer dans [!DNL Jira] et [!DNL Workfront] :

1. Connectez-vous à [!DNL Jira].
1. Accédez au problème [!DNL Jira] lié à l’élément [!DNL Workfront].
1. Développez le menu **[!UICONTROL Plus]** et cliquez sur **[!UICONTROL Journal du travail]**.

1. Dans le champ **[!UICONTROL Durée de la visite]**, indiquez la durée de travail sur ce problème. Vous devez spécifier l’heure à l’aide des périodes suivantes :

   * [!UICONTROL Semaines] (w)
   * [!UICONTROL Days] (d)
   * [!UICONTROL Hours] (h)

1. Continuez à ajouter des informations à votre entrée horaire, y compris une **[!UICONTROL description du travail]**, puis cliquez sur **[!UICONTROL Journal]**.\
   L’heure est ajoutée à l’onglet **[!UICONTROL Journal de travail]** de l’élément [!DNL Jira], ainsi qu’à l’élément [!DNL Workfront] qui y est lié.\
   La description de travail de l’entrée d’heure est enregistrée comme note sur l’entrée d’heure dans [!DNL Workfront].

### Temps de connexion de [!DNL Jira] à un élément [!DNL Workfront]

Vous pouvez consigner l’heure uniquement à l’élément [!DNL Workfront] lié à partir du problème [!DNL Jira] sans enregistrer cette heure jusqu’au problème [!DNL Jira].

1. Connectez-vous à [!DNL Jira].
1. Accédez à un problème [!DNL Jira] lié à un élément [!DNL Workfront].

   Les détails de l’élément [!DNL Workfront] doivent s’afficher dans le panneau de droite [!DNL Workfront] du problème.

1. Cliquez sur l’icône **[!UICONTROL Durée du journal]** .

1. Indiquez les **[!UICONTROL Heures]** et **[!UICONTROL Minutes]** que vous souhaitez enregistrer pour le problème.

1. Cliquez sur **[!UICONTROL Consigner le temps]**.

   L’heure est ajoutée à l’élément [!DNL Workfront] .

   Cette fois n’est pas ajoutée à l’onglet [!UICONTROL Journal de travail] du problème [!DNL Jira].

## Commentaire d&#39;un problème [!DNL Jira] lié {#comment-from-a-linked-jira-issue}

Lorsque vous commentez un élément [!DNL Jira] du panneau de droite [!DNL Workfront] dans [!DNL Jira], le commentaire est également ajouté à l’onglet [!UICONTROL Mises à jour] de l’élément lié dans Workfront.

Pour commenter de [!DNL Jira] à un élément [!DNL Workfront] :

1. Connectez-vous à [!DNL Jira].
1. Accédez à un problème [!DNL Jira] lié à un élément [!DNL Workfront].

   Les détails de l’élément [!DNL Workfront] doivent s’afficher dans le panneau de droite [!DNL Workfront] du problème.

1. Cliquez sur l’icône **[!UICONTROL Comments]** dans le panneau [!DNL Workfront] ou sur l’onglet **[!UICONTROL Comments]** .

1. Commencez à saisir un commentaire, puis cliquez sur **[!UICONTROL Envoyer]**.

   Le commentaire est ajouté à ce qui suit :

   * Onglet **[!DNL Workfront]** du problème [!DNL Jira].
   * Onglet **[!UICONTROL Comments]** du problème [!DNL Jira].
   * Onglet **[!UICONTROL Mises à jour]** de l’élément lié dans Workfront.
