---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Créer une file d’attente des demandes
description: Vous pouvez mettre en place une file d’attente des demandes dans laquelle les personnes peuvent saisir des demandes occasionnelles qui ne sont pas un travail prévu dans un projet. Par exemple, une file d’attente des demandes du centre d’assistance peut être mise en place pour capturer toutes les demandes des personnes qui parviennent au service informatique.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '2653'
ht-degree: 100%

---


# Créer une file d’attente des demandes

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

Vous pouvez mettre en place une file d’attente des demandes dans laquelle les personnes peuvent saisir des demandes occasionnelles qui ne sont pas un travail prévu dans un projet. Par exemple, une file d’attente des demandes du centre d’assistance peut être mise en place pour capturer toutes les demandes des personnes qui parviennent au service informatique.

Cet article décrit comment créer une file d’attente dans laquelle les personnes peuvent soumettre des demandes. Pour plus d’informations sur la manière de soumettre une nouvelle demande à une file d’attente, voir [Copier et soumettre des demandes](../create-requests/copy-and-submit-requests.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <p>Nouvelle licence : standard </p>
   Ou
   <p>Licence actuelle : plan </p> </td> 
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


<!--old access levels: 
You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b></p> 
   
   <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator
-->

## Vue d’ensemble des files d’attente des demandes

Vous configurez une file d’attente des demandes en tant que projet. Lorsque vous désignez le projet comme file d’attente des demandes, la file d’attente devient accessible à partir de la zone Demandes d’Adobe Workfront. Lorsque vous personnalisez la file d’attente des demandes, vous personnalisez également le formulaire que les personnes remplissent lorsqu’elles soumettent leurs demandes.

Cet article décrit comment créer une file d’attente des demandes à partir d’un projet existant. Toutefois, pour assurer la cohérence de votre processus de réception des demandes ou pour y ajouter plusieurs couches à des fins de reporting et d’amélioration de la gestion, vous pouvez également configurer d’autres éléments constitutifs d’une file d’attente des demandes, décrits dans le tableau suivant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Détails de la file d’attente</td> 
   <td> <p>Vous devez configurer un projet en tant que file d’attente des demandes dans la zone Détails de la file d’attente. Cette étape est obligatoire. </p> <p>Pour plus d’informations, voir la section <a href="#create-a-request-queue" class="MCXref xref">Créer une file d’attente des demandes</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Groupes de sujets</td> 
   <td> <p>Il s’agit de menus supplémentaires qui classent les demandes en fonction de caractéristiques communes. Par exemple, pour une file d’attente des demandes informatiques, vous pouvez avoir des groupes de rubriques « Sur site » et « À distance ». </p> <p>Pour plus d’informations, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Créer des groupes de rubriques</a>. </p> <p>Ce champ est facultatif.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rubriques de file d’attente</td> 
   <td> <p>Il s’agit de menus supplémentaires qui classent les demandes appartenant au même groupe de rubriques en fonction de caractéristiques communes. Un groupe de rubriques peut contenir plusieurs rubriques de file d’attente. </p> <p>Par exemple, le groupe de rubriques « Sur site » de la file d’attente des demandes informatiques peut contenir les rubriques de la file d’attente « Matériel », « Logiciel » et « Réseau ». </p> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Créer des rubriques de files d’attente</a>. </p> <p>Ce champ est facultatif.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Règles de transmission</td> 
   <td> <p>Elles vous permettent d’acheminer chaque demande vers une personne, une fonction, une équipe ou un projet. </p> <p>Pour plus d’informations, consultez la section <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Créer des règles de routage</a>. </p> <p>Ce champ est facultatif.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Créer une file d’attente des demandes

Lorsque vous configurez un projet en tant que file d’attente des demandes, le statut du projet doit être Actuel pour s’afficher dans la zone Demandes de Workfront.

>[!TIP]
>
>Votre administrateur ou administratrice Workfront ou de groupes peut vous assigner un modèle de mise en page personnalisé qui peut ne pas inclure certaines des sections décrites dans les étapes suivantes.


Pour créer une file d’attente des demandes, procédez comme suit :

1. Accédez au projet que vous souhaitez configurer en tant que file d’attente des demandes.
1. (Facultatif) Cliquez sur Détail du projet dans le panneau de gauche et ajoutez une Description au projet dans la zone Vue d’ensemble. ************ Cette information s’affiche sur toutes les nouvelles demandes.
1. Cliquez sur Détails de la file d’attente dans le panneau de gauche. **** Vous devrez peut-être cliquer sur **Afficher plus**, puis sur **Détails de la file d’attente**.

   La section Détails de la file d’attente s’ouvre.

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Indiquez les informations suivantes :

   * **Publier en tant que file d’attente des requêtes d’aide : sélectionnez cette option pour identifier ce projet comme une file d’attente des demandes d’aide.** Tous les problèmes entrants sont considérés comme des demandes.\
     Lorsque cette option n’est pas sélectionnée, le projet se comporte comme un projet standard dans Workfront et tous les problèmes entrants sont des problèmes.

   * **Qui peut ajouter des requêtes à cette file d’attente : sélectionnez les personnes qui ont le droit d’ajouter des demandes à cette file d’attente.** Vous pouvez autoriser les groupes de personnes suivants à voir la file d’attente des demandes dans leur zone Demandes de la barre de navigation globale lors de l’ajout d’une nouvelle demande :

     | Qui peut saisir des demandes. | Description |
     |---|---|
     | Quiconque | Toute personne utilisant Workfront et disposant d’un compte actif peut afficher cette file d’attente des demandes et y ajouter des demandes. |
     | Personnes disposant d’un accès en affichage pour ce projet | Les personnes ayant des autorisation d’affichage sur le projet peuvent afficher cette file d’attente et y ajouter des demandes. |
     | Personnes de l’entreprise affectées à ce projet | Les personnes qui font partie de l’entreprise associée à ce projet peuvent afficher cette file d’attente et y ajouter des demandes. Si une entreprise est associée au projet, le nom de l’entreprise est indiqué entre parenthèses après ce paramètre. |
     | Personnes du groupe affectées à ce projet | Les personnes qui appartiennent au groupe associé à ce projet peuvent afficher les demandes de cette file d’attente et en ajouter. Si un groupe est associé au projet, le nom du groupe est indiqué entre parenthèses après ce paramètre, en caractères gris. |

     {style="table-layout:auto"}

   * **Partager avec ces liens : les options suivantes vous permettent de fournir un accès direct à la file d’attente des demandes et aux formulaires qui y sont associés à des personnes extérieures à Workfront ou à des utilisateurs et utilisatrices de Workfront utilisant une page externe.** Pour plus d’informations sur l’intégration d’une file d’attente des demandes dans un tableau de bord en tant que page externe, voir [Intégrer une file d’attente des demandes dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Les personnes doivent déjà avoir des droits d’accès à la file d’attente des demandes pour pouvoir obtenir un accès direct. L’utilisation de l’une ou l’autre des options décrites ici n’octroie pas automatiquement l’accès aux personnes.

     >[!TIP]
     >
     >Les personnes doivent d’abord se connecter à Workfront avant de pouvoir accéder à la file d’attente des demandes lorsqu’elles accèdent à la page File d’attente des demandes à partir d’une autre application.

      * **URL d’accès direct :** lorsqu’une personne accède à cette URL à partir d’un navigateur, elle est directement dirigée vers la section Nouvelle demande de la zone Demandes et cette demande est sélectionnée par défaut pour elle.

        ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >Vous pouvez afficher une file d’attente des demandes dans un tableau de bord en tant que page externe. Dans ce cas, la file d’attente des demandes est présélectionnée, mais vous pouvez sélectionner n’importe quelle autre file d’attente des demandes dans le champ Type de demande. Les personnes peuvent modifier le type de demande. Les éléments de navigation des demandes s’affichent également.

      * **Code intégré :** utilisez ce code HTML pour intégrer le formulaire de file d’attente des demandes sous forme d’iframe dans n’importe quelle page HTML.\
        Si les personnes ne sont pas déjà authentifiées auprès de Workfront lorsqu’elles affichent la page où le code est intégré, la boîte de dialogue de connexion à Workfront s’affiche. Une fois les personnes connectées, le formulaire de la file d’attente des demandes s’affiche.

        >[!NOTE]
        >
        >Lors de l’affichage d’une file d’attente des demandes dans un iframe, seul le formulaire de demande s’affiche, le nom de la demande est présélectionné et grisé. La personne ne peut pas modifier le type de demande. Les éléments de navigation de la zone Demandes ne s’affichent pas.

        Pour que le formulaire de file d’attente des demandes s’affiche lorsque vous utilisez ce code intégré, vous devez activer le paramètre « Autoriser l’incorporation de Workfront dans une structure » dans la configuration de votre système. Pour plus d’informations sur l’activation de l’intégration de Workfront dans un iframe, voir Configurer les préférences de sécurité du système. [](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) Si ce paramètre n’est pas activé, l’iframe est laissé vide.

        Vous pouvez régler divers aspects de l’affichage du formulaire intégré, comme suit :

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Fonctionnalité</strong> </p> </th> 
           <th> <p><strong>Solution</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Ajuster la taille de l’image</p> </td> 
           <td> <p>Modifiez les attributs « largeur » et « hauteur ».</p> <p>Par défaut, la largeur est de « 500 » et la hauteur de « 600 ».</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Diriger les utilisateurs et utilisatrices vers une rubrique de file d’attente ou un groupe de sujets spécifique</p> </td> 
           <td> <p>Ajoutez le paramètre « chemin d’accès » à l’URL src. Vous pouvez trouver le paramètre de chemin d’accès en naviguant vers la rubrique de file d’attente ou le groupe de sujets dans le formulaire non incorporé et en inspectant l’URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Afficher et autoriser les utilisateurs et utilisatrices à modifier la liste déroulante des groupes de sujets préconfigurés</p> </td> 
           <td> <p>Utilisez le paramètre « chemin d’accès » en ajoutant le paramètre <code>showPreSelectedOptions=true</code> à <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Détecter l’envoi du formulaire</p> </td> 
           <td> <p>Ajoutez un listener d’événements « message » à la fenêtre de votre page web et vérifiez si  est . <code>event.data.type</code><code>requestSubmitted</code> <code>event.data.newIssueID</code> prendra la valeur de l’ID du problème créé.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Types de demandes :** sélectionnez parmi les options par défaut ci-dessous.

     L’administrateur ou administratrice Workfront peut renommer les types de demande par défaut. Pour plus d’informations sur le renommage des types de demandes, voir [Personnaliser les types de problèmes par défaut](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Rapport sur les bogues
      * Modifier l’ordre
      * Problème
      * Demande

        Ce champ est obligatoire et vous devez sélectionner au moins une option.

     >[!NOTE]
     >
     >Les types de demandes ne s’affichent en tant que sélection dans la zone Demandes que si le type de demande est sélectionné à la fois dans les pages Détails de la file d’attente et Rubrique de file d’attente. Pour plus d’informations sur la configuration de la zone Détails de la file d’attente d’un projet, voir [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Chaque type sélectionné ici sera disponible sur le formulaire (vous pouvez en sélectionner plusieurs). Le fait de sélectionner plus d’un type de demande peut aider à organiser les demandes multiples entrantes.\
     Par exemple, si vous utilisez le formulaire dans une file d’attente des demandes pour un projet informatique, les types de demandes suivants peuvent être introduits dans la file d’attente : matériel, logiciel, corrections de bug et problèmes.

   * **Durée par défaut :** la durée par défaut est le temps qu’il faut généralement pour traiter un problème. Elle devient la valeur par défaut pour tous les problèmes entrants et peut être modifiée manuellement. La durée est généralement fixée en heures, jours ou semaines. La durée par défaut d’un problème est la même que celle des heures prévues pour ce problème. La date d’achèvement prévue du problème est calculée sur la base de ce champ.\
     La durée par défaut du problème est 1 jour ou 8 heures. Si votre administrateur ou administratrice Workfront a défini le nombre d’heures habituelles par journée de travail comme étant inférieur à 8 heures, la durée par défaut des problèmes est toujours de 8 heures. Par exemple, si le nombre d’heures habituelles par journée de travail est fixé à 7 heures, la durée par défaut des problèmes est 1,14 jour ou 8 heures. Pour plus d’informations sur la configuration du système Heures habituelles par journée de travail, voir la section « Calculs de chronologie » dans l’article [Configurer les préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Les personnes appartenant à la même entreprise hériteront d’autorisations identiques pour toutes les demandes.** Lorsque cette option est sélectionnée, toutes les demandes soumises à la file d’attente sont visibles par les utilisateurs et utilisatrices de la même entreprise. Les utilisateurs et utilisatrices peuvent consulter ces demandes dans la section Toutes les demandes, située dans la zone Demandes. Au moment où ce paramètre est activé ou désactivé, il a un impact sur toutes les demandes futures ; il n’a pas d’impact rétroactif sur les informations.
   * **Si une personne effectue une demande, accorder automatiquement : lorsqu’une personne dépose une demande dans la file d’attente, elle se voit automatiquement accorder le niveau d’autorisation que vous avez choisi pour cette demande.** Sélectionnez l’un des niveaux d’autorisation suivants :

      * **Accès en affichage**
      * **Accès en contribution**. Il s’agit de la sélection par défaut.
      * **Accès en gestion**

     Pour plus d’informations sur le modèle des autorisations Workfront, voir [Vue d’ensemble du partage des autorisations sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     Définir des autorisations ici permet de gagner du temps, plutôt que de devoir accorder des autorisations pour chaque demande entrante. Le choix de cette option a un impact sur toutes les demandes futures, mais n’a pas d’impact rétroactif sur les demandes existantes.

   * **Approbation par défaut : associez un processus d’approbation à cette file d’attente.** Seuls les processus d’approbation des problèmes sont visibles dans ce menu déroulant. Tous les problèmes envoyés à cette file d’attente seront associés à ce processus d’approbation. Votre administrateur ou administratrice Workfront doit définir les processus d’approbation au niveau du système avant que vous puissiez les associer aux files d’attente. Les utilisateurs et utilisatrices disposant d’un accès administratif aux processus d’approbation peuvent également créer des processus d’approbation spécifiques à un groupe.

     >[!IMPORTANT]
     >
     >Si le groupe du projet change, le processus d’approbation spécifique au groupe lié aux problèmes existants devient un processus d’approbation à usage unique. Pour plus d’informations sur la manière dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir [Comment les modifications apportées aux groupes et aux processus d’approbation affectent les processus d’approbation attribués](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Si plusieurs rubriques de file d’attente sont associées à une file d’attente des demandes, nous vous recommandons plutôt d’associer les processus d’approbation aux rubriques de file d’attente. Pour plus d’informations sur la création de rubriques de file d’attente, voir [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Tenez compte des points suivants lorsque vous ajoutez des processus d’approbation aux files d’attente des demandes :

      * Seuls les processus d’approbation actifs sont affichés dans la liste.
      * Les processus d’approbation à l’échelle du système et du groupe s’affichent dans la liste. Un processus d’approbation associé à un groupe autre que celui du projet ne s’affiche pas dans la liste.

   * **Route par défaut : associer une règle de routage à cette file d’attente des demandes.** Les règles de routage permettent d’attribuer automatiquement de nouveaux problèmes soumis à une file d’attente des demandes à la bonne ressource (utilisateur ou utilisatrice, fonction ou équipe) ainsi qu’au bon projet. Tous les problèmes soumis à cette file d’attente seront associés à cette règle de routage. Vous devez configurer les règles de routage avant qu’elles ne s’affichent dans la section Détails de la file d’attente et avant de pouvoir les associer à une file d’attente des demandes.\
     Si plusieurs sujets de file d’attente sont associés à une file d’attente des demandes, nous vous recommandons plutôt d’associer des règles de routage aux sujets de file d’attente. Pour plus d’informations sur la création de règles de routage, voir [Créer des règles de routage](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Champs Nouveau problème :** dans la section **Afficher les champs sélectionnés suivants pour tous les utilisateurs et toutes les utilisatrices**, sélectionnez les champs que vous souhaitez rendre visibles à toutes les personnes qui soumettent une demande au projet ou qui ajoutent un problème au projet ou aux tâches.

     >[!TIP]
     >
     >Les champs Nouveau problème sélectionnés dans la section Détails de la file d’attente sont également associés à tout nouveau problème ajouté au projet <!--this is confusing: or to the tasks in the Issues section-->.

     Lorsque vous activez les champs Affecté à, Fonction ou Équipe, ceux-ci sont toujours renommés en Affectations dans le formulaire de demande, mais vous ne pouvez spécifier que le type d’affectation sélectionné ici.

     >[!NOTE]
     >
     >Si vous avez sélectionné Affecté à dans la zone Détails de la file d’attente, vous ne pouvez saisir que des utilisateurs et utilisatrices dans le champ Affectations du formulaire de demande. Dans ce cas, vous ne pouvez pas saisir de fonctions ou d’équipe.

   * **Documents** : si vous choisissez d’afficher la section Documents dans le nouveau formulaire de demande, sélectionnez l’emplacement de la section de chargement des documents. Sélectionnez l’une des options suivantes :

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Avant les formulaires personnalisés</td> 
        <td><span>La section Documents s’affiche au bas du formulaire de demande.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Avant les formulaires personnalisés</td> 
        <td> <p><span>La section Documents s’affiche entre les champs Workfront et les champs personnalisés du formulaire de demande.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Afficher tous les champs sélectionnés et non sélectionnés : sélectionnez les utilisateurs et utilisatrices qui doivent voir tous les champs du nouveau formulaire de demande.** Les options suivantes contrôlent l’accès aux champs du formulaire.

     | Utilisateurs et utilisatrices pouvant voir tous les champs du formulaire de demande | Description |
     |---|---| 
     | Tous les utilisateurs et utilisatrices (licences de plan) | Toutes les personnes disposant d’une licence de plan peuvent voir les champs sélectionnés et non sélectionnés. |
     | Personnes disposant d’un accès en affichage pour ce projet (licence de plan) | Les utilisateurs et utilisatrices disposant d’une licence de plan et ayant également des droits d’affichage pour ce projet peuvent voir les champs sélectionnés et non sélectionnés. Les autres utilisateurs et utilisatrices pouvant soumettre des demandes pour ce projet ne peuvent voir que les champs sélectionnés. |
     | Aucun utilisateur | Personne ne peut voir les champs non sélectionnés. Tous les utilisateurs et utilisatrices pouvant soumettre des demandes pour ce projet ne peuvent voir que les champs sélectionnés. |

   * **Formulaires personnalisés** : sélectionnez un formulaire personnalisé à associer à la file d’attente des demandes. Seuls les formulaires personnalisés de problèmes peuvent être sélectionnés dans ce menu déroulant. Les formulaires sélectionnés seront associés à tous les problèmes soumis à la file d’attente des demandes. Vous devez créer des formulaires personnalisés de problèmes avant de pouvoir les afficher dans la section Détails de la file d’attente. Si plusieurs rubriques de file d’attente sont associées à une file d’attente des demandes, nous vous recommandons plutôt d’associer des formulaires personnalisés aux rubriques de file d’attente. Pour plus d’informations sur la création de sous-sections pour la file d’attente des demandes, voir [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![](assets/custom-forms-on-queue-details.png)

     Si plusieurs formulaires personnalisés sont associés à la file d’attente des demandes, faites glisser les formulaires pour les trier dans l’ordre souhaité, dans la section **Réorganiser les formulaires**.

     >[!TIP]
     >
     >Les formulaires personnalisés ajoutés à la section Détails de la file d’attente sont également associés à toute nouvelle question ajoutée au projet <!--this is confusiong: or the tasks in the Issues  section-->.

1. Continuez à sélectionner les informations pour les paramètres dans la zone **Paramètres de la file d’attente des e-mails** pour permettre aux utilisateurs et utilisatrices d’envoyer des demandes par e-mail au projet de file d’attente des demandes.

   Pour plus d’informations, voir la section [Autoriser les utilisateurs et utilisatrices à envoyer un problème par e-mail dans un projet de file d’attente des demandes](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Cliquer sur **Enregistrer**.\
   Votre projet a été configuré pour être une file d’attente des demandes et les utilisateurs et utilisatrices peuvent maintenant y ajouter des demandes.

1. (Facultatif) Pour améliorer la fonctionnalité de la file d’attente des demandes, créez des sous-sections supplémentaires pour votre file d’attente, ainsi que des règles pour acheminer les demandes entrantes vers l’équipe, la personne cessionnaire ou le projet approprié.

   * Pour plus d’informations sur la création de sous-sections pour la file d’attente des demandes, voir les articles [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) et [Créer des groupes de sujets](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).
   * Pour plus d’informations sur la transmission des demandes vers la personne cessionnaire, l’équipe et le projet appropriés, voir [Créer des règles de routage](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
