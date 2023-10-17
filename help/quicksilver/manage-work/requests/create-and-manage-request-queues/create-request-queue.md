---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Création d’une file d’attente de requête
description: Vous pouvez configurer une file d’attente de requêtes dans laquelle les utilisateurs peuvent saisir des requêtes occasionnelles qui ne sont pas planifiées pour un projet.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: 5db9a4869e1321bd268e80f786d157fbb41c0656
workflow-type: tm+mt
source-wordcount: '2655'
ht-degree: 2%

---

# Création d’une file d’attente de requête

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

Vous pouvez configurer une file d’attente de requêtes dans laquelle les utilisateurs peuvent saisir des requêtes occasionnelles qui ne sont pas planifiées pour un projet. Par exemple, une file d’attente de demandes du service d’assistance peut être configurée pour capturer toutes les demandes d’utilisateurs envoyées à un service informatique.

Cet article décrit comment créer une file d’attente de requêtes dans laquelle les utilisateurs peuvent envoyer des requêtes. Pour plus d’informations sur la manière d’envoyer une nouvelle requête à une file d’attente de requêtes, voir [Copie et envoi de requêtes](../create-requests/copy-and-submit-requests.md).

## Exigences d’accès

<!--drafted for P&P: replace the table below with this:

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
   <td> 
   <p>Current license: Stadard </p>
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator
-->

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> <p><b>NOTE</b></p>

<p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Gestion des autorisations pour le projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Présentation des files d’attente de requête

Vous configurez une file d’attente de demandes en tant que projet. Lorsque vous définissez le projet comme une file d’attente des demandes, la file d’attente devient accessible à partir de la zone Demandes d’Adobe Workfront. Lorsque vous personnalisez la file d’attente des demandes, vous personnalisez également le formulaire que les utilisateurs remplissent lorsqu’ils envoient les demandes.

Cet article décrit comment créer une file d’attente de requêtes à partir d’un projet existant. Cependant, pour assurer la cohérence de votre processus d’ingestion de requêtes ou y ajouter plusieurs calques à des fins de création de rapports et de meilleure gestion, vous pouvez également configurer d’autres blocs de construction d’une file d’attente de requêtes, qui sont décrits dans le tableau suivant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Détails de la file d'attente</td> 
   <td> <p>Vous devez configurer un projet en tant que file d’attente de requêtes dans la zone Détails de la file d’attente. Cette étape est obligatoire. </p> <p>Pour plus d’informations, voir <a href="#create-a-request-queue" class="MCXref xref">Création d’une file d’attente de requête</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Groupes de sujets</td> 
   <td> <p>Il s’agit de menus supplémentaires qui classent les requêtes en fonction de fonctionnalités communes. Par exemple, pour une file d’attente de demandes informatiques, vous pouvez avoir des groupes de rubriques "Sur site" et "À distance". </p> <p>Pour plus d’informations, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Création de groupes de rubriques</a>. </p> <p>Cette option est facultative.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rubriques de file d'attente</td> 
   <td> <p>Il s’agit de menus supplémentaires qui classent les requêtes appartenant au même groupe de rubriques en fonction de fonctionnalités communes. Un groupe de rubriques peut contenir plusieurs rubriques de file d’attente. </p> <p>Par exemple, le groupe de rubriques "Sur site" pour la file d’attente des demandes informatiques peut contenir les rubriques "Matériel", "Logiciel" et "Réseau". </p> <p>Pour plus d’informations, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Création de rubriques de file d’attente</a>. </p> <p>Cette option est facultative.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Règles de transmission</td> 
   <td> <p>Ils vous permettent d’acheminer chaque demande vers un utilisateur, un rôle de tâche, une équipe ou vers un projet. </p> <p>Pour plus d’informations, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Création de règles de routage</a>. </p> <p>Cette option est facultative.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Création d’une file d’attente de requête

Lorsque vous configurez un projet en tant que file d’attente des demandes, l’état du projet doit être Actuel pour s’afficher dans la zone Demandes de Workfront.

>[!TIP]
>
>L’administrateur de Workfront ou de groupe peut vous affecter à un modèle de mise en page personnalisé qui peut ne pas inclure certaines des sections décrites dans les étapes suivantes.


Pour créer une file d’attente de requête :

1. Accédez au projet que vous souhaitez configurer en tant que file d’attente des demandes.
1. (Facultatif) Cliquez sur **Détails du projet** dans le panneau de gauche et ajoutez une **Description** au projet dans le **Présentation** zone. Ces informations s’affichent sur toutes les nouvelles requêtes.
1. Cliquez sur **Détails de la file** dans le panneau de gauche. Vous devrez peut-être cliquer sur **Afficher plus**, puis **Détails de la file**.

   Cette opération ouvre la section Détails de la file d’attente .

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Indiquez les informations suivantes :

   * **Publier en tant que file d’attente de demande d’aide :** Sélectionnez cette option pour identifier ce projet en tant que file d’attente de demandes. Tous les problèmes entrants sont considérés comme des requêtes.\
     Lorsque cette option n’est pas sélectionnée, le projet se comporte comme un projet standard dans Workfront et tous les problèmes entrants sont des problèmes.

   * **Qui peut ajouter des requêtes à cette file d’attente :** Sélectionnez les utilisateurs qui ont accès à l’ajout de requêtes à cette file d’attente. Vous pouvez permettre aux groupes de personnes suivants d’afficher la file d’attente des demandes dans la zone Requêtes de la barre de navigation globale lorsqu’ils ajoutent une nouvelle requête :

     | Qui peut saisir des requêtes | Description |
     |---|---|
     | Quiconque | Tout utilisateur Workfront disposant d’un compte actif peut afficher cette file d’attente de requêtes et y ajouter des requêtes. |
     | Personnes disposant d&#39;un accès en affichage pour ce projet | Les utilisateurs disposant des autorisations d’affichage sur le projet peuvent afficher et ajouter des requêtes à cette file d’attente. |
     | Personnes de l&#39;entreprise affectées à ce projet | Les utilisateurs appartenant à la société associée à ce projet peuvent afficher et ajouter des requêtes à cette file d’attente. Si une société est associée au projet, son nom est indiqué entre parenthèses après ce paramètre. |
     | Personnes du groupe affectées à ce projet | Les utilisateurs appartenant au groupe associé à ce projet peuvent afficher et ajouter des requêtes à cette file d’attente. Si un groupe est associé au projet, son nom est indiqué entre parenthèses après ce paramètre, en police grise. |

     {style="table-layout:auto"}

   * **Partagez avec ces liens :** Les options suivantes vous permettent de fournir un accès direct à la file d’attente des demandes et aux formulaires qui lui sont associés à des utilisateurs en dehors de Workfront ou à des utilisateurs de Workfront à l’aide d’une page externe. Pour plus d’informations sur l’intégration d’une file d’attente de requêtes dans un tableau de bord en tant que page externe, voir [Incorporation d’une file d’attente de requêtes dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Les utilisateurs doivent déjà disposer de droits d’accès à la file d’attente des demandes pour obtenir un accès direct. L’utilisation de l’une des options décrites ici n’accorde pas automatiquement l’accès aux utilisateurs.

     >[!TIP]
     >
     >Les utilisateurs doivent d’abord se connecter à Workfront avant d’accéder à la file d’attente des demandes lorsqu’ils accèdent à la page File d’attente des demandes à partir d’une autre application.

      * **URL d’accès direct :** Lorsqu’un utilisateur accède à cette URL à partir d’un navigateur, il est dirigé directement vers la section Nouvelle requête de la zone Demandes . Cette requête est sélectionnée par défaut pour l’utilisateur.

        ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >Vous pouvez afficher une file d’attente des requêtes dans un tableau de bord en tant que page externe. Dans ce cas, la file d’attente des demandes est présélectionnée, mais vous pouvez sélectionner toute autre file d’attente des demandes dans le champ Type de demande . Les utilisateurs peuvent modifier le type de requête. Les composants de navigation des requêtes s’affichent également.

      * **Code incorporé :** Utilisez ce code de HTML pour incorporer le formulaire de file d’attente des demandes en tant qu’iframe dans n’importe quelle page de HTML.\
        Si les utilisateurs ne sont pas déjà authentifiés dans Workfront lorsqu’ils affichent la page sur laquelle le code est incorporé, la boîte de dialogue de connexion Workfront s’affiche. Une fois les utilisateurs connectés, le formulaire File d’attente des demandes s’affiche.

        >[!NOTE]
        >
        >Lors de l’affichage d’une file d’attente de requête dans un iframe, seul le formulaire de requête s’affiche, le nom de la requête est présélectionné et grisé. L’utilisateur ne peut pas modifier le type de requête. Les composants de navigation de la zone Demandes ne s’affichent pas.

        Pour que le formulaire de file d’attente des requêtes s’affiche lors de l’utilisation de ce code incorporé, vous devez activer le paramètre &quot;Autoriser l’incorporation de Workfront dans un iframe&quot; dans la configuration de votre système. Pour plus d’informations sur l’activation de l’incorporation de Workfront dans un iframe, voir [Configuration des préférences de sécurité système](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Si ce paramètre n’est pas activé, l’iframe s’affiche comme vide.

        Vous pouvez ajuster différents aspects de l’affichage du formulaire incorporé, comme suit :

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
           <td> <p>Modifiez les attributs "largeur" et "hauteur".</p> <p>Par défaut, la largeur est "500" et la hauteur est "600".</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Orienter les utilisateurs vers une rubrique ou un groupe de rubriques de file d’attente spécifique</p> </td> 
           <td> <p>Ajoutez le paramètre "path" à l'URL src. Vous pouvez trouver le paramètre de chemin d’accès en accédant à la rubrique ou au groupe de rubriques de votre choix dans le formulaire non incorporé et en inspectant l’URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Afficher et autoriser les utilisateurs à modifier la liste déroulante Groupe de rubriques préconfigurée</p> </td> 
           <td> <p>Utilisez le paramètre "path" en ajoutant la variable <code>showPreSelectedOptions=true</code> au paramètre <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Détecter le moment où le formulaire a été envoyé</p> </td> 
           <td> <p>Ajoutez un écouteur d’événement "message" à la fenêtre de votre page web et vérifiez si <code>event.data.type</code> is <code>requestSubmitted</code>. <code>event.data.newIssueID</code> est défini sur l’identifiant du problème créé.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Types de requête :** Sélectionnez l’une des options par défaut ci-dessous.

     L’administrateur Workfront peut renommer les types de requêtes par défaut. Pour plus d’informations sur le changement de nom des types de requête, voir [Personnalisation des types de problèmes par défaut](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Rapport sur les bogues
      * Modifier l&#39;ordre
      * Problème
      * Demande

        Il s’agit d’un champ obligatoire et vous devez sélectionner au moins une option.

     >[!NOTE]
     >
     >Les types de requête s’affichent sous forme de sélection dans la zone Requêtes uniquement si le type de requête est sélectionné dans les pages Détails de la file d’attente et Rubrique de la file d’attente. Pour plus d’informations sur la configuration de la zone Détails de la file d’attente d’un projet, voir [Création de rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Chaque type sélectionné ici sera disponible sur le formulaire (vous pouvez en sélectionner plusieurs). La sélection de plusieurs types peut vous aider à organiser plusieurs requêtes entrantes.\
     Par exemple, si vous utilisez le formulaire sur une file d’attente de requêtes pour un projet informatique, les types de requêtes suivants peuvent s’afficher dans la file d’attente : matériel, logiciel, correctifs de bogues et problèmes.

   * **Durée par défaut :** La durée par défaut correspond à la durée généralement nécessaire pour résoudre un problème. Cela devient la valeur par défaut de tous les problèmes entrants et peut être modifié manuellement. La durée est généralement définie en heures, jours ou semaines. La durée par défaut d’un problème est la même que les heures planifiées sur le problème. La date d’achèvement prévue du problème se calcule d’après ce champ.\
     La durée par défaut du problème est de 1 jour ou 8 heures. Si l’administrateur de Workfront définit la durée type des heures par jour de travail sur moins de 8 heures, la durée par défaut pour les problèmes est toujours de 8 heures. Par exemple, si la valeur &quot;Heures par jour de travail standard&quot; est définie sur 7 heures, la durée par défaut pour les problèmes est de 1,14 jour ou 8 heures. Pour plus d’informations sur la configuration du système Heures par jour de travail standard, consultez la section &quot;Calcul de la chronologie&quot; de l’article. [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Les personnes appartenant à la même entreprise hériteront d&#39;autorisations identiques pour toutes les demandes.:** Lorsque cette option est sélectionnée, toutes les requêtes envoyées dans la file d’attente sont visibles pour les utilisateurs de la même société. Les utilisateurs peuvent afficher ces requêtes dans la section Toutes les requêtes , située dans la zone Demandes . Au moment où ce paramètre est activé ou désactivé, il a un impact sur toutes les futures demandes ; il n’a pas d’impact rétroactif sur les informations.
   * **Lorsqu’une personne émet une demande, elle accorde automatiquement :** Lorsqu’un utilisateur envoie une demande à la file d’attente des demandes, il se voit automatiquement octroyer le niveau d’autorisation que vous choisissez d’accorder à cette demande. Sélectionnez l’un des niveaux d’autorisation suivants :

      * **Afficher l’accès**
      * **Accès aux contributions**. Il s’agit de la sélection par défaut.
      * **Gérer l’accès**

     Pour plus d’informations sur le modèle d’autorisations Workfront, voir [Présentation des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     La définition des autorisations permet de gagner du temps, plutôt que d’avoir à accorder des autorisations pour chaque requête entrante. Le choix de cette option a un impact sur toutes les requêtes futures, mais n’a aucune incidence rétroactive sur les requêtes existantes.

   * **Approbation par défaut**: associez un processus d’approbation à cette file d’attente de demandes. Seuls les processus d’approbation des problèmes sont visibles dans ce menu déroulant. Tous les problèmes soumis à cette file d’attente seront associés à ce processus de validation. Votre administrateur Workfront doit définir des processus d’approbation au niveau du système avant de pouvoir les associer aux files d’attente de demandes. Les utilisateurs disposant d’un accès administratif aux processus de validation peuvent également créer des processus de validation spécifiques à un groupe.

     >[!IMPORTANT]
     >
     >Si le groupe du projet change, le processus d’approbation spécifique au groupe associé aux problèmes existants devient un processus d’approbation à usage unique. Pour plus d’informations sur la façon dont les modifications apportées au groupe du projet ou au processus d’approbation affectent les paramètres d’approbation, voir [Comment les modifications du processus d’approbation et de groupe affectent-elles les processus d’approbation affectés ?](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Si plusieurs rubriques de file d’attente sont associées à une file d’attente de demandes, il est recommandé d’associer plutôt les processus d’approbation aux rubriques de la file d’attente. Pour plus d’informations sur la création de rubriques de file d’attente, voir [Création de rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Tenez compte des points suivants lors de l’ajout de processus d’approbation aux files d’attente de demande :

      * Seuls les processus de validation actifs s&#39;affichent dans la liste.
      * Les processus de validation à l’échelle du système et spécifiques aux groupes s’affichent dans la liste. Un processus de validation associé à un groupe autre que celui du projet ne s’affiche pas dans la liste.

   * **Itinéraire par défaut**: associez une règle de routage à cette file d’attente de requêtes. Utilisez les règles de routage pour affecter automatiquement les nouveaux problèmes envoyés à une file d’attente des requêtes à la ressource appropriée (utilisateur, rôle de tâche ou équipe) et au projet approprié. Tous les problèmes envoyés à cette file d’attente seront associés à cette règle de routage. Vous devez configurer les règles de routage avant qu’elles ne s’affichent dans la section Détails de la file d’attente et avant de pouvoir les associer à la file d’attente des demandes.\
     Si plusieurs rubriques de file d’attente sont associées à une file d’attente de demandes, il est recommandé d’associer plutôt les règles de routage aux rubriques de la file d’attente. Pour plus d’informations sur la création de règles de routage, voir [Création de règles de routage](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Nouveaux champs de problème :** Dans le **Afficher les champs sélectionnés suivants à tous les utilisateurs** , sélectionnez les champs que vous souhaitez voir pour tous les utilisateurs qui envoient une requête au projet ou qui ajoutent un problème au projet ou aux tâches.

     >[!TIP]
     >
     >Les nouveaux champs de problème sélectionnés dans la section Détails de la file d’attente sont également associés à tout nouveau problème ajouté au projet. <!--this is confusing: or to the tasks in the Issues section-->.

     Lorsque vous activez l’un des champs Affecté à, Rôle de tâche ou Équipe, ils sont toujours renommés Affectations dans le formulaire de demande, mais vous ne pouvez spécifier que le type d’affectation sélectionné ici.

     >[!NOTE]
     >
     >Si vous avez sélectionné Affecté à dans la zone Détails de la file d’attente, vous ne pouvez saisir que les utilisateurs dans le champ Affectations du formulaire de requête. Dans ce cas, vous ne pouvez pas entrer de rôles de tâche ou d’équipe.

   * **Documents**: si vous choisissez d’afficher la section Documents dans le nouveau formulaire de demande, sélectionnez l’emplacement de la section de téléchargement du document. Sélectionnez l’une des options suivantes :

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

   * **Afficher tous les champs sélectionnés et non sélectionnés sur :** Sélectionnez les utilisateurs qui doivent afficher tous les champs du nouveau formulaire de demande. Les options suivantes contrôlent l’accès aux champs du formulaire.

     | Quels utilisateurs peuvent voir tous les champs du formulaire de requête ? | Description |
     |---|---| 
     | Tous les utilisateurs (formule des licences) | Tous les utilisateurs qui disposent d’une licence Plan peuvent voir les champs sélectionnés ainsi que les champs non sélectionnés. |
     | Personnes disposant d&#39;un accès en affichage pour ce projet (licence de plan) | Les utilisateurs disposant d’une licence Plan disposant également des droits d’affichage sur ce projet peuvent voir les champs sélectionnés ainsi que les champs non sélectionnés. Les autres utilisateurs qui peuvent envoyer des requêtes à ce projet peuvent afficher uniquement les champs sélectionnés. |
     | Aucun utilisateur | Aucun utilisateur ne peut voir les champs non sélectionnés. Tous les utilisateurs qui peuvent envoyer des requêtes à ce projet ne peuvent afficher que les champs sélectionnés. |

   * **Forms personnalisée**: sélectionnez un formulaire personnalisé à associer à la file d’attente des demandes. Seul Problème : le Forms personnalisé est disponible pour la sélection dans ce menu déroulant. Les formulaires sélectionnés seront associés à tous les problèmes envoyés à la file d’attente des demandes. Vous devez créer des formulaires personnalisés avant de pouvoir les afficher dans la section Détails de la file d’attente .
Si plusieurs rubriques de file d’attente sont associées à une file d’attente de requêtes, nous vous recommandons d’associer plutôt des formulaires personnalisés aux rubriques de file d’attente. Pour plus d’informations sur la création de sous-sections pour la file d’attente des demandes, voir [Création de rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![](assets/custom-forms-on-queue-details.png)

     Si plusieurs formulaires personnalisés sont associés à la file d’attente des demandes, faites-les glisser et déposez-les pour les trier dans l’ordre souhaité, dans la variable **Réorganiser Forms** .

     >[!TIP]
     >
     >Les formulaires personnalisés ajoutés à la section Détails de la file d’attente sont également associés à tout nouveau problème ajouté au projet. <!--this is confusiong: or the tasks in the Issues  section-->.

1. Continuez à sélectionner les informations des paramètres dans la **Paramètres de la file d’attente des emails** pour permettre aux utilisateurs d’envoyer par courrier électronique des requêtes au projet de file d’attente des demandes.

   Pour plus d’informations, voir [Autorisation des utilisateurs à envoyer par courrier électronique un problème dans un projet de file d’attente des demandes](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Cliquer sur **Enregistrer**.\
   Votre projet a maintenant été configuré pour être une file d’attente de requêtes. Les utilisateurs peuvent désormais y ajouter des requêtes.

1. (Facultatif) Pour améliorer la fonctionnalité File d’attente des demandes, créez des sous-sections supplémentaires pour votre file d’attente, ainsi que des règles pour acheminer les requêtes entrantes vers l’équipe, la personne désignée ou le projet approprié.

   * Pour plus d’informations sur la création de sous-sections pour la file d’attente des demandes, voir les articles [Création de rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) et [Création de groupes de rubriques](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).
   * Pour plus d’informations sur le routage des requêtes vers la personne désignée, l’équipe et le projet approprié, voir [Création de règles de routage](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
