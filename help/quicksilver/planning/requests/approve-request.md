---
title: Approuver une demande dans Adobe Workfront Planning
description: Lorsque l’utilisateur envoie une demande à un formulaire de demande associé à une approbation dans Adobe Workfront Planning, les approbateurs reçoivent une notification et un e-mail concernant l’approbation en attente. Ils doivent approuver la demande avant que Workfront Planning ne crée un objet.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: 99e26d4249162e46da1a73301e68bdf30436a81d
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 7%

---

# Approuver une demande dans Adobe Workfront Planning

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Lorsque l’utilisateur envoie une demande à un formulaire de demande associé à une approbation dans Adobe Workfront Planning, les approbateurs reçoivent une notification et un e-mail concernant l’approbation en attente. Ils doivent approuver la demande avant que Workfront Planning ne crée un objet.

Cet article décrit comment un gestionnaire d’espace de travail peut approuver une demande soumise pour que Workfront Planning crée un enregistrement.

Nous vous recommandons de consulter également les articles suivants :

* [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Envoi de requêtes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md)
* [Ajouter une approbation à un formulaire de demande](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Considérations relatives à l’approbation des demandes

* Les demandes envoyées s’affichent dans l’onglet Planification de la section Soumises de la zone des Demandes de Workfront avec l’un des statuts de demande suivants :

   * **Révision en attente** : ce statut s&#39;affiche lorsqu&#39;aucun approbateur n&#39;a ouvert l&#39;objet de la demande.
   * **En révision** : le statut **En attente de révision** passe à **En révision** lorsqu’au moins un approbateur ouvre l’objet de la demande. Le statut de la demande reste **En révision** jusqu&#39;à ce que tous les approbateurs aient approuvé la demande.
   * **Approuvé** : lorsqu&#39;un approbateur approuve l&#39;objet de la demande, son statut individuel devient **Approuvé**, mais le statut global de l&#39;objet de la demande reste **En révision** jusqu&#39;à ce que tous les approbateurs aient pris leurs décisions. Lorsque tous les approbateurs approuvent une demande, le statut de la demande devient **Approuvé**.
   * **Terminé** : si tous les approbateurs approuvent l&#39;objet de la demande, son statut passe à **Terminé** ou si la demande n&#39;avait pas besoin d&#39;approbation.
   * **Rejeté** : si un approbateur rejette l&#39;objet de la demande, le statut devient **Rejeté**. Aucun enregistrement n&#39;est créé et une nouvelle demande doit être soumise pour créer l&#39;enregistrement.

* Vous pouvez afficher les informations d&#39;approbation sur un enregistrement créé en soumettant un formulaire de demande dans les champs Date d&#39;approbation par et Date d&#39;approbation . Pour plus d’informations, voir [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Packages Adobe Workfront</p></td> 
   <td> 
<p>Tout package Workfront et tout package Planning</p>
Ou
<p>Tout package de workflow et tout package Planning</p>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Tous</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérez les autorisations d’un espace de travail et d’un type d’enregistrement</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Valider une demande de création d’enregistrement

Une fois que les utilisateurs ont ajouté des demandes à un formulaire de demande de type enregistrement associé à une approbation, la demande est envoyée aux approbateurs.

Les approbateurs reçoivent les notifications suivantes sur une demande en attente d&#39;approbation :

* Une notification in-app
* Notification par e-mail

>[!NOTE]
>
>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour que les utilisateurs puissent recevoir des notifications par e-mail et in-app.

Vous pouvez approuver des demandes de création d’enregistrements à partir de la demande elle-même <span class="preview">ou à partir du widget Mes approbations sur l’Accueil.</span>

* [Approuver une demande à partir de la demande dans Workfront Planning](#approve-a-request-from-the-request-in-workfront-planning)
* [Approuver une demande à partir du widget Mes approbations de l’Accueil](#approve-a-request-from-the-my-approvals-widget-in-home)

### Approuver une demande à partir de la demande dans Workfront Planning

1. (Conditionnel) Si vous utilisez l’expérience de requête héritée dans Workfront, ouvrez la requête en effectuant l’une des opérations suivantes :

   * Si vous avez accès à Workfront Planning et que vous pouvez afficher au moins un espace de travail, cliquez sur **Menu principal** ![Menu principal des points](assets/dots-menu.png) dans le coin supérieur droit de l’écran, ou sur **Menu principal** ![Menu principal des lignes](assets/lines-menu.png) dans le coin supérieur gauche, le cas échéant, puis cliquez sur **Demandes** > **Submitted** Planning **, et cliquez sur la demande avec le statut** En attente de révision **ou** En révision **&#x200B;**.

     >[!TIP]
     >
     >Si vous n’avez pas accès à Workfront Planning, ou si vous n’avez pas accès à des espaces de travail, vous pouvez uniquement accéder à une demande pour l’approuver à l’aide de vos notifications par e-mail ou in-app.

   * Cliquez sur l’icône de zone **Notifications** ![Icône de zone de notifications dans Unified Shell](assets/notifications-area-icon-unified-shell.png) dans le coin supérieur droit de l’écran, puis cliquez sur la notification d’une demande en attente de votre approbation pour ouvrir la demande.
   * Accédez à la notification par e-mail dans votre e-mail qui vous informe qu’une demande est en attente de votre approbation, puis cliquez sur **Ouvrir la demande** pour ouvrir la demande. <!--add the name of the button here, from the email-->

   La page de requête s’ouvre en mode lecture seule.

   ![Page de requête en lecture seule au statut de révision](assets/read-only-reqeust-page-in-review-status.png)
1. Si vous utilisez la nouvelle expérience de demande dans Workfront, cliquez sur **Menu principal** ![Menu principal des points](assets/dots-menu.png) dans le coin supérieur droit de l’écran, ou sur **Menu principal** ![Menu principal des lignes](assets/lines-menu.png) dans le coin supérieur gauche, le cas échéant, cliquez sur **Demandes**, puis cliquez sur la demande à approuver avec le statut **En attente de révision** ou **En révision**.
1. (Facultatif) Cliquez sur l’icône **Approbations** ![Icône Approbations](assets/approvals-icon.png) dans le coin supérieur droit de la demande pour afficher les approbateurs.
1. Cliquez sur **Vérifier et approuver** puis choisissez l’une des options suivantes :

   * **Approuver** : permet d’approuver la demande. Un enregistrement est immédiatement créé pour le type d&#39;enregistrement associé au formulaire de demande une fois que tous les approbateurs ont approuvé la demande.
   * **Rejeter** : la demande est rejetée, même si vous êtes le seul approbateur à la rejeter. Aucun enregistrement n&#39;est créé pour le type d&#39;enregistrement associé au formulaire de demande.

   L’utilisateur qui a soumis la demande reçoit un e-mail et des notifications in-app lorsque sa demande est approuvée ou rejetée.

   Le statut de la demande est alors modifié comme suit, selon la décision d’approbation :

   * **Terminé** : la demande est approuvée.
   * **Rejeté** : la demande est rejetée.

   La demande reste dans l’onglet Planification de la section Soumis de la zone Demandes de Workfront.

<div class="preview">

### Approuver une demande à partir du widget Mes approbations de l’Accueil

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, ou (le cas échéant) cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) en haut à gauche, puis cliquez sur **[!UICONTROL Accueil]**.

   Ou

   Cliquez sur l’icône [!UICONTROL Accueil] ![Icône Accueil](/help/_includes/assets/home-icon-30x29.png) dans le coin supérieur gauche d’Adobe Workfront, puis recherchez le widget Mes approbations .

1. Recherchez l’objet à approuver ou à rejeter.

1. (Facultatif) Ajoutez un commentaire en cliquant sur la flèche déroulante en regard de Approuver ou Rejeter, en saisissant la note, puis en cliquant sur Ajouter.

1. Choisissez l’une des options suivantes :

   * **Approuver** : permet d’approuver la demande. Un enregistrement est immédiatement créé pour le type d&#39;enregistrement associé au formulaire de demande une fois que tous les approbateurs ont approuvé la demande.
   * **Rejeter** : la demande est rejetée, même si vous êtes le seul approbateur à la rejeter. Aucun enregistrement n&#39;est créé pour le type d&#39;enregistrement associé au formulaire de demande.

   L’utilisateur qui a soumis la demande reçoit un e-mail et des notifications in-app lorsque sa demande est approuvée ou rejetée.

   Le statut de la demande est alors modifié comme suit, selon la décision d’approbation :

   * **Terminé** : la demande est approuvée.
   * **Rejeté** : la demande est rejetée.

</div>
