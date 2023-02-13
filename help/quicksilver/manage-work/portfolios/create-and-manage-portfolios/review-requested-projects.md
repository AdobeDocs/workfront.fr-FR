---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Examen des projets demandés
description: Les demandes de projet s’affichent en tant que projets avec l’état [!UICONTROL Demandé] dans Adobe Workfront. Cet article décrit comment passer en revue les demandes de projet.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: cf3466759a7263c446525b97dd2748ad17d0f7a6
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Examen des projets demandés

Lorsque plusieurs demandes de projet sont soumises à révision, le bureau de gestion de projet ou le comité du portefeuille peut se réunir pour examiner les demandes envoyées et déterminer les approbations des demandes de projet. Les demandes de projet s’affichent en tant que projets avec l’état [!UICONTROL Demandé] in [!DNL Adobe Workfront].

Vous pouvez envoyer une demande de révision de projet en effectuant l’une des opérations suivantes :

* Remplacez l’état du projet par **[!UICONTROL Demandé]**.
* Procédez comme suit : [!UICONTROL Analyse de cas] du projet et soumettez-le à validation.\
   Pour plus d’informations sur l’exécution d’une analyse de cas pour un projet, voir [Création d’une analyse de cas pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Vous pouvez passer en revue les projets demandés dans les domaines suivants de [!DNL Adobe Workfront]:

* Dans un rapport de projet
* Dans un portfolio

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Business] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès à [!UICONTROL View] ou version ultérieure à Portfolio</p> <p>Accès à [!UICONTROL Modifier] dans Projets</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations [!UICONTROL Afficher] ou supérieures sur le portfolio</p> <p>Autorisations [!UICONTROL Gérer] sur les projets pour mettre à jour leur état</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Vérification des projets demandés dans un rapport de projet

Vous pouvez créer un rapport pour les projets afin d’afficher les projets dont l’état est [!UICONTROL Demandé].

Pour plus d’informations sur l’approbation des demandes de projet en créant un rapport de projet, voir [[!UICONTROL Approbation de l’analyse de cas en créant un rapport de projet]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report) dans [Approbation d’une analyse de cas](../../../manage-work/projects/define-a-business-case/approve-business-case.md). 

## Examiner les projets demandés dans un portfolio

1. Accédez au portefeuille dont vous souhaitez consulter les projets demandés.
1. Cliquez sur &#x200B;**[!UICONTROL Projets]** dans le panneau de gauche
1. Dans la **[!UICONTROL Filtrer]** menu déroulant, sélectionnez **[!UICONTROL Demandé]**.

   Uniquement les projets dont l’état est **[!UICONTROL Demandé]** s’affiche dans la liste.

   >[!TIP]
   >
   > En plus de disposer d’un état de **[!UICONTROL Demandé]**, les projets doivent être associés au Portfolio sélectionné à afficher dans cette liste.

1. Cliquez sur le nom d’un projet dans la liste pour l’ouvrir.
1. Cliquez sur **[!UICONTROL Détails du projet]** dans le panneau de gauche.
1. Effectuez l’une des opérations suivantes :

   * Cliquez sur **[!UICONTROL Analyse de cas]**, puis cliquez sur **[!UICONTROL Approuver]** ou **[!UICONTROL Rejeter]** dans le [!UICONTROL Résumé des cas d’affaires] zone à approuver ou rejeter l’analyse de cas.

      ![approve_or_reject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

      Le statut du projet passe à **[!UICONTROL Approuvé]** si l’analyse de cas est approuvée.

      Le statut du projet passe à **[!UICONTROL Rejetés]** si l&#39;affaire Business est rejetée.

      >[!NOTE]
      Aucune notification n’avertit l’utilisateur qui a soumis l’approbation de l’analyse de cas si sa demande de projet a été approuvée ou rejetée. 

      Ou

   * Remplacez l’état du projet par un autre état dans la variable **[!UICONTROL État]** menu déroulant.

      ![](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)
 

 
