---
title: Modification du profil d’un utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur Adobe Workfront, vous pouvez créer de nouveaux utilisateurs et gérer les profils des utilisateurs existants.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 155a2a8f5f266006629a28917a6a7565a95b37a9
workflow-type: tm+mt
source-wordcount: '3325'
ht-degree: 0%

---

# Modification du profil d’un utilisateur

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

En tant qu’administrateur Adobe Workfront, vous pouvez créer des utilisateurs et gérer les profils des utilisateurs existants. Pour plus d’informations sur la création d’utilisateurs, voir [Ajout d’utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard</p>
   Ou
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez disposer de l’une des options suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
     <li> <p>La variable <b>Utilisateurs</b> dans votre niveau d’accès configuré sur <b>Modifier</b> accès, avec <b>Créer</b> et au moins l’une des deux <b>Administration des utilisateurs</b> options activées sous <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
     <ul><li> Administration des utilisateurs (tous les utilisateurs)</li>
     <li>Administration des utilisateurs (utilisateurs du groupe)</li></ul>
     <p>If  <b>Administration des utilisateurs (utilisateurs de groupe)</b> est activé, vous devez être un administrateur de groupe pour qu’un groupe auquel l’utilisateur est membre puisse modifier l’utilisateur.</p> 
     <p>Pour plus d’informations sur la variable <b>Utilisateurs</b> paramétrer un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table> 
*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Modification d’un profil utilisateur

{{step-1-to-users}}

1. Sélectionnez l’utilisateur, puis cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png).

   La zone Modifier l’utilisateur s’affiche.

1. Dans le **Modifier l’utilisateur** , modifiez les informations suivantes, puis cliquez sur **Enregistrer les modifications** à tout moment :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Infos personnelles </td> 
      <td> 
       <ul> 
        <li><p><b>Prénom</b></p></li>
        <li><p><b>Nom de famille</b></p></li> 
        <li> <p><b>Adresse électronique :</b> L’adresse électronique d’un utilisateur est également son nom d’utilisateur dans Workfront. Ce champ est sensible à la casse et doit être unique. Si un utilisateur tente d’ajouter une adresse électronique non unique trois fois dans une fenêtre de 10 minutes, une réponse reCAPTCHA s’affiche.</p> <p> Sélectionnez la variable <b>Je ne suis pas un robot</b> avant de pouvoir continuer.</p><p>Si vous utilisez la liste autorisée d’email et que vous saisissez un domaine d’email qui ne figure pas dans la liste, l’utilisateur ne recevra pas de notifications par email. Pour plus d’informations sur la liste autorisée, voir <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configuration de votre liste autorisée de messagerie</a>.</p> </li> 
        <li> <p><b>Réinitialiser le mot de passe</b>: cliquez sur ce lien pour réinitialiser le mot de passe de l’utilisateur. Vous devez saisir votre propre mot de passe avant de pouvoir réinitialiser le mot de passe d’un autre utilisateur.</p> <p>Pour réinitialiser le mot de passe d’un autre utilisateur, vous devez être un administrateur Workfront ou un administrateur de groupe.</p> <p><b>REMARQUE</b>:  
          <ul> 
           <li> <p>Si vous êtes administrateur de groupe, vous ne pouvez réinitialiser les mots de passe que pour les utilisateurs des groupes où vous êtes désigné administrateur. En outre, l’autorisation Administrateur utilisateur (utilisateurs de groupe) doit être activée dans votre niveau d’accès :</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Ce paramètre est désactivé par défaut. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </li> 
           <li> <p>Vous ne pouvez pas réinitialiser le mot de passe d’un administrateur Workfront.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; Nom d’utilisateur</b>: si votre administrateur Workfront a activé une intégration SSO avec Workfront, le nom d’utilisateur SSO s’affiche dans ce champ. Le type de configuration SSO activé pour votre instance Workfront est visible dans ce champ. </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; Authentification</b>: si votre administrateur Workfront a activé une intégration SSO avec Workfront et mis à jour tous les utilisateurs pour SSO, ce champ est sélectionné par défaut. Le type de configuration SSO activé pour votre instance Workfront est visible dans ce champ.</p> <p>Lorsque ce champ est sélectionné, l’utilisateur doit se connecter à Workfront avec ses informations d’identification SSO. Si vous la décochez, ils pourront se connecter à Workfront avec leurs informations d’identification Workfront.</p> <p>Pour plus d’informations sur la configuration de Workfront avec une solution d’authentification unique, voir <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Présentation de l’authentification unique dans Adobe Workfront</a></p> <p>Pour plus d’informations sur la mise à jour des utilisateurs pour SSO, voir <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Mise à jour des utilisateurs pour l’authentification unique</a>.</p> 
        <p><b>REMARQUE</b>:</p> 
        <p> Si vous êtes administrateur de groupe, vous pouvez modifier la variable &lt;sso configuration=""&gt; uniquement pour les utilisateurs des groupes dans lesquels vous êtes désigné comme tel. En outre, l’autorisation Administration des utilisateurs (utilisateurs du groupe) doit être activée dans votre niveau d’accès.
        <p>Si vous êtes administrateur de groupe et que l’autorisation Administrateur utilisateur (Tous les utilisateurs) est activée dans votre niveau d’accès, vous pouvez modifier la variable &lt;sso configuration=""&gt; pour tous les utilisateurs.</p> </li> 
        <li><b>Job Info :</b> Informations sur la tâche, comme son titre (dans la section <b>Titre</b> et quel domaine d’expertise l’utilisateur est responsable (dans la variable <b>Me parler</b> ).</li> 
        <li><p><b>Coordonnées</b>: numéro de téléphone de l’utilisateur (dans la variable <b>Numéro de téléphone, Ext.</b>, et <b>Numéro de mobile</b> ) et l’adresse (dans la variable <b>Adresse, Ville, État, Code postal, Pays</b> ).</p>
        <p>Si l’utilisateur est activé pour Unified User Management (UUM) ou Adobe Identity Management System (IMS), la variable <b>Pays</b> dans la section Coordonnées de contact , accepte uniquement les valeurs de code de pays (par exemple, US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Préférences </td> 
      <td> 
       <ul> 
      <li> <p><b>Fuseau horaire :</b> Fuseau horaire de l’utilisateur.</p> <p>Pour plus d’informations sur l’aide apportée aux utilisateurs par le biais de Workfront dans les fuseaux horaires, voir <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Utilisation des fuseaux horaires</a>.</p> </li> 
       <li><b>Paramètres régionaux des emails</b>: langue de messagerie préférée de l’utilisateur. Cela a une incidence sur le format des nombres et des dates dans les emails provenant de Workfront à cet utilisateur.</li>

   <li><b>Réception d’emails à partir de cet environnement de test</b>: cochez cette option si vous souhaitez recevoir des notifications par e-mail de l’environnement actuellement connecté.
      <p><b>NOTE</b></p>
      <p>Cette option est disponible uniquement dans les environnements Aperçu et Sandbox. Par défaut, les notifications électroniques sont activées dans l’environnement de production. </p>
      </li>

   <li><b>Afficher le pourcentage terminé à l’état de mise à jour</b>: cochez cette option si vous souhaitez afficher une barre de pourcentage dans la zone Mise à jour des tâches de cet utilisateur, lors de l’utilisation de l’expérience de commentaire héritée. Pour plus d’informations, voir <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">Nouvelle expérience de commentaire</a>.</li> 
       <li><b>Envoyer le travail que je m’assigne à mon onglet Travail</b>: cochez cette option si vous souhaitez que tout ce que l’utilisateur se donne à lui-même apparaisse directement dans la liste Travailler sur de la zone Accueil . La valeur par défaut est de répertorier tous les éléments affectés à un utilisateur dans sa liste Prêt à démarrer ou Non prêt dans la zone Accueil.</li> 
       <li><b>Générer automatiquement des bons à tirer lors du téléchargement de documents</b>: cochez cette option si vous souhaitez que les documents que l’utilisateur charge génèrent immédiatement un BAT. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td> <p>Sélectionnez les notifications électroniques qui doivent être activées pour le nouvel utilisateur.</p> <p>Vous pouvez sélectionner des notifications instantanées ainsi que des notifications de résumé quotidiennes.</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configuration des notifications d’événement pour tous les membres du système</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accès</td> 
      <td> 
       <ul> 
      <li><b>Est actif :</b> Cochez cette case pour indiquer que l’utilisateur est actif. Les utilisateurs actifs utilisent une licence Workfront. L’effacement de la case désactive l’utilisateur et l’empêche de se connecter à Workfront.</li> 
       <li> <p><b>Niveau d’accès :</b> Sélectionnez le niveau d’accès à affecter à cet utilisateur.</p> 
       <p>Lorsque vous attribuez un niveau d’accès à un utilisateur, vous pouvez attribuer un niveau égal ou inférieur à votre propre niveau d’accès.</p>
       <p>Par exemple, si votre niveau d’accès est Plan, vous ne pouvez pas lui attribuer le niveau d’accès Administrateur. Cependant, vous ne pouvez pas attribuer un niveau d’accès inférieur par défaut à votre propre niveau d’accès si l’administrateur Workfront a activé des autorisations autres que les autorisations par défaut au niveau d’accès qui ne sont pas également activées dans votre propre niveau d’accès. </p>
       <p>Par exemple, si vous disposez d’une licence Plan sans accès aux tâches de suppression, vous ne pouvez pas attribuer à une personne une licence Work ayant accès aux tâches de suppression, bien que la licence Work soit inférieure à la licence Plan. Pour plus d’informations, voir  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> 
       <p>Pour plus d’informations sur les niveaux d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurer l’accès à Adobe Workfront</a>.</p>
       <p> <b>REMARQUE :</b></p> 
       <p> Si votre entreprise utilise le nouveau modèle d’accès (Standard/Clair/Contributeur), vous ne pouvez pas réaffecter un utilisateur standard ou léger à un niveau d’accès Contributeur si cet utilisateur a déjà atteint sa limite de décision pour le mois. </p><p>Pour plus d’informations sur le nouveau modèle d’accès, voir <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">Nouveaux niveaux d’accès - Aperçu</a>. </p><p>Pour plus d’informations sur les limites de décision, voir <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Présentation des documents et des BAT limités pour les utilisateurs non payants</a>.</p></li> 
       <li> <p><b>Modèle de mise en page</b>: choisissez un modèle de disposition pour l’utilisateur. Ce modèle de mise en page a la priorité sur tout modèle de mise en page affecté au groupe d’accueil, à l’équipe d’accueil ou au rôle de Principal de l’utilisateur. Pour plus d’informations sur la priorité d’affectation des modèles de mise en page, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Création et gestion des modèles de mise en page</a>.</p> <p><b>REMARQUE</b>:  <p>La liste suivante décrit la manière dont la liste des modèles disponibles dans ce champ dépend de votre accès :</p> 
       <ul> 
       <li>En tant qu’administrateur Workfront, vous pouvez consulter tous les modèles de mise en page au niveau du système et du groupe.</li> 
       <li>En tant qu’administrateur de groupe, vous pouvez voir un modèle de mise en page au niveau du système, ainsi que les modèles associés aux groupes que vous gérez.</li> 
       <li>En tant qu’utilisateur disposant d’une licence Plan et d’un accès pour modifier les utilisateurs, vous ne pouvez afficher que les modèles de mise en page au niveau du système.</li> 
       </ul> <p>Pour plus d’informations sur les modèles de mise en page au niveau du groupe, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Création et gestion des modèles de mise en page</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisation </td> 
      <td> 
       <ul> 
      <li><b>Société</b>: entreprise de l’utilisateur. Les utilisateurs ne peuvent être associés qu’à une seule entreprise. Vous devez créer une société avant de pouvoir l’associer à un utilisateur. Seules les entreprises actives s’affichent dans la liste. Pour plus d’informations sur la création d’entreprises, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Création et modification d’entreprises</a>.</li> 
      <li><b>Rapports à :</b> Si vous avez spécifié une société pour l’utilisateur, vous pouvez également spécifier le responsable direct de l’utilisateur dans ce champ. Un utilisateur ne peut avoir qu’un seul gestionnaire. Ce champ ne s’affiche pas si l’utilisateur n’est pas d’abord associé à une entreprise. </li> 
      <li><b>Rapports directs :</b> Si vous avez spécifié une société pour l’utilisateur, vous pouvez également spécifier les rapports directs de l’utilisateur. Un utilisateur peut avoir plusieurs rapports directs. Ce champ ne s’affiche pas si l’utilisateur n’est pas d’abord associé à une entreprise.</li> 
      <li><b>Équipe Accueil</b>: spécifiez l’équipe d’accueil de l’utilisateur. Les utilisateurs ne peuvent avoir qu’une seule équipe d’accueil. L’équipe Accueil est importante lors de l’attribution d’un modèle de mise en page ou de la définition du bouton Travailler dessus pour les tâches et les problèmes assignés à l’utilisateur. </li> 
      <li><b>Autres équipes</b>: les utilisateurs peuvent appartenir à plusieurs équipes. Un utilisateur peut afficher les tâches affectées à l’une de ses équipes dans sa zone d’accueil. </li> 
      <li> <p><b>Groupe d’accueil :</b> Sélectionnez un groupe approprié pour affecter l’utilisateur. Cela permet à l’utilisateur d’accéder aux objets partagés avec le groupe. Vous pouvez également partager des modèles de mise en page avec le groupe d’accueil de l’utilisateur.</p> <p>Il s’agit d’un champ obligatoire. Chaque utilisateur doit être associé à un groupe d’accueil. Si vous n’en sélectionnez pas un, votre groupe est désigné comme groupe d’accueil du nouvel utilisateur.</p> <p><b>REMARQUE</b>:</p> 
      <p> Vous ne pouvez affecter un groupe à un utilisateur que si l’une des conditions suivantes est vraie :</p>
      <ul><li>vous êtes un administrateur Workfront.</li>
      <li>vous êtes administrateur du groupe</li>
      <li>le groupe est public.</li></ul> 
      <li> <p><b>Autres groupes</b>: les utilisateurs peuvent appartenir à plusieurs groupes. Vous ne pouvez affecter un groupe à un utilisateur que si vous êtes administrateur de Workfront, que vous êtes administrateur du groupe ou que le groupe est public.</p> <p><b>IMPORTANT</b>:</p> 
      <p>L’ajout d’un utilisateur à plus de 100 groupes peut entraîner des problèmes de performances dans n’importe quelle zone de Workfront qui charge la liste des groupes.</p> <p>Pour plus d’informations sur les groupes publics, voir <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Création d’un groupe</a>.</p> <p>Pour plus d’informations sur les groupes, voir <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Présentation des groupes</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planification des ressources </td> 
      <td> 
       <ul>
       <li>
       <b>Temps de travail</b>: représente le pourcentage de temps équivalent à temps complet (ETR) disponible pour le travail réel de l’utilisateur, sans compter les frais généraux. Le temps de travail doit être un nombre décimal maximum de 1 et ne peut pas être égal à 0. Par exemple, une disponibilité de 20 % pour le travail réel serait de 0,2.

   La valeur par défaut du champ est 1, ce qui indique qu’un utilisateur passe l’intégralité de son éditeur de texte enrichi sur le travail réel lié au projet.

   Le système utilise ce nombre pour calculer la disponibilité de l’utilisateur pour le travail réel lié au projet.

   Pour plus d’informations sur la création de plannings dans Workfront, voir <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Création d’un planning</a>.

   La planification d’exceptions et de congés peut également affecter la capacité de l’utilisateur.

   Workfront calcule la disponibilité d’un utilisateur en fonction des préférences de gestion des ressources de votre zone Configuration. Pour plus d’informations, voir <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configuration des préférences de gestion des ressources</a>.

   <b>CONSEIL</b>

   Définissez la valeur Durée du travail sur 1 pour indiquer que l’utilisateur est disponible pour le travail lié au projet et qu’il dispose de son équivalent à temps plein.
   </li> 
      <li> <b>Planifier la désactivation</b>: cochez cette case si vous souhaitez programmer la désactivation de cet utilisateur à une certaine date et à une certaine heure. </li> 
       <li><b>Date planifiée de désactivation</b>: date et heure auxquelles l’utilisateur est désactivé. Pour plus d’informations sur la planification de la désactivation des utilisateurs, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Planification de la désactivation pour les utilisateurs</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactivation ou réactivation d’un utilisateur</a>.</li> 
       <li> <p><b>Rôle de Principal</b>: rôle de tâche principal que l’utilisateur peut remplir dans Workfront. Chaque tâche et problème auquel l’utilisateur est affecté est également affecté à ce rôle de tâche. Les rôles de tâche sont essentiels dans la gestion des ressources. Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Plan avec accès administrateur ou si vous êtes administrateur Workfront. Pour plus d’informations sur la configuration des utilisateurs disposant d’un accès administrateur, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> <p>Seuls les rôles de tâche actifs s’affichent dans la liste. </p> </li> 
       <li>Si vous avez sélectionné une <b>Rôle de Principal</b>, la variable <b>Pourcentage de disponibilité de l’éditeur de texte enrichi</b> s’affiche. Indiquez le pourcentage de temps du planning de l’utilisateur attribué à ce rôle de tâche. La valeur par défaut du pourcentage de disponibilité de l’éditeur de texte enrichi pour le rôle de Principal est de 100 %. </li> 
       <li> <p><b>Autres rôles</b>: un utilisateur peut avoir plusieurs rôles de tâche dans Workfront. Les rôles de tâche sont essentiels dans la gestion des ressources. Le nombre de rôles de tâche qu’un utilisateur peut remplir n’est pas limité. Cependant, nous vous recommandons de ne pas affecter un utilisateur à un trop grand nombre de rôles de tâche, car la gestion des ressources peut devenir trop complexe pour ces utilisateurs.<p>Seuls les rôles de tâche actifs s’affichent dans la liste. Pour plus d’informations sur les rôles de tâche, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Création et gestion des rôles de tâche</a>.</p> <p>Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Plan avec accès administrateur ou si vous êtes administrateur Workfront. <br>Pour plus d’informations sur la configuration des utilisateurs disposant d’un accès administrateur, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
       <li> <p>(Conditionnel) Si vous avez sélectionné une ou plusieurs <b>Autres rôles</b>, la variable <b>Pourcentage de disponibilité de l’éditeur de texte enrichi</b> s’affiche pour chaque rôle. Indiquez le pourcentage de temps du planning de l’utilisateur attribué à chaque rôle de tâche. La valeur par défaut pour le pourcentage de disponibilité de l’éditeur de texte enrichi pour les autres rôles est de 0 %.</p> <p><b>REMARQUE</b>: si d’autres rôles ont une disponibilité de l’éditeur de texte enrichi de 0 %, ils ne s’affichent pas dans le planificateur de ressources, sauf si les utilisateurs sont affectés à des tâches dans ces rôles.</p> <p> <img alt="user_settings_fields_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>REMARQUE</b>: <p>La somme de tous les <b>Pourcentages de disponibilité de l’éditeur de texte enrichi</b> pour tous les rôles, doit être égal à 100 %. Chaque pourcentage de disponibilité de l’éditeur de texte enrichi calcule les heures disponibles pour chaque rôle par utilisateur dans le planificateur de ressources. Les Heures disponibles pour chaque rôle par utilisateur dépendent de l’heure disponible pour l’utilisateur.</p> <p>L’heure disponible pour l’utilisateur est calculée par Workfront selon la méthode sélectionnée par l’administrateur Workfront pour calculer l’éditeur de texte enrichi dans les préférences de gestion des ressources.</p> <p>Pour plus d’informations sur le calcul de la disponibilité de l’utilisateur, voir <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Présentation du calcul des heures et de l’éditeur de texte enrichi pour les utilisateurs et les rôles dans le planificateur de ressources</a>.</p> <p>Pour plus d’informations sur la configuration des préférences de gestion des ressources, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configuration des préférences de gestion des ressources</a>.</p> </p>
       <span class="preview"><p>(Facultatif) Les affectations de rôles de tâche à date effective sont utilisées dans les calculs financiers si le rôle de tâche de l’utilisateur change au cours d’un projet.</p><p>Cliquez sur <b>Définition des rôles par date</b>, sélectionnez la variable <b>Rôle de Principal</b> et <b>Autres rôles</b>, puis saisissez le pourcentage d’attribution pour chaque rôle. Les rôles peuvent être identiques aux rôles existants (en utilisant différents pourcentages) ou de nouveaux rôles. Sélectionnez la variable <b>Date de début</b> lorsque ces rôles deviennent actifs. Il peut s’agir d’une date ultérieure. Lorsque les rôles les plus récents deviennent actifs, vous pouvez cliquer sur <b>Afficher les rôles précédents</b> pour afficher les rôles précédents inactifs.</p> </li></span>
       <li> <p><b>Planification</b>: associez une planification à l’utilisateur. Le planning de l’utilisateur calcule la chronologie des tâches auxquelles l’utilisateur est affecté.</p> <p>Vous devez créer une planification avant de pouvoir l’associer à un utilisateur. Pour plus d’informations sur la création de plannings, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Création d’un planning</a>.</p> <p><b>REMARQUE</b>: il est recommandé que le planning que vous associez à l’utilisateur corresponde au fuseau horaire de l’utilisateur.</p> </li> 
       <li> <p><b>Profil de feuille de calcul</b>: associez un profil de feuille de temps à l’utilisateur pour vous assurer que les feuilles de temps sont générées automatiquement pour l’utilisateur.</p> <p><b>REMARQUE</b>: la liste des profils disponibles dans ce champ dépend de votre accès :
       <ul>
       <li>En tant qu’administrateur Workfront, vous pouvez consulter tous les profils de feuille de calcul au niveau du système et de tous les groupes.</li>
       <li>En tant qu’administrateur de groupe, vous pouvez consulter les profils de feuille de temps au niveau du système, ainsi que ceux associés aux groupes que vous gérez.</li>
       <li>En tant qu’utilisateur disposant d’une licence Plan et d’un accès pour modifier les utilisateurs, vous ne pouvez afficher que les profils de feuille de temps au niveau du système. Pour plus d’informations sur les profils de feuille de calcul au niveau du groupe, voir <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Création, modification et affectation de profils de feuille de temps</a>.</li>
      </ul></p> </li> 
       <li><b>Type d’heure par défaut</b>: sélectionnez le type d’heure par défaut pour l’utilisateur. Il s’agit du type d’heure utilisé par défaut lorsque l’utilisateur consigne l’heure.</li> 
       <li><b>Types d’heure disponibles</b>: sélectionnez les types d’heures qui doivent être disponibles pour l’utilisateur. Ces types d’heure sont visibles partout dans Workfront, où l’utilisateur peut consigner l’heure. Un utilisateur peut uniquement afficher les types d’heures activés au niveau du projet ainsi qu’au niveau de l’utilisateur. Pour plus d’informations sur les types d’heures disponibles pour les utilisateurs, voir <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Définition des types d’heures et de la disponibilité des feuilles de temps</a>.</li> 
       <li><b>Temps de connexion :</b> Indiquez si l’utilisateur doit se connecter aux tâches en heures ou en jours. Pour plus d’informations, voir <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configurer si l’heure est connectée en heures ou en jours</a>.</li>

   <li> <b>FTE</b>: il s’agit de l’équivalent temps plein de l’utilisateur. Workfront utilise ce nombre pour calculer la disponibilité de l’utilisateur en fonction de la planification par défaut uniquement lorsque les préférences de gestion des ressources au niveau du système sont définies sur la planification par défaut.

   <p>L’éditeur de texte enrichi indique le temps que l’utilisateur peut consacrer à son travail. Cela inclut les frais généraux et le temps passé sur le projet. Par exemple, le temps passé dans les réunions ou la formation est également inclus dans l’éditeur de texte enrichi.</p>

   L’éditeur de texte enrichi doit être un nombre décimal maximum de 1 et ne peut pas être égal à 0. Par exemple, si la valeur de l’éditeur de texte enrichi est 0,5 et que la planification par défaut dans Workfront est de 40 heures, l’utilisateur est disponible pendant 20 heures par semaine.

   La valeur par défaut du champ est 1.

   Planifiez des exceptions, des heures de congé et la valeur du temps de travail peut affecter la disponibilité de l’utilisateur.

   Workfront calcule la disponibilité d’un utilisateur en fonction des préférences de gestion des ressources de votre zone Configuration.

   Si les préférences de gestion des ressources au niveau du système sont définies sur la planification de l’utilisateur, la valeur que vous indiquez ici est ignorée et l’utilisateur est considéré comme disponible selon ce qui est spécifié dans sa planification.

   Pour plus d’informations, voir <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configuration des préférences de gestion des ressources</a>.

   Pour plus d’informations sur la création de plannings dans Workfront, voir <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Création d’un planning</a>.
   </li>

   <li><b>Pools de ressources</b>: associez l’utilisateur aux pools de ressources. Pour plus d’informations, voir <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Association des pools de ressources aux utilisateurs </a>.</li>

   <li><b>Taux de coût</b>: montant du coût par heure pour l’utilisateur.
      <p>Pour consulter les taux de coût en vigueur à la date, cliquez sur <strong>Taux d’ajout</strong>. Saisissez la valeur du taux de coût pour la période et attribuez une Date de début et une Date de fin, le cas échéant. Le Taux de coût 1 n'aura pas de date de début et le dernier Taux de coût n'aura pas de date de fin.</p><p>Certaines dates sont ajoutées automatiquement. Par exemple, si le Taux de coût 1 n’a pas de date de fin et que vous ajoutez le Taux de coût 2 avec une date de début du 1er mai 2023, une date de fin du 30 avril 2023 est ajoutée au Taux de coût 1 afin qu’il n’y ait aucune différence.</p></li>

   <li><b>Taux de facturation</b>: montant de la facturation par heure pour l’utilisateur.
      <p>Pour connaître les taux de facturation en vigueur à la date, cliquez sur <strong>Taux d’ajout</strong>. Saisissez la valeur du taux de facturation pour la période et attribuez une date de début et une date de fin selon vos besoins. Le taux de facturation 1 ne comporte pas de date de début et le dernier taux de facturation n’a pas de date de fin.</p> <p>Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de facturation 1 ne comporte pas de date de fin et que vous ajoutez une seconde avec une date de début du 1er mai 2023, une date de fin du 30 avril 2023 est ajoutée au taux de facturation 1 afin qu’il n’y ait aucune différence.</p><p> <img alt="Coût utilisateur et taux de facturation" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulaires personnalisés</td> 
      <td><p>Associez un formulaire personnalisé utilisateur existant à cet utilisateur. Vous devez créer un formulaire personnalisé pour pouvoir l’associer à un utilisateur. Seuls les formulaires personnalisés actifs s’affichent dans la liste. Les champs que vous n’avez pas accès à la modification ne s’affichent pas dans un formulaire personnalisé individuel.</p> <p><span class="preview"><strong>Remarque :</strong> Les fonctionnalités avancées de formulaire personnalisé telles que les champs de recherche externe et les champs natifs de Workfront ne sont disponibles que lorsque vous ouvrez l’enregistrement de l’utilisateur sur la page de détails, et non dans la boîte de dialogue Modifier l’utilisateur . (Dans la liste des utilisateurs, cliquez sur le nom de l’utilisateur pour ouvrir les détails.)</span></p> <p>Pour plus d’informations sur la création de formulaires personnalisés, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Création ou modification d’un formulaire personnalisé</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Commentaire</td> 
      <td>Saisissez le commentaire à envoyer aux utilisateurs et à la zone Mises à jour de leurs profils utilisateur.</td> 
     </tr> 
    </tbody> 
   </table>
