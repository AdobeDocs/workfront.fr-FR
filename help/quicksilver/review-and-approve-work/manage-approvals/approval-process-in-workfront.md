---
content-type: overview
product-area: projects
navigation-topic: approvals
title: Vue d’ensemble du processus d’approbation
description: Vous pouvez créer un processus d’approbation et le joindre à un objet pour vous assurer que les personnes désignées vérifient certaines modifications avant la progression de l’objet.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: e4de185f172b173dcc3ad966afa69ffb3bc479eb
workflow-type: tm+mt
source-wordcount: '1752'
ht-degree: 100%

---

# Vue d’ensemble du processus d’approbation

<!-- Audited: 12/2023 -->

Vous pouvez créer un processus d’approbation et le joindre à un objet pour vous assurer que les personnes désignées vérifient certaines modifications avant la progression de l’objet.

Cette option est disponible pour les types d’objets suivants dans Adobe Workfront :

* Élément de travail (projet, tâche ou problème, modèle, tâche de modèle)
* Document
* Épreuve

Cet article contient des informations générales sur les processus d’approbation associés aux éléments de travail.
Pour obtenir des instructions sur la création d’un processus d’approbation, voir [Créer un processus d’approbation pour les éléments de travail](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Types de processus d’approbation pour les éléments de travail

Si vous êtes administrateur ou administratrice d’Adobe Workfront ou utilisateur ou utilisatrice disposant d’un accès administratif aux processus d’approbation, vous pouvez créer les processus d’approbation suivants pour les projets, tâches et problèmes :

* **Processus d’approbation globale au niveau du système** : les utilisateurs et utilisatrices peuvent les joindre à l’un des éléments suivants :

   * un projet, une tâche ou un problème dans la section Approbations
   * Dans la zone Modifier le projet de la zone Processus d’approbation par défaut de la tâche
   * Dans la section Détails de la file d’attente ou Rubrique de la file d’attente d’un projet dans les zones Processus d’approbation par défaut. Le projet doit être activé en tant que file d’attente des demandes.

* **Processus d’approbation globale au niveau du groupe** : les utilisateurs et utilisatrices peuvent les joindre aux éléments suivants :

   * un projet, une tâche ou un problème appartenant au groupe associé au processus d’approbation dans la section Approbations
   * Dans la zone Modifier le projet de la zone Processus d’approbation par défaut de la tâche pour un projet appartenant au groupe associé au processus d’approbation
   * Dans la section Détails de la file d’attente ou Rubrique de la file d’attente d’un projet dans les zones Processus d’approbation par défaut. Le projet doit être activé en tant que file d’attente des demandes et appartenir au groupe associé au processus d’approbation.

  Pour plus d’informations sur la création d’un processus d’approbation au niveau du système ou du groupe, voir [Créer un processus d’approbation pour les éléments de travail](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **Processus d’approbation à usage unique** : à utiliser avec un projet, une tâche, un problème, un modèle ou une tâche de modèle unique. Ce type de processus d’approbation affecte uniquement l’objet qui lui est associé et ne peut être associé à aucun autre objet.

  Pour plus d’informations sur la création d’un processus d’approbation à usage unique, voir [Associer un processus d’approbation nouveau ou existant au travail](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Cet article utilise le terme « processus d’approbation globale » pour faire la différence avec le terme « processus d’approbation à usage unique ». Un processus d’approbation globale peut être utilisé à plusieurs reprises.
>
>Le terme « processus d’approbation globale au niveau du groupe » fait référence à un processus d’approbation qui peut être utilisé à plusieurs reprises pour des éléments et dont les statuts sont associés uniquement à un groupe spécifique.

Pour plus d’informations sur la création d’un processus d’approbation au niveau du système ou d’un processus d’approbation au niveau du groupe, voir [Créer un processus d’approbation pour des éléments de travail](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Considérations relatives aux processus d’approbation

* Vous devez créer le projet, la tâche, le problème, le modèle ou la tâche de modèle avant que le processus d’approbation puisse y être associé.
* Un processus d’approbation est toujours associé à deux éléments essentiels :

   * Chaque processus d’approbation correspond à un certain statut d’élément de travail dans le système Workfront. Lorsque vous modifiez le statut d’un élément de travail, une approbation jointe de ce statut nécessite que le changement de statut soit confirmé avant que le nouveau statut puisse être affecté à l’élément.

     >[!TIP]
     >
     >
     >   
     >   
     >   * Vous pouvez associer une approbation au niveau du groupe à un statut global ou au niveau du groupe.
     >   * Vous ne pouvez pas modifier le statut d’un élément à l’aide d’un processus d’approbation et le remplacer par un statut autre que celui associé au processus d’approbation.
     >   
     >   
     >     Par exemple, si une approbation de tâche est associée au statut En cours, la tâche passe automatiquement au statut En cours lorsque l’approbation est accordée. Elle ne peut pas passer automatiquement au statut Terminé ou à tout autre statut qui n’est pas associé à l’approbation.
     >   
     >   
     >

   * Les entités associées à un processus d’approbation peuvent être des utilisateurs ou utilisatrices, des fonctions ou des équipes. L’acceptation ou le rejet de l’approbation incombe en dernier ressort aux utilisateurs et utilisatrices. Vous pouvez affecter des approbations aux personnes qui occupent une certaine fonction dans le projet.Par exemple, vous pouvez affecter une approbation à un ou une propriétaire de projet ou à un sponsor.Pour plus d’informations, voir [Créer un processus d’approbation pour des éléments de travail](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

     Les scénarios suivants sont possibles :

      * Lorsque vous affectez une approbation à des fonctions, tout membre de l’équipe de projet associé à la fonction peut prendre une décision sur l’approbation. Le rôle associé à l’approbation peut être soit son rôle de Principal, soit tout autre rôle.

        Pour plus d’informations sur l’équipe de projet, voir [Vue d’ensemble de l’équipe de projet](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * Lorsque vous affectez une approbation à une équipe, tout membre de cette équipe peut prendre une décision sur l’approbation. L’équipe associée à l’approbation peut être son équipe principale ou n’importe quelle autre équipe.

        Pour plus d’informations sur les rôles et les équipes d’un utilisateur ou d’une utilisatrice, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Lorsque vous créez un élément de travail, un processus d’approbation n’est pas automatiquement associé. Vous devez en joindre un manuellement si vous souhaitez l’utiliser. Pour plus d’informations sur l’association d’un processus d’approbation à un élément, voir [Associer un processus d’approbation nouveau ou existant au travail](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* L’administrateur ou l’administratrice Workfront ou un utilisateur ou une utilisatrice ayant un accès administratif aux processus d’approbation peut créer des processus d’approbation globale à l’échelle du système à utiliser dans l’ensemble du système. Un administrateur ou une administratrice de groupe disposant d’un accès administratif aux processus d’approbation peut créer un processus d’approbation globale à l’échelle du groupe qui ne sera utilisé que par un certain groupe qu’il ou elle gère.
* Si vous ne souhaitez pas utiliser un processus d’approbation globale prédéfini à l’échelle du système ou du groupe pour un élément de travail, vous pouvez créer et lui associer un processus d’approbation à usage unique lorsque vous disposez des autorisations de gestion pour l’objet auquel vous souhaitez joindre le processus d’approbation.

  >[!NOTE]
  >
  >Vous ne pouvez utiliser un processus d’approbation à usage unique qu’une seule fois pour l’élément spécifique en vue duquel il a été créé. Vous pouvez associer des statuts globaux ainsi que des statuts à l’échelle du groupe pour les processus d’approbation à usage unique pour les projets, tâches, problèmes, modèles et tâches de modèle.

* Lorsque vous associez un processus d’approbation à l’échelle du groupe à un élément à l’aide de statuts personnalisés à l’échelle du groupe, la modification du groupe du projet peut créer un conflit entre les statuts d’approbation du groupe précédent et ceux existant à l’échelle du système. Envisagez de supprimer les processus d’approbation à l’échelle du groupe sur le projet, ou ses tâches ou problèmes avant de mettre à jour le groupe. Pour plus d’informations sur la création de processus d’approbation à l’échelle du groupe, voir [Processus d’approbation à l’échelle du groupe](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). Pour plus d’informations sur la création de statuts de groupe personnalisés, voir [Créer ou modifier un statut de groupe](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). Pour plus d’informations sur la mise à jour du groupe d’un projet, voir [Modifier des projets](../../manage-work/projects/manage-projects/edit-projects.md).

## Le workflow du processus d’approbation

Cette section explique les points suivants concernant l’approbation des éléments de travail :

* [Comment les processus d’approbation reposent sur les statuts](#how-approval-processes-rely-on-statuses)
* [Comment un workflow standard utilise un processus d’approbation](#how-a-typical-workflow-uses-an-approval-process)

### Comment les processus d’approbation reposent sur les statuts {#how-approval-processes-rely-on-statuses}

L’ajout d’un statut à un processus d’approbation permet de s’assurer que l’élément passe par plusieurs services dans le bon ordre.

**Exemple :** vous pouvez joindre au statut de service marketing un processus d’approbation qui nécessite l’approbation du service financier. Ensuite, lorsqu’une personne change le statut d’un élément de travail en « Service marketing », l’élément ne peut pas être déplacé vers ce service tant que le service financier ne l’a pas approuvé.

Pour plus d’informations sur les statuts des éléments de travail, consultez les articles suivants :

* [Accéder à la liste des statuts des projets du système](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [Accéder à la liste des statuts des tâches système](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [Accéder à la liste des statuts des problèmes du système](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### Comment un workflow standard utilise un processus d’approbation {#how-a-typical-workflow-uses-an-approval-process}

Le scénario suivant illustre la manière dont un processus d’approbation permet aux utilisateurs et utilisatrices d’approuver le travail au fur et à mesure qu’un objet Workfront progresse dans un workflow en plusieurs étapes dans cet ordre :

1. L’administrateur ou l’administratrice Workfront ou un utilisateur ou une utilisatrice disposant d’un accès administratif aux processus d’approbation crée un processus d’approbation pour un projet, une tâche ou un problème.

   >[!NOTE]
   >
   >Vous pouvez associer des processus d’approbation de projet à un modèle et des processus d’approbation de tâche à une tâche de modèle. Ensuite, lorsqu’une personne utilise le modèle pour créer un projet, le processus d’approbation devient respectivement un processus d’approbation de projet ou de tâche. Un processus d’approbation à usage unique associé à un modèle ou une tâche de modèle reste un processus d’approbation à usage unique pour les projets et les tâches.

1. Un utilisateur ou une utilisatrice disposant de l’autorisation Gérer pour le projet, la tâche ou le problème associe le processus d’approbation à l’élément ou crée une approbation à usage unique pour l’élément.
1. Un utilisateur ou une utilisatrice affecté à l’élément de travail change son statut en statut qui lance le processus d’approbation. Ensuite, le processus d’approbation commence. (La personne qui a créé le processus d’approbation a défini la relation entre le statut et le processus d’approbation.)
1. Les approbateurs ou approbatrices désignés reçoivent une notification sur le processus d’approbation en attente et ils révisent l’élément de travail.
1. Le processus d’approbation se termine une fois que les approbateurs ou approbatrices désignés ont approuvé toutes les étapes du processus. Ou, s’ils rejettent une étape, le statut est réinitialisé à un statut prédéfini ou un problème est créé. (La personne qui a créé le processus d’approbation a défini laquelle de ces étapes automatisées se produit après un rejet.)

**Exemple :** une équipe publicitaire a créé un statut nommé Prêt pour impression et un processus d’approbation appelé Approbation de rédacteur ou rédactrice/de concepteur ou conceptrice qu’elle associe à ce statut. Ce processus d’approbation est configuré pour :

* Exiger l’approbation du concepteur ou de la conceptrice et du rédacteur ou de la rédactrice de l’équipe
* S’exécuter chaque fois qu’une personne modifie le statut d’une tâche en Prêt pour impression

Le ou la propriétaire du projet de brochure associe le processus d’approbation de rédacteur ou rédactrice/concepteur ou conceptrice au projet de brochure.

Lorsqu’une personne du projet change le statut en Prêt pour impression, le rédacteur ou la rédactrice et le concepteur ou la conceptrice reçoivent des notifications leur demandant d’approuver ou de refuser. Au cours du processus d’approbation, lorsqu’ils délibèrent sur son approbation ou non, le statut des projets s’affiche comme Prêt pour impression - En attente d’approbation.

Une fois que les deux personnes ont approuvé la brochure dans Workfront, le statut du projet change en Prêt pour impression.

## Processus d’approbation des documents

Les approbations de documents sont utilisées pour une approbation plus générale. Les commentaires sont capturés au format chat dans l’onglet Mises à jour. Vous pouvez utiliser les boutons d’approbation pour approuver, rejeter ou approuver avec des modifications.

Pour ajouter des approbateurs ou approbatrices à un document après son chargement dans Workfront, voir [Demander l’approbation d’un document](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Processus d’approbation de l’épreuve

Les approbations de l’épreuve servent à une révision plus approfondie et comprennent généralement des workflows plus complexes. Les commentaires sont capturés avec des outils de balisage dans la visionneuse de relecture. Vous pouvez utiliser les boutons d’approbation pour approuver, rejeter ou approuver avec des modifications.

Pour ajouter un workflow automatisé à une épreuve de document et désigner certains utilisateurs ou certaines utilisatrices comme approbateurs ou approbatrices de l’épreuve dans le workflow, voir [Créer une épreuve avancée avec un workflow automatisé](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Configurer les paramètres des processus d’approbation d’élément de travail

En tant qu’administrateur ou administratrice Workfront, vous pouvez configurer les paramètres globaux pour les processus d’approbation d’élément de travail dans votre système. Ces paramètres déterminent différentes règles pour les processus d’approbation, comme la durée pendant laquelle une décision d’approbation peut rester ouverte ou la manière dont vous gérez les délégations d’approbation dans votre système. Pour plus d’informations sur les paramètres du processus d’approbation, voir [Configurer les paramètres d’approbation globale](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
