---
product-area: documents
navigation-topic: approvals
title: Demande d’approbation de documents
description: Vous pouvez demander l’approbation d’un document dans Adobe Workfront à des gestionnaires ou à d’autres utilisateurs. Vous pouvez également demander l’approbation de documents à des personnes n’ayant pas de compte Workfront si votre administrateur Workfront a activé cette fonctionnalité, comme décrit dans Configuration des préférences de sécurité du système.
author: Courtney
feature: Work Management
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Demande d’approbation de documents

Vous pouvez demander l’approbation d’un document dans Adobe Workfront à des gestionnaires ou à d’autres utilisateurs. Vous pouvez également demander l’approbation de documents à des personnes sans compte Workfront si votre administrateur Workfront a activé cette fonctionnalité, comme décrit dans la section [Configuration des préférences de sécurité système](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage ou accès supérieur à Projets, Tâches, Problèmes, Modèles, Portfolios, Programmes, Rapports, Tableaux de bord et Calendriers, Documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Consulter l’objet associé à l’accès ou à l’approbation de la demande ou un accès supérieur à cet objet </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Demande d’approbation de document

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Recherchez le document dont vous avez besoin.

1. Faites défiler l’écran vers le bas jusqu’à **Approbations** dans le résumé, puis commencez à saisir le texte **Ajouter un approbateur** zone de texte. Vous pouvez ajouter des utilisateurs Workfront par nom ou des utilisateurs externes par courrier électronique.

1. Si votre administrateur Adobe Workfront a activé la possibilité de collaborer avec des personnes qui n’utilisent pas Workfront, comme décrit à la section [Configuration des préférences de sécurité système](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), vous pouvez saisir leurs adresses électroniques pour les inclure.

   Vous ne pouvez pas demander l’approbation d’équipes ou de groupes.

1. Répétez l’étape précédente pour ajouter d’autres approbateurs.

## Réenvoyer une validation sur une nouvelle version

Les décisions d’approbation de document ne sont pas automatiquement réinitialisées lorsque vous chargez une nouvelle version. Par exemple, si votre document est approuvé avec des modifications, la décision indique &quot;modifications&quot; comme décision, même si vous téléchargez une nouvelle version avec les modifications spécifiées. Vous pouvez annuler la décision sur une nouvelle version si vous soumettez manuellement à nouveau la validation.

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Recherchez le document dont vous avez besoin.

1. Faites défiler l’écran vers le bas jusqu’à **Approbations** dans la section Résumé, cliquez sur l’icône Plus, puis sur Resubmit.

   ![](assets/nwe-resubmit-approval-350x149.png)

## Suppression d’une demande d’approbation de document

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Recherchez le document dont vous avez besoin.

1. Faites défiler l’écran vers le bas jusqu’à **Approbations** dans le résumé, puis cliquez sur le bouton **Plus** en ligne avec le nom de l’approbateur et sélectionnez **Supprimer**.

   La demande de validation est supprimée et l’approbateur reçoit une notification indiquant que sa validation n’est plus nécessaire. Leur accès au partage lié à l’approbation est également supprimé.

## Envoyer un rappel à un approbateur

Vous pouvez envoyer un message pour rappeler à un approbateur que vous attendez ses commentaires.

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Recherchez le document dont vous avez besoin.

1. Faites défiler l’écran vers le bas jusqu’à **Approbations** dans le résumé, puis cliquez sur le bouton **Plus** en ligne avec le nom de l’approbateur et sélectionnez **Rappel**.

   L&#39;approbateur reçoit une notification l&#39;informant que la validation est toujours en attente. Si cela est activé, il peut également recevoir un rappel par courrier électronique.
