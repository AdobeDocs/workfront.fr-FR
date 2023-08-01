---
content-type: overview
product-area: projects
navigation-topic: manage-projects
title: Gestion des informations dans la zone Aperçu du projet
description: Gestion des informations dans la zone Aperçu du projet
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6113bc62-18f2-4558-bc2f-986b1e7d1a83
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 4%

---

# Gestion des informations dans la zone Aperçu du projet

<!--
<p>(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

Vous pouvez afficher ou modifier les informations d’un projet en accédant à la zone Aperçu de la section Détails du projet . Il existe un nombre limité de champs que vous pouvez afficher ou modifier dans cette zone. Pour plus d’informations sur la modification de toutes les informations d’un projet, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

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
   <td role="rowheader"> <p role="rowheader">Licence Adobe Workfront*</p> </td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage de l’accès ou d’une version ultérieure à la console Projets </p>

<p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher l’accès au projet pour afficher des informations limitées sur le projet</p> 
   <p>Gérer l’accès au projet pour modifier les informations le concernant</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Accès à la section Aperçu

1. Accédez au projet dont vous souhaitez afficher la section Aperçu .
1. Cliquez sur **Détails du projet** dans le panneau de gauche.
1. La variable **Présentation** doit s’afficher en premier dans le cadre des détails du projet et doit être développé par défaut.

   Ou

   Cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png) dans le coin supérieur droit de la section Détails, puis cliquez sur **Présentation**. La zone Aperçu s’ouvre alors pour modification.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront a configuré votre modèle de mise en page, la section Aperçu peut ne pas être répertoriée en premier, auquel cas elle est réduite. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. (Conditionnel) S’il existe un champ spécifique qui doit être mis à jour sur un projet, mais qui ne s’affiche pas dans cette section, cliquez sur la **Plus de menu** ![](assets/more-icon.png) en regard du nom du projet, puis **Modifier** pour afficher d’autres champs de projet.

   Pour plus d’informations sur la modification de projets, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Modifiez ou consultez les champs du tableau ci-dessous qui s’affichent dans le **Présentation** .\
   Pour modifier un champ disponible, cliquez ou cliquez sur **+Ajouter** pour ajouter des informations à un champ vide.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront a configuré votre modèle de mise en page, il se peut que tous les champs ne s’affichent pas. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader"><b>Champ</b></td> 
      <td><b>Description</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Décrivez l’objectif de ce projet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td>Insérez toute URL dans ce champ. Il peut s’agir d’une URL Workfront ou de toute autre URL. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorité</td> 
      <td>Sert de priorité ou d’importance désignée du projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Statut</td> 
      <td> <p>État du projet. </p> <p>Conseil : Vous ne pouvez pas terminer un projet tant que toutes les tâches et tous les problèmes ne sont pas terminés. Si le mode d’achèvement du projet est défini sur Automatique, vous ne pouvez pas terminer un projet manuellement. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type de condition</td> 
      <td>Détermine si le gestionnaire définit la condition du projet ou si Workfront le fait. Pour plus d’informations sur la condition du projet, voir l’article <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Présentation de la condition et du type de condition du projet</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mode horaire</td> 
      <td>Définit la planification du projet. Par exemple, si le projet est planifié à partir de la date de début ou de la date de fin. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date et heure de début planifiées</td> 
      <td> Date prévue de début du projet. Ce paramètre est manuellement défini par le chef de projet lorsque le projet est planifié à partir de la date de début. Workfront définit automatiquement cette date lorsque le projet est planifié à partir de la date de fin, en fonction de la durée des tâches du projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date et heure d’achèvement prévues</td> 
      <td> Date à laquelle le projet est prévu. Ce paramètre est manuellement défini par le chef de projet lorsque le projet est planifié à partir de la date de fin. Workfront définit automatiquement cette date lorsque le projet est planifié à partir de la date de début, en fonction de la durée des tâches du projet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Portfolio</td> 
      <td>Portefeuille associé au projet. Vous devez créer le portfolio avant de pouvoir l’ajouter à un projet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Programme</td> 
      <td>Programme associé au portefeuille du projet. Vous devez créer le programme avant de pouvoir l’ajouter à un projet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groupe</td> 
      <td> <p>Groupe associé au projet.</p> <p>Vous pouvez vous assurer que vous sélectionnez le groupe approprié en pointant dessus et en cliquant sur l’icône d’information. <img src="assets/info-icon.png"> qui s’affiche en regard de celle-ci. Une info-bulle s’affiche, répertoriant les informations relatives au groupe, telles que la hiérarchie des groupes au-dessus de celui-ci et ses administrateurs.</p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> 
      Par défaut, l’un des groupes suivants est automatiquement associé à un projet lors de sa création, sauf si vous spécifiez un autre groupe :
        <ul> 
         <li> <p><span>Lorsque le projet est créé à partir de la zone Projets , le groupe d’accueil du créateur du projet est associé au projet.</span> </p> </li> 
         <li> <p><span>Lorsque le projet est créé à partir de la page principale d’un groupe dans la zone Configuration, ce groupe est automatiquement associé au projet.</span> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entreprise</td> 
      <td>Société associée au projet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Propriétaire du projet </td> 
      <td>C'est le propriétaire du projet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sponsor du projet</td> 
      <td> <p>Voici la Principale partie prenante du projet. Il s'agit généralement d'un cadre supérieur qui supervise et soutient le projet, ou c'est la personne responsable du budget.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gestionnaire des ressources</td> 
      <td> <p>Il s’agit de la personne qui peut gérer les ressources utilisateur dans le projet. </p> <p>Pour plus d’informations sur les gestionnaires de ressources, reportez-vous à l’article <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md" class="MCXref xref">Désignation des gestionnaires de ressources pour un projet ou un modèle </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Lors de la mise à jour des champs Propriétaire du projet, Parrain du projet et Gestionnaire de ressources, notez l’avatar, le rôle Principal de l’utilisateur ou son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques.
   >
   >Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher à mesure que vous les ajoutez.
   > 
   >Pour que les utilisateurs puissent afficher les courriers électroniques de leurs utilisateurs, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir [Accorder l’accès aux utilisateurs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. Consultez les champs suivants de la section Aperçu . Vous ne pouvez pas modifier les champs suivants :

   | Champ | Description |
   |---|---|
   | Numéro de référence | Il s’agit d’un champ généré automatiquement qui a toujours une valeur unique pour chaque projet. |
   | Date de début prévisionnelle | Il s’agit de la date &quot;en temps réel&quot; du début du travail en fonction des travaux terminés et du travail restant. |
   | Date d&#39;achèvement prévisionnelle | Il s’agit de la date &quot;en temps réel&quot; de fin du projet, basée sur l’état d’avancement des tâches terminées et sur les mises à jour de progression des tâches qui sont soit nouvelles, soit en cours. |
   | Heures prévues | Heures prévues sur le projet. Ces heures sont un total des heures planifiées pour chaque tâche. |
   | Heures effectives | Heures de connexion au projet. Ces heures correspondent au total des heures consignées sur le projet, les tâches ou les problèmes du projet. |
   | Durée prévue | Durée du projet, basée sur la période entre la première date de début planifiée d’une tâche et la dernière date de fin planifiée d’une tâche du projet. |
   | Durée effective | Durée réelle du projet, basée sur la période entre la première date de début réelle d’une tâche et la dernière date de fin réelle d’une tâche du projet. |
   | Date d’entrée | Date et heure de création du projet. |
   | Entré par | Nom de l’utilisateur qui a créé le projet. |
   | Date de dernière mise à jour | Date et heure de la dernière mise à jour du projet. |
   | Dernière mise à jour par | Nom de l’utilisateur qui a mis à jour le projet pour la dernière fois. |
   | Modèle |   |


1. Si votre société a acheté une licence supplémentaire pour le planificateur de scénario Adobe Workfront et que les informations du projet sont publiées à partir d’une initiative liée, passez en revue les informations suivantes sur l’initiative dans la zone du planificateur de scénario :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><b>Champ</b></td> 
      <td><b>Description</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader"><span>Durée de l’initiative</span> </td> 
      <td><span>Durée de l’initiative correspondante lorsque le projet est lié à une initiative. Ce champ n’est pas modifiable.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Date de la dernière publication</span> </td> 
      <td><span>Date à laquelle le projet a été publié pour la dernière fois à partir d’une initiative correspondante.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Date de début de l'initiative</span> </td> 
      <td><span>Premier jour du mois de début de l’initiative, lorsque le projet est lié à une initiative.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Date de fin de l'initiative</span> </td> 
      <td><span>Dernier jour du mois de fin de l’initiative, lorsque le projet est lié à une initiative. </span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Rôles de tâche d’initiative dans les ETR et les Heures</span> </td> 
      <td> <p>Informations sur les rôles d’emploi associés et leur attribution de temps pour l’initiative. Cela inclut :</p> 
       <ul> 
        <li>Nom du rôle de tâche</li> 
        <li>Nombre d’ETR</li> 
        <li> <p>Nombre d’heures pour tous les ETR</p> <p>Vous pouvez estimer le nombre de rôles d’emploi nécessaires à votre plan ou à votre initiative à l’aide d’heures ou d’EPT. </p> <p>Pour plus d’informations, voir <a href="../../../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Créer et modifier des plans dans le planificateur de scénarios</a>. </p> </li> 
       </ul> <p>Conseil : <span>Si le nombre de rôles d’emploi est différent pour chaque mois de l’initiative, ce champ affiche le nombre maximal de rôles requis pour l’initiative. Par exemple, si vous avez besoin d’un consultant pour janvier et d’un consultant pour février, la colonne affiche 2ETR et le nombre d’heures correspondant pour 2 ETR pour tous les mois.</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Pour plus d’informations sur la liaison de projets à des initiatives, voir [Mettre à jour ou créer des projets en publiant des initiatives dans le planificateur de scénarios](../../../scenario-planner/publish-scenarios-update-projects.md).

1. Cliquez sur **Enregistrer les modifications**.
