---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: Modifier un processus de validation
description: Si vous êtes administrateur d’Adobe Workfront ou si vous disposez d’un accès administratif aux processus d’approbation, vous pouvez afficher et modifier tous les processus d’approbation du système.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1953'
ht-degree: 5%

---

# Modifier un processus de validation

Si vous êtes administrateur d’Adobe Workfront ou si vous disposez d’un accès administratif aux processus d’approbation, vous pouvez afficher et modifier tous les processus d’approbation du système.

Si vous êtes administrateur de groupe, vous pouvez visualiser et modifier les processus de validation associés au ou aux groupes que vous gérez.

Pour plus d’informations sur la création de processus de validation, voir [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* Lorsque vous éditez un processus d’approbation globale déjà utilisé, vos modifications affectent tous les objets du système qui y sont déjà associés.
>* Si vous ajoutez un nouvel approbateur à l’étape en cours sur un processus d’approbation qui a déjà commencé sur un objet, le processus de réinitialisation de cet objet et les approbateurs doivent recommencer.
>
>  Cependant, si vous apportez les modifications suivantes à un processus d’approbation qui a déjà démarré sur un objet, ce processus se poursuit sans interruption :
>
>* Ajouter une étape au-delà de l’étape actuelle
>* Ajouter un approbateur supplémentaire avant l’étape en cours

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux processus d’approbation si vous n’êtes pas administrateur système</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Modifier un processus de validation existant

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).
1. (Conditionnel) Si vous modifiez un processus d’approbation au niveau du système, cliquez sur **Traitements** > **Approbations** dans le panneau de gauche.

   Ou

   Si vous modifiez un processus d’approbation au niveau du groupe, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).
   1. Cliquez sur le nom du groupe pour lequel vous souhaitez répertorier ou gérer les processus d’approbation de groupe.
   1. Dans le panneau de gauche, cliquez sur **Approbations**. Vous devrez peut-être cliquer sur **Afficher plus** en premier.

1. Cliquez sur le bouton **Approbations de projet**, **Approbations de tâches** ou **Approbations des problèmes** selon le type de processus de validation que vous souhaitez éditer.

1. Sélectionnez le processus de validation que vous souhaitez modifier, puis cliquez sur **Modifier** en haut de la liste. La boîte de dialogue Modifier le processus de validation s’affiche.

   ![](assets/edit-approval-process-global-area-new.png)

1. Indiquez les informations suivantes dans la zone qui s’affiche :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom du processus d'approbation</td> 
      <td>Saisissez un nom explicite pour le processus de validation. Les utilisateurs voient ce nom lorsqu’ils appliquent le processus d’approbation à un objet, comme décrit dans la section <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associer un processus d’approbation nouveau ou existant au travail</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Saisissez une description du processus de validation. Cela s’affiche dans la variable <b>Approbations</b> dans la section <b>Configuration</b> en regard du nom du processus d’approbation.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Est actif</td> 
      <td> <p>Laissez cette option activée si vous souhaitez que d’autres utilisateurs puissent joindre le processus d’approbation aux projets, tâches et problèmes qu’ils créent. </p> <p>Cette option est activée par défaut.</p> <p>Conseil : Le fait de marquer un processus d’approbation comme inactif s’avère utile lorsque votre entreprise n’a plus besoin de l’utiliser, mais que vous souhaitez conserver des informations historiques sur son utilisation.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ce processus d’approbation peut être utilisé par </td> 
      <td> <p>Si vous souhaitez que le processus d’approbation soit disponible pour les projets, tâches, problèmes et modèles appartenant uniquement à un groupe particulier, commencez à saisir le nom du groupe, puis sélectionnez le nom qui s’affiche :</p> 
       <ul> 
        <li>Si vous êtes administrateur système ou que vous avez un accès administratif aux processus d’approbation, n’importe quel groupe du système apparaît lorsque vous saisissez son nom. <b>Tous les groupes</b> est sélectionné par défaut. </li> 
        <li>Si vous êtes un administrateur de groupe sans accès administratif aux processus de validation, vous pouvez attribuer le processus de validation à n'importe quel groupe que vous gérez lorsque vous saisissez son nom. Le <b>Tous les groupes</b> n’est pas disponible.</li> 
       </ul> <p>Cette option n’est pas disponible pour les processus de validation à usage unique.</p> <p><b>AVERTISSEMENT</b>: Lorsque vous apportez des modifications au processus d’approbation spécifique au groupe, les processus d’approbation existants qui ont déjà été associés à des tâches peuvent changer. Pour plus d’informations sur ces modifications, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Comment les modifications du processus d’approbation et de groupe affectent-elles les processus d’approbation affectés ?</a>.</p> <p>Pour plus d’informations sur la liste et la gestion des processus d’approbation de votre groupe à partir de la page de votre groupe, voir <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Processus de validation au niveau du groupe</a>. </p> <p>Pour plus d’informations sur l’accès administratif aux processus de validation, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Configurez un chemin pour le processus de validation à l’aide des options suivantes.

   Un chemin d’accès permet de spécifier ce qui doit se produire dans le processus d’approbation. Vous créez des étapes dans un chemin pour indiquer qui doit effectuer le travail d’approbation et dans quel ordre.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Démarrer un processus d’approbation lorsque le statut est défini sur</p> </td> 
      <td> <p>Sélectionnez l’état qui déclenchera le processus d’approbation sur les tâches. Lorsqu’une personne met à jour un élément de travail à cet état, son processus d’approbation commence. </p> <p>Le même état ne peut pas être sélectionné pour plusieurs chemins de processus d’approbation.</p> <p>Les états disponibles dépendent de ce qui est sélectionné sous l’option . <b>Cette validation peut être utilisée par</b> (comme expliqué dans le tableau ci-dessus) :</p> 
      <ul> 
      <li> If <b>Tous les groupes</b> est sélectionné, seuls les états verrouillés à l’échelle du système sont disponibles. <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>Si un groupe spécifique est sélectionné, seuls les états disponibles pour ce groupe sont disponibles.</p> </li> 
      </ul> <p>Pour plus d’informations sur le fonctionnement du processus d’approbation avec les états, voir la section <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Comment les processus d’approbation reposent sur les états</a> dans l’article <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Présentation du processus de validation</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom de l'étape</td> 
      <td>(Facultatif) Saisissez un nom décrivant la première étape du chemin. Si vous ne spécifiez pas de nom d’étape, le nom par défaut est <b>Phase 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approbateurs</td> 
      <td> <p>Commencez à saisir le nom de l’utilisateur, de l’équipe ou du rôle de tâche que vous souhaitez désigner comme approbateur pour cette étape, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante. Vous pouvez uniquement ajouter des utilisateurs, des rôles de tâche et des équipes principaux. </p>

   <p><b>CONSEIL</b>:</p>

   <p>Lors de l’ajout d’un utilisateur en tant qu’approbateur, notez l’avatar, le rôle Principal de l’utilisateur ou son adresse électronique pour distinguer les utilisateurs portant des noms identiques. Les utilisateurs doivent être associés à au moins un rôle de tâche pour l’afficher à mesure que vous les ajoutez.</p>
      <p>Pour que les utilisateurs puissent afficher les courriers électroniques de leurs utilisateurs, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Accorder l’accès aux utilisateurs</a></p>.

   <p><b>NOTE</b>:

   L’ajout d’un utilisateur, d’une équipe ou d’un rôle en tant qu’approbateur ne leur accorde pas automatiquement des autorisations sur l’objet associé à cette approbation. Ils reçoivent des autorisations sur l’objet lorsque l’étape d’approbation est déclenchée. Dans le cas contraire, les objets doivent être partagés avec eux avant de pouvoir prendre une décision concernant la validation. </p>
   <p>Vous pouvez également désigner une personne comme approbateur en spécifiant son rôle. Vous pouvez, par exemple, désigner comme approbateur un propriétaire de projet, un parrain de projet, un propriétaire de Portfolio, un propriétaire de programme ou un responsable de projet. Ces options s’affichent automatiquement lorsque vous commencez à saisir du texte.</p> 
      <p><b>IMPORTANT</b>:  
      <ul> 
      <li> Lorsque vous affectez une approbation au parrain du projet et qu’aucune personne n’est désignée comme parrain d’un projet, l’approbation est réaffectée au propriétaire du projet. Si personne n’est désigné comme propriétaire du projet, l’approbation est attribuée à l’administrateur Workfront. </li> 
      <li> Lorsque vous affectez une approbation à un rôle et à une option <b>L’approbateur ne doit pas appartenir à l’équipe de projet.</b> est désactivé, mais aucun rôle de l’équipe de projet ne correspond au rôle lors de l’approbation ; l’approbation est réaffectée au propriétaire du projet. Pour plus d’informations sur les paramètres d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configuration des paramètres d’approbation globaux</a>.
      </li> 
      <li>Lorsque vous affectez une approbation au propriétaire du projet et qu’aucune personne n’est désignée comme propriétaire d’un projet, l’approbation est réaffectée à l’administrateur Workfront principal, comme indiqué dans la section Informations sur le client de la zone Configuration. Pour plus d’informations, voir <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configuration des informations de base pour votre système</a>.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>Lorsque vous attribuez des rôles de tâche en tant qu’approbateurs, tous les utilisateurs associés à ce rôle de tâche qui font également partie de l’équipe de projet peuvent prendre une décision concernant l’approbation. </p> 
      <p>Lorsque vous attribuez une équipe comme approbateur, tout utilisateur de cette équipe peut prendre une décision sur l’approbation. </p> 
      <p>Pour plus d’informations sur l’équipe de projet, voir <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Présentation de l’équipe de projet</a>. Pour plus d’informations sur la validation d’un travail, voir <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Valider le travail </a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">Une seule décision est requise.</td> 
      <td>(S’affiche uniquement si vous ajoutez plusieurs approbateurs à l’étape) Sélectionnez cette option si l’un des approbateurs de l’étape peut approuver ou rejeter l’élément de travail au cours de cette étape. Cette action permet à l’élément de travail de quitter l’étape.  
      <p>Lorsque cette option n’est pas sélectionnée, tous les approbateurs identifiés doivent approuver ou rejeter l’étape (dans n’importe quel ordre) avant que l’élément ne quitte l’étape. Si l’un des approbateurs rejette l’étape, le processus interrompt et recommence afin que les modifications requises puissent être apportées. Ensuite, les approbateurs peuvent valider ou rejeter à nouveau l’étape.</p> 
      <p>Lorsqu’une équipe est désignée comme approbateur, tout membre de l’équipe peut accorder ou refuser une étape.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Ajouter une étape</p> </td> 
      <td>(Facultatif) Ajoutez une autre étape au chemin à l’aide des options expliquées dans les trois lignes ci-dessus. Vous pouvez ajouter autant d’étapes que nécessaire au chemin.</td> 
     </tr>
     <tr> 
      <td role="rowheader"> Choisissez ce qui se passe lorsque la validation est rejetée</td> 
      <td> <p>Sélectionnez l’action que vous souhaitez entreprendre si l’élément de travail est rejeté à n’importe quelle étape du chemin :</p> 
      <ul> <li><strong>Création d’un problème</strong>: (Disponible uniquement pour les processus d’approbation de projet et de tâche) Un problème est créé dans le projet ou la tâche où le processus d’approbation est en cours d’exécution. La ressource affectée par défaut sur la tâche ou le propriétaire du projet est affecté au problème. Par défaut, le nom du problème créé est <strong>Approbation rejetée (nom du projet ou de la tâche)</strong>. Il s’agit d’un problème de rejet, saisi sous la tâche ou le projet, selon le processus d’approbation où le rejet s’est produit.</li> 
      <li> <p><strong>Définir l’état sur</strong>: Sélectionnez l’une des options suivantes :</p> 
      <ul> <li><strong>État précédent</strong>: Le projet, la tâche ou le problème rejeté revient à l’état avant l’état qui active le processus d’approbation.</li> 
      <li> <p><strong>Tout autre état de la liste</strong>: L’objet rejeté passe à l’état que vous choisissez, comme En attente. Vous pouvez choisir l’un des états par défaut ou un état personnalisé que vous avez ajouté à votre système Workfront.</p> <p>Si vous sélectionnez un statut associé à un processus d’approbation, comme le statut Rejeté pour un chemin d’approbation, l’objet rejeté passe au statut sélectionné et est marqué comme « En attente d’approbation ». </p>
      <p>Par exemple, si vous sélectionnez En attente pour le statut Rejeté alors que le statut En attente est associé à un processus d’approbation, le statut de l’objet rejeté devient « En attente d’approbation » et une approbation est nécessaire.</p>    <p>Pour un processus d’approbation à l’échelle du système, seuls les états à l’échelle du système sont disponibles.</p> <p>Pour un processus d’approbation spécifique à un groupe, tous les statuts de groupe sont disponibles. Cela inclut tous les états personnalisés que l’administrateur du groupe a créés spécifiquement pour le groupe, ainsi que tous les états à l’échelle du système. </p> <p>Pour plus d’informations sur le fonctionnement du processus d’approbation avec les états, voir la section <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Comment les processus d’approbation reposent sur les états</a> dans l’article <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Présentation du processus de validation</a>.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Cliquez sur **Ajouter un chemin** pour ajouter un autre chemin au processus d’approbation, en faisant référence à la liste des options de l’étape précédente.

   Le nouveau chemin doit être associé à un autre état. Le chemin se déclenche lorsque l’élément est mis à jour pour afficher cet état. Vous ne pouvez pas avoir deux chemins pour le même état.

1. Cliquer sur **Enregistrer**.
1. (Facultatif) Effectuez l’une des opérations suivantes :

   * Associez le processus d’approbation à des projets, tâches ou problèmes spécifiques sur votre système, comme décrit dans la section [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * En dehors de Workfront, informez les utilisateurs que le processus d’approbation est disponible pour qu’ils puissent l’associer à leurs projets, tâches ou problèmes, comme décrit dans la section [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Créez un autre processus de validation qui sera déclenché si ce processus de validation est rejeté et que l’élément prend un autre statut. Vous pouvez ainsi associer les processus de validation.
