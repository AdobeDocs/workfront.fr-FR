---
content-type: overview
product-area: projects
navigation-topic: approvals
title: Présentation du processus de validation
description: Vous pouvez créer un processus d’approbation et le joindre à un objet pour vous assurer que les utilisateurs désignés révisent certaines modifications avant la progression de l’objet.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# Présentation du processus de validation

Vous pouvez créer un processus d’approbation et le joindre à un objet pour vous assurer que les utilisateurs désignés révisent certaines modifications avant la progression de l’objet.

Cette option est disponible pour les types d’objets suivants dans Adobe Workfront :

* Élément de travail (projet, tâche ou problème, modèle, tâche de modèle)
* Document
*  Épreuve

Pour plus d’informations sur la création d’un processus de validation, voir [Créer un processus d’approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Cet article contient des informations générales sur les processus d’approbation associés aux tâches.

## Types de processus de validation

Si vous êtes administrateur d’Adobe Workfront ou utilisateur disposant d’un accès administratif aux processus de validation, vous pouvez créer les processus d’approbation suivants pour les projets, tâches et problèmes :

* **Processus d’approbation globale au niveau du système**: les utilisateurs peuvent les joindre à l’une des fonctions suivantes :

   * Un projet, une tâche ou un problème dans la section Validations
   * Dans la zone Modifier le projet, la zone Processus d’approbation par défaut de la tâche
   * Dans la section Détails de la file d’attente ou Rubrique de la file d’attente d’un projet, dans les zones Processus d’approbation par défaut. Le projet doit être activé en tant que file d’attente de demandes.

* **Processus d’approbation globale au niveau du groupe**: les utilisateurs peuvent les joindre à ce qui suit :

   * Un projet, une tâche ou un problème appartenant au groupe associé au processus d’approbation dans la section Validations
   * Dans la zone Modifier le projet, la zone Processus d’approbation par défaut de la tâche d’un projet appartenant au groupe associé au processus d’approbation
   * Dans la section Détails de la file d’attente ou Rubrique de la file d’attente d’un projet, dans les zones Processus d’approbation par défaut. Le projet doit être activé en tant que file d’attente des demandes et doit appartenir au groupe associé au processus d’approbation.

  Pour plus d’informations sur la création d’un processus d’approbation au niveau du système ou du groupe, voir [Créer un processus d’approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **Processus d’approbation à usage unique**: à utiliser avec un seul projet, tâche, problème, modèle ou tâche de modèle. Ce type de processus de validation affecte uniquement l&#39;objet qui lui est associé et ne peut être associé à aucun autre objet.

  Pour plus d’informations sur la création d’un processus de validation à usage unique, voir [Associer un processus d’approbation nouveau ou existant au travail](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Cet article utilise le terme &quot;processus d’approbation globale&quot; pour différencier le terme &quot;processus d’approbation à usage unique&quot;. Un processus d’approbation globale peut être utilisé à plusieurs reprises.
>
>Le terme &quot;processus d’approbation globale au niveau du groupe&quot; fait référence à un processus d’approbation qui peut être utilisé à plusieurs reprises pour des éléments et dont les états sont associés uniquement à un groupe spécifique.

Pour plus d’informations sur la création d’un processus d’approbation au niveau du système ou d’un processus d’approbation au niveau du groupe, voir [Créer un processus d’approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Considérations relatives aux processus d’approbation

* Vous devez créer la tâche de projet, de tâche, de publication, de modèle ou de modèle avant que le processus de validation puisse y être associé.
* Un processus de validation est toujours associé à deux éléments essentiels :

   * Chaque processus d’approbation correspond à un certain état de tâche dans le système Workfront. Lorsque vous modifiez l’état d’un élément de travail, une approbation jointe de cet état nécessite que le changement d’état soit confirmé avant que le nouvel état puisse être attribué à l’élément.

     >[!TIP]
     >
     >
     >   
     >   
     >   * Vous pouvez associer une approbation au niveau du groupe à un état global ou à un état au niveau du groupe.
     >   * Vous ne pouvez pas modifier l’état d’un élément à l’aide d’un processus de validation et le remplacer par un état autre que celui associé au processus de validation.
     >   
     >   
     >     Par exemple, si une validation de tâche est associée à l&#39;état En cours, la tâche passe automatiquement à l&#39;état En cours lors de l&#39;approbation. Il ne peut pas modifier automatiquement son statut en Terminé ou tout autre statut qui n&#39;est pas associé à la validation.
     >   
     >   
     >

   * Les entités associées à un processus d’approbation peuvent être des utilisateurs, des rôles de tâche ou des équipes. L’acceptation ou le rejet de la validation incombe en dernier ressort aux utilisateurs. Vous pouvez affecter des approbations aux utilisateurs qui remplissent un certain rôle dans le projet. Par exemple, vous pouvez affecter une approbation à un propriétaire de projet ou à un parrain. Pour plus d’informations, voir [Créer un processus d’approbation pour les tâches](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

     Les scénarios suivants existent :

      * Lorsque vous affectez une approbation aux rôles de tâche, tout utilisateur de l’équipe de projet associé au rôle de tâche peut prendre une décision sur l’approbation. Le rôle associé à l’approbation peut être soit son rôle de Principal, soit tout autre rôle.

        Pour plus d’informations sur l’équipe de projet, voir [Présentation de l’équipe de projet](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * Lorsque vous attribuez une approbation à une équipe, tout membre de cette équipe peut prendre une décision sur la validation. L’équipe associée à la validation peut être soit son équipe d’accueil, soit n’importe quelle autre équipe.

        Pour plus d’informations sur les rôles et les équipes d’un utilisateur, voir [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Lorsque vous créez un élément de travail, un processus d’approbation n’est pas automatiquement associé. Vous devez en joindre une manuellement si vous souhaitez en utiliser une. Pour plus d’informations sur l’association d’un processus d’approbation à un élément, voir [Associer un processus d’approbation nouveau ou existant au travail](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* L’administrateur de Workfront ou un utilisateur ayant un accès administratif aux processus d’approbation peut créer des processus d’approbation globale au niveau du système à utiliser dans l’ensemble du système. Un administrateur de groupe ayant un accès administratif aux processus d’approbation peut créer un processus d’approbation globale au niveau du groupe pour une utilisation uniquement par un certain groupe qu’il gère.
* Si vous ne souhaitez pas utiliser un processus d’approbation globale prédéfini au niveau du système ou du groupe pour un élément de travail, vous pouvez créer et lui associer un processus d’approbation à usage unique lorsque vous disposez des autorisations de gestion pour l’objet pour lequel vous souhaitez joindre le processus d’approbation.

  >[!NOTE]
  >
  Vous ne pouvez utiliser un seul processus d’approbation qu’une seule fois pour l’élément spécifique pour lequel il a été créé. Vous pouvez associer des états globaux ainsi que des états au niveau du groupe pour les processus d’approbation à usage unique pour les projets, tâches, problèmes, modèles et tâches de modèle.

* Lorsque vous associez un processus d’approbation au niveau du groupe à un élément à l’aide d’états personnalisés au niveau du groupe, la modification du groupe du projet peut créer un conflit entre les états d’approbation du groupe précédent et ceux existant au niveau du système. Envisagez de supprimer les processus d’approbation au niveau du groupe sur le projet, ou ses tâches ou problèmes avant de mettre à jour le groupe. Pour plus d’informations sur la création de processus d’approbation au niveau du groupe, voir [Processus de validation au niveau du groupe](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). Pour plus d’informations sur la création d’états de groupe personnalisés, voir [Création ou modification d’un état de groupe](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). Pour plus d’informations sur la mise à jour du groupe d’un projet, voir [Modification de projets](../../manage-work/projects/manage-projects/edit-projects.md).

## Processus d’approbation

Cette section explique les points suivants concernant l’approbation des tâches :

* [Comment les processus d’approbation reposent sur les états](#how-approval-processes-rely-on-statuses)
* [Comment un workflow type utilise un processus d’approbation](#how-a-typical-workflow-uses-an-approval-process)

### Comment les processus d’approbation reposent sur les états {#how-approval-processes-rely-on-statuses}

L’ajout d’un état à un processus d’approbation permet de s’assurer que l’élément passe par plusieurs services dans le bon ordre.

**Exemple :** Vous pouvez joindre à ce statut un processus d’approbation qui nécessite l’approbation du service financier. Ensuite, lorsqu’une personne change l’état d’un élément de travail en &quot;Service marketing&quot;, l’élément ne peut pas être déplacé vers ce service tant que le service financier ne s’y est pas déconnecté.

Pour plus d’informations sur les états des tâches, consultez les articles suivants :

* [Accéder à la liste des états des projets système](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [Accéder à la liste des états des tâches système](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [Accéder à la liste des statuts des problèmes système](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### Comment un workflow type utilise un processus d’approbation {#how-a-typical-workflow-uses-an-approval-process}

Le scénario suivant illustre la manière dont un processus d’approbation permet aux utilisateurs d’approuver le travail au fur et à mesure qu’un objet Workfront progresse dans un workflow en plusieurs étapes dans cet ordre :

1. L’administrateur Workfront ou un utilisateur disposant d’un accès administratif aux processus d’approbation crée un processus d’approbation pour un projet, une tâche ou un problème.

   >[!NOTE]
   >
   Vous pouvez associer des processus d’approbation de projet à un modèle et des processus d’approbation de tâche à une tâche de modèle. Ensuite, lorsqu’une personne utilise le modèle pour créer un projet, le processus d’approbation devient un processus d’approbation de projet ou de tâche, respectivement. Un processus de validation à usage unique associé à une tâche de modèle ou de modèle reste un processus de validation à usage unique pour les projets et les tâches.

1. Un utilisateur disposant de l’autorisation Gérer pour le projet, la tâche ou le problème associe le processus d’approbation à l’élément ou crée une approbation à usage unique pour l’élément.
1. Un utilisateur affecté à l’élément de travail passe à l’état qui initie le processus d’approbation et le processus d’approbation commence. (La personne qui a créé le processus de validation a défini la relation entre le statut et le processus de validation.)
1. Les approbateurs désignés reçoivent une notification sur le processus d’approbation en attente et ils passent en revue l’élément de travail.
1. Le processus d’approbation se termine une fois que les approbateurs désignés ont approuvé toutes les étapes du processus. Ou, s’ils rejettent une étape, l’état est réinitialisé à un état prédéfini ou un problème est créé. (La personne qui a créé le processus d’approbation a défini laquelle de ces étapes automatisées se produit après un rejet.)

**Exemple :** Une équipe publicitaire a créé un état nommé Ready for Printing (Prêt pour l’impression) et un processus d’approbation appelé Designer/Copywriter Signoff (Approbation de rédacteur) qu’elle associe à cet état. Ce processus de validation est paramétré pour :

* Exiger l’approbation du concepteur et du rédacteur de l’équipe
* Lancer chaque fois qu’une personne modifie l’état d’une tâche en Ready for Printing (Prêt pour impression)

Le propriétaire d’un projet de brochure associe le processus d’approbation de l’application de signature Designer/Copywriter au projet de brochure.

Lorsqu’une personne du projet passe le statut Prêt pour l’impression, le rédacteur et le concepteur reçoivent des notifications lui demandant de l’approuver ou de le refuser. Au cours du processus de validation, lorsqu’ils délibèrent sur son approbation ou non, le statut des projets s’affiche comme Prêt pour l’impression - En attente d’approbation.

Une fois que les deux utilisateurs ont approuvé la brochure dans Workfront, l’état du projet passe à Ready for Printing (Prêt pour impression).

## Processus de validation des documents

Les validations de documents sont utilisées pour une validation plus générale. Les commentaires sont capturés au format de conversation dans l’onglet Mises à jour . Vous pouvez utiliser les boutons de validation pour approuver, rejeter ou approuver les modifications.

Pour ajouter des approbateurs à un document après son téléchargement vers Workfront, reportez-vous à la section [Demande d’approbation de documents](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Processus de validation des BAT

Les validations de BAT sont utilisées pour une révision plus approfondie et comprennent généralement des workflows plus complexes. Les commentaires sont capturés avec des outils de balisage dans la visionneuse de vérification. Vous pouvez utiliser les boutons de validation pour approuver, rejeter ou approuver les modifications.

Pour ajouter un workflow automatisé à un BAT de document et désigner certains utilisateurs comme approbateurs du BAT dans le workflow, voir [Créer un BAT avancé avec un workflow automatisé](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Configuration des paramètres des processus d’approbation des tâches

En tant qu’administrateur de Workfront, vous pouvez configurer les paramètres globaux pour les processus d’approbation des tâches dans votre système. Ces paramètres déterminent différentes règles pour les processus d’approbation, comme la durée pendant laquelle une décision d’approbation doit rester ouverte ou la manière dont vous gérez la délégation d’approbation dans votre système. Pour plus d’informations sur les paramètres du processus d’approbation, voir [Configuration des paramètres d’approbation globaux](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
