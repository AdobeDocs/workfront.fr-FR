---
content-type: overview
title: Vue d’ensemble du résumé
description: Vous pouvez utiliser le panneau Résumé pour réviser et mettre à jour les informations de l’élément de travail directement à partir d’une liste de tâches ou de problèmes, de documents ou d’autres zones de  [!DNL Adobe Workfront]  qui affichent les tâches et les problèmes.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 5d6e9788ccbae7a8970cff56558233a57ceee1ab
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 100%

---

# Vue d’ensemble du [!UICONTROL résumé]

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

Vous pouvez utiliser le panneau [!UICONTROL Résumé] pour réviser et mettre à jour les informations de l’élément de travail directement à partir d’une liste de tâches, de problèmes, de documents ou d’autres zones de [!DNL Adobe Workfront] qui affichent les tâches et les problèmes.

Votre administrateur ou administratrice Workfront ou de groupes peut modifier les zones et les champs qui s’affichent dans le panneau Résumé. Ils ou elles peuvent ajouter jusqu’à 16 champs au panneau Résumé.

>[!IMPORTANT]
>
>Nous vous recommandons d’ajouter des champs que vous devez fréquemment mettre à jour dans le panneau Résumé, afin que vous puissiez facilement y accéder et les mettre à jour sans accéder à la page principale de l’objet.
>
>Par exemple, vous pouvez ajouter les champs fréquemment mis à jour suivants au panneau Résumé de tâches et de problèmes :
>
>* Statut
>* Pourcentage d’achèvement
>* Date d&#39;engagement
>* Date d&#39;achèvement prévue
>* Condition



Le tableau suivant présente les zones où vous pouvez localiser et utiliser le panneau [!UICONTROL Résumé] :

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td><b>Tâches</b></td> 
  </tr> 
  <tr> 
   <td> <p>Listes de tâches dans un(e)</p> 
    <ul> 
     <li>Projet</li> 
     <li>Sous-tâche</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Tâches dans les zones de travail [!UICONTROL Unassigned] et [!UICONTROL Assigned] de l’[!UICONTROL Workload Balancer]</td> 
  </tr> 
   <tr> 
   <td>Tâches dans une [!UICONTROL Timesheet]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><b>Problèmes</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Listes des problèmes dans un(e)</p> 
    <ul> 
     <li>Projet</li> 
     <li>Tâche</li> 
     <li>Sous-tâche</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problèmes dans la zone [!UICONTROL Assigned Work] de l’[!UICONTROL Workload Balancer]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problèmes dans la section [!UICONTROL Submitted] de la zone [!UICONTROL Requests]</td> 
  </tr> 
</tr> 
   <tr> 
   <td>Problèmes dans une [!UICONTROL Timesheet]</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td><b>Documents</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Zone [!UICONTROL Documents]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Section [!UICONTROL Documents] d’un objet (projet, tâche, problème, programme, portfolio, modèle, tâche de modèle, utilisateur ou utilisatrice)</td> 
  </tr> 
 </tbody> 
</table>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront administrators can customize the Summary in the Layout Template. For more information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
-->

Cet article décrit comment accéder au panneau [!UICONTROL Résumé] et l’utiliser pour les tâches et les problèmes dans des listes.

Pour plus d’informations sur l’accès au [!UICONTROL Résumé] dans l’[!UICONTROL Équilibreur de charge de travail], voir [Mettre à jour des éléments de travail dans l’[!UICONTROL Équilibreur de charge de travail] à l’aide du [!UICONTROL Résumé]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Pour plus d’informations sur l’accès au [!UICONTROL Résumé] pour les documents, voir Vue d’ensemble du [[!UICONTROL Résumé] pour les documents](../../documents/managing-documents/summary-for-documents.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>Nouvelle : contributeur ou contributrice ou supérieure</p>
   Ou
   <p>Actuel :[!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuration du niveau d’accès</strong></td> 
   <td> <p>Accès [!UICONTROL View] ou supérieur aux tâches, problèmes, documents</p> <p>Accès [!UICONTROL View] ou supérieur à tout objet pour lequel vous souhaitez afficher le [!UICONTROL Summary] de documents</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations [!UICONTROL View] ou supérieures sur une tâche, un problème ou un document</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront]. Pour plus d’informations, consultez les [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Afficher le panneau [!UICONTROL Résumé] dans une liste de tâches ou de problèmes

1. Accédez à une tâche ou à un problème et sélectionnez un élément dans la liste.
1. Cliquez sur l’icône **[!UICONTROL Résumé]** ![](assets/qs-summary-in-new-toolbar-small.png)

   ou

   Cliquez sur l’icône **[!UICONTROL Ouvrir le résumé]** ![](assets/open-summary-with-text-nwe.png) dans la section [!UICONTROL Envoyé] de la zone [!UICONTROL Demandes].

   Une fois le résumé ouvert, il le reste lorsque vous sélectionnez ou cliquez sur d’autres tâches ou problèmes et reste ouvert jusqu’à ce que vous le fermiez manuellement.

   >[!TIP]
   >
   >Vous ne pouvez sélectionner qu’une seule tâche ou un seul problème à la fois pour afficher ses détails dans le panneau [!UICONTROL Résumé].

   ![Panneau Résumé](assets/summary-panel-for-task-new-comments.png)

1. (Facultatif) Pour fermer le panneau [!UICONTROL Résumé], effectuez l’une des opérations suivantes :

   * Dans une liste de tâches ou de problèmes, cliquez sur l’icône **[!UICONTROL Ouvrir le résumé]** ![](assets/summary-panel-icon.png)

     Ou

     Cliquez sur l’icône **X** dans le coin supérieur droit du panneau [!UICONTROL Résumé].

   * Dans la section [!UICONTROL Envoyé] de la zone [!UICONTROL Demandes], cliquez sur l’icône **[!UICONTROL Fermer le résumé]** ![](assets/close-summary-with-text-nwe.png)

     Ou

     Cliquez sur l’icône **X** dans le coin supérieur droit du panneau Résumé.

## [!UICONTROL Pourcentage d&#39;achèvement]

Utilisez la barre de progression en haut du [!UICONTROL Résumé] pour mettre à jour le pourcentage d’achèvement de la tâche ou du problème que vous avez sélectionné. Saisissez un nombre ou faites glisser la barre vers le pourcentage approprié.

![Pourcentage d’achèvement dans le panneau Résumé](assets/summary-overview-percent-complete.png)

## [!UICONTROL Mises à jour]

Utilisez la section [!UICONTROL Mises à jour] du [!UICONTROL Résumé] pour afficher les mises à jour récentes et effectuer des mises à jour sur la tâche ou le problème que vous avez sélectionné. Cliquez sur **[!UICONTROL Tout afficher]** pour accéder directement à l’onglet [!UICONTROL Mises à jour] de la tâche.

![Section Mises à jour dans le panneau Résumé](assets/summary-updates-section.png)

## [!UICONTROL Documents]

Utilisez la section [!UICONTROL Documents] du [!UICONTROL Résumé] pour afficher les documents associés à la tâche ou au problème que vous avez sélectionné. Cliquez sur la miniature pour ouvrir un aperçu du document. Pour accéder directement à l’onglet [!UICONTROL Documents] de la tâche ou du problème, cliquez sur le titre **[!UICONTROL Documents]**.

![Section Documents dans le panneau Résumé](assets/summary-documents-section.png)

## [!UICONTROL Détails]

Utilisez la section [!UICONTROL Détails] du [!UICONTROL Résumé] pour afficher les détails généraux de l’élément de travail, effectuer des affectations ou ajouter des dates de début. Cliquez sur **[!UICONTROL Tout afficher]** pour accéder directement à l’onglet [!UICONTROL Détails] de la tâche ou du problème.

>[!NOTE]
>
>Les champs qui apparaissent dans cette section sont les mêmes que ceux qui apparaissent dans le panneau de droite de la page d’accueil. Vous pouvez personnaliser ces champs [Personnaliser l’[!UICONTROL Accueil] et le [!UICONTROL Résumé] à l’aide d’un modèle de disposition](../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

![Section Détails dans le panneau Résumé](assets/summary-details-section.png)

## [!UICONTROL Sous-tâches]

Cette section n’est disponible que pour les tâches. Utilisez la section [!UICONTROL Sous-tâches] du [!UICONTROL Résumé] pour afficher les sous-tâches [!UICONTROL Nouveau], [!UICONTROL En cours] et [!UICONTROL Fermé] de la tâche que vous avez sélectionnée. Cliquez sur le menu déroulant **[!UICONTROL Statut]** pour basculer entre les statuts. Pour accéder directement à l’onglet [!UICONTROL Sous-tâches] de la tâche, cliquez sur le titre **[!UICONTROL Sous-tâches]**.

Si vous n’avez pas ajouté de sous-tâche à la tâche, cliquez sur **[!UICONTROL Ajoutez-en un ici]** pour accéder directement à l’onglet [!UICONTROL Sous-tâches] de la tâche.

![Section Sous-tâches dans le panneau Résumé](assets/summary-subtasks-section.png)

## [!UICONTROL Heures]

Utilisez la section [!UICONTROL Heures] du [!UICONTROL Résumé] pour consigner les heures de la tâche ou du problème que vous avez sélectionné. Cliquez sur **[!UICONTROL Consigner le temps]** et saisissez vos heures. Pour accéder directement à l’onglet Heures de la tâche ou du problème, cliquez sur le titre **[!UICONTROL Heures]**.

Le nombre d’heures dans le [!UICONTROL Résumé] indique les heures que vous consignez. Les autres utilisateurs et utilisatrices auront des nombres totaux d’heures différents dans le [!UICONTROL Résumé] en fonction du temps qu’ils consignent sur la tâche.

S’il n’y a pas d’[!UICONTROL heures] prévues sur la tâche ou le problème et que vous avez consigné le temps, la barre des heures s’affiche en rouge.

![Section Heures dans le panneau Résumé](assets/summary-hours-section.png)

## Approbations

Utilisez la section [!UICONTROL Approbations] du [!UICONTROL Résumé] pour afficher les approbations associées à la tâche ou au problème que vous avez sélectionné. Si vous n&#39;avez ajouté aucune approbation, sélectionnez une approbation existante dans le menu déroulant ou cliquez sur **[!UICONTROL Créer un processus d’approbation à usage unique]** pour accéder directement à l’onglet [!UICONTROL Approbations] sur la tâche ou le problème.

Pour accéder directement à l’onglet [!UICONTROL Approbations] sur la tâche ou le problème, cliquez sur le titre **[!UICONTROL Approbations]**.

![Section Approbations du panneau Résumé](assets/summary-approvals-section.png)
