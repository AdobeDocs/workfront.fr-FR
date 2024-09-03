---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Vue d’ensemble des personnes propriétaires et sponsors du projet
description: Vous pouvez désigner une personne propriétaire du projet et une personne sponsor du projet pour un projet.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: 111c776af19fbc2982c14cc9d3b3778d37bc0be3
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 100%

---

# Vue d’ensemble des personnes propriétaires et sponsors du projet

<!-- Audited: 1/2024 -->

Vous pouvez désigner une personne propriétaire du projet et une personne sponsor du projet pour un projet.

La personne propriétaire du projet est responsable de l’achèvement du projet à temps et dans le respect du budget.

La personne sponsor du projet, partie prenante importante du projet, investit des ressources dans le projet. L’achèvement du projet bénéficie généralement à la personne sponsor du projet.

Pour plus d’informations sur la mise à jour de la personne propriétaire ou sponsor d’un projet, voir [Mettre à jour les personnes propriétaires et sponsors des projets](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Propriétaires de projet

Vous pouvez désigner la personne responsable d’un projet en spécifiant un ou une propriétaire sur un projet ou un modèle.

Vous ne pouvez définir qu’une seule personne propriétaire de projet par projet.

Le champ Propriétaire du projet permet de réaliser les actions suivantes :

* Vous ne pouvez désigner qu’une seule personne comme propriétaire du projet.
* Vous pouvez désigner les personnes propriétaires du projet comme approbatrices des heures du projet.
* Vous pouvez désigner la personne propriétaire du projet comme approbatrice générique lors de la définition des processus d’approbation de projet, de tâche ou de problème. Pour plus d’informations sur les approbations, voir [Modifier un processus d’approbation](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >Lorsque vous accordez une approbation à la personne propriétaire du projet et qu’il n’existe pas de personne propriétaire de projet, l’approbation est alors accordée à l’équipe principale d’administration de Workfront, comme indiqué dans la section de la section Infos client de la zone de configuration. Pour plus d’informations, consultez la section [Configurer des informations de base pour votre système](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
  >


* Vous pouvez activer certaines notifications qui ne sont diffusées qu’à la personne propriétaire du projet.

  Pour plus d’informations sur les notifications par e-mail, voir la section [Configurer les notifications d’événement pour tous les utilisateurs et les utilisatrices du système](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) dans l’article [Configurer les notifications d’événement pour tous les utilisateurs et les utilisatrices du système](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Vous pouvez afficher le champ Propriétaire du projet dans un rapport ou une liste.

  Vous pouvez également afficher le champ Propriétaire du projet dans une vue, un regroupement ou une invite.

  Par exemple, vous pouvez copier l’expression en mode texte suivante dans un filtre pour afficher les projets appartenant à la personne connectée :

  ```
  ownerID=$$USER.ID
  ```

Pour plus d’informations sur la création de rapports, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE:&nbsp;drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Sponsors du projet

Vous pouvez désigner n’importe quelle personne du système comme sponsor du projet. Il s’agit généralement d’une personne responsable, cadre ou partie prenante qui a besoin de savoir comment le projet se déroule.

Tenez compte de ce qui suit lors de l’affectation d’une personne sponsor de projet :

* La personne sponsor du projet n’a aucun accès supplémentaire au projet, mais elle est ajoutée aux notifications par e-mail du projet. Pour plus d’informations sur les notifications, voir l’article [Configurer les notifications d’événement pour tous les utilisateurs et les utilisatrices du système](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Vous ne pouvez désigner qu’une seule personne responsable de projet.
* Vous pouvez désigner la personne sponsor du projet comme approbatrice générique lors de la définition des processus d’approbation de projet, de tâche ou de problème. Pour plus d’informations sur les approbations, voir [Modifier un processus d’approbation](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >si aucune personne sponsor de projet n’est désignée et que vous accordez une approbation à la personne sponsor du projet, celle-ci est alors accordée à la personne propriétaire du projet. Si aucune personne propriétaire de projet n’est désignée, l’approbation est accordée à la personne chargée de l’administration de Workfront.

* Vous pouvez afficher le champ Sponsor du projet dans un rapport ou une liste.

  Vous pouvez également afficher le champ Sponsor du projet dans une vue, un regroupement ou une invite.

  Par exemple, vous pouvez copier l’expression en mode texte suivante dans un filtre pour afficher les projets sponsorisés par la personne connectée :

  ```
  sponsorID=$$USER.ID
  ```

   

  Pour plus d’informations sur la création de rapports, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->
