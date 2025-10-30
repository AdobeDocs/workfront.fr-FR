---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Réviser des projets demandés
description: Les demandes de projet s’affichent en tant que projets avec le statut [!UICONTROL Demandé] dans Adobe Workfront. Cet article décrit comment examiner les demandes de projet.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: 7fef704355fad677f2bdf40e630ea0146a9e1d58
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 78%

---

# Réviser des projets demandés

<!--Audited: 10/2025-->

Lorsque plusieurs demandes de projet sont soumises pour examen, le bureau de gestion de projets ou le comité du portfolio peut se réunir pour examiner les demandes envoyées et décider des approbations des demandes de projet. Les demandes de projet s’affichent en tant que projets avec le statut [!UICONTROL Demandé] dans [!DNL Adobe Workfront].

Vous pouvez envoyer une demande d’examen de projet en effectuant l’une des opérations suivantes :

* Changer le statut du projet sur **[!UICONTROL Demandé]**.
* Effectuer le [!UICONTROL Business case] du projet et le soumettre pour approbation.\
   Pour plus d’informations sur l’exécution du business case d’un projet, voir [Créer le business case d’un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Vous pouvez examiner les projets demandés dans les zones suivantes d’[!DNL Adobe Workfront] :

* Dans un rapport de projet
* Dans un portfolio

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquet</td> 
   <td><p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>[!UICONTROL Standard] </p> 
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en [!UICONTROL View] ou de niveau supérieur aux portfolios</p> <p>[!UICONTROL Edit] l’accès aux Projets</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de [!UICONTROL View] ou de niveau supérieur sur le portfolio</p> <p>Autorisations de [!UICONTROL Manage] sur les projets pour mettre à jour leur statut</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] access or higher to Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] permissions or higher on the portfolio</p> <p>[!UICONTROL Manage] permissions on the projects to update their status</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Examiner les projets demandés dans un rapport de projet

Vous pouvez créer un rapport de projets afin d’afficher les projets dont le statut est [!UICONTROL Demandé].

Pour plus d’informations sur l’approbation des demandes de projet par la création d’un rapport de projet, consultez la section [[!UICONTROL Approuver l’analyse de rentabilité par la création d’un rapport de projet]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report) dans [Approuver une analyse de rentabilité](../../../manage-work/projects/define-a-business-case/approve-business-case.md).

## Vérifier les projets demandés dans un portfolio

1. Accédez au portfolio dont vous souhaitez vérifier les projets demandés.
1. Cliquez sur **[!UICONTROL Projets]** dans le panneau de gauche
1. Dans le menu déroulant **[!UICONTROL Filtre]**, sélectionnez **[!UICONTROL Demandé]**.

   Seuls les projets dont le statut est **[!UICONTROL Demandé]** s’affichent dans la liste.

   >[!TIP]
   >
   > En plus d’avoir le statut **[!UICONTROL Demandé]**, les projets doivent être associés au Portfolio sélectionné pour s’afficher dans cette liste.

1. Cliquez sur le nom d’un projet dans la liste pour l’ouvrir.
1. Cliquez sur **[!UICONTROL Détails du projet]** dans le panneau de gauche.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur **[!UICONTROL Analyse de rentabilité]**, puis sur **[!UICONTROL Approuver]** ou **[!UICONTROL Rejeter]** dans la zone [!UICONTROL Résumé de l&#39;analyse de rentabilité] pour approuver ou rejeter l&#39;analyse de rentabilité.

     ![approve_or_reject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

     Le statut du projet passe à **[!UICONTROL Approuvé]** si le business case est approuvé.

     Le statut du projet passe à **[!UICONTROL Rejeté]** si le business case est rejeté.

     >[!NOTE]
     >
     >L’utilisateur ou utilisatrice qui a soumis l’approbation du business case ne reçoit aucune notification si sa demande de projet a été approuvée ou rejetée.

     Ou

   * Remplacez le statut du projet par un autre statut dans le menu déroulant **[!UICONTROL Statut]**.

     ![Modifier le statut du projet dans la liste déroulante](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)



