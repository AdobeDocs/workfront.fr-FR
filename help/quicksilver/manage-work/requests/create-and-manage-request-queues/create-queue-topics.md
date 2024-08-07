---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Créer des rubriques de file d’attente
description: Les rubriques de file d’attente fonctionnent conjointement avec les règles de routage pour affecter automatiquement le travail entrant à un utilisateur, un rôle de tâche, une équipe ou pour le placer sur un projet. Les rubriques de la file d’attente définissent les conditions nécessaires à la mise en oeuvre de la règle de routage.
author: Alina
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 18%

---

# Créer des rubriques de file d’attente

<!-- Audited: 12/2023 -->

Les rubriques de file d’attente fonctionnent conjointement avec les règles de routage pour affecter automatiquement le travail entrant à un utilisateur, un rôle de tâche, une équipe ou pour le placer sur un projet. Les rubriques de la file d’attente définissent les conditions nécessaires à la mise en oeuvre de la règle de routage.

Le nombre de rubriques de file d’attente pouvant être affectées à un groupe de rubriques ou à un projet n’est pas limité. Les rubriques de file d’attente sont un type d’objet à rapporter.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
    <p>Nouvelle : standard</p>
    <p>ou</p>
    <p>Actuelle : formule</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Autorisations de gestion pour le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Création d’une rubrique de file d’attente

1. Créez une règle d’acheminement, un groupe de rubriques et un formulaire personnalisé, si vous prévoyez de les associer à votre rubrique de file d’attente.\
   Pour plus d’informations sur la création de règles de routage, de groupes de rubriques ou de formulaires personnalisés, reportez-vous aux articles suivants :

   * [Créer des règles de routage](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [Créer des groupes de sujets](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [Concevoir un formulaire avec le créateur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)

1. Accédez au projet que vous avez choisi d’activer en tant que file d’attente des demandes d’aide et où vous souhaitez créer une rubrique de file d’attente.\
   Pour plus d’informations sur la désignation d’un projet comme file d’attente de demandes d’aide, voir [Création d’une file d’attente de demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Vous pouvez organiser les rubriques de file d’attente associées sous un groupe de rubriques. Le demandeur disposera ainsi d’une série de menus déroulants lors de l’exécution d’une requête.

   Ou

   Vous pouvez imbriquer les rubriques de la file d’attente directement sous le projet désigné comme une file d’attente de demande d’aide, sans groupe de rubriques.

   Pour plus d’informations sur la création de groupes de rubriques, voir [Création de groupes de rubriques](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. Cliquez sur **Rubriques de la file d’attente** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Rubriques de la file d’attente**.
1. Cliquez sur **Nouvelle rubrique de file d’attente**.
1. Sur le formulaire **New Queue Topic**, saisissez ce qui suit :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nom</strong> </td> 
      <td> Nom de la rubrique de file d’attente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Décrivez la file d’attente des demandes. La description s’affiche lorsque les utilisateurs sélectionnent la rubrique de la file d’attente dans le processus d’envoi d’une nouvelle demande. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ajouter au groupe de rubriques</strong> </td> 
      <td> S’il n’existe aucun groupe de rubriques sur le projet, le nom du projet est défini par défaut comme groupe de rubriques.<br>Si vous souhaitez créer d’autres groupes de rubriques à partir de cet emplacement, sélectionnez <strong>Créer un groupe de rubriques</strong> dans le menu déroulant.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_inside_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formulaires personnalisés</strong> </td> 
      <td>Sélectionnez les formulaires personnalisés à associer à la rubrique de la file d’attente. Vous devez créer des formulaires personnalisés pour les problèmes avant de pouvoir les associer aux rubriques de la file d’attente. Pour plus d’informations sur la création de formulaires personnalisés, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Concevoir un formulaire avec le concepteur de formulaires</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approbation par défaut</strong></td> 
      <td> <p>Associez un processus d’approbation à cette rubrique de file d’attente. Seuls les processus d’approbation des problèmes sont visibles dans ce menu déroulant. Tous les problèmes envoyés à cette file d’attente seront associés à ce processus d’approbation. Votre administrateur Adobe Workfront doit définir des processus d’approbation au niveau du système avant de pouvoir les associer aux rubriques de la file d’attente. <span>Un utilisateur disposant d’un accès administratif aux processus d’approbation peut également créer des processus d’approbation spécifiques à un groupe.</span> Pour plus d’informations sur la création de processus d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Création d’un processus d’approbation pour les tâches</a>.<br></p> 
       <div> 
        <p>Important : Si le groupe du projet change, le processus d’approbation spécifique au groupe associé aux problèmes existants devient un processus d’approbation à usage unique. Pour plus d’informations sur la manière dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Comment les modifications apportées aux groupes et aux processus d’approbation affectent les processus d’approbation attribués</a>.</p> 
        <p>Tenez compte des points suivants lors de l’ajout de processus d’approbation aux rubriques de la file d’attente : </p> 
        <ul style="list-style-type: circle;"> 
         <li>Seuls les processus d’approbation actifs sont affichés dans la liste. </li> 
         <li> <p>Les processus d’approbation à l’échelle du système et du groupe s’affichent dans la liste. Un processus d’approbation associé à un groupe autre que celui du projet ne s’affiche pas dans la liste.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Durée par défaut</strong> </td> 
      <td>Il s’agit de la durée par défaut de la requête. La date de fin planifiée de la requête est calculée en fonction de cette valeur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Itinéraire par défaut</strong> </td> 
      <td>Indiquez la règle de routage que vous souhaitez associer à la rubrique de la file d’attente. Vous devez créer la règle de routage avant de pouvoir la joindre à une rubrique de file d’attente. Pour plus d’informations, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md">Création de règles de routage</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Types de requête</strong> </td> 
      <td> <p>Sélectionnez le type de requêtes que cette rubrique de file d’attente stocke. Les options visibles sont définies dans l’onglet <strong>Détails de la file d’attente</strong> du projet. Il s’agit d’un champ obligatoire. </p>

   <p><b>NOTE</b> :

   Les types s’affichent sous forme de sélection dans la zone Requêtes uniquement si le type de requête est sélectionné dans les pages Détails de la file d’attente et Rubrique de la file d’attente. Pour plus d’informations sur la configuration de la zone Détails de la file d’attente d’un projet, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Création d’une file d’attente de requêtes</a>. </p> <p>Choisissez parmi les types suivants :</p>
   <ul>
   <li>Rapport sur les bogues</li>
   <li>Modifier l&#39;ordre</li>
   <li>Problème</li>
   <li>Demande</li>
   </ul> <p>Votre administrateur Workfront a peut-être renommé certaines de ces options. </p> </td>
   </tr> 
    </tbody> 
   </table>

   ![Nouvelle boîte de rubrique de file d’attente](assets/new-queue-topic-box.png)

1. Cliquer sur **Enregistrer**.\
   La rubrique de file d’attente est désormais disponible et est visible dans la zone Demandes de Workfront, après la sélection d’une file d’attente de requêtes et d’un groupe de rubriques.
