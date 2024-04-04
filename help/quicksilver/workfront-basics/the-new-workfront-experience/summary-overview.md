---
content-type: overview
title: Aperçu du résumé
description: Vous pouvez utiliser le panneau Résumé pour passer en revue et mettre à jour les informations des éléments de travail directement à partir d’une liste de problèmes de tâches, de documents ou d’autres zones de [!DNL Adobe Workfront] qui affichent les tâches et les problèmes.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 5d6e9788ccbae7a8970cff56558233a57ceee1ab
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 2%

---

# [!UICONTROL Résumé] aperçu

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

Vous pouvez utiliser la variable [!UICONTROL Résumé] pour examiner et mettre à jour les informations des éléments de travail directement à partir d’une liste de tâches, de problèmes, de documents ou d’autres zones de [!DNL Adobe Workfront] qui affichent les tâches et les problèmes.

Votre administrateur Workfront ou de groupe peut modifier les zones et les champs qui s’affichent dans le panneau Résumé. Ils peuvent ajouter jusqu’à 16 champs au panneau Résumé.

>[!IMPORTANT]
>
>Nous vous recommandons d’ajouter des champs que vous devez fréquemment mettre à jour dans le panneau Résumé, afin que vous puissiez facilement y accéder et les mettre à jour sans accéder à la page principale de l’objet.
>
>Par exemple, vous pouvez ajouter les champs suivants fréquemment mis à jour aux tâches et aux problèmes des panneaux de résumé :
>
>* Statut
>* Pourcentage d&#39;achèvement
>* Date d&#39;engagement
>* Date d&#39;achèvement prévue
>* Condition



Le tableau suivant répertorie les zones où vous pouvez localiser et utiliser la variable [!UICONTROL Résumé] panel :

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td><b>Tâches</b></td> 
  </tr> 
  <tr> 
   <td> <p>Listes de tâches dans une</p> 
    <ul> 
     <li>Projet</li> 
     <li>Sous-tâche</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Tâches dans les zones de travail [!UICONTROL non affecté] et [!UICONTROL Affecté] de l’[!UICONTROL équilibreur de charge de travail]</td> 
  </tr> 
   <tr> 
   <td>Tâches dans une [!UICONTROL Feuille de calcul]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><b>Problèmes</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Listes de problèmes dans</p> 
    <ul> 
     <li>Projet</li> 
     <li>Tâche</li> 
     <li>Sous-tâche</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problèmes dans la zone [!UICONTROL Affecté Work] de l’[!UICONTROL Workload Balancer]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problèmes dans la section [!UICONTROL Envoyé] de la zone [!UICONTROL Demandes]</td> 
  </tr> 
</tr> 
   <tr> 
   <td>Problèmes dans une feuille de calcul [!UICONTROL]</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td><b>Documents</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Zone [!UICONTROL Documents]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Section [!UICONTROL Documents] d’un objet (projet, tâche, problème, programme, portefeuille, modèle, tâche de modèle, utilisateur)</td> 
  </tr> 
 </tbody> 
</table>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront administrators can customize the Summary in the Layout Template. For more information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
-->

Cet article décrit comment accéder à et utiliser le [!UICONTROL Résumé] pour les tâches et les problèmes dans les listes.

Pour plus d’informations sur l’accès au [!UICONTROL Résumé] dans le [!UICONTROL Équilibreur de charge de travail], voir [Mise à jour des tâches dans [!UICONTROL Équilibreur de charge de travail] en utilisant la variable [!UICONTROL Résumé]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Pour plus d’informations sur l’accès au [!UICONTROL Résumé] pour les documents, voir [[!UICONTROL Résumé] présentation des documents](../../documents/managing-documents/summary-for-documents.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Nouveau : contributeur ou version ultérieure</p>
   Ou
   <p>Actuel :[!UICONTROL Request] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuration du niveau d’accès</strong></td> 
   <td> <p>[!UICONTROL Affichage] ou accès supérieur à Tâches, Problèmes, Documents</p> <p>[!UICONTROL Affichage] ou un accès supérieur à tout objet pour lequel vous souhaitez afficher des documents [!UICONTROL Résumé]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations [!UICONTROL View] ou supérieures pour une tâche, un problème ou un document</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Afficher la variable [!UICONTROL Résumé] dans une liste de tâches ou de problèmes

1. Accédez à une tâche ou à un problème et sélectionnez un élément dans la liste.
1. Cliquez sur le bouton **[!UICONTROL Résumé]** icon ![](assets/qs-summary-in-new-toolbar-small.png)

   ou

   Cliquez sur le bouton **[!UICONTROL Résumé ouvert]** icon ![](assets/open-summary-with-text-nwe.png) dans le [!UICONTROL Envoyé] de la [!UICONTROL Demandes] zone.

   Une fois le résumé ouvert, il reste ouvert lorsque vous cliquez ou sélectionnez d’autres tâches ou problèmes et reste ouvert jusqu’à ce que vous le fermiez manuellement.

   >[!TIP]
   >
   >Vous ne pouvez sélectionner qu’une seule tâche ou un seul problème à la fois pour afficher leurs détails dans la variable [!UICONTROL Résumé] du panneau.

   ![Panneau Résumé](assets/summary-panel-for-task-new-comments.png)

1. (Facultatif) Pour fermer la variable [!UICONTROL Résumé] effectuez l’une des opérations suivantes :

   * Dans une liste de tâches ou de problèmes, cliquez sur le bouton **[!UICONTROL Résumé ouvert]** icon ![](assets/summary-panel-icon.png)

     Ou

     Cliquez sur le bouton **X** dans le coin supérieur droit de la [!UICONTROL Résumé] du panneau.

   * Dans le [!UICONTROL Envoyé] de la [!UICONTROL Demandes] , cliquez sur la zone **[!UICONTROL Fermer le résumé]** icon ![](assets/close-summary-with-text-nwe.png)

     Ou

     Cliquez sur le bouton **X** dans le coin supérieur droit du panneau Résumé.

## [!UICONTROL Pourcentage d&#39;achèvement]

Utilisez la barre de progression en haut de la [!UICONTROL Résumé] pour mettre à jour le pourcentage terminé pour la tâche ou le problème que vous avez sélectionné. Saisissez un nombre ou faites glisser la barre vers le pourcentage approprié.

![Pourcentage terminé dans le panneau Résumé](assets/summary-overview-percent-complete.png)

## [!UICONTROL Mises à jour]

Utilisez la variable [!UICONTROL Mises à jour] de la [!UICONTROL Résumé] pour afficher les mises à jour récentes et effectuer des mises à jour sur la tâche ou le problème que vous avez sélectionné. Cliquez sur **[!UICONTROL Afficher tout]** pour accéder directement au [!UICONTROL Mises à jour] de la tâche.

![Section Mises à jour du panneau Résumé](assets/summary-updates-section.png)

## [!UICONTROL Documents]

Utilisez la variable [!UICONTROL Documents] de la [!UICONTROL Résumé] pour afficher les documents associés à la tâche ou au problème que vous avez sélectionné. Cliquez sur la miniature pour ouvrir un aperçu du document. Pour accéder directement au [!UICONTROL Documents] sur la tâche ou le problème, cliquez sur l’onglet **[!UICONTROL Documents]** titre.

![Section Documents dans le panneau Résumé](assets/summary-documents-section.png)

## [!UICONTROL Détails]

Utilisez la variable [!UICONTROL Détails] de la [!UICONTROL Résumé] pour afficher les détails généraux de l’élément de travail, effectuer des affectations ou ajouter des dates de début. Cliquez sur **[!UICONTROL Afficher tout]** pour accéder directement au [!UICONTROL Détails] sur la tâche ou le problème.

>[!NOTE]
>
>Les champs qui apparaissent dans cette section sont les mêmes que ceux qui apparaissent dans le panneau de droite de l’écran d’accueil. Vous pouvez personnaliser ces champs [Personnaliser [!UICONTROL Accueil] et [!UICONTROL Résumé] utilisation d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

![Section Détails du panneau Résumé](assets/summary-details-section.png)

## [!UICONTROL Sous-tâches]

Cette section n’est disponible que pour les tâches. Utilisez la variable [!UICONTROL Sous-tâches] de la [!UICONTROL Résumé] pour afficher [!UICONTROL Nouveau], [!UICONTROL En cours], et [!UICONTROL Fermé] sous-tâches sur la tâche que vous avez sélectionnée. Cliquez sur le bouton **[!UICONTROL État]** menu déroulant pour basculer entre les états. Pour accéder directement au [!UICONTROL Sous-tâches] sur la tâche, cliquez sur l’onglet **[!UICONTROL Sous-tâches]** Titre &#x200B;.

Si vous n’avez ajouté aucune sous-tâche à la tâche, cliquez sur **[!UICONTROL En ajouter un ici]** pour accéder directement au [!UICONTROL Sous-tâches] de la tâche.

![section Sous-tâches du panneau Résumé](assets/summary-subtasks-section.png)

## [!UICONTROL Heures]

Utilisez la variable [!UICONTROL Heures] de la [!UICONTROL Résumé] pour consigner les heures sur la tâche ou le problème que vous avez sélectionné. Cliquez sur **[!UICONTROL Temps journal]** et saisissez vos heures. Pour accéder directement à l’onglet Heures de la tâche ou du problème, cliquez sur le bouton **[!UICONTROL Heures]** titre.

Le nombre d’heures dans la variable [!UICONTROL Résumé] affiche les heures que vous enregistrez. Les autres utilisateurs auront des totaux d’heure différents dans la variable [!UICONTROL Résumé] selon l’heure à laquelle ils se connectent à la tâche.

S’il n’y a pas de planification [!UICONTROL heures] sur la tâche ou le problème et que vous avez consigné l’heure, la barre d’heures s’affiche en rouge.

![Section Heures dans le panneau Résumé](assets/summary-hours-section.png)

## Approbations

Utilisez la variable [!UICONTROL Approbations] de la [!UICONTROL Résumé] pour afficher les validations associées à la tâche ou au problème sélectionné. Si vous n&#39;avez ajouté aucune validation, sélectionnez une validation existante dans le menu déroulant ou cliquez sur **[!UICONTROL Créer un processus d’approbation à usage unique]** pour accéder directement au [!UICONTROL Approbations] sur la tâche ou le problème.

Pour accéder directement au [!UICONTROL Approbations] sur la tâche ou le problème, cliquez sur l’onglet **[!UICONTROL Approbations]** titre.

![Section Approbations du panneau Résumé](assets/summary-approvals-section.png)
