---
title: Création d’un processus d’approbation pour les éléments de travail
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Vous pouvez créer un processus d’approbation que les utilisateurs et utilisatrices peuvent joindre à un élément de travail (projet, tâche, problème, modèle ou tâche de modèle), à un document ou à une épreuve. Un processus d’approbation permet de s’assurer que les personnes cessionnaires désignées pour l’objet vérifient certaines modifications avant la progression de l’objet dans le système.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '2174'
ht-degree: 99%

---

# Créer un processus d’approbation pour les éléments de travail

<!-- Audited: 12/2023 -->

<!--see below the "hidden" content for the redesigned tabs - August 2023-->

Vous pouvez créer un processus d’approbation que les utilisateurs et utilisatrices peuvent joindre à un élément de travail (projet, tâche, problème, modèle ou tâche de modèle), à un document ou à une épreuve. Un processus d’approbation permet de s’assurer que les personnes cessionnaires désignées pour l’objet vérifient certaines modifications avant la progression de l’objet dans le système.

Cet article décrit comment créer un processus d’approbation global au niveau du système ou du groupe pour les éléments de travail (projet, tâche, problème, modèle ou tâche de modèle).

Pour plus d’informations sur les approbations associées aux documents ou aux épreuves, voir les articles suivants :

* [Demander l’approbation de documents](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [Vue d’ensemble du workflow automatisé](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>Les utilisateurs et utilisatrices peuvent également créer un processus d’approbation à usage unique pour un projet, une tâche, un problème, un modèle ou une tâche de modèle pour lesquels des autorisations de gestion leur ont été accordées.
>
>Cet article utilise le terme « processus d’approbation global » pour le différencier du processus d’approbation à usage unique. Un processus d’approbation globale peut être utilisé à plusieurs reprises.
>
>Au niveau du groupe, un processus d’approbation global est limité aux éléments de travail et aux statuts qui appartiennent au groupe.
>
>Pour plus d’informations sur les processus d’approbation à usage unique, voir [Vue d’ensemble du processus d’approbation](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) et [Associer un processus d’approbation nouveau ou existant à un travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouvelle formule : standard </p>
 <p>ou</p> 
<p>Formule actuelle : formule </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Si vous êtes un administrateur ou une administratrice Workfront ou si vous disposez d’un accès administratif aux processus d’approbation, vous pouvez créer un processus d’approbation au niveau du système ou un processus d’approbation au niveau du groupe pour un groupe particulier.</p> 
   <p>Si vous êtes administrateur ou administratrice de groupes, vous pouvez créer des processus d’approbation au niveau du groupe pour les groupes que vous gérez.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un processus d’approbation global au niveau du système ou du groupe pour les éléments de travail

{{step-1-to-setup}}

1. (Le cas échéant) Si vous créez un processus d’approbation au niveau du système, cliquez sur **Processus** > **Approbations** dans le panneau de gauche.

   Ou

   Si vous créez un processus d’approbation au niveau du groupe, cliquez sur **Groupes** ![](assets/groups-icon.png), sur le nom du groupe, puis sur **Approbations**.

   <!--hidden for the new tab redesign - August 2023: 
   ![](assets/approvals-area-in-setup-processes.png)
   -->

1. Sélectionnez l’onglet **Approbations de projets**, **Approbations de tâches**, ou **Approbations de problèmes**.

1. Cliquez sur **Nouveau processus d’approbation**.
1. Spécifiez les informations suivantes dans la zone qui s’affiche :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom du processus d’approbation</td> 
      <td><p>Saisissez un nom explicite pour le processus d’approbation. Les utilisateurs et utilisatrices voient ce nom lors de l’application du processus d’approbation à un objet, comme décrit dans <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associer un processus d’approbation nouveau ou existant à un travail</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td><p>Saisissez une description du processus d’approbation. Cela s’affiche dans la section <b>Approbations</b> dans la zone <b>Configuration</b> à côté du nom du processus d’approbation.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Est active</td> 
      <td> <p>Laissez cette option activée si vous voulez que d’autres personnes puissent joindre le processus d’approbation aux projets, tâches et problèmes qu’elles créent. </p> <p>Cette option est activée par défaut.</p> <p> Conseil : marquer un processus d’approbation comme inactif est utile lorsque votre organisation n’a plus besoin de l’utiliser, mais que vous souhaitez conserver des informations historiques sur son utilisation.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ce processus d’approbation peut être utilisé par </td> 
      <td> <p>Si vous souhaitez que le processus d’approbation soit disponible pour les projets, les tâches, les problèmes et les modèles appartenant uniquement à un groupe particulier, commencez à saisir le nom du groupe, puis sélectionnez le nom lorsqu’il apparaît :</p> 
       <ul> 
       <li>Si vous êtes administrateur ou administratrice système ou si vous disposez d’un accès administratif aux processus d’approbation, vous pouvez voir n’importe quel groupe dans le système lorsque vous saisissez son nom. <b>Tous les groupes</b> est sélectionné par défaut. </li> 
       <li>Si vous êtes un administrateur ou une administratrice de groupes sans accès administratif aux processus d’approbation, vous pouvez attribuer le processus d’approbation à n’importe quel groupe que vous gérez lorsque vous saisissez son nom. L’option <b>Tous les groupes</b> n’est pas disponible.</li> 
       </ul> 
       <p>Cette option n’est pas disponible pour les processus d’approbation à usage unique.</p> 
       <p><b>AVERTISSEMENT</b> : si vous modifiez le processus d’approbation spécifique au groupe, les processus d’approbation existants déjà associés aux éléments de travail peuvent changer. Pour plus d’informations sur ces modifications, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Comment les modifications des groupes et des processus d’approbation affectent les processus d’approbation attribués</a>.</p> 
       <p>Pour plus d’informations sur la manière de répertorier et de gérer les processus d’approbation de votre groupe à partir de sa page, voir <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Processus d’approbation au niveau du groupe</a>. </p> 
       <p>Pour plus d’informations sur l’accès administratif aux processus d’approbation, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder un accès administratif à certaines zones aux utilisateurs et aux utilisatrices</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Configurez un chemin pour le processus d’approbation en utilisant les options suivantes.

   Un chemin est l’endroit où vous spécifiez ce qui doit se passer dans le processus d’approbation. Vous créez des étapes dans un chemin pour indiquer qui doit effectuer le travail d’approbation et dans quel ordre il doit être fait.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Démarrer un processus d’approbation lorsque le statut est défini sur</p> </td> 
      <td> <p>Sélectionnez le statut qui déclenchera le processus d’approbation des éléments de travail. Lorsqu’un élément de travail est mis à jour dans ce statut, le processus d’approbation démarre. </p> <p>Le même statut ne peut pas être sélectionné pour plusieurs processus d’approbation.</p> <p>Les statuts disponibles sont basés sur ce qui est sélectionné sous l’option <b>Ce processus d’approbation peut être utilisé par</b> (expliqué dans le tableau ci-dessus) :</p> 
       <ul> 
       <li> Si l’option <b>Tous les groupes</b> est sélectionnée, seuls les statuts de l’ensemble du système sont disponibles.
       <li> <p>Si un groupe spécifique est sélectionné, seuls les statuts disponibles pour ce groupe le sont.</p> </li> 
       </ul> <p>Pour plus d’informations sur le fonctionnement du processus d’approbation avec les statuts, voir la section <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Comment les processus d’approbation s’appuient sur les statuts</a> dans l’article <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Vue d’ensemble du processus d’approbation</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom de l’étape</td> 
      <td>(Facultatif) Saisissez un nom décrivant la première étape du chemin. Si vous ne spécifiez pas de nom d’étape, le nom par défaut est <b>Étape 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approbateurs</td> 
      <td> <p>Commencez à saisir le nom de l’utilisateur ou de l’utilisatrice, de l’équipe ou de la fonction que vous souhaitez désigner comme personne responsable de l’approbation pour cette étape, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante. Vous ne pouvez ajouter que des personnes, des <span>fonctions</span> et des équipes actives. </p>

   <p><b>CONSEIL</b> :</p>

   <p>lorsque vous ajoutez un utilisateur ou une utilisatrice comme personne responsable de l’approbation, vérifiez son avatar, son rôle principal ou son adresse e-mail pour distinguer les doublons. Les personnes doivent être associées à au moins une fonction pour l’afficher à mesure que vous les ajoutez.</p>
      <p>Pour pouvoir voir les adresses e-mail des utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, consultez <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Accorder l’accès aux utilisateurs et utilisatrices</a>. </p>

   <p><b>NOTE</b> :

   l’ajout d’un utilisateur ou d’une utilisatrice, d’une équipe ou d’un rôle en tant que responsable de l’approbation ne lui donne pas automatiquement des droits sur l’objet associé à cette approbation. Les autorisations sur l’objet leur sont accordées lorsque l’étape d’approbation est déclenchée. Sinon, les objets doivent être partagés avant qu’une décision d’approbation ne puisse être prise. </p> <p>Vous pouvez également désigner une personne comme responsable de l’approbation en précisant sa fonction spécifique. Par exemple, une personne peut être affectée comme responsable de l’approbation, qu’elle soit gestionnaire, propriétaire ou sponsor d’un projet, d’un programme ou d’un portfolio. Ces options apparaissent automatiquement lorsque vous commencez à saisir du texte.</p>

   <p><b>IMPORTANT</b> :  
       <ul> 
       <li> <p>si aucune personne sponsor de projet n’est désignée et que vous accordez une approbation à la personne sponsor du projet, celle-ci est alors accordée à la personne propriétaire du projet. Si aucune personne propriétaire de projet n’est désignée, l’approbation est accordée à la personne chargée de l’administration de Workfront. </p> </li> 
      </ul> 
       <ul> 
       <li> <p>Lorsque vous accordez une approbation à un rôle et que l’option Personne chargée de l’approbation ne faisant pas partie de l’équipe de projet (pour les processus d’approbation qui incluent un rôle) est désactivée mais qu’aucun rôle de l’équipe de projet ne correspond au rôle de l’approbation, l’approbation est accordée à la personne propriétaire du projet<b></b>. Pour plus d’informations sur les paramètres d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurer les paramètres d’approbation globaux</a>.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>Lorsque vous accordez une approbation à la personne propriétaire du projet et qu’il n’existe pas de personne propriétaire de projet, l’approbation est alors accordée à l’équipe principale d’administration de Workfront, comme indiqué dans la section Infos client de la zone de configuration. Pour plus d’informations, voir <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configurer les informations de base de votre système</a>.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>Vous pouvez répéter ce processus pour ajouter, à cette étape, plusieurs personnes chargées de l’approbation. Une étape unique peut inclure une combinaison d’utilisateurs et d’utilisatrices, d’équipes et de fonctions en tant que responsables de l’approbation. Il n’y a pas de limite au nombre de personnes chargées de l’approbation que vous pouvez ajouter à une étape.</p> <p><b>IMPORTANT</b> :  <p>quand des fonctions se voient accorder une responsabilité d’approbation, tous les utilisateurs et utilisatrices ayant cette fonction et faisant partie de l’équipe de projet peuvent prendre une décision d’approbation. </p> <p>Lorsque vous désignez une équipe comme responsable de l’approbation, chaque personne de cette équipe peut prendre une décision d’approbation. </p> <p>Pour plus d’informations sur l’équipe de projet, voir <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Vue d’ensemble de l’équipe de projet</a>. Pour plus d’informations sur l’approbation du travail, voir <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Approuver du travail</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Une seule décision est requise <br> <br>(ne s’affiche que si vous ajoutez à l’étape plusieurs personnes chargées de l’approbation). </td> 
      <td> <p>Sélectionnez cette option si l’une des personnes chargées de l’approbation de l’étape peut approuver ou rejeter le document de travail au cours de cette étape. Cette action permet à l’élément de travail de quitter l’étape. </p> <p>Si cette option n’est pas sélectionnée, tous les approbateurs et approbatrices identifiés doivent approuver ou rejeter l’étape (dans n’importe quel ordre) avant que l’élément ne quitte l’étape. Si l’une des personnes approbatrices rejette l’étape, le processus s’interrompt et recommence afin que les modifications nécessaires puissent être apportées. Les approbateurs et approbatrices peuvent ensuite approuver ou rejeter à nouveau l’étape.</p> <p>Si une équipe est désignée comme approbatrice, toute personne membre de l’équipe peut approuver ou rejeter une étape.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Ajouter une étape</p> </td> 
      <td><p>(Facultatif) Ajoutez une autre étape au chemin d’accès, à l’aide des options décrites dans les trois lignes ci-dessus. Vous pouvez ajouter autant d’étapes au chemin que nécessaire.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sélectionnez ce qui se passe en cas de rejet de l’approbation :</p> </td> 
      <td> <p>Sélectionnez l’action à entreprendre si l’élément de travail est refusé à l’une des étapes du chemin d’accès :</p> 
       <ul> 
       <li><b>Créer un problème : (disponible uniquement pour les processus d’approbation des projets et des tâches) un problème est créé dans le projet ou la tâche où le processus d’approbation est en cours. </b> La ressource affectée par défaut à la tâche, ou la personne propriétaire du projet, est affectée au problème. Par défaut, le nom du problème créé est Approbation refusée (&lt;Project or Task Name&gt;). <b></b> Il s’agit d’un problème de rejet, saisi sous la tâche ou le projet, en fonction du processus d’approbation dans lequel le rejet s’est produit.</li> 
       <li> <p><b>Définir le statut sur</b> : choisissez l’une des options suivantes :</p> 
       <ul> 
       <li><b>Statut précédent</b> : le projet, la tâche ou le problème rejeté revient au statut antérieur à celui qui active le processus d’approbation.</li> 
       <li><p><b>Tout autre statut dans la liste : l’objet refusé passe au statut de votre choix, par exemple Suspendu. </b> Vous pouvez choisir l’un des statuts par défaut ou un statut personnalisé que vous avez ajouté à votre système Workfront.</p>
       <p>Si vous sélectionnez un statut associé à un processus d’approbation en tant que statut de rejet, l’objet rejeté passe au statut sélectionné et sera marqué comme « Approbation en attente ».</p> 
       <p> Par exemple, si vous définissez le statut de rejet sur Suspendu alors que le statut Suspendu est associé à un processus d’approbation, le statut de l’objet rejeté devient « Suspendu - Approbation en attente » et une approbation est alors nécessaire.</p>

   </tr> 
    </tbody> 
   </table>

1. (Facultatif) Cliquez sur **Ajouter un chemin** pour ajouter un autre chemin au processus d’approbation, en vous référant à la liste d’options de l’étape précédente.

   Le nouveau chemin doit être associé à un autre statut. Le chemin se déclenche lorsque l’élément est mis à jour pour afficher ce statut. Il ne peut y avoir deux chemins pour le même statut.

1. Cliquer sur **Enregistrer**.
1. Maintenant que le processus d’approbation est créé, poursuivez avec l’une des étapes suivantes :

   * Associez le processus d’approbation à des projets, des tâches ou des problèmes spécifiques dans votre système, comme décrit dans [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * En dehors de Workfront, informez les utilisateurs et utilisatrices que le processus d’approbation est disponible et qu’ils peuvent l’associer à leurs projets, tâches ou problèmes, comme décrit dans [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Créez un autre processus d’approbation qui est déclenché si ce processus d’approbation est rejeté et que l’élément adopte un autre statut. Cela vous permet de relier les processus d’approbation entre eux.

Pour plus d’informations sur la modification d’un processus d’approbation, voir [Modifier un processus d’approbation](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

## Associer un processus d’approbation à un élément de travail

Si vous souhaitez créer un processus d’approbation pour un élément de travail (projet, tâche ou problème), vous devez procéder comme suit :

1. Créez d’abord le processus d’approbation.
1. Créez l’élément de travail.
1. Associez le processus d’approbation à l’élément de travail.

Pour savoir comment associer un processus d’approbation à un élément de travail, voir [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Tout utilisateur ou utilisatrice de Workfront disposant d’autorisations de gestion d’un projet, d’une tâche ou d’un problème peut créer des processus d’approbation à usage unique qui ne seront utilisés que pour l’objet où ils ont été créés. Pour plus d’informations, voir [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Permettre aux utilisateurs et utilisatrices de modifier les processus d’approbation globaux pour un seul élément de travail

Par défaut, les utilisateurs et utilisatrices disposant d’autorisations de gestion des projets, des tâches et des problèmes peuvent créer des processus d’approbation à usage unique. Pour plus d’informations sur l’ajout de processus d’approbation à usage unique aux projets, tâches et problèmes, voir la section [Associer un processus d’approbation à usage unique à un projet, une tâche, un problème, un modèle ou une tâche de modèle](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) dans l’article [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

Les utilisateurs et utilisatrices peuvent également modifier les paramètres d’un processus d’approbation global associé à un élément de travail. Ces modifications n’affectent que le projet, la tâche ou le problème associé au processus d’approbation à l’échelle du système. Pour plus d’informations, voir la section [Modifier un processus d’approbation global pour l’utiliser sur un objet spécifique](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process) dans l’article [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
