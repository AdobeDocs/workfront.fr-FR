---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Présentation des propriétaires et des sponsors de projet
description: Vous pouvez désigner un propriétaire de projet et un parrain de projet pour un projet.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Présentation des propriétaires et des sponsors de projet

Vous pouvez désigner un propriétaire de projet et un parrain de projet pour un projet.

Le propriétaire du projet est la personne responsable de la fin du projet à temps et selon le budget.

Le parrain du projet est un acteur important du projet qui a des ressources investies dans ce projet. L’achèvement du projet bénéficie généralement au parrain du projet.

Pour plus d’informations sur la mise à jour du propriétaire ou du parrain d’un projet, voir [Mettre à jour les propriétaires et les sponsors de projet](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Propriétaires de projet

Vous pouvez désigner le responsable d’un projet en spécifiant un propriétaire de projet sur un projet ou un modèle.

Vous ne pouvez définir qu’un seul propriétaire de projet pour un projet.

Les éléments suivants sont possibles à l’aide du champ Propriétaire du projet :

* Vous ne pouvez désigner qu’un seul utilisateur comme propriétaire de projet.
* Vous pouvez désigner les propriétaires de projet comme approbateurs horaires du projet.
* Vous pouvez désigner le propriétaire du projet comme approbateur générique lors de la définition des processus d’approbation de projet, de tâche ou d’émission. Pour plus d’informations sur les validations, voir [Modifier un processus de validation](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >Lorsque vous affectez une approbation au propriétaire du projet et qu’aucune personne n’est désignée comme propriétaire d’un projet, l’approbation est réaffectée à l’administrateur Workfront principal, comme indiqué dans la section Informations sur le client de la zone Configuration. Pour plus d’informations, voir [Configuration des informations de base pour votre système](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).


* Vous pouvez activer certaines notifications qui ne sont diffusées qu’au propriétaire du projet.

   Pour plus d’informations sur les notifications électroniques, voir la section [Configuration des notifications d’événement pour tous les membres du système](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) dans l’article [Configuration des notifications d’événement pour tous les membres du système](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Vous pouvez afficher le champ Propriétaire du projet dans un rapport ou une liste.

   Vous pouvez également afficher le champ Propriétaire du projet dans une vue, un regroupement ou une invite.

   Par exemple, vous pouvez copier l’expression de mode de texte suivante dans un filtre pour afficher les projets appartenant à l’utilisateur connecté : 

   ```
   ownerID=$$USER.ID
   ```

Pour plus d’informations sur la création de rapports, voir l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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

## Partenaires du projet

Vous pouvez désigner n’importe quel utilisateur du système comme responsable de projet. Le parrain du projet est généralement un responsable, un cadre ou une partie prenante qui a besoin de savoir ce qui se passe avec le projet.

Tenez compte de ce qui suit lors de l’affectation d’un sponsor de projet :

* Le parrain du projet n’a aucun accès supplémentaire au projet, mais il est ajouté aux notifications par e-mail du projet. Pour plus d’informations sur les notifications, voir l’article [Configuration des notifications d’événement pour tous les membres du système](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Vous ne pouvez désigner qu’un seul responsable de projet.
* Vous pouvez désigner le parrain du projet comme approbateur générique lors de la définition des processus d’approbation de projet, de tâche ou d’émission. Pour plus d’informations sur les validations, voir [Modifier un processus de validation](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >Lorsque vous affectez une approbation au parrain du projet et qu’aucune personne n’est désignée comme parrain d’un projet, l’approbation est réaffectée au propriétaire du projet. Si personne n’est désigné comme propriétaire du projet, l’approbation est attribuée à l’administrateur Workfront.

* Vous pouvez afficher le champ Sponsor de projet dans un rapport ou une liste.

   Vous pouvez également afficher le champ Sponsor de projet dans une vue, un regroupement ou une invite.

   Par exemple, vous pouvez copier l’expression de mode de texte suivante dans un filtre pour afficher les projets sponsorisés par l’utilisateur connecté :

   ```
   sponsorID=$$USER.ID
   ```

    

   Pour plus d’informations sur la création de rapports, voir l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
