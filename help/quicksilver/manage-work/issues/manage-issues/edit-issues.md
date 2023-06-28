---
product-area: projects
navigation-topic: manage-issues
title: Modification des problèmes
description: Vous pouvez modifier les informations sur les problèmes que vous avez créés ou que d’autres utilisateurs ont créés s’ils ont partagé les problèmes avec vous.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: 716b5a151585aa314cd9db67237d2ed085e817c1
workflow-type: tm+mt
source-wordcount: '2467'
ht-degree: 3%

---

# Modification des problèmes

Vous pouvez modifier les informations sur les problèmes que vous avez créés ou que d’autres utilisateurs ont créés s’ils ont partagé les problèmes avec vous.

Vous pouvez modifier une seule publication ou modifier des problèmes dans une liste. Pour plus d’informations sur la modification des problèmes dans une liste, voir [Modifier les problèmes dans une liste](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

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
   <td> <p>Requête ou supérieure</p> <p>Vérification d’une licence ou d’une licence supérieure pour modifier des problèmes dans la section Problèmes d’une tâche ou d’un projet</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux problèmes de votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Accorder l’accès aux problèmes</a>. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Attribuez des autorisations à un problème pour le modifier dans la zone Détails du problème. </p> <p>Gérer les autorisations d’un problème pour le modifier dans la zone Modifier le problème</p> <p> Pour plus d’informations sur l’octroi d’autorisations aux problèmes, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Partage d’un problème </a></p> <p>Pour plus d’informations sur la demande d’autorisations supplémentaires, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Limites lors de la modification de problèmes

Certaines restrictions peuvent vous empêcher de modifier des problèmes.

* Vous ne pouvez pas modifier les problèmes qui se trouvent dans un processus d’approbation. Vous pouvez uniquement consigner l’heure ou mettre à jour l’état sur un problème qui se trouve dans Autorisation en attente.
* Vous pouvez modifier et ajouter des documents aux problèmes d’un projet dont l’état est Terminé, Mort ou En attente d’approbation est uniquement lorsque votre administrateur Workfront ou un administrateur de groupe a activé cette fonctionnalité dans la zone Préférences du projet. Pour plus d’informations sur la définition des préférences de projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Modification d’un seul problème

Vous pouvez modifier un problème à l’aide des zones Modifier le problème ou Détails du problème . Les étapes suivantes décrivent la modification d’un problème dans la zone Modifier le problème.

1. Accédez au **Menu Principal**.
1. Cliquez sur **Projets**, puis cliquez sur le nom d’un projet pour l’ouvrir.
1. (Facultatif) Cliquez sur **Tâches** , puis cliquez sur le nom d’une tâche pour l’ouvrir.
1. Cliquez sur **Problèmes** dans le panneau de gauche.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. (Facultatif) Pour modifier des informations limitées sur un problème, cliquez sur **Détails du problème** dans le panneau de gauche.

   ![](assets/qs-issue-details-icon-highlighted-and-expanded-on-issue-350x206.png)

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront ou votre administrateur de groupe a modifié votre modèle de mise en page, les champs de la zone Détails du problème peuvent être réorganisés ou non. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Pour modifier les informations de la section Détails , procédez comme suit :

   1. (Facultatif) Cliquez sur le **Réduire tout** dans le coin supérieur droit pour réduire toutes les zones.
   1. (Facultatif et conditionnel) Lorsqu’une zone est réduite, cliquez sur le bouton **flèche pointant vers la droite** ![](assets/right-pointing-arrow.png) en regard de chaque zone pour développer la zone à modifier.
   1. (Facultatif) Pour joindre un formulaire personnalisé, commencez à saisir le nom d’un formulaire dans le champ **Ajouter un formulaire personnalisé** puis sélectionnez-la lorsqu’elle s’affiche dans la liste, puis cliquez sur **Enregistrer les modifications**.
   1. (Facultatif) Cliquez sur le **Exporter** icon ![](assets/export.png) pour exporter les informations d’aperçu et de formulaires personnalisés vers un fichier de PDF, cliquez sur **Exporter**. Sélectionnez l’une des options suivantes :

      * Sélectionner tout (s’affiche uniquement lorsqu’au moins un formulaire personnalisé est joint)
      * Vue d’ensemble
      * Nom d’un ou de plusieurs formulaires personnalisés

      Le fichier du PDF est téléchargé sur votre ordinateur.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Pour plus d’informations, voir [Exportation de formulaires personnalisés et de détails d’objet](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

   Pour plus d’informations sur les champs visibles dans la section Détails du problème, continuez à modifier le problème dans la zone Modifier le problème comme décrit ci-dessous.

1. Pour modifier toutes les informations relatives à un problème, sélectionnez-le dans une liste, puis cliquez sur **Modifier** en haut de la liste

   Ou

   Cliquez sur le nom d’un problème dans une liste, puis cliquez sur le bouton **Plus** en regard du nom du problème, puis **Modifier.**

   Le **Modifier le problème** s’affiche.

   >[!IMPORTANT]
   >
   >Pour afficher le lien Modifier, vous devez disposer des autorisations de gestion du problème.

   Tous les champs de problème sont disponibles dans la zone Modifier le problème et sont regroupés par zones répertoriées dans le panneau de gauche.

1. Pensez à spécifier des informations dans l’une des sections suivantes :

   * [Nom de l&#39;événement](#issue-name)
   * [Vue d’ensemble](#overview)
   * [Affectations](#assignments)
   * [Formulaires personnalisés](#Custom%C2%A0F)
   * [Paramètres](#settings)

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront configure le modèle de mise en page, les champs de la zone Modifier le problème peuvent être différents dans votre environnement. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
   >
   >La plupart des champs répertoriés dans les sections ci-dessous sont également accessibles à partir de la zone Nouveau problème lorsque vous créez un problème. Les sections sous lesquelles se trouvent les champs ne correspondent pas à la zone Nouveau problème. Pour plus d’informations sur la création de problèmes, voir [Création de problèmes](../../issues/manage-issues/create-issues.md).

### Nom de l&#39;événement {#issue-name}

1. Commencez à modifier un problème comme décrit ci-dessus.
1. Cliquez sur **Nom du problème**.

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. Mettez à jour le **Nom du problème** champ .
1. Cliquez sur **Enregistrer** ou continuez à modifier les sections suivantes.

### Vue d’ensemble {#overview}

1. Commencez à modifier un problème comme décrit ci-dessus.
1. Cliquez sur **Présentation**.

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. Mettez à jour ou consultez l’un des champs du tableau suivant :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td> <p>Ajoutez des informations supplémentaires sur le problème.</p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader">Section d’informations de base</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Statut</td> 
      <td> <p>Sélectionnez l’état du problème. Pour plus d’informations sur les états des problèmes, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Accéder à la liste des statuts des problèmes système</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorité</td> 
      <td> <p>Il s’agit d’un indicateur visuel qui vous permet de hiérarchiser les problèmes.</p> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Aucun</strong> </p> </li> 
        <li> <p><strong>Faible</strong> </p> </li> 
        <li> <p><strong>Normal</strong> </p> </li> 
        <li> <p><strong>Élevé</strong> </p> </li> 
        <li> <p><strong>Urgent</strong> </p> </li> 
       </ul> <p>Selon les préférences du projet sélectionnées par votre administrateur Workfront, les noms des priorités peuvent être différents pour vous. Pour plus d’informations sur la modification des priorités, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Créer et personnaliser des priorités</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gravité</td> 
      <td> <p>Ceci est un indicateur visuel qui indique la gravité du problème décrit dans le problème. Les problèmes de gravité sont spécifiques. Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p style="font-weight: bold;">Décoratif</p> </li> 
        <li> <p style="font-weight: bold;">Cause de la confusion</p> </li> 
        <li> <p style="font-weight: bold;">Bogue qui a une solution</p> </li> 
        <li> <p style="font-weight: bold;">Bogue sans solution</p> </li> 
        <li> <p style="font-weight: bold;">Erreur fatale</p> </li> 
       </ul> <p>Selon les préférences du projet sélectionnées par l’administrateur de Workfront, les noms des ruptures peuvent être différents pour vous. Pour plus d’informations sur la modification des tailles, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">Création ou personnalisation des gravité de problème</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Saisissez un lien Web qui renvoie aux informations sur le problème.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type</td> 
      <td> <p>Selon les Propriétés de la file d’attente sélectionnées par votre chef de projet dans la zone Détails de la file d’attente du projet, vous pouvez peut-être spécifier le type de problème. Sélectionnez l’une des options suivantes dans le <b>Type</b> menu déroulant : </p> 
       <ul> 
        <li> <p><strong>Rapport sur les bogues</strong> </p> </li> 
        <li> <p><strong>Modifier l'ordre</strong> </p> </li> 
        <li> <p><strong>Problème</strong> </p> </li> 
        <li> <p><strong>Demande</strong> </p> </li> 
       </ul> <p>Selon les préférences du projet sélectionnées par votre administrateur Workfront, les noms des types de problèmes peuvent être différents pour vous.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Contact principal</td> 
      <td>Par défaut, le contact Principal est le créateur du problème. Pour le modifier, commencez à saisir le nom de tout utilisateur principal dans Workfront, puis sélectionnez-le dans la liste. Un problème ne peut avoir qu’un seul contact Principal.<br> Si vous modifiez le contact Principal, le contact Principal d’origine a toujours l’accès Gérer au problème. Lorsque vous partagez un problème, vous devez supprimer manuellement cet accès de la zone Accès au problème .

   <b>CONSEIL</b>

   Lors de l’ajout d’un utilisateur Contact Principal, notez l’avatar, le rôle Principal de l’utilisateur et son adresse électronique pour faire la distinction entre les utilisateurs portant des noms identiques. Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher à mesure que vous les ajoutez.


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date et heure de validation</td> 
      <td> <p>Il s’agit de la date à laquelle la personne désignée du problème estime que le problème sera terminé. Seuls les cessionnaires peuvent modifier ce champ.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date de début planifiée</td> 
      <td>Par défaut, la Date de début planifiée correspond à la date et à l’heure de création du problème. Vous pouvez mettre à jour la variable <strong>Date de début planifiée</strong> du problème. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date et heure d’achèvement prévues</td> 
      <td> Par défaut, la date d’achèvement planifiée est de 24 heures à partir de la date de début planifiée par défaut. Par défaut, les problèmes ont une durée d’1 jour. Vous pouvez mettre à jour la variable <strong>Date d’achèvement prévue</strong> du problème.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date et heure de début réelles</td> 
      <td>La date de début réelle est automatiquement renseignée lorsque vous définissez l’état du problème sur <strong>En cours</strong>. Vous pouvez mettre à jour la variable <strong>Date de début réelle</strong> du problème. Vous pouvez mettre à jour manuellement la date, si nécessaire. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Date et heure de fin réelles</td> 
      <td>La date d’achèvement réelle est automatiquement renseignée lorsque vous définissez l’état du problème sur <strong>Fermé</strong> ou<strong>Résolu</strong>. Vous pouvez mettre à jour la variable <strong>Date d’achèvement réelle</strong> pour le problème. Vous pouvez mettre à jour manuellement la date, si nécessaire.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Résolu par</td> 
      <td> <p>Cela indique si le problème est résolu par un autre objet. Vous pouvez choisir si ce problème est résolu par une tâche, un projet ou un autre problème dans le menu déroulant, puis commencer à saisir le nom de la tâche, du projet ou du problème qui résoudra le problème. Sélectionnez-le lorsqu’il apparaît dans la liste.</p>

   <b>NOTE</b>

   Lorsque vous sélectionnez un objet pour résoudre un problème, l’état du problème est lié à l’état de l’objet de résolution et ne peut pas être modifié sur le problème. Pour plus d’informations sur la résolution d’objets, voir <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Présentation de la résolution et des objets résolvables </a>.

   <b>CONSEIL</b>

   Lorsque l’administrateur de votre système ou de votre groupe ajoute le champ &quot;Résolu par&quot; à un en-tête personnalisé de problème, le champ devient &quot;Résolution du problème&quot;, &quot;Résolution de la tâche&quot; ou &quot;Résolution du projet&quot; lorsqu’un objet de résolution est associé au problème.

   Vous ne pouvez pas modifier ce champ lorsqu’il s’affiche dans l’en-tête du problème. Pour plus d’informations sur la personnalisation des en-têtes de problème, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">Personnalisation des en-têtes d’objet à l’aide d’un modèle de mise en page </a>
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">Résolution d’un problème, résolution d’une tâche ou résolution d’un projet</td> 
      <td>Nom associé de la publication, de la tâche ou du problème qui résout le problème.  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">Ceci résout</td> 
      <td>Le nom associé du problème qui se termine lorsque le problème auquel vous accédez est résolu.  </td> 
     </tr>


   </tbody> 
   </table>





1. Cliquez sur **Enregistrer** ou continuez à modifier les sections suivantes.

#### Affectations {#assignments}

1. Commencez à modifier le problème comme décrit ci-dessus.
1. Cliquez sur **Affectations** dans le panneau de gauche.

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. Cliquez sur **Recherche de personnes, de rôles et d’équipes** et commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe que vous souhaitez affecter à la tâche, puis cliquez dessus ou appuyez sur Entrée lorsqu’il s’affiche dans la liste.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >Si le nom de l’utilisateur contient un caractère spécial, vous devez l’inclure dans le champ de recherche.

   >[!TIP]
   >
   >Vous pouvez affecter plusieurs utilisateurs, rôles de tâche ou équipes. Vous ne pouvez affecter que des utilisateurs, des rôles de tâche et des équipes principaux.
   >
   >
   >Si un utilisateur, un rôle de tâche ou une équipe a été affecté avant d’être désactivé, il reste attribué à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
   >
   >* Réaffectez l’élément de travail aux principales ressources.
   >* Associez les utilisateurs d’une équipe désactivée à une équipe principale et réaffectez l’élément de travail à l’équipe principale.

1. (Facultatif) Indiquez si une personne désignée est la personne désignée Principale sur le problème, en pointant la souris sur le nom de la personne désignée et en cliquant sur **Rendre Principal**. Une équipe ne peut pas être la Principale personne désignée pour un problème.
1. Mettez à jour les champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Heures prévues</td> 
      <td> <p>Il s’agit de la durée réelle requise par les personnes désignées de la question pour la terminer. Saisissez le nombre d’heures planifiées pour le problème.<br></p> <p>Remarque : La modification des heures planifiées de la publication ne modifie pas la date d’achèvement prévue de la publication. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Rôle du cessionnaire</td> 
      <td> <p>Sélectionnez un rôle dans la <strong>Le rôle du cessionnaire</strong> menu déroulant lorsque vous avez sélectionné une personne comme personne désignée. Il s’agit du rôle que la personne désignée peut remplir sur ce problème. </p> <p><b>CONSEIL</b>

   Seuls les rôles de tâche associés à chaque personne désignée dans son profil s’affichent dans le menu déroulant.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer** ou continuez à modifier les sections suivantes.

### Forms personnalisée

1. Commencez à modifier un problème comme décrit ci-dessus.
1. Cliquez sur **Forms personnalisée**.

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. Dans le **Ajouter un formulaire personnalisé** , sélectionnez le ou les formulaires personnalisés à associer au problème. Vous devez créer les formulaires personnalisés avant qu’ils ne soient disponibles pour la sélection dans ce champ. Seuls les principaux formulaires personnalisés s’affichent dans la liste. Pour plus d’informations sur la création de formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Vous pouvez ajouter jusqu’à dix formulaires personnalisés à un problème.

1. (Conditionnel) Si vous avez joint un formulaire personnalisé au problème, modifiez les champs du formulaire. Vous devez spécifier tous les champs requis avant de pouvoir enregistrer le problème.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront définit les autorisations pour les sections de votre formulaire personnalisé, tout le monde ne peut pas afficher ou modifier les mêmes champs sur un formulaire personnalisé donné. Les autorisations de modification des champs d’une section d’un formulaire personnalisé dépendent des autorisations dont vous disposez sur le problème lui-même. Pour plus d’informations sur la définition des autorisations sur les sections d’un formulaire personnalisé, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Pour plus d’informations sur la définition des autorisations de problème, voir [Partage d’un problème](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. Cliquez sur **Enregistrer** ou continuez à modifier la section suivante.

### Paramètres {#settings}

1. Commencez à modifier un problème comme décrit ci-dessus.
1. Cliquez sur **Paramètres**.

   ![](assets/settings-section-edit-issue-box-nwe-350x240.png)

   Mettez à jour les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processus d'approbation</td> 
      <td> 
       <div> 
       <p>Sélectionnez un processus d’approbation à associer au problème. Votre administrateur Workfront doit définir des processus d’approbation au niveau du système avant de pouvoir les associer à des problèmes. Utilisateurs disposant d’un accès administratif aux processus de validation <span> Vous pouvez également créer des processus d’approbation spécifiques à un groupe.</span>Pour plus d’informations sur la création de processus d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Créer un processus d’approbation pour les tâches</a>. </p> 
       <p>Tenez compte des points suivants lors de l’ajout de processus de validation : </p> 
       <ul> 
       <li>Seuls les principaux processus de validation s'affichent dans la liste. </li> 
       <li> <p>Les processus de validation à l’échelle du système et spécifiques aux groupes s’affichent dans la liste. Un processus de validation associé à un groupe autre que celui du projet ne s’affiche pas dans la liste.</p> <p>Important : Si le groupe du projet change, le processus d’approbation spécifique au groupe devient un processus d’approbation à usage unique. Pour plus d’informations sur la façon dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Comment les modifications du processus d’approbation et de groupe affectent-elles les processus d’approbation affectés ?</a>. </p> </li> 
       <li> <p>Vous pouvez définir des processus d’approbation par défaut qui seront automatiquement associés aux problèmes lors de la création de files d’attente de demandes ou de rubriques de files d’attente. Pour plus d’informations sur la mise à jour des détails de la file d’attente, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Création d’une file d’attente de requête</a>. Pour plus d’informations sur la création de rubriques de file d’attente, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Création de rubriques de file d’attente</a>. </p> </li> 
       <li>Lorsque des problèmes de modification en masse se produisent, les scénarios suivants se présentent : 
       <ul> 
       <li><p>Lorsque vous sélectionnez plusieurs problèmes dans le même groupe, les processus d’approbation au niveau du système et spécifiques au groupe s’affichent dans ce champ.</p></li> 
       <li><p>Lorsque vous sélectionnez plusieurs problèmes de différents groupes, seuls les processus de validation au niveau du système s’affichent dans ce champ.</p></li> 
       <li><p>Lorsque l’un des problèmes est associé à un processus d’approbation à usage unique, celui-ci est remplacé par le processus d’approbation au niveau du système ou du groupe que vous sélectionnez. </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications de rappel</td> 
      <td> <p>Cochez la case correspondant aux notifications de rappel que vous souhaitez joindre à ce problème. Toutes les notifications de rappel pour les problèmes s’affichent. Votre administrateur Workfront doit configurer les notifications de rappel avant de pouvoir les sélectionner en cas de problème. Pour plus d’informations sur la configuration des notifications de rappel, voir <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configuration des notifications de rappel</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer.**

## Modification d’un problème dans l’en-tête du problème (limité)

Vous pouvez modifier un nombre limité d’informations dans l’en-tête de la publication.

L’administrateur du système ou du groupe peut personnaliser les champs affichés dans l’en-tête du problème. Pour plus d’informations, voir [Personnalisation des en-têtes d’objet à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

![](assets/issue-header-350x19.png)

Par défaut, les champs suivants sont inclus dans l’en-tête du problème :

* Nom de l’événement
* Pourcentage d’achèvement
* Affectations
* Date et heure d’achèvement prévues
* Statut
* Prenez des décisions d’approbation si vous êtes défini comme approbateur dans un processus d’approbation actuel.
