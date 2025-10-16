---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Créer des rubriques de file d’attente
description: Les rubriques de file d’attente fonctionnent conjointement avec les règles de transmission pour affecter automatiquement le travail entrant à une personne, une fonction, une équipe ou pour le placer sur un projet. Les rubriques de la file d’attente définissent les conditions nécessaires à la mise en œuvre de la règle de transmission.
author: Becky
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '964'
ht-degree: 79%

---

# Créer des rubriques de file d’attente

<!-- Audited: 12/2023 -->

Les rubriques de file d’attente fonctionnent conjointement avec les règles de transmission pour affecter automatiquement le travail entrant à une personne, une fonction, une équipe ou pour le placer sur un projet. Les rubriques de la file d’attente définissent les conditions nécessaires à la mise en œuvre de la règle de transmission.

Le nombre de rubriques de file d’attente pouvant être affectées à un groupe de rubriques ou à un projet n’est pas limité. Les rubriques de file d’attente sont un type d’objet sur lequel un rapport peut être créé.

Vous pouvez créer des rubriques de file d&#39;attente pour des projets individuels ou pour des modèles de projet.

Une fois créées, vous ne pouvez pas déplacer les rubriques de file d’attente d’un projet ou modèle à un autre.

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
    <p>Standard</p>
    <p>Plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Autorisations de gestion pour le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une rubrique de file d’attente

1. Créez une règle de transmission, un groupe de rubriques et un formulaire personnalisé, si vous prévoyez de les associer à votre rubrique de file d’attente.\
   Pour plus d’informations sur la création de règles de transmission, de groupes de rubriques ou de formulaires personnalisés, reportez-vous aux articles suivants :

   * [Créer des règles de transmission](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [Créer des groupes de rubriques](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)

1. Accédez au projet ou au modèle que vous avez choisi d’activer en tant que file d’attente des demandes d’aide et à l’emplacement où vous souhaitez créer une nouvelle rubrique de file d’attente.\
   Pour plus d’informations sur la désignation d’un projet comme file d’attente des demandes d’aide, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Vous pouvez organiser les rubriques de file d’attente associées sous un groupe de rubriques. La personne à l’origine de la demande disposera ainsi d’une série de menus déroulants lors d’une demande.

   Ou

   Vous pouvez imbriquer les rubriques de la file d’attente directement sous le projet désigné comme une file d’attente des demandes d’aide, sans groupe de rubriques.

   Pour plus d’informations sur la création de groupes de rubriques, voir [Créer des groupes de rubriques](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. Cliquez sur **Rubriques de file d’attente** dans le panneau de gauche.
1. Cliquez sur **Nouvelle rubrique de file d’attente**.
1. Sur le formulaire **Nouvelle rubrique de file d’attente**, saisissez le texte suivant :

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
      <td>Décrivez la file d’attente des demandes. La description s’affiche lorsque les personnes sélectionnent la rubrique de la file d’attente dans le processus d’envoi d’une nouvelle demande. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ajouter au groupe de rubriques</strong> </td> 
      <td> S’il n’existe aucun groupe de rubriques sur le projet, le nom du projet est défini par défaut comme groupe de rubriques.<br>Si vous souhaitez créer d’autres groupes de rubriques à partir de cet emplacement, sélectionnez <strong>Créer un groupe de rubriques</strong> dans le menu déroulant.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formulaires personnalisés</strong> </td> 
      <td>Sélectionnez les formulaires personnalisés à associer à la rubrique de file d’attente. Vous devez créer des formulaires personnalisés pour les problèmes avant de pouvoir les associer aux rubriques de file d’attente. Pour plus d’informations sur la création de formulaires personnalisés, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Créer un formulaire personnalisé</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approbation par défaut</strong></td> 
      <td> <p>Associez un processus d’approbation à cette rubrique de file d’attente. Seuls les processus d’approbation des problèmes sont visibles dans ce menu déroulant. Tous les problèmes envoyés à cette file d’attente seront associés à ce processus d’approbation. Votre administrateur ou administratrice Adobe Workfront doit définir des processus d’approbation au niveau du système avant de pouvoir les associer aux rubriques de file d’attente. <span>Une personne disposant d’un accès administratif aux processus d’approbation peut également créer des processus d’approbation spécifiques à un groupe.</span>Pour plus d’informations sur la création de processus d’approbation, voir la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Créer un processus d’approbation pour les éléments de travail</a>.<br></p> 
       <div> 
        <p>Important : si le groupe du projet change, le processus d’approbation spécifique au groupe, associé aux problèmes existants, devient un processus d’approbation à usage unique. Pour plus d’informations sur la façon dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir la section <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Effets des modifications du processus d’approbation et de groupe sur les processus d’approbation affectés</a>.</p> 
        <p>Tenez compte des points suivants lors de l’ajout de processus d’approbation aux rubriques de file d’attente : </p> 
        <ul style="list-style-type: circle;"> 
         <li>Seuls les processus d’approbation actifs sont affichés dans la liste. </li> 
         <li> <p>Les processus d’approbation à l’échelle du système et spécifiques au groupe s’affichent dans la liste. Un processus d’approbation associé à un groupe autre que celui du projet ne s’affiche pas dans la liste.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Durée par défaut</strong> </td> 
      <td>Il s’agit de la durée par défaut de la demande. La date d’achèvement prévue de la demande est calculée en fonction de cette valeur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Route par défaut</strong> </td> 
      <td>Indiquez la règle de transmission que vous souhaitez associer à la rubrique de file d’attente. Vous devez créer la règle de transmission avant de pouvoir la joindre à une rubrique de file d’attente. Pour plus d’informations, voir la section <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md">Créer des règles de transmission</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Types de demandes</strong> </td> 
      <td> <p>Sélectionnez le type des demandes conservées dans cette rubrique de file d’attente. Les options visibles sont définies dans l’onglet <strong>Détails de la file d’attente</strong> du projet. Champ obligatoire. </p> 
       <p><b>NOTE</b> :</p>
      <p>Les types s’affichent sous forme de sélection dans la zone Demandes uniquement si le type de demande est sélectionné dans les pages Détails de la file d’attente et Rubrique de file d’attente. Pour plus d’informations sur la configuration de la zone Détails de la file d’attente d’un projet, voir la section <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Créer une file d’attente de demandes</a>. </p> <p>Choisissez parmi les types suivants :</p> 
       <ul> 
        <li>Rapport sur les bogues</li> 
        <li>Modifier l'ordre</li> 
        <li>Problème</li> 
        <li>Demande</li> 
       </ul> <p>Votre équipe d’administration Workfront a peut-être renommé certaines de ces options. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![Zone Nouvelle rubrique de file d’attente](assets/new-queue-topic-box.png)

1. Cliquer sur **Enregistrer**.\
   La rubrique de file d’attente est désormais disponible et visible dans la zone Demandes de Workfront, après la sélection d’une file d’attente de demandes et d’un groupe de rubriques.

## Modifier une rubrique de file d&#39;attente

Pour modifier une rubrique de file d&#39;attente existante :

1. Accédez au projet ou au modèle contenant la rubrique de file d&#39;attente à modifier.
1. Cliquez sur **Rubriques de file d’attente** dans le panneau de gauche.
1. Cliquez sur la rubrique de file d’attente que vous souhaitez modifier.

Pour plus d’informations sur les options de modification disponibles, voir [Création d’une rubrique de file d’attente](#create-a-queue-topic) dans cet article.

## Supprimer une rubrique de file d&#39;attente

Vous pouvez supprimer une ou plusieurs rubriques de file d&#39;attente en même temps.

1. Accédez au projet ou au modèle contenant la rubrique de file d&#39;attente à supprimer.
1. Cliquez sur **Rubriques de file d’attente** dans le panneau de gauche.
1. Cliquez sur la case en regard du nom de chaque rubrique de file d&#39;attente à supprimer. Une coche apparaît dans la case.
1. Cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/delete-icon.png) en haut de la page.

