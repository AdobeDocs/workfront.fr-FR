---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Réviser des projets demandés
description: Les demandes de projet s’affichent en tant que projets dont l’état est [!UICONTROL Demandé] dans Adobe Workfront. Cet article décrit comment passer en revue les demandes de projet.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: cf3466759a7263c446525b97dd2748ad17d0f7a6
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 17%

---

# Réviser des projets demandés

Lorsque plusieurs demandes de projet sont soumises à révision, le bureau de gestion de projet ou le comité du portefeuille peut se réunir pour examiner les demandes envoyées et déterminer les approbations des demandes de projet. Les demandes de projet s’affichent en tant que projets dont l’état est [!UICONTROL Demandé] dans [!DNL Adobe Workfront].

Vous pouvez envoyer une demande de révision de projet en effectuant l’une des opérations suivantes :

* Remplacez l’état du projet par **[!UICONTROL Requested]**.
* Exécutez le [!UICONTROL Business Case] du projet et envoyez-le pour approbation.\
   Pour plus d’informations sur l’exécution d’une analyse de cas pour un projet, voir [Création d’une analyse de cas pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Vous pouvez passer en revue les projets demandés dans les zones suivantes de [!DNL Adobe Workfront] :

* Dans un rapport de projet
* Dans un portfolio

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!UICONTROL Business] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès à [!UICONTROL View] ou version ultérieure à Portfolio</p> <p>Accès à [!UICONTROL Modifier] dans Projets</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la manière dont l’équipe d’administration [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations [!UICONTROL Afficher] ou supérieures sur le portfolio</p> <p>Autorisations [!UICONTROL Gérer] sur les projets pour mettre à jour leur état</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Vérification des projets demandés dans un rapport de projet

Vous pouvez créer un rapport pour les projets afin de déterminer les projets dont l’état est [!UICONTROL Demandé].

Pour plus d’informations sur l’approbation des demandes de projet en créant un rapport de projet, reportez-vous à la section [[!UICONTROL Approbation de l’analyse de cas par création d’un rapport de projet]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report) dans [Approuver une analyse de cas](../../../manage-work/projects/define-a-business-case/approve-business-case.md). 

## Examiner les projets demandés dans un portfolio

1. Accédez au portefeuille dont vous souhaitez consulter les projets demandés.
1. Cliquez sur &#x200B;**[!UICONTROL Projets]** dans le panneau de gauche.
1. Dans le menu déroulant **[!UICONTROL Filter]**, sélectionnez **[!UICONTROL Requested]**.

   Seuls les projets dont l’état est **[!UICONTROL Requested]** s’affichent dans la liste.

   >[!TIP]
   >
   > Outre le statut **[!UICONTROL Demandé]**, les projets doivent être associés au Portfolio sélectionné à afficher dans cette liste.

1. Cliquez sur le nom d’un projet dans la liste pour l’ouvrir.
1. Cliquez sur **[!UICONTROL Détails du projet]** dans le panneau de gauche.
1. Effectuez l’une des opérations suivantes :

   * Cliquez sur **[!UICONTROL Business Case]**, puis sur **[!UICONTROL Approve]** ou **[!UICONTROL Reject]** dans la zone [!UICONTROL Business Case Summary] pour approuver ou rejeter l’analyse de cas.

     ![approve_or_reject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

     Le statut du projet passe à **[!UICONTROL Approuvé]** si l’analyse de cas est approuvée.

     L’état du projet est remplacé par **[!UICONTROL Rejected]** si le dossier Business est rejeté.

     >[!NOTE]
     >
     >Aucune notification n’avertit l’utilisateur qui a soumis l’approbation de l’analyse de cas si sa demande de projet a été approuvée ou rejetée. 

     Ou

   * Remplacez l’état du projet par tout autre état dans le menu déroulant **[!UICONTROL Status]** .

     ![](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)
 

 
