---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: Modification d’un processus d’approbation
description: Si vous êtes administrateur ou administratrice Adobe Workfront ou si vous disposez d’un accès administratif aux processus d’approbation, vous pouvez voir et modifier tous les processus d’approbation du système.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '1950'
ht-degree: 99%

---

# Modifier un processus d’approbation

Si vous êtes administrateur ou administratrice Adobe Workfront ou si vous disposez d’un accès administratif aux processus d’approbation, vous pouvez voir et modifier tous les processus d’approbation du système.

Si vous êtes administrateur ou administratrice de groupes, vous pouvez voir et modifier les processus d’approbation associés au(x) groupe(s) que vous gérez.

Pour plus d’informations sur la création de processus d’approbation, voir [Créer un processus d’approbation pour des éléments de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* Lorsque vous modifiez un processus d’approbation global déjà utilisé, vos modifications affectent tous les objets du système qui y sont associés.
>* Si vous ajoutez un nouvel approbateur ou une nouvelle approbatrice à l’étape en cours d’un processus d’approbation qui a déjà commencé pour un objet, le processus de cet objet est réinitialisé et les approbateurs et approbatrices doivent recommencer.
>
>  Toutefois, si vous apportez les modifications suivantes dans un processus d’approbation qui a déjà commencé pour un objet, ce processus se poursuit sans interruption :
>
>* Ajouter une étape après l’étape actuelle
>* Ajouter un approbateur ou une approbatrice supplémentaire avant l’étape actuelle

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès administratif aux processus d’approbation si vous n’êtes pas administrateur ou administratrice du système</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Modifier un processus d’approbation existant

{{step-1-to-setup}}

1. (Le cas échéant) Si vous modifiez un processus d’approbation au niveau du système, cliquez sur **Processus** > **Approbations** dans le panneau de gauche.

   Ou

   Si vous modifiez un processus d’approbation au niveau du groupe, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).
   1. Cliquez sur le nom du groupe pour lequel vous souhaitez répertorier ou gérer les processus d’approbation de groupe.
   1. Dans le panneau de gauche, cliquez sur **Approbations**. Il se peut que vous deviez d’abord cliquer sur **Afficher plus**.

1. Cliquez sur l’onglet **Approbations de projets**, **Approbations de tâches**, ou **Approbations de problèmes**, en fonction du type de processus d’approbation que vous souhaitez modifier.

1. Sélectionnez le processus d’approbation que vous souhaitez modifier, puis cliquez sur **Modifier** en haut de la liste. La boîte de dialogue Modifier le processus d’approbation s’affiche.

   ![](assets/edit-approval-process-global-area-new.png)

1. Spécifiez les informations suivantes dans la zone qui s’affiche :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom du processus d'approbation</td> 
      <td>Saisissez un nom explicite pour le processus d’approbation. Les utilisateurs et utilisatrices voient ce nom lorsqu’ils appliquent le processus d’approbation à un objet, comme décrit dans <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associer un processus d’approbation nouveau ou existant au travail</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Saisissez une description du processus d’approbation. Elle s’affiche dans la section <b>Approbations</b> dans la zone <b>Configuration</b> à côté du nom du processus d’approbation.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Est active</td> 
      <td> <p>Laissez cette option activée si vous voulez que d’autres personnes puissent attacher le processus d’approbation aux projets, tâches et problèmes qu’elles créent. </p> <p>Cette option est activée par défaut.</p> <p>Conseil : marquer un processus d’approbation comme inactif est utile lorsque votre organisation n’a plus besoin de l’utiliser, mais que vous souhaitez conserver des informations historiques sur son utilisation.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ce processus d’approbation peut être utilisé par </td> 
      <td> <p>Si vous souhaitez que le processus d’approbation soit disponible pour les projets, les tâches, les problèmes et les modèles appartenant uniquement à un groupe particulier, commencez à saisir le nom du groupe, puis sélectionnez le nom lorsqu’il apparaît :</p> 
       <ul> 
        <li>Si vous êtes administrateur ou administratrice système ou si vous disposez d’un accès administratif aux processus d’approbation, vous pouvez voir n’importe quel groupe dans le système lorsque vous saisissez son nom. <b>Tous les groupes</b> est sélectionné par défaut. </li> 
        <li>Si vous êtes un administrateur ou une administratrice de groupes sans accès administratif aux processus d’approbation, vous pouvez attribuer le processus d’approbation à n’importe quel groupe que vous gérez lorsque vous saisissez son nom. L’option <b>Tous les groupes</b> n’est pas disponible.</li> 
       </ul> <p>Cette option n’est pas disponible pour les processus d’approbation à usage unique.</p> <p><b>AVERTISSEMENT</b> : lorsque vous modifiez le processus d’approbation spécifique au groupe, les processus d’approbation existants qui ont déjà été associés aux éléments de travail peuvent changer. Pour plus d’informations sur ces modifications, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Comment les modifications des groupes et des processus d’approbation affectent les processus d’approbation attribués</a>.</p> <p>Pour plus d’informations sur la manière de répertorier et de gérer les processus d’approbation de votre groupe à partir de sa page, voir <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Processus d’approbation au niveau du groupe</a>. </p> <p>Pour plus d’informations sur l’accès administratif aux processus d’approbation, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones</a>.</p> </td> 
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
      <td> <p>Sélectionnez le statut qui déclenchera le processus d’approbation des éléments de travail. Lorsqu’un élément de travail est mis à jour dans ce statut, le processus d’approbation démarre. </p> <p>Le même statut ne peut pas être sélectionné pour plusieurs processus d’approbation.</p> <p>Les statuts disponibles sont basés sur ce qui est sélectionné dans l’option <b>Cette approbation peut être utilisée par</b> (expliquée dans le tableau ci-dessus) :</p> 
      <ul> 
      <li> Si l’option <b>Tous les groupes</b> est sélectionnée, seuls les statuts verrouillés à l’échelle du système sont disponibles. <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>Si un groupe spécifique est sélectionné, seuls les statuts disponibles pour ce groupe le sont.</p> </li> 
      </ul> <p>Pour plus d’informations sur le fonctionnement du processus d’approbation avec les statuts, voir la section <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Comment les processus d’approbation reposent sur les statuts</a> dans l’article <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Vue d’ensemble du processus d’approbation</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nom de l'étape</td> 
      <td>(Facultatif) Saisissez un nom décrivant la première étape du chemin. Si vous ne spécifiez pas de nom d’étape, le nom par défaut est <b>Étape 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approbateurs</td> 
      <td> <p>Commencez à saisir le nom de l’utilisateur ou de l’utilisatrice, de l’équipe ou de la fonction que vous souhaitez désigner comme personne responsable de l’approbation pour cette étape, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante. Vous ne pouvez ajouter que des utilisateurs et utilisatrices, fonctions et équipes actifs. </p>

   <p><b>CONSEIL</b> :</p>

   <p>Lorsque vous ajoutez un utilisateur ou une utilisatrice comme personne responsable de l’approbation, vérifiez son avatar, son rôle principal ou son adresse e-mail pour distinguer les doublons. Les utilisateurs et utilisatrices doivent être associés à au moins une fonction pour l’afficher à mesure que vous les ajoutez.</p>
      <p>Pour que les utilisateurs et utilisatrices puissent afficher les e-mails de leurs utilisateurs et utilisatrices, le paramètre Afficher les coordonnées doit être activé dans votre niveau d’accès. Pour plus d’informations, voir <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Accorder l’accès aux utilisateurs et utilisatrices</a></p>.

   <p><b>NOTE</b> :

   l’ajout d’un utilisateur ou d’une utilisatrice, d’une équipe ou d’un rôle en tant que responsable de l’approbation ne lui donne pas automatiquement des droits sur l’objet associé à cette approbation. Les autorisations sur l’objet leur sont accordées lorsque l’étape d’approbation est déclenchée. Sinon, les objets doivent être partagés avant qu’une décision d’approbation ne puisse être prise. </p>
   <p>Vous pouvez également désigner une personne comme responsable de l’approbation en précisant sa fonction spécifique. Par exemple, une personne peut être affectée comme responsable de l’approbation, qu’elle soit gestionnaire, propriétaire ou sponsor d’un projet, d’un programme ou d’un portfolio. Ces options apparaissent automatiquement lorsque vous commencez à saisir du texte.</p> 
      <p><b>IMPORTANT</b> :  
      <ul> 
      <li> si aucune personne sponsor de projet n’est désignée et que vous accordez une approbation à la personne sponsor du projet, celle-ci est alors accordée à la personne propriétaire du projet. Si aucune personne propriétaire de projet n’est désignée, l’approbation est accordée à la personne chargée de l’administration de Workfront. </li> 
      <li> Lorsque vous affectez une approbation à un rôle et que l’option <b>L’approbateur ou l’approbatrice ne doit pas nécessairement faire partie de l’équipe du projet</b> est désactivée, mais qu’aucun rôle de l’équipe de projet ne correspond au rôle de l’approbation, cette dernière est réaffectée à la personne propriétaire du projet. Pour plus d’informations sur les paramètres d’approbation, voir <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Configurer les paramètres d’approbation globaux</a>.
      </li> 
      <li>Lorsque vous accordez une approbation à la personne propriétaire du projet et qu’il n’existe pas de personne propriétaire de projet, l’approbation est alors accordée à l’équipe principale d’administration de Workfront, comme indiqué dans la section de la section Infos client de la zone de configuration. Pour plus d’informations, voir <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configurer les informations de base de votre système</a>.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>Quand des fonctions se voient accorder une responsabilité d’approbation, tous les utilisateurs et utilisatrices ayant cette fonction et faisant partie de l’équipe de projet peuvent prendre une décision d’approbation. </p> 
      <p>Lorsque vous désignez une équipe comme responsable de l’approbation, chaque personne de cette équipe peut prendre une décision d’approbation. </p> 
      <p>Pour plus d’informations sur l’équipe du projet, voir <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Vue d’ensemble de l’équipe du projet</a>. Pour plus d’informations sur l’approbation du travail, voir <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Approuver du travail</a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">Une seule décision est requise.</td> 
      <td>(Ne s’affiche que si vous ajoutez plusieurs approbateurs et approbatrices à l’étape) Sélectionnez cette option si l’une des personnes approbatrices de l’étape peut approuver ou rejeter l’élément de travail au cours de cette étape. Cette action permet à l’élément de travail de quitter l’étape.  
      <p>Si cette option n’est pas sélectionnée, tous les approbateurs et approbatrices identifiés doivent approuver ou rejeter l’étape (dans n’importe quel ordre) avant que l’élément ne quitte l’étape. Si l’une des personnes approbatrices rejette l’étape, le processus s’interrompt et recommence afin que les modifications nécessaires puissent être apportées. Les approbateurs et approbatrices peuvent ensuite approuver ou rejeter à nouveau l’étape.</p> 
      <p>Si une équipe est désignée comme approbatrice, toute personne membre de l’équipe peut approuver ou rejeter une étape.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Ajouter une étape</p> </td> 
      <td>(Facultatif) Ajoutez une autre étape au chemin d’accès, à l’aide des options décrites dans les trois lignes ci-dessus. Vous pouvez ajouter autant d’étapes au chemin que nécessaire.</td> 
     </tr>
     <tr> 
      <td role="rowheader"> Sélectionnez ce qui se passe en cas de rejet de l’approbation :</td> 
      <td> <p>Sélectionnez l’action à entreprendre si l’élément de travail est rejeté à l’une des étapes du chemin d’accès :</p> 
      <ul> <li><strong>Créer un problème</strong> : (disponible uniquement pour les processus d’approbation des projets et des tâches) Un problème est créé dans le projet ou la tâche où le processus d’approbation est en cours. La ressource affectée par défaut à la tâche, ou la personne propriétaire du projet, est affectée au problème. Par défaut, le nom du problème créé est <strong>Approbation rejetée (Nom du projet ou de la tâche)</strong>. Il s’agit d’un problème de rejet, saisi sous la tâche ou le projet, en fonction du processus d’approbation dans lequel le rejet s’est produit.</li> 
      <li> <p><strong>Définir le statut sur</strong> : choisissez l’une des options suivantes :</p> 
      <ul> <li><strong>Statut précédent</strong> : le projet, la tâche ou le problème rejeté(e) revient au statut antérieur à celui qui active le processus d’approbation.</li> 
      <li> <p><strong>Tout autre statut dans la liste</strong> : l’objet rejeté passe au statut de votre choix, par exemple Suspendu. Vous pouvez choisir l’un des statuts par défaut ou un statut personnalisé que vous avez ajouté à votre système Workfront.</p> <p>Si vous sélectionnez un statut associé à un processus d’approbation, comme le statut de refus pour un chemin d’approbation, l’objet rejeté passe au statut sélectionné et sera marqué comme « Approbation en attente ».</p>
      <p>Par exemple, si vous sélectionnez Suspendu pour le statut de refus alors que le statut Suspendu est associé à un processus d’approbation, le statut de l’objet rejeté devient « Suspendu - Approbation en attente » et une approbation est nécessaire.</p>    <p>Pour un processus d’approbation à l’échelle du système, seuls les statuts applicables à l’ensemble du système sont disponibles.</p> <p>Pour un processus d’approbation spécifique à un groupe, tous les statuts du groupe sont disponibles. Cela inclut tous les statuts personnalisés que l’administrateur ou l’administratrice a créés spécifiquement pour le groupe, ainsi que tous les statuts applicables à l’ensemble du système. </p> <p>Pour plus d’informations sur le fonctionnement du processus d’approbation avec les statuts, voir la section <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Comment les processus d’approbation reposent sur les statuts</a> dans l’article <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Vue d’ensemble du processus d’approbation</a>.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Cliquez sur **Ajouter un chemin** pour ajouter un autre chemin au processus d’approbation, en vous référant à la liste d’options de l’étape précédente.

   Le nouveau chemin doit être associé à un autre statut. Le chemin se déclenche lorsque l’élément est mis à jour pour afficher ce statut. Il ne peut y avoir deux chemins pour le même statut.

1. Cliquer sur **Enregistrer**.
1. (Facultatif) Effectuez l’une des opérations suivantes :

   * Associez le processus d’approbation à des projets, des tâches ou des problèmes spécifiques dans votre système, comme décrit dans [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * En dehors de Workfront, informez les utilisateurs et utilisatrices que le processus d’approbation est disponible et qu’ils peuvent l’associer à leurs projets, tâches ou problèmes, comme décrit dans [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Créez un autre processus d’approbation qui est déclenché si ce processus d’approbation est rejeté et que l’élément adopte un autre statut. Cela vous permet de relier les processus d’approbation entre eux.
