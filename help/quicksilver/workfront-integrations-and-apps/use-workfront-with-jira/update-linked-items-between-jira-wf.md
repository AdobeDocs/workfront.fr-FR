---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Mettre à jour les éléments liés entre  [!DNL Jira]  et  [!DNL Adobe Workfront]
description: Lorsque vous liez des problèmes  [!DNL Jira]  à des tâches ou des problèmes  [!DNL Adobe Workfront] , vos utilisateurs et utilisatrices peuvent mettre à jour des éléments dans une application. L’équivalent de cet élément est également mis à jour pour les personnes travaillant dans la seconde application.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '1657'
ht-degree: 92%

---

# Mettre à jour les éléments liés entre [!DNL Jira] et [!DNL Adobe Workfront]

>[!IMPORTANT]
>
>Pour offrir des intégrations plus stables et plus évolutives, nous passons à une approche d’intégration moderne et flexible à l’aide de Workfront Automation and Integration (Fusion). Dans le cadre de ce processus de transition, l’intégration Workfront for Jira ne sera plus disponible après le **28 février 2026**.
>
>Nous vous recommandons d’utiliser l’automatisation et l’intégration de Workfront pour les besoins d’intégration de votre organisation à Jira.
>
>Pour une présentation de l’automatisation et de l’intégration de Workfront, consultez [Présentation d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Pour plus d’informations sur les fonctionnalités spécifiques des modules d’automatisation et d’intégration de Workfront pour Jira, voir [Modules logiciels Jira](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Lorsque vous liez des problèmes [!DNL Jira] à des tâches ou des problèmes [!DNL Adobe Workfront], vos utilisateurs et utilisatrices peuvent mettre à jour des éléments dans une application. Les équivalents de ces éléments sont également mis à jour pour les personnes travaillant dans la seconde application.

Pour plus d’informations sur la liaison d’éléments entre [!DNL Workfront] et [!DNL Jira], voir la section [Lier des éléments entre Adobe Workfront et Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Lors de la configuration de [!DNL Workfront] pour [!DNL Jira], vous pouvez, en tant qu’administrateur ou administratrice système [!DNL Jira], configurer certains champs d’une application afin de les synchroniser avec les champs des éléments liés de l’autre application.

Pour plus d’informations sur la synchronisation des champs entre des éléments liés de [!DNL Jira] et [!DNL Workfront], voir la section [Configurer [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Tous</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Accès Jira</td> 
   <td> <p>Accès pour l’administration système</p> <p>Important : nous vous recommandons de créer des comptes d’administrateur système distincts dans Jira et Workfront à dédier à cette intégration, plutôt que d’utiliser des comptes existants qui peuvent être associés aux utilisateurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de pouvoir lier des éléments entre [!DNL Workfront] et [!DNL Jira], vous devez procéder comme suit :

* Installez [!DNL Workfront for Jira].

  Pour obtenir des instructions sur l’installation de [!DNL Workfront for Jira], voir la section [Installer  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurez [!DNL Workfront for Jira].

  Pour obtenir des instructions sur la configuration de [!DNL Workfront for Jira], voir la section [Configurer  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Liez des éléments entre [!DNL Workfront] et [!DNL Jira].

  Pour obtenir des instructions, voir la section [Lier des éléments entre  [!DNL Adobe Workfront]  et  [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Mettre à jour des éléments liés dans [!DNL Workfront]

Si vous travaillez principalement dans [!DNL Workfront], vous pouvez mettre à jour vos éléments de travail dans [!DNL Workfront]. Leurs équivalents dans [!DNL Jira] se mettent également à jour. Cette mise à jour se fait par l’intégration de [!DNL Workfront] pour [!DNL Jira], qui ne nécessite pas que vous disposiez d’une licence [!DNL Jira].

À condition que votre administrateur ou administratrice [!DNL Workfront] ait configuré [!DNL Workfront for Jira] pour qu’il synchronise les champs entre les éléments liés, certains champs que vous mettez à jour dans [!DNL Workfront] se mettent également à jour pour le problème [!DNL Jira] lié. Pour plus d’informations sur la mise à jour des éléments dans [!DNL Workfront], voir la section [Modifier des problèmes](../../manage-work/issues/manage-issues/edit-issues.md) et [Modifier des tâches](../../manage-work/tasks/manage-tasks/edit-tasks.md).

La liste suivante indique les champs [!DNL Workfront] qui se synchronisent avec les champs [!DNL Jira] sur les éléments liés :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Champ [!DNL Workfront] mis à jour</strong> </th> 
   <th><strong>Champ [!DNL Jira] synchronisé/mise à jour</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue or Task name]</td> 
   <td> <p>[!UICONTROL Issue name]</p> <p>Un commentaire sur le changement de nom est ajouté à l’onglet <strong>[!DNL Workfront]</strong> du problème [!DNL Jira].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Description]</td> 
   <td> <p> [!UICONTROL Issue Description]</p> <p>Un commentaire sur la description mise à jour est ajouté à l’onglet <strong>[!DNL Workfront]</strong> du problème [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Uploaded Documents]</p> <p>Note : les documents liés à des éléments [!DNL Workfront] provenant d’un serveur externe ne sont pas transférés aux problèmes [!DNL Jira]. Seuls les documents chargés directement vers des éléments [!DNL Workfront] sont également mis à jour vers les problèmes [!DNL Jira] liés.</p> </td> 
   <td> <p>[!UICONTROL Attachments]</p> <p>Un commentaire concernant les pièces jointes chargées est ajouté à l’onglet <strong>[!DNL Workfront]</strong> du problème [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>[!UICONTROL Due Date]</p> <p>Un commentaire sur la modification de la [!UICONTROL Due Date] est ajouté à l’onglet[!DNL Workfront] du problème [!DNL Jira].</p> <p>Note : vous devez activer la <strong>[!UICONTROL Due Date]</strong> pour vos problèmes [!DNL Jira] pour pouvoir voir ce champ mis à jour dans [!UICONTROL Jira].</p> </td> 
  </tr> 
  <tr> 
   <td>Formulaires personnalisés et champs personnalisés</td> 
   <td> <p> Afficher dans le panneau de droite de [!DNL Workfront] du problème [!DNL Jira]. <br>Seuls les champs personnalisés ayant une valeur réelle s’affichent dans le panneau.<br></p> <p>Note : les sections Formulaires personnalisés s’affichent avec le niveau d’accès de l’administrateur ou administratrice [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Priority]</td> 
   <td>S’affiche dans le panneau droit de [!DNL Workfront] du problème [!DNL Jira]. <br>Cela ne met pas à jour le champ <strong>[!UICONTROL Priority]</strong> du problème dans [!DNL Jira].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log time]</td> 
   <td> <p>Un commentaire sur le temps consigné est ajouté dans l’onglet <strong>[!DNL Workfront]</strong> du problème [!DNL Jira]. Cela inclut le nom de la personne qui consigne le temps, ainsi que la personne pour laquelle le temps est consigné, si ce ne sont pas les mêmes personnes. Aucune heure n’est consignée dans l’onglet <strong>[!UICONTROL Work log]</strong> de [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>Le commentaire est ajouté à l’onglet <strong>[!DNL Workfront]</strong> du problème [!DNL Jira]. Il n’est pas ajouté à l’onglet <strong>[!UICONTROL Comments]</strong> du problème [!DNL Jira].</p> <p>Note : lorsque vous liez manuellement deux éléments existants, les commentaires ajoutés à l’élément [!DNL Workfront] avant sa liaison avec [!DNL Jira] ne se synchronisent pas avec le problème [!DNL Jira].</p> <p>Les commentaires Jira se synchronisent avec Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## Mettre à jour des éléments liés dans [!DNL Jira]

Si vous travaillez principalement dans [!DNL Jira], vous pouvez mettre à jour vos tâches dans [!DNL Jira] et leurs homologues dans [!DNL Workfront] se mettront également à jour. Vous n’avez pas besoin d’avoir une licence [!DNL Workfront] pour les éléments [!DNL Workfront] liés à vos problèmes [!DNL Jira] pour recevoir les mises à jour que vous effectuez dans [!DNL Jira].

À condition que votre administrateur ou administratrice [!DNL Workfront] ait configuré [!DNL Workfront] pour [!DNL Jira] pour synchroniser les champs entre les éléments liés, certains champs que vous mettez à jour dans [!DNL Jira] se mettent également à jour pour l’élément [!DNL Workfront] lié.

La liste suivante indique quels champs [!DNL Jira] synchroniser avec les champs [!DNL Workfront] sur les éléments liés.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Champ [!DNL Jira] mis à jour</strong> </th> 
   <th><strong>Champ/mise à jour[!DNL Workfront] ayant fait la synchronisation</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue Status]</td> 
   <td> <p> [!UICONTROL Issue or Task Status]</p> <p>Le statut du problème dans [!DNL Jira] se synchronise avec les statuts suivants, ou avec des statuts qui correspondent aux statuts suivants, dans Workfront :</p> 
    <ul> 
     <li> <p>[!UICONTROL New] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL In Progress] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Note : le statut [!DNL Jira] se synchronise avec le premier statut [!DNL Workfront] qui correspond au statut approprié.</p> <p>Pour plus d’informations sur les statuts des éléments dans [!DNL Workfront], voir <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Créer ou modifier un statut</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Issue Attachments]</td> 
   <td> [!UICONTROL Issue or Task Documents]<br>Un commentaire sur le chargement d’un nouveau document dans [!DNL Jira] est ajouté à l’onglet [!UICONTROL Updates] du problème ou de la tâche [!DNL Workfront]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p> Un commentaire sur le changement de la [!UICONTROL Due Date] dans [!DNL Jira] est ajouté à l’onglet [!UICONTROL Updates] du problème ou de la tâche [!DNL Workfront].</p> <p>Note : aucune date ne change dans le problème ou la tâche [!DNL Workfront].</p> </td> 
  </tr> 
  <tr> 
   <td> Consigner le temps dans le panneau droit de [!DNL Workfront] ou à partir du menu [!UICONTROL More] du problème [!DNL Jira]<br></td> 
   <td> <p>Heures<br>En plus d’ajouter les heures consignées dans Jira à l’élément [!DNL Workfront] lié, un commentaire sur le temps consigné est ajouté à l’onglet [!UICONTROL Updates] de l’élément [!DNL Workfront].</p> <p>Pour plus d’informations sur le temps consignés sur les problèmes [!DNL Jira] liés, notamment la mise à jour de la personne [!DNL Jira] qui consigne le temps dans [!DNL Workfront], voir <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Consigner le temps pour les éléments [!DNL Jira] et [!DNL Workfront] liés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Commentaires<br><br></td> 
   <td> <p>Des commentaires sont ajoutés à l’onglet [!UICONTROL Updates] du problème ou de la tâche [!DNL Workfront] si le paramètre <strong>[!UICONTROL Comments]</strong> dans la section [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] de l’onglet [!UICONTROL Setup] est défini sur <strong>[!UICONTROL Always]</strong>.</p> <p>Pour plus d’informations sur la configuration des paramètres Workfront dans [!DNL Jira], voir <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configurer [!DNL Workfront for Jira]</a>.</p> <p>Pour plus d’informations sur les commentaires sur les éléments issus des problèmes [!DNL Jira] liés, voir <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Commenter à partir d’un problème [!DNL Jira]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Consigner le temps à partir des problèmes [!DNL Jira] liés

Le temps que vous enregistrez pour un élément [!DNL Jira] dans [!DNL Jira] sera également transféré à l’élément [!DNL Workfront] lié, quel que soit l’emplacement où vous consignez le temps dans [!DNL Jira].\
Lorsque vous vous connectez à Jira dans le panneau [!DNL Workfront], le temps n’est enregistré que dans [!DNL Workfront].\
Le temps que vous enregistrez dans [!DNL Workfront] n’a aucune incidence sur le temps du problème lié dans [!DNL Jira].

>[!NOTE]
>
>Si l’heure est ajoutée à un élément [!DNL Jira] lié à une tâche [!DNL Workfront], le [!UICONTROL type d’heure] pour l’heure dans [!DNL Workfront] est [!UICONTROL Heure de la tâche]. Si l’heure est ajoutée à un élément [!DNL Jira] lié à un problème [!DNL Workfront], le [!UICONTROL type d’heure] pour l’heure dans [!DNL Workfront] est [!UICONTROL Heure du problème].

Un commentaire est ajouté à l’onglet **[!DNL Workfront]** dans [!DNL Jira] et à l’onglet **[!UICONTROL Mises à jour]** de l’élément dans [!DNL Workfront] pour enregistrer la consignation de l’heure.\
L’heure est également affichée dans l’onglet **[!UICONTROL Heures]** de l’élément [!DNL Workfront].

* [Consigner les heures pour les éléments  [!DNL Jira]  et  [!DNL Workfront]  liés](#log-time-for-linked-jira-and-workfront-items)
* [Consigner les heures à partir de  [!DNL Jira]  vers un élément  [!DNL Workfront] &#x200B;](#log-time-from-jira-to-a-workfront-item)

### Consigner les heures pour les éléments [!DNL Jira] et [!DNL Workfront] liés

Vous pouvez consigner les heures à partir d’un problème [!DNL Jira] lié à un élément [!DNL Workfront], et les heures seront consignées à la fois sur le problème [!DNL Jira] et sur l’élément [!DNL Workfront].

>[!IMPORTANT]
>
>Si la personne qui consigne les heures dans [!DNL Jira] n’existe pas dans [!DNL Workfront], l’intégration crée une personne active dans Workfront si l’option **[!UICONTROL Créer automatiquement un utilisateur ou une utilisatrice dans [!DNL Workfront] si l’utilisateur ou utilisatrice de [!DNL Jira] n’a pas de compte *[!DNL Workfront]]** est définie sur&#x200B;**[!UICONTROL &#x200B; Toujours &#x200B;]**. Cette personne ne dispose pas d’une licence [!DNL Workfront]. Vous pouvez affecter des personnes actives à des éléments de travail dans [!DNL Workfront], mais vous ne pouvez pas les inclure dans les mises à jour. Pour plus d’informations sur la configuration de la création automatique d’utilisateurs et utilisatrices [!DNL Workfront] à partir de [!DNL Jira], voir [Configurer  [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Pour consigner les heures d’un élément dans [!DNL Jira] et les faire enregistrer à la fois dans [!DNL Jira] et dans [!DNL Workfront], procédez comme suit :

1. Connectez-vous à [!DNL Jira].
1. Accédez au problème [!DNL Jira] qui est lié à l’élément [!DNL Workfront].
1. Développez le menu **[!UICONTROL Plus]** et cliquez sur **[!UICONTROL Consigner le travail]**.

1. Dans le champ **[!UICONTROL Temps passé]**, indiquez le temps passé à travailler sur ce problème. Vous devez spécifier les heures à l’aide des périodes suivantes :

   * [!UICONTROL Semaines] (w)
   * [!UICONTROL Jours] (d)
   * [!UICONTROL Heures] (h)

1. Continuez à ajouter des informations à votre saisie horaire, y compris une **[!UICONTROL Description du travail]**, puis cliquez sur **[!UICONTROL Consigner]**.\
   Les heures sont ajoutée à l’onglet **[!UICONTROL Consigner le travail]** de l’élément [!DNL Jira], ainsi qu’à l’élément [!DNL Workfront] qui lui est lié.\
   La description du travail de la saisie horaire est enregistrée en tant que note sur la saisie horaire dans [!DNL Workfront].

### Consigner les heures à partir de [!DNL Jira] sur un élément [!DNL Workfront]

Vous pouvez consigner les heures uniquement sur l’élément [!DNL Workfront] lié à partir du problème [!DNL Jira] sans enregistrer ces heures sur le problème [!DNL Jira].

1. Connectez-vous à [!DNL Jira].
1. Accédez à un problème [!DNL Jira] lié à un élément [!DNL Workfront].

   Les détails de l’élément [!DNL Workfront] doivent s’afficher dans le panneau droit [!DNL Workfront] du problème.

1. Cliquez sur l’icône **[!UICONTROL Consigner les heures]**.

1. Indiquez le nombre d’**[!UICONTROL heures]** et de **[!UICONTROL minutes]** que vous souhaitez consigner pour le problème.

1. Cliquez sur **[!UICONTROL Consigner les heures]**.

   Les heures sont ajoutées à l’élément [!DNL Workfront].

   Ces heures ne sont pas ajoutées à l’onglet [!UICONTROL Journal de travail] du problème [!DNL Jira].

## Commenter à partir d’un problème [!DNL Jira] lié {#comment-from-a-linked-jira-issue}

Lorsque vous faites un commentaire sur un élément [!DNL Jira] à partir du panneau droit de [!DNL Workfront] dans [!DNL Jira], le commentaire est également ajouté à l’onglet [!UICONTROL Mises à jour] de l’élément lié dans Workfront.

Pour commenter de [!DNL Jira] vers un élément [!DNL Workfront], procédez comme suit :

1. Connectez-vous à [!DNL Jira].
1. Accédez à un problème [!DNL Jira] lié à un élément [!DNL Workfront].

   Les détails de l’élément [!DNL Workfront] doivent s’afficher dans le panneau droit de [!DNL Workfront] du problème.

1. Cliquez sur l’icône **[!UICONTROL Commentaires]** dans le panneau [!DNL Workfront] ou dans l’onglet **[!UICONTROL Commentaires]**.

1. Commencez à saisir un commentaire, puis cliquez sur **[!UICONTROL Envoyer]**.

   Le commentaire est ajouté à ce qui suit :

   * Onglet **[!DNL Workfront]** du problème [!DNL Jira].
   * Onglet **[!UICONTROL Commentaires]** du problème [!DNL Jira].
   * Onglet **[!UICONTROL Mises à jour]** de l’élément lié dans Workfront.
