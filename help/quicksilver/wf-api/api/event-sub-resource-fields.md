---
content-type: api
navigation-topic: api-navigation-topic
title: Champs de ressource d’abonnement à un événement
description: Champs de ressource d’abonnement à un événement
author: Becky
feature: Workfront API
exl-id: 54859930-7619-4b93-8dff-29b10e43d6d5
source-git-commit: 012d53d4773ea8fa377ea7c65cea6cc411ef5321
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 10%

---

# Champs de ressource d’abonnement à un événement

Les champs de ressource d’abonnement à un événement représentent des déclencheurs pour les événements qui entraînent l’envoi d’un message sortant vers un point de terminaison configuré par un abonnement à un événement. Lorsqu’un champ de ressource est modifié, un événement UPDATE est déclenché.

Le tableau suivant répertorie les champs disponibles pour les ressources d’abonnement aux événements :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Ressource</th> 
   <th>objCode</th> 
   <th>Champ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Affectation</td> 
   <td>ASSGN</td> 
   <td>realWorkCompleted</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>realWorkPerDayStartDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> assignmentPercent </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> avgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> classifierID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> customerID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isPrimary</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isTeamAssignment </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> objCode </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> opTaskID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projgAvgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projUserAffectationPercentage </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> securityRootID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>statut</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>TeamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>work</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workPerDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workPerDayList</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workRequired</td> 
  </tr> 
  <tr> 
   <td>Entreprise</td> 
   <td>CMPY</td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> extRefID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> groupID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> objCode </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> parameterValues </td> 
  </tr> 
  <tr> 
  <tr> 
   <td>Tableau de bord</td> 
   <td>PTLTAB</td> 
   <td>ID d’accesseur</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>docID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>lastUpdateDate</p> <p>Remarque : LastUpdateDate ne déclenche un événement que la première fois qu’il est mis à jour au cours de chaque journée. </p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portalProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>Document</td> 
   <td>DOCU</td> 
   <td>ID d’accesseur</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentVersionID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customer:isAdvancedDocMgmtEnabled</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>documentRequestID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupes</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdatedByID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>noteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>referenceNumber</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>releaseVersionID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>DocumentVersion</span> </td> 
   <td><span>DOCV</span> </td> 
   <td><span>ID d’accesseur</span> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>activeProofStages</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentID</span> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>documentProviderID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>docSize</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>entryDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>entryByID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>poste</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalIntegrationType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalStorageID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>fileName</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>fileType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>location</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>objCode</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofApprovalStatusID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofedByUserID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDeadlineDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofName</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofOwnerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofPages</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofProgress</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofStageID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>version</span> </td> 
  </tr> 
  <tr> 
   <td>Frais</td> 
   <td>EXPNS</td> 
   <td> realAmount </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> realUnitAmount </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> billingRecordID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> categoryID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customFormsIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>effectiveDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>expObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>dépenseTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isBillable</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isReemboursable </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isReremboursement </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objectCategories</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledAmount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledUnitAmount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjectName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjID</td> 
  </tr> 
  <tr> 
   <td>Heure</td> 
   <td>HOUR</td> 
   <td>ID d’accesseur</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> realCost </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvedOnDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>dupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>externalTimesheetID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>heures</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hourTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectOverheadID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>statut</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetID</td> 
  </tr> 
  <tr> 
   <td>Problème</td> 
   <td>OPTASK</td> 
   <td>ID d’accesseur</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>kanbanBoardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>priorité</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueTopicID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejetIssueID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveProjectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sourceObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sourceTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>statut</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submitByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>TeamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationID</td> 
  </tr> 
  <tr> 
   <td>Note</td> 
   <td>NOTE</td> 
   <td>ID d’accesseur</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachDocumentID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachWorkID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachWorkUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>auditRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>documentID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>externalServiceID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>noteText</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentEndorsementID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentJournalEntryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>proofActionID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>richTextNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>subject</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>threadID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>PORT</td> 
   <td>ID d’accesseur</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>alignScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td>PRGM</td> 
   <td>ID d’accesseur</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>PROJ</td> 
   <td>ID d’accesseur</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>alignScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachmentRateCardID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertiOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertiOpTaskOriginatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currency</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>deliverableScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
    <tr> 
   <td> </td> 
   <td> </td> 
   <td>issueWorkflowAutomationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
<tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>milestonePathID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>popAccountID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>priorité</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejetIssueID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resourcePoolID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sponsorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>statut</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submitByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskWorkflowAutomationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>TeamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>ProofApproval</span> </td> 
   <td><span>PRFAPL</span> </td> 
   <td><span>ID d’accesseur</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>approverDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>approverID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>customerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentVersionID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>isAwaitDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>objCode</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofCreationDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>requesterID</span> </td> 
  </tr> 
  <tr> 
   <td>Rapport</td> 
   <td>PTLSEC</td> 
   <td>ID d’accesseur</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>appGlobalID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>filterID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastViewedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>preferredID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>publicRunAsUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>reportFolderID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>runAsUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledReportID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>viewID</td> 
  </tr> 
  <tr> 
   <td>Tâche</td> 
   <td>TÂCHE</td> 
   <td>ID d’accesseur</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertiOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertiOpTaskOriginatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>iterationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>kanbanBoardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>milestoneID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>priorité</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recurrenceRuleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejetIssueID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>statut</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submitByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>TeamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationID</td> 
  </tr> 
  <tr> 
   <td>Modèle</td> 
   <td>TMPL</td> 
   <td>ID d’accesseur</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>deliverableScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>issueWorkflowAutomationID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>milestonePathID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>priorité</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portfolioID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceNumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sponsorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskWorkflowAutomationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>TeamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workflowAutomationID</td> 
  </tr> 
  <tr> 
   <td>Feuille de temps</td> 
   <td>TSHET</td> 
   <td>approverID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approversListString</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>displayName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>endDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hasNotes</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hoursDuration</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isEditable</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hoursHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>régulierHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>startDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>statut</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>totalHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td>UTILISATEUR</td> 
   <td>accessLevelID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>categoryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>defaultHourTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>delegationToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>eauthUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>emailAddr</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>homeGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>homeTeamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isActive</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastEnteredNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastLoginDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>latestUpdateNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>layoutTemplateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>logTimeInDays</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>managerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>objCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parameterValues*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portalProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resourcePoolID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>title</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiTemplateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uumUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workHoursPerDay </td> 
  </tr> 
 </tbody> 
</table>

&#42;Une valeur parameterValue est une valeur de champ personnalisée associée à diverses ressources (ou objets) Workfront. Un message sortant d’abonnement à un événement comprend une liste complète de paramètreValues (champs personnalisés) renseignées.
