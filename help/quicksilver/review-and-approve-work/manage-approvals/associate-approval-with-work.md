---
product-area: projects
navigation-topic: approvals
title: Associer un processus d’approbation nouveau ou existant au travail
description: Cet article décrit comment associer les processus d’approbation aux tâches. Pour plus d’informations sur l’association d’approbations avec des BAT ou des documents, consultez les articles suivants.
author: Courtney and Alina
feature: Work Management
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: 7dbb9ca9b26f17710a7897e98dca109b5c886bd7
workflow-type: tm+mt
source-wordcount: '1869'
ht-degree: 0%

---

# Associer un processus d’approbation nouveau ou existant au travail

Cet article décrit comment associer les processus d’approbation aux tâches. Pour plus d’informations sur l’association d’approbations avec des BAT ou des documents, consultez les articles suivants :

* [Créer un BAT avancé avec un workflow automatisé](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Demande d’approbation de documents](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

Vous pouvez associer un processus d’approbation global ou à usage unique à un élément de travail dans Adobe Workfront. Les scénarios suivants existent :

* Associez un processus d’approbation globale existant à un projet, une tâche, un problème, un modèle ou une tâche de modèle. Certains processus d’approbation globale sont disponibles pour tous les groupes du système. Les processus d’approbation globale au niveau du groupe ne sont disponibles que pour certains groupes.
* Créez un processus d’approbation à usage unique et associez-le à une tâche, à une tâche, à un problème, à un modèle ou à une tâche de modèle existante.

>[!NOTE]
>
>Cet article utilise le terme &quot;processus d’approbation globale&quot; pour différencier le terme &quot;processus d’approbation à usage unique&quot;. Un processus d’approbation globale peut être utilisé à plusieurs reprises.
>
>Le terme &quot;processus d’approbation globale au niveau du groupe&quot; fait référence à un processus d’approbation qui peut être utilisé à plusieurs reprises pour des éléments et dont les états sont associés uniquement à un groupe spécifique.

Pour plus d’informations sur les processus de validation, voir [Présentation du processus de validation](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Pour plus d’informations sur la création d’un processus d’approbation globale, voir [Créer un processus d’approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Modifier l’accès ou une version ultérieure à Projets, tâches, problèmes ou modèles</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations pour le projet, la tâche, le problème ou le modèle</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Considérations relatives à l’association de processus d’approbation à des tâches

Outre les considérations décrites ci-dessous, nous vous recommandons de revoir les considérations générales concernant les processus d’approbation dans Workfront. Pour plus d’informations, voir [Présentation du processus de validation](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* Vous devez créer la tâche de projet, de tâche, de publication, de modèle ou de modèle avant que le processus de validation puisse y être associé.
* Lorsque vous joignez un processus d’approbation à un élément pour un état qui a été transmis et dans lequel l’élément est actuellement, le processus d’approbation ne sera pas déclenché et aucune notification n’est envoyée aux approbateurs.

   **Exemple :** Si une tâche est dans l’état Terminé et que vous joignez un processus de validation associé à l’état Terminé, la validation ne se déclenche pas.

* Lorsque vous attachez un processus d’approbation au premier état d’un élément (en utilisant un modèle pour les tâches et les projets, en utilisant les paramètres Configuration de la file d’attente pour les problèmes ou en définissant les Paramètres de tâche d’un projet pour les nouvelles tâches), les processus d’approbation sont ignorés si la validation envoyée est rappelée. Dans ce cas, les approbateurs ne reçoivent aucune notification.

   Pour plus d’informations sur le rappel des validations, voir [Afficher les approbations](../../review-and-approve-work/manage-approvals/view-approvals.md).

   >[!TIP]
   >
   >Le premier état d’une tâche ou d’un problème est Nouveau. Le premier état d’un projet est l’état sélectionné par votre administrateur Workfront dans les préférences du projet de votre système. Pour plus d’informations, voir [Configuration des préférences de projet à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* L’association des processus d’approbation à un objet n’est pas enregistrée dans la zone Mises à jour de l’objet.
* Vous ne pouvez pas associer un processus de validation à une tâche parente.
* L’ajout d’un utilisateur, d’une équipe ou d’un rôle en tant qu’approbateur ne leur accorde pas automatiquement des autorisations sur l’objet associé à cette approbation. Ils reçoivent des autorisations sur l’objet lorsque l’étape d’approbation est déclenchée. Dans le cas contraire, les objets doivent être partagés avec eux avant de pouvoir prendre une décision concernant la validation.

Les sections suivantes décrivent les différentes méthodes d’association d’un processus d’approbation à un projet, à une tâche ou à un problème.

## Associer un processus d’approbation globale à un élément de travail {#associate-a-global-approval-process-with-a-work-item}

Vous pouvez associer un processus d’approbation globale à un élément de travail (projet, tâche, problème, modèle, tâche de modèle).

Le processus d’approbation globale doit être disponible pour le groupe associé à l’élément de travail ou pour tous les groupes du système.

>[!NOTE]
Vous pouvez associer des processus d’approbation de projet à un modèle et des processus d’approbation de tâche à une tâche de modèle. Ensuite, lorsqu’une personne utilise le modèle pour créer un projet, le processus d’approbation devient un processus d’approbation de projet ou de tâche, respectivement. Un processus de validation à usage unique associé à une tâche de modèle ou de modèle reste un processus de validation à usage unique pour les projets et les tâches.

Pour plus d’informations sur la façon dont les administrateurs de Workfront peuvent configurer un processus d’approbation globale pour tous les groupes du système et sur la manière dont les administrateurs de groupe peuvent créer des approbations pour un groupe, voir [Créer un processus d’approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
Vous pouvez également modifier un processus global d’approbation pour répondre à vos besoins spécifiques. Pour plus d’informations, voir la section [Modification d’un processus d’approbation global en vue d’une utilisation sur un objet spécifique](#modify-a-global-approval-process-for-use-on-a-specific-object) dans cet article.

Pour associer un processus d’approbation globale existant à un projet, une tâche, un problème, un modèle ou une tâche de modèle :

1. Accédez à l’élément de travail auquel vous souhaitez associer un processus d’approbation.
1. Cliquez sur **Approbations** dans le panneau de gauche.

   Vous devrez peut-être cliquer sur **Afficher plus**, puis cliquez sur **Approbations**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   Le processus de validation sélectionné s’affiche.

1. Développez l’objet **Utiliser existant** et sélectionnez un processus de validation existant.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   Le processus de validation sélectionné s’affiche.

   ![](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. Cliquer sur **Enregistrer**.
1. (Facultatif) Cliquez sur Modifier le processus d’approbation si vous souhaitez modifier la validation existante que vous avez jointe à l’élément. Le processus global d’approbation est ainsi transformé en processus d’approbation à usage unique. Pour plus d’informations, voir la section [Modification d’un processus d’approbation global en vue d’une utilisation sur un objet spécifique](#modify-a-global-approval-process-for-use-on-a-specific-object) dans cet article.

## Modification d’un processus d’approbation global en vue d’une utilisation sur un objet spécifique {#modify-a-global-approval-process-for-use-on-a-specific-object}

L’administrateur ou l’administrateur de groupe Workfront crée des processus d’approbation globaux que vous pouvez utiliser, comme décrit dans la section [Créer un processus d’approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

La modification d’un processus d’approbation globale associé à un élément est identique à la modification d’un processus d’approbation à usage unique.

Vous pouvez modifier un processus d’approbation globale en fonction des besoins spécifiques du projet, de la tâche ou du problème que vous associez à celui-ci.

>[!IMPORTANT]
Lorsque vous modifiez un processus d’approbation globale, il devient un processus d’approbation à usage unique qui ne peut être utilisé que sur l’objet sur lequel vous l’avez modifié. Le processus d&#39;approbation globale reste inchangé.
Tenez compte des restrictions suivantes lors de la modification d’un processus d’approbation globale :
* Le processus d’approbation n’est modifié que pour le projet, la tâche ou le problème auquel vous associez le processus d’approbation.
* Les modifications futures apportées par un administrateur au processus d’approbation globale d’origine ne reflètent pas le processus d’approbation globale que vous avez modifié.
>


Pour modifier un processus de validation déjà associé à un élément :

1. Ajoutez un processus d’approbation globale au projet, à la tâche ou au problème.

   Pour obtenir des instructions, reportez-vous à la section [Associer un processus d’approbation globale à un élément de travail](#associate-a-global-approval-process-with-a-work-item) dans cet article.

   >[!IMPORTANT]
   Assurez-vous de cliquer sur **Enregistrer** lors de l&#39;ajout de la validation.

1. Une fois le processus d’approbation globale ajouté, cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png) dans le coin supérieur droit de la page d’approbation. Cette action transforme le processus d’approbation global ou au niveau du groupe en un processus d’approbation à usage unique.
1. Apportez toute modification au processus d’approbation existant. Pour plus d’informations, voir la section [Associer un processus d’approbation à usage unique à une tâche de projet, de tâche, de problème, de modèle ou de modèle](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) dans cet article.
1. Cliquez sur **Enregistrer**, puis cliquez sur **Enregistrer** pour confirmer que vous souhaitez convertir le processus d’approbation globale en processus d’approbation à usage unique disponible uniquement sur cet objet.

## Associer un processus d’approbation à usage unique à une tâche de projet, de tâche, de problème, de modèle ou de modèle {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

Vous pouvez créer un processus d’approbation à usage unique à utiliser uniquement sur un projet, une tâche ou un problème spécifique.

Vous pouvez également associer un processus de validation à usage unique à une tâche de modèle ou de modèle afin qu’elle soit disponible sur les projets et tâches créés à partir du modèle.

>[!NOTE]
Vous pouvez associer un processus d’approbation à usage unique à n’importe quel état au niveau du système ou du groupe pour une tâche de projet, de tâche, de problème, de modèle ou de modèle. Pour plus d’informations sur les états Workfront, voir [Création ou modification d’un état](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

La création d&#39;un processus d&#39;approbation permet ainsi de créer un processus d&#39;approbation personnalisé en fonction de vos besoins. Cependant, le processus d’approbation ne peut plus être associé à d’autres tâches à l’avenir.

Vous pouvez également modifier un processus d’approbation global pour un élément spécifique et qui devient également un processus d’approbation à usage unique. Pour plus d’informations, voir la section [Modification d’un processus d’approbation global en vue d’une utilisation sur un objet spécifique](#modify-a-global-approval-process-for-use-on-a-specific-object) dans cet article.

Pour créer un processus de validation à usage unique :

1. Accédez à la tâche de projet, de tâche, de problème, de modèle ou de modèle à laquelle vous souhaitez associer un processus de validation.
1. Cliquez sur **Approbations** dans le panneau de gauche.

   Vous devrez peut-être cliquer sur **Afficher plus** > **Approbations**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Cliquez sur **Créer une utilisation unique**.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. Suivez les étapes commençant par l’étape 6 de la section &quot;Création d’un processus d’approbation globale au niveau du système ou du groupe pour les tâches&quot; de l’article. [Créer un processus d’approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   Une fois que vous avez joint le processus de validation à usage unique, il s’affiche sous la forme &quot;`<Custom>`&quot; dans le champ Processus de validation de la boîte d’édition des modèles et des tâches de modèle. Pour plus d’informations sur la modification de modèles ou de tâches de modèle, reportez-vous aux articles suivants :
   * [Modifier des modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   * [Modifier une tâche de modèle](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)


   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## Supprimer ou supprimer un processus d’approbation d’un élément de travail

Vous pouvez supprimer un processus d’approbation global ou au niveau du groupe ou supprimer un processus d’approbation à usage unique d’un projet, d’une tâche ou d’un problème qui lui était précédemment associé.

Les scénarios suivants existent : 

* La suppression du processus d’approbation global ou au niveau du groupe ne supprime pas l’approbation. La validation reste disponible pour une utilisation ultérieure.
* La suppression d’un processus d’approbation d’utilisateur unique le supprime de Workfront et il ne peut pas être récupéré.

Pour supprimer ou supprimer un processus d’approbation d’un élément de travail :

1. Accédez à la tâche de projet, de tâche, de problème, de modèle ou de modèle dans laquelle vous souhaitez supprimer un processus de validation que vous avez précédemment ajouté.
1. Cliquez sur **Approbations** dans le panneau de gauche.

   Vous devrez peut-être cliquer sur **Afficher plus** > **Approbations**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Cliquez sur l’une des icônes suivantes dans le coin supérieur droit de la section Validations , selon le type de validation associé à l’élément :

   * **La suppression** icon ![](assets/remove-icon---x-in-circle.png) pour les approbations globales ou de niveau groupe.
   * **La suppression** icon ![](assets/delete.png) pour les validations à usage unique.

1. Cliquez sur **Supprimer** ou **Supprimer** pour confirmer.

   Le processus d’approbation est supprimé de l’élément de travail.

## Associer automatiquement un processus d’approbation aux tâches

Vous pouvez associer automatiquement un processus de validation à des tâches à l’aide des workflows suivants :

* Pour les projets et les tâches, vous pouvez associer un processus de validation à un modèle. Vous pouvez joindre un processus d’approbation existant à l’onglet Validations de modèle ou l’onglet Approbations de tâches de modèle . Pour plus d’informations sur l’association d’une validation existante à un élément de travail, voir [Associer un processus d’approbation globale à un élément de travail](#associate-a-global-approval-process-with-a-work-item) dans cet article.
* Pour les nouvelles tâches sur un projet existant, vous pouvez associer un processus d’approbation globale ou un processus d’approbation globale au niveau du groupe dans la zone Paramètres de tâche de la zone Modifier le projet . Pour plus d’informations, reportez-vous à la section &quot;Paramètres de tâche&quot; de l’article. [Modification de projets](../../manage-work/projects/manage-projects/edit-projects.md).
* Pour les problèmes, vous pouvez associer une approbation à chaque nouveau problème ajouté à un projet en associant un processus d’approbation existant à une file d’attente de demandes. Pour plus d’informations sur la configuration des files d’attente de requête, voir [Création d’une file d’attente de requête](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
