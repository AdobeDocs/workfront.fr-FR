---
product-area: documents
navigation-topic: approvals
title: Demander l’approbation de documents
description: Vous pouvez demander l’approbation d’un document à des responsables ou à d’autres utilisateurs et utilisatrices dans Adobe Workfront. Vous pouvez également demander l’approbation de documents à des personnes qui n’ont pas de compte Workfront si votre équipe d’administration Workfront a activé cette fonctionnalité, comme décrit dans la section Configurer les préférences de sécurité du système.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 2503b6e628e4860a5652c620d8e4d0eea2414443
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 98%

---

# Demander l’approbation de documents

Vous pouvez demander l’approbation d’un document à des responsables ou à d’autres utilisateurs et utilisatrices dans Adobe Workfront. Vous pouvez également demander l’approbation de documents à des personnes qui n’ont pas de compte Workfront si votre équipe d’administration Workfront a activé cette fonctionnalité, comme décrit dans la section [Configurer les préférences de sécurité du système](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Contribuer ou plus</p>
   <p>Révision ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Affichage ou accès supérieur pour Projets, Tâches, Problèmes, Modèles, Portfolios, Programmes, Rapports, Tableaux de bord, Calendriers et Documents</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer l’accès à l’objet associé à la demande d’accès ou d’approbation </p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Demander l’approbation d’un document

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Recherchez le document dont vous avez besoin.

1. Faites défiler la page jusqu’à la section **Approbations** dans le résumé et commencez à taper dans la zone de texte **Ajouter un approbateur ou une approbatrice**. Vous pouvez ajouter des utilisateurs ou utilisatrices Workfront par leur nom ou des personnes externes par leur adresse e-mail.

1. Si votre équipe d’administration Adobe Workfront a activé la possibilité de collaborer avec des personnes qui n’utilisent pas Workfront, comme décrit dans la section [Configurer les préférences de sécurité du système](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), vous pouvez saisir leurs adresses e-mail pour les inclure.

   Vous ne pouvez pas demander l’approbation d’équipes ou de groupes.

1. Répétez l’étape précédente pour ajouter d’autres approbateurs et approbatrices.

## Soumettre à nouveau une approbation sur une nouvelle version

Les décisions d’approbation des documents ne sont pas automatiquement réinitialisées lorsque vous chargez une nouvelle version. Par exemple, si votre document est approuvé avec des modifications, la décision indique « modifications », même si vous chargez une nouvelle version avec les modifications spécifiées. Vous pouvez annuler la décision sur une nouvelle version si vous soumettez à nouveau l’approbation manuellement.

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Recherchez le document dont vous avez besoin.

1. Faites défiler la page jusqu’à la section **Approbations** dans le résumé, cliquez sur l’icône Plus, puis sur Soumettre à nouveau.

   ![Envoyer à nouveau la validation](assets/nwe-resubmit-approval-350x149.png)

## Supprimer une demande d’approbation de document

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Recherchez le document dont vous avez besoin.

1. Faites défiler la page jusqu’à la section **Approbations** dans le résumé, puis cliquez sur le menu **Plus** en ligne avec le nom de l’approbateur ou l’approbatrice et sélectionnez **Supprimer**.

   La demande d’approbation est supprimée et l’approbateur ou l’approbatrice reçoit une notification indiquant que son approbation n’est plus nécessaire. L’accès au partage lié à l’approbation est également supprimé.

## Envoyer un rappel à un approbateur ou à une approbatrice

Vous pouvez envoyer un message pour rappeler à un approbateur ou une approbatrice que vous attendez son feedback sur un document.

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Recherchez le document dont vous avez besoin.

1. Faites défiler la page jusqu’à la section **Approbations** dans le résumé, puis cliquez sur le menu **Plus** en ligne avec le nom de l’approbateur ou l’approbatrice et sélectionnez **Rappeler**.

   L’approbateur ou l’approbatrice reçoit une notification l’informant que l’approbation est toujours en attente. Cette personne peut également recevoir un rappel par e-mail si cette option est activée.
