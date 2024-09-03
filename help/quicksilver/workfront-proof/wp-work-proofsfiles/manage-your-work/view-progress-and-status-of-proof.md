---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Afficher la progression et le statut d’une épreuve dans  [!DNL Workfront Proof]
description: La progression de la relecture indique le travail effectué sur une épreuve entre le moment où vous envoyez l’épreuve aux personnes réviseuses et le moment où elles prennent une décision sur l’épreuve.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 8fd85595-1403-490e-9d52-2ba5b01457b7
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 100%

---

# Afficher la progression et le statut d’une épreuve dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

## Comprendre la progression de la relecture

La progression de la relecture indique le travail effectué sur une épreuve entre le moment où vous envoyez l’épreuve aux personnes réviseuses et le moment où elles prennent une décision sur l’épreuve.

* [Icônes de progression](#progress-icons)
* [Niveaux de progression de la relecture](#levels-of-proof-progress)

### Icônes de progression {#progress-icons}

Les icônes de progression, S, O, C et D, apparaissent dans la barre de progression pour indiquer la progression de la relecture.

![proof_edit_existing_progress.png](assets/proof-edit-existing-progress-350x78.png)

Elles indiquent les informations suivantes sur une épreuve :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Icône de progression</strong> </p> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt="proof_progress_sent_icon.png"> </p> </td> 
   <td> <p><strong>Envoyée</strong>. L’épreuve a été envoyée aux personnes réviseuses.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-opened-icon.png" alt="proof_progress_opened_icon.png"> </p> <p> </p> </td> 
   <td> <p><strong>Ouverte</strong>. Une personne réviseuse a ouvert la page Détails de l’épreuve ou a ouvert l’épreuve elle-même dans la visionneuse de relecture.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-comment-icon.png" alt="proof_progress_comment_icon.png"> </p> </td> 
   <td> <p><strong>Commentaires</strong>. Les personnes réviseuses (personnes qui peuvent faire des commentaires) ont fait des commentaires sur l’épreuve.</p> <p>Si aucune personne réviseuse n’est désignée pour l’épreuve, cette icône ne s’affiche pas.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt="proof_progress_decision_icon.png"> </p> </td> 
   <td> <p><strong>Décision</strong>. Une personne réviseuses a pris une décision sur l’épreuve.</p> <p>Si aucune personne approbatrice (preneuse de décision) n’est désignée pour l’épreuve, cette icône ne s’affiche pas. </p> </td> 
  </tr> 
 </tbody> 
</table>

Ces icônes peuvent apparaître dans les couleurs suivantes pour indiquer certaines informations sur la progression de l’épreuve :

* **Vert**. Terminée.
* **Blanc**. Non terminée.
* **Orange**. Non terminée et échéance inférieure à 24 heures.
* **Rouge**. Non terminée et échéance dépassée.

### Niveaux de progression de la relecture {#levels-of-proof-progress}

Workfront Proof utilise les icônes de progression pour suivre la progression d’une épreuve à chacun des niveaux suivants :

* Pour chaque personne réviseuse, en fonction de l’activité de cette personne sur l’épreuve.
* Pour chaque étape, en fonction de la progression de la personne réviseuse sur l’étape qui est le plus en retard dans le processus de relecture. Pour plus d’informations, voir [Vue d’ensemble des étapes de workflow automatisé](../../../review-and-approve-work/proofing/proofing-overview/stages.md).
* Pour l’épreuve, en fonction de la progression de l’étape (groupe de personnes réviseuses) qui est le plus en retard dans le processus de relecture.

Pour un exemple de la façon dont [!DNL Workfront Proof] détermine la progression à l’aide de la personne réviseuse ou de l’étape qui est le plus en retard, supposons que trois personnes réviseuses sur une épreuve doivent prendre une décision. Si deux d’entre elles ont pris leur décision mais que la troisième ne l’a pas fait, la barre de progression de l’épreuve n’affiche pas le D en vert en raison de la décision en suspens.

Si le paramètre [!UICONTROL Personne décisionnaire principale] est sélectionné sur une épreuve et que la personne décisionnaire principale envoie une décision, le D dans la barre de progression de l’épreuve devient vert pour toutes les personnes réviseuses, car aucune autre décision n’est requise.

De même, si le paramètre [!UICONTROL Une seule décision requise] est sélectionné sur une épreuve et qu’une personne réviseuse envoie une décision, le D dans la barre de progression de l’épreuve devient vert pour toutes les personnes réviseuses, car aucune autre décision n’est requise.

## Compréhension du statut de l’épreuve

Le statut de l’épreuve affiche le statut des décisions requises pour l’épreuve.

![proof_edit_existing_status.png](assets/proof-edit-existing-status-350x78.png)\
Les options de statut standard sont les suivantes :

* En attente
* Approuvé
* Approuvé avec des modifications
* Modifications requises
* Non pertinent

Si des décisions personnalisées sont configurées dans votre compte, les options de statut reflètent vos paramètres de décision personnalisée.

Le statut de l’épreuve dépend du participant du « pire cas ». Par exemple, supposons qu’il y ait trois décisions sur l’épreuve : deux ont le statut **Acceptée** et la troisième a le statut **Rejetée**. La décision du « pire cas de Rejetée annule les autres décisions et le statut général de l’épreuve est indiqué comme **Rejeté**.

## Affichage de la progression et du statut {#viewing-progress-and-status}

Vous pouvez afficher la progression et le statut des épreuves, des étapes et des réviseurs et réviseuses à chaque étape.

* [Résumé de l’épreuve](#proof-summary)
* [Menu Actions de l’étape](#stage-actions-menu)
* [Dans la section [!UICONTROL Résumé], vous pouvez également accéder aux menus des actions des réviseurs et réviseuses, à condition que vous disposiez des droits de modification sur l’épreuve. Pour plus d’informations, voir Profils d’autorisations d’épreuve dans Workfront Proof et Gérer les rôles d’épreuve dans Workfront Proof. Le menu [!UICONTROL Actions du réviseur ou de la réviseuse] (1) s’affiche lorsque vous pointez sur les détails du réviseur ou de la réviseuse et vous permet d’effectuer les opérations suivantes :](#in-the-summary-section-you-can-also-access-the-reviewer-actions-menus-provided-you-have-edit-rights-on-the-proof-for-more-information-see-proof-permissions-profiles-in-workfront-proof-and-manage-proof-roles-in-workfront-proof-the-reviewer-actions-menu-1-appears-when-you-hover-over-the-reviewer-s-details-and-allows-you-to)
* [Menu des actions de l’épreuve](#proof-actions-menu)

### Résumé de l’épreuve {#proof-summary}

Chaque épreuve du dossier comporte un résumé extensible qui vous permet d’afficher et de modifier rapidement les détails de l’épreuve.

Pour développer ou réduire le résumé :

1. Cliquez sur la flèche située à gauche de l’épreuve en mode Tableau de bord ou Liste.

![Summary_expandable.png](assets/summary-expandable-350x68.png)

Le résumé comprend les éléments suivants :

* Workflow (2)
* Version (3)
* Dossier (4)
* État (5)\
   ![summary_2.png](assets/summary-2-350x160.png)

Dans le résumé, vous pouvez afficher et modifier les détails suivants de votre épreuve :

* Progression de la relecture (1)
* Progression de chaque étape (2)
* Date d’échéance définie pour l’étape (3)
* Détails du réviseur ou de la réviseuse :

   * Nombre de commentaires et de réponses de chaque réviseur et réviseuse (4)
   * Progression de chaque réviseur et réviseuse (5)
   * Décision (si une décision a inclus des signatures électroniques, une icône indiquant cette information s’affiche en regard de la décision.) (6)
   * Rôle sur l’épreuve (7)
   * Paramètres des alertes par e-mail (8)

>[!NOTE]
>
>Votre capacité à modifier les détails de l’épreuve dépend de vos droits sur l’épreuve (voir [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) et [Gérer les rôles d’épreuve dans [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![summary_details_3.png](assets/summary-details-3-350x160.png)

### Menu [!UICONTROL Actions de l’étape]  {#stage-actions-menu}

Chaque étape de votre workflow comporte un menu distinct, qui vous permet d’effectuer des actions en masse liées aux réviseurs et réviseuses de cette étape.

Le menu [!UICONTROL Actions de l’étape] s’affiche lorsque vous pointez sur la section Étape (1) et vous permet de

* [!UICONTROL Envoyer un message à tous] (2)
* [!UICONTROL Partager] (3)
* [!UICONTROL Supprimer l’étape] (4)

>[!NOTE]
>
>La disponibilité de ces options dépend de vos droits sur l’épreuve (voir [Profils d’autorisations d’épreuve de dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) et [Gérer les rôles d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![Stage_actions_menu.png](assets/stage-actions-menu-350x161.png)

Dans la section Résumé, vous pouvez également accéder aux menus des actions des personnes en charge de la révision à condition que vous disposiez des droits de modification sur l’épreuve. Pour plus d’informations, voir [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) et [Gérer des rôles d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md). Le menu Actions du réviseur ou de la réviseuse (1) s’affiche lorsque vous passez la souris sur les détails du réviseur ou de la réviseuse et vous permet d’effectuer les opérations suivantes :

* Envoyer un message à la personne en charge de la révision (2)
* Modifier les détails de la personne en charge de la révision (3) : permet de modifier le nom d’affichage, le rôle dans l’épreuve et l’alerte par e-mail de cette personne.
* En faire la personne propriétaire de l’épreuve (4)
* En faire la principale personne décisionnaire (5)
* Retirer de l’épreuve (6)

>[!NOTE]
>
>La visibilité de ces options dépend de vos droits sur l’épreuve (voir [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) et [Gérer des rôles d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![Reviewer_actions_menu.png](assets/reviewer-actions-menu-350x135.png)

### Menu des actions de l’épreuve {#proof-actions-menu}

Chaque épreuve dispose également d’un menu (1) qui vous permet d’effectuer les actions suivantes :

* Vous pouvez accéder à la page Détails de l’épreuve (2)
* Partager l’épreuve avec d&#39;autres personnes (3)
* Envoyer un message aux personnes en charge de la révision (4)
* Créer une nouvelle version de l’épreuve (5)
* Copier l’épreuve (6)
* Télécharger le fichier d’origine (7)
* Partager les liens de l’épreuve (8)
* Imprimer les commentaires (9)
* Demander un résumé Excel de l’épreuve (10)
* Verrouiller l’épreuve (11)
* Supprimer l’épreuve (12)

![Proof_actions_menu__1_.png](assets/proof-actions-menu--1--350x158.png)

>[!NOTE]
>
>La disponibilité de ces options dépend de vos droits sur l’épreuve (voir [Profils d’autorisations d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) et [Gérer des rôles d’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

Pour plus d’informations sur l’affichage de la progression et du statut de l’épreuve dans [!DNL Workfront], voir [Voir la progression et le statut](#viewing-progress-and-status).

Pour plus d’informations sur l’affichage de la progression et du statut dans la visionneuse de relecture de l’application de bureau, voir [Vérifier un workflow dans la visionneuse de relecture](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-workflow.md).
