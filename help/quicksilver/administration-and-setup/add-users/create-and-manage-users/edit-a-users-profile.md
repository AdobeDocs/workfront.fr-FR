---
title: Modification du profil d’un utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer de nouveaux utilisateurs et utilisatrices et gérer les profils existants.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: e9d1e35a9c94143a84eb2007985a42f0960a09f7
workflow-type: tm+mt
source-wordcount: '3261'
ht-degree: 94%

---

# Modifier le profil d’un utilisateur ou d’une utilisatrice

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

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer des utilisateurs et utilisatrices et gérer les profils existants. Pour plus d’informations sur la création d’utilisateurs et utilisatrices, voir [Ajouter des utilisateurs et utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p><p>Ou</p><p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur système. </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De ces deux options, si <b>User Admin (Group Users)</b> est activé, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier un profil utilisateur

{{step-1-to-users}}

1. Sélectionnez l’utilisateur ou l’utilisatrice, puis cliquez sur l’icône **Modifier** ![](assets/edit-icon.png).

   La zone Modifier l’utilisateur ou l’utilisatrice s’affiche.

1. Dans la zone **Modifier l’utilisateur ou l’utilisatrice**, modifiez les informations suivantes, puis cliquez sur **Enregistrer les modifications** à tout moment :

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
        <li> <p><b>Adresse e-mail :</b> l’adresse e-mail d’un utilisateur ou d’une utilisatrice correspond à son nom dans Workfront. Ce champ est sensible à la casse et doit être unique. Si un utilisateur ou une utilisatrice tente d’ajouter une adresse e-mail non unique trois fois en moins de 10 minutes, une réponse reCAPTCHA s’affiche.</p> <p> Sélectionnez <b>Je ne suis pas un robot</b> pour pouvoir continuer.</p><p>Si vous utilisez la liste autorisée d’e-mails et que vous saisissez un domaine d’e-mail qui ne figure pas dans la liste, l’utilisateur ou l’utilisatrice ne recevra pas de notifications par e-mail. Pour plus d’informations sur la liste autorisée, voir <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configurer votre liste autorisée d’e-mails</a>.</p> </li> 
        <li> <p><b>Réinitialisation du mot de passe</b> : cliquez sur ce lien pour réinitialiser le mot de passe de l’utilisateur ou de l’utilisatrice. Vous devez saisir votre propre mot de passe avant de pouvoir réinitialiser le mot de passe d’un autre utilisateur ou d’une autre utilisatrice.</p> <p>Pour réinitialiser le mot de passe d’une autre personne, vous devez être administrateur ou administratrice Workfront ou de groupes.</p> <p><b>NOTE</b> :  
          <ul> 
           <li> <p>Si vous êtes administrateur ou administratrice de groupes, vous ne pouvez réinitialiser les mots de passe que des personnes membres des groupes que vous administrez. En outre, l’autorisation Administration des utilisateurs et utilisatrices (utilisateurs et utilisatrices de groupe) doit être activée dans votre niveau d’accès :</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Ce paramètre est désactivé par défaut. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </li> 
           <li> <p>Vous ne pouvez pas réinitialiser le mot de passe d’un administrateur ou d’une administratrice Workfront.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;SSO Configuration&gt; Nom d’utilisateur ou d’utilisatrice</b> : si votre équipe d’administration Workfront a activé une intégration SSO avec Workfront, le nom d’utilisateur ou d’utilisatrice SSO s’affiche dans ce champ. Le type de configuration SSO activé pour votre instance Workfront apparaît dans ce champ. </li> 
        <li> <p><b>Autoriser l’authentification &lt;SSO Configuration&gt; uniquement</b> : si votre équipe d’aministration Workfront a activé une intégration SSO avec Workfront et mis à jour tous les utilisateurs et utilisatrices pour la SSO, ce champ est sélectionné par défaut. Le type de configuration SSO activé pour votre instance Workfront apparaît dans ce champ.</p> <p>Lorsque ce champ est sélectionné, l’utilisateur ou l’utilisatrice doit se connecter à Workfront avec ses informations d’identification SSO. Si vous la décochez, les utilisateurs et utilisatrices pourront se connecter à Workfront avec leurs informations d’identification Workfront.</p> <p>Pour plus d’informations sur la configuration de Workfront avec une solution d’authentification unique (SSO), voir <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Vue d’ensemble de l’authentification unique dans Adobe Workfront</a>.</p> <p>Pour plus d’informations sur la mise à jour des utilisateurs et utilisatrices pour la solution SSO, voir <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Mise à jour des utilisateurs et utilisatrices pour l’authentification unique</a>.</p> 
        <p><b>NOTE</b> :</p> 
        <p> Si vous êtes administrateur ou administratrice de groupes, vous pouvez modifier les champs &lt;SSO Configuration&gt; uniquement pour les utilisateurs et utilisatrices des groupes que vous administrez. En outre, l’autorisation Administration des utilisateurs et utilisatrices (utilisateurs et utilisatrices du groupe) doit être activée dans votre niveau d’accès.
        <p>Si vous êtes administrateur ou administratrice de groupes et que l’autorisation Administration des utilisateurs et utilisatrices (tous les utilisateurs et utilisatrices) est activée dans votre niveau d’accès, vous pouvez modifier les champs &lt;SSO Configuration&gt; pour tous les utilisateurs et toutes les utilisatrices.</p> </li> 
        <li><b>Informations sur le traitement :</b> informations sur le traitement, telles que son titre (dans le champ <b>Titre</b>) ou le domaine d’expertise pour lequel l’utilisateur ou l’utilisatrice est responsable (dans le champ <b>Me parler de</b>).</li> 
        <li><p><b>Coordonnées</b> : numéro de téléphone de l’utilisateur ou de l’utilisatrice (dans les champs <b>Numéro de téléphone, ext.</b>, et <b>Numéro de téléphone portable</b>) et adresse (dans les champs <b>Adresse, Ville, État, Code postal, Pays</b>).</p>
        <p>Si Unified User Management (UUM) ou Adobe Identity Management System (IMS) sont activés pour l’utilisateur ou l’utilisatrice, le champ <b>Pays</b> dans la section Coordonnées accepte uniquement les valeurs de code de pays (par exemple, US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Préférences </td> 
      <td> 
       <ul> 
      <li> <p><b>Fuseau horaire :</b> fuseau horaire des utilisateurs et utilisatrices.</p> <p>Pour plus d’informations sur l’aide apportée aux utilisateurs et utilisatrices par le biais de Workfront dans les différents fuseaux horaires, voir <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Utilisation des fuseaux horaires</a>.</p> </li>

   <li><p><b>Locale d’e-mail</b> : paramètres régionaux d’e-mails préférés des utilisateurs et utilisatrices. Cela affecte le format des nombres et des dates dans les e-mails envoyés par Workfront à cet utilisateur ou cette utilisatrice.</p>
      <p><b>REMARQUE :</b> Lorsque votre organisation se trouve dans l’expérience unifiée de l’Adobe, les préférences linguistiques de l’utilisateur sont stockées dans son profil d’Adobe et la langue de l’email n’est pas utilisée. Pour plus d’informations sur l’accès à ces préférences, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></li>

   <li><b>Recevoir des e-mails de cet environnement de test</b> : cochez cette option si vous souhaitez recevoir des notifications par e-mail de l’environnement actuellement connecté.
      <p><b>NOTE</b></p>
      <p>Cette option n’est actuellement disponible que dans les environnements Prévisualisation et Sandbox. Par défaut, les notifications par e-mail sont activées dans l’environnement de production. </p>
      </li>

   </li> 
       <li><b>Envoyez du travail que je m’assigne à mon onglet Travail sur l’onglet </b> : ce paramètre fait référence à une fonctionnalité obsolète qui a été supprimée de Workfront.</li> 
       <li><b>Générer automatiquement des épreuves lors du chargement de documents</b> : cochez cette option si vous souhaitez que les documents que l’utilisateur ou l’utilisatrice charge génèrent immédiatement une épreuve. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td> <p>Sélectionnez les notifications par e-mail qui doivent être activées pour le nouvel utilisateur ou la nouvelle utilisatrice.</p> <p>Vous pouvez sélectionner des notifications instantanées ou une synthèse des notifications quotidienne.</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurer les notifications d’événements pour tous les utilisateurs et utilisatrices du système</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accès</td> 
      <td> 
       <ul> 
      <li><b>Est actif :</b> cochez cette case pour indiquer que l’utilisateur ou l’utilisatrice est actif. Les utilisateurs et utilisatrices actifs utilisent une licence Workfront. L’effacement de la case désactive l’utilisateur ou l’utilisatrice et l’empêche de se connecter à Workfront.</li> 
       <li> <p><b>Niveau d’accès :</b> sélectionnez le niveau d’accès à affecter à cet utilisateur ou cette utilisatrice.</p> 
       <p>Lorsque vous attribuez un niveau d’accès à un utilisateur ou à une utilisatrice, vous pouvez attribuer un niveau égal ou inférieur à votre propre niveau d’accès.</p>
       <p>Par exemple, si votre niveau d’accès est Planificateur, vous ne pouvez pas lui attribuer le niveau d’accès Administrateur ou Administratrice. Cependant, vous ne pouvez pas attribuer un niveau d’accès inférieur par défaut à votre propre niveau d’accès si l’administrateur ou l’administratrice Workfront a activé des autorisations autres que les autorisations par défaut au niveau d’accès qui ne sont pas également activées dans votre propre niveau d’accès. </p>
       <p>Par exemple, si vous disposez d’une licence Plan sans accès aux tâches de suppression, vous ne pouvez pas attribuer à une personne une licence Travail ayant accès aux tâches de suppression, bien que la licence Travail soit inférieure à la licence Plan. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>. </p> 
       <p>Pour plus d’informations sur les niveaux d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurer l’accès à Adobe Workfront</a>.</p>
       <p> <b>REMARQUE :</b></p> 
       <p> Si votre entreprise utilise le nouveau modèle d’accès (Standard/Light/Contributeur ou Contributrice), vous ne pouvez pas réaffecter un utilisateur Standard ou Light à un niveau d’accès Contributeur ou Contributrice si cet utilisateur ou cette utilisatrice a déjà atteint sa limite de décision pour le mois. </p><p>Pour plus d’informations sur le nouveau modèle d’accès, voir <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">Vue d’ensemble des nouveaux niveaux d’accès</a>. </p><p>Pour plus d’informations sur les limites de décision, voir <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Vue d’ensemble du statut de décision limitée des documents et de l’épreuve pour les utilisateurs et utilisatrices non payants</a>.</p></li> 
       <li> <p><b>Modèle de mise en page</b> : choisissez un modèle de mise en page pour l’utilisateur ou l’utilisatrice. Ce modèle de mise en page a la priorité sur tout modèle de mise en page affecté au groupe principal, à l’équipe principale ou à la fonction principale de l’utilisateur ou l’utilisatrice. Pour plus d’informations sur la priorité d’affectation des modèles de mise en page, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Créer et gérer des modèles de mise en page</a>.</p> <p><b>REMARQUE</b> :  <p>La liste suivante décrit la manière dont la liste des modèles disponibles dans ce champ dépend de votre accès :</p> 
       <ul> 
       <li>En tant qu’administrateur ou administratrice Workfront, vous pouvez consulter tous les modèles de mise en page au niveau du système et du groupe.</li> 
       <li>En tant qu’administrateur ou administratrice de groupes, vous pouvez voir le modèle de disposition au niveau du système, ainsi que ceux associés aux groupes que vous gérez.</li> 
       <li>Si vous disposez d’une licence de plan et d’un accès à la modification des utilisateurs et utilisatrices, vous ne pouvez voir que les modèles de disposition au niveau du système.</li> 
       </ul> <p>Pour plus d’informations sur les modèles de disposition au niveau du groupe, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Créer et gérer des modèles de disposition</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisation </td> 
      <td> 
       <ul> 
      <li><b>Entreprise</b> : entreprise des utilisateurs et utilisatrices. Les personnes ne peuvent être associées qu’à une seule entreprise. Vous devez créer une entreprise avant de pouvoir l’associer à une personne. Seules les entreprises actives sont affichées dans la liste. Pour plus d’informations sur la création d’entreprises, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Créer et modifier des entreprises</a>.</li> 
      <li><b>Rend compte à :</b> si vous avez spécifié une entreprise pour l’utilisateur ou l’utilisatrice, vous pouvez également indiquer la personne responsable directe de l’utilisateur ou utilisatrice dans ce champ. Un utilisateur ou une utilisatrice ne peut avoir qu’une seule personne responsable. Ce champ ne s’affiche pas si l’utilisateur ou utilisatrice n’est pas d’abord associé à une entreprise. </li> 
      <li><b>Rapports directs :</b> si vous avez spécifié une entreprise pour l’utilisateur ou l’utilisatrice, vous pouvez également indiquer les rapports directs de l’utilisateur ou utilisatrice. Un utilisateur ou une utilisatrice peut avoir plusieurs rapports directs. Ce champ ne s’affiche pas si l’utilisateur ou utilisatrice n’est pas d’abord associé à une entreprise.</li> 
      <li><b>Équipe principale</b> : indiquez l’équipe principale de l’utilisateur ou utilisatrice. Les personnes ne peuvent avoir qu’une seule équipe principale. L’équipe principale est importante lors de l’attribution d’un modèle de disposition ou de la définition du bouton Travailler dessus pour les tâches et les problèmes assignés à l’utilisateur ou utilisatrice. </li> 
      <li><b>Autres équipes</b> : les personnes peuvent appartenir à plusieurs équipes. Un utilisateur ou une utilisatrice peut afficher les éléments de travail affectés à l’une de ses équipes dans sa zone d’accueil. </li> 
      <li> <p><b>Groupe principal :</b> sélectionnez un groupe en guise de groupe principal des personnes. La personne peut ainsi accéder aux objets partagés avec le groupe. Vous pouvez également partager des modèles de disposition avec le groupe principal de l’utilisateur ou utilisatrice.</p> <p>Champ obligatoire. Chaque utilisateur et utilisatrice doit être associé à un groupe principal. Si vous n’en sélectionnez pas, votre groupe d’accueil est désigné comme groupe d’accueil du nouvel utilisateur.</p> <p><b>REMARQUE</b> :</p> 
      <p> Vous ne pouvez affecter un groupe à une personne que si l’une des conditions suivantes est vraie :</p>
      <ul><li>Vous êtes un administrateur ou une administratrice Workfront.</li>
      <li>Vous êtes l’administrateur ou l’administratrice du groupe.</li>
      <li>Le groupe est public.</li></ul> 
      <li> <p><b>Autres groupes</b> : les personnes peuvent appartenir à plusieurs groupes. Vous ne pouvez affecter un groupe à un utilisateur ou une utilisatrice que si vous êtes un administrateur ou une administratrice Workfront, que si vous êtes administrateur ou administratrice du groupe ou que si le groupe est public.</p> <p><b>IMPORTANT</b> :</p> 
      <p>L’ajout d’une personne à plus de 100 groupes peut entraîner des problèmes de performances dans n’importe quelle zone de Workfront qui charge la liste des groupes.</p> <p>Pour plus d’informations sur les groupes publics, voir <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Créer un groupe</a>.</p> <p>Pour plus d’informations sur les groupes, voir <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Vue d’ensemble des groupes</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planification des ressources </td> 
      <td> 
       <ul>
       <li>
       <b>Temps de travail</b> : représente le pourcentage du temps équivalent temps plein (FTE) que la personne peut consacrer au travail effectif, hors durée supplémentaire. Le temps de travail doit être un nombre décimal inférieur ou égal à 1 et ne peut pas être égal à 0. Par exemple, une disponibilité de 20 % pour le travail effectif serait de 0,2.

   La valeur par défaut de ce champ est 1, ce qui indique que la personne consacre la totalité de son équivalent temps complet au travail réel lié au projet.

   Le système utilise ce nombre pour calculer la disponibilité de la personne quant au travail réel lié au projet.

   Pour plus d’informations sur la création de plannings dans Workfront, voir <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Créer un planning</a>.

   Les exceptions au planning et les congés peuvent également affecter la capacité de la personne.

   Workfront calcule la disponibilité d’une personne en fonction des préférences de gestion des ressources dans votre zone de configuration. Pour plus d’informations, voir <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurer les préférences de gestion des ressources</a>.

   <b>CONSEIL</b>

   Définissez la valeur Temps de travail sur 1 pour indiquer que la personne est disponible pour effectuer le travail lié au projet pendant la totalité de son équivalent temps plein.
   </li> 
      <li> <b>Planifier la désactivation</b> : cochez cette case si vous souhaitez programmer la désactivation de cette personne à une certaine date et à une certaine heure. </li> 
       <li><b>Date de désactivation planifiée</b> : date et heure auxquelles l’utilisateur ou l’utilisatrice sont désactivés. Pour plus d’informations sur la planification de la désactivation des utilisateurs et des utilisatrices, consultez la section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Planification de la désactivation des utilisateurs et des utilisatrices</a> dans <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactivation ou réactivation d’un utilisateur ou d’une utilisatrice</a>.</li> 
       <li> <p><b>Rôle principal</b> : le rôle principal de tâche que l’utilisateur ou l’utilisatrice peut remplir dans Workfront. Chaque tâche et chaque problème affecté à un utilisateur ou à une utilisatrice est également affecté à cette fonction. Les fonctions sont essentielles à la gestion des ressources. Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Plan avec un accès utilisateur administratif, ou si vous êtes un administrateur ou une administratrice Workfront. Pour plus d’informations sur la configuration des utilisateurs et des utilisatrices disposant d’un accès d’administration, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder un accès aux utilisateurs et aux utilisatrices</a>.</p> <p>Seules les fonctions actives s’affichent dans la liste. </p> </li> 
       <li>Si vous avez sélectionné une <b>fonction principale</b>, le champ <b>Pourcentage d’équivalent temps complet</b> s’affiche. Indiquez le pourcentage de temps du planning de l’utilisateur ou de l’utilisatrice affecté à cette fonction. La valeur par défaut du pourcentage de disponibilité équivalent temps complet pour le rôle principal est de 100 %. </li> 
       <li> <p><b>Autres fonctions</b> : un utilisateur ou une utilisatrice peut avoir plusieurs fonctions dans Workfront. Les fonctions sont essentielles à la gestion des ressources. Une personne peut remplir un nombre illimité de fonctions. Toutefois, nous recommandons de ne pas affecter un nombre excessivement élevé de fonctions à une personne, car la gestion des ressources pourrait devenir trop complexe pour ces personnes.<p>Seules les fonctions actives s’affichent dans la liste. Pour plus d’informations sur les fonctions, consultez la section <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Créer et gérer des fonctions</a>.</p> <p>Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Plan avec un accès utilisateur administratif, ou si vous êtes un administrateur ou une administratrice Workfront. <br>Pour plus d’informations sur la configuration des utilisateurs et des utilisatrices disposant d’un accès d’administration consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder un accès aux utilisateurs et aux utilisatrices</a>.</p> </li> 
       <li> <p>(Le cas échéant) Si vous avez sélectionné une ou plusieurs <b>Autres fonctions</b>, le champ <b>Pourcentage de disponibilité de temps complet</b> s’affiche pour chaque fonction. Indiquez le pourcentage de temps du planning de l’utilisateur ou de l’utilisatrice affecté à chaque fonction. La valeur par défaut du pourcentage de disponibilité équivalent temps complet pour les autres rôles est de 0 %.</p> <p><b>NOTE</b> : dans le planificateur de ressources, si d’autres fonctions ont un pourcentage de disponibilité de temps complet de 0 %, elles ne s’affichent pas, à moins que des tâches de ces fonctions ne soient affectées à des utilisateurs et des utilisatrices.</p> <p> <img alt="user_settings_fields_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTE</b> : <p>La somme de tous les <b>pourcentages de disponibilité de l’équivalent temps complet</b> pour toutes les fonctions, doit être égale à 100 %. Chaque pourcentage de disponibilité équivalent temps complet calcule les heures disponibles pour chaque rôle par personne dans le planificateur de ressources. Les heures disponibles pour chaque rôle par personne dépendent du temps disponible pour la personne.</p> <p>Le temps disponible pour la personne est calculé par Workfront en fonction de la méthode sélectionnée par l’administration Workfront pour calculer l’équivalent temps complet dans les préférences de gestion des ressources.</p> <p>Pour plus d’informations sur le calcul de la disponibilité de l’utilisateur ou de l’utilisatrice, consultez la section <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Vue d’ensemble du calcul des heures et de l’équivalent temps complet pour les utilisateurs et les utilisatrices et les fonctions dans le planificateur de ressources</a>.</p> <p>Pour plus d’informations sur la configuration des préférences de gestion des ressources, consultez la section <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurer les préférences de gestion des ressources</a>.</p> </p>
       <span class="preview"><p>(Facultatif) Les affectations de fonctions par date d’entrée en vigueur sont utilisées dans les calculs financiers si la fonction de l’utilisateur ou de l’utilisatrice change au cours d’un projet.</p><p>Cliquez sur <b>Définir les fonctions par date</b>, sélectionnez <b>Fonction principale</b> et <b>Autres fonctions</b>, puis saisissez le pourcentage d’affectation pour chaque fonction. Les fonctions peuvent être les mêmes que les fonctions existantes (en utilisant des pourcentages différents), ou de nouvelles fonctions. Sélectionnez la <b>Date de début</b> lorsque ces fonctions deviennent actives. Il peut s’agir d’une date future. Lorsque les fonctions les plus récentes deviennent actives, vous pouvez cliquer sur <b>Afficher les fonctions précédentes</b> pour afficher les fonctions précédentes inactives.</p> </li></span>
       <li> <p><b>Planning</b> : associer un planning à l’utilisateur ou à l’utilisatrice. Le planning de l’utilisateur ou de l’utilisatrice calcule la chronologie des tâches qui lui sont affectées.</p> <p>Vous devez créer un planning avant de pouvoir l’associer à un utilisateur ou à une utilisatrice. Pour plus d’informations sur la création de plannings, consultez la section <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Créer un planning</a>.</p> <p><b>NOTE</b> : nous recommandons que l’horaire associé à l’utilisateur ou à l’utilisatrice corresponde à son fuseau horaire.</p> </li> 
       <li> <p><b>Profil de feuille de temps</b> : pour vous assurer que les feuilles de temps sont générées automatiquement pour l’utilisateur ou l’utilisatrice, associez lui un profil de feuille de temps.</p> <p><b>NOTE</b> : la liste des profils disponibles dans ce champ dépend de votre accès :
       <ul>
       <li>En tant que membre de l’équipe d’administration de Workfront, vous pouvez consulter tous les profils de feuille de temps au niveau du système et de tous les groupes.</li>
       <li>En tant qu’administrateur ou administratrice de groupes, vous pouvez voir les profils de feuille de temps au niveau du système, ainsi que ceux associés aux groupes que vous gérez.</li>
       <li>En tant qu’utilisateur ou utilisatrice disposant d’une licence intégrale et d’un accès pour modifier les utilisateurs et les utilisatrices, vous ne pouvez afficher que les profils de feuille de temps au niveau du système. Pour plus d’informations sur les profils de feuille de temps au niveau du groupe, consultez la section <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Créer, modifier et affecter des profils de feuille de temps</a>.</li>
      </ul></p> </li> 
       <li><b>Type d’heure par défaut</b> : sélectionner le type d’heure par défaut pour l’utilisateur ou l’utilisatrice. Il s’agit du type d’heure utilisé par défaut lorsque l’utilisateur ou l’utilisatrice consigne les heures.</li> 
       <li><b>Types d’heure disponibles</b> : sélectionner les types d’heures qui doivent être disponibles pour l’utilisateur ou l’utilisatrice. Ces types d’heures sont visibles dans tous les emplacements Workfront où l’utilisateur ou l’utilisatrice peut consigner des heures. Une personne ne peut voir que les types d’heures qui sont activés au niveau du projet et au niveau de la personne. Pour plus d’informations sur les types d’heures disponibles pour les utilisateurs, voir <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Définition des types d’heures et disponibilité</a>.</li> 
       <li><b>Temps de connexion :</b> sélectionner si l’utilisateur ou l’utilisatrice doit consigner le temps des éléments de travail en heures ou en jours. Pour plus d’informations, consultez la section <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configurer si le temps est enregistré en heures ou en jours</a>.</li>

   <li> <b>Équivalent temps complet</b> : il s’agit de l’équivalent temps complet de l’utilisateur ou de l’utilisatrice. Workfront utilise ce nombre pour calculer la disponibilité de la personne en fonction du planning par défaut uniquement lorsque les préférences de gestion des ressources au niveau du système sont définies sur « Le planning par défaut ».

   <p>L’équivalent temps complet indique le temps que la personne peut consacrer au travail. Cela comprend les durées supplémentaires, ainsi que le temps consacré au travail sur les projets. Par exemple, le temps passé en réunion ou en formation est également inclus dans l’équivalent temps complet.</p>

   L’équivalent temps complet doit être un nombre décimal inférieur ou égal à 1 et ne peut pas être égal à 0. Par exemple, si la valeur de l’équivalent temps complet est de 0,5 et que l’horaire par défaut dans Workfront est de 40 heures, la personne est disponible 20 heures par semaine.

   La valeur par défaut de ce champ est 1.

   Les exceptions de planning, les congés éventuels et la valeur du temps de travail peuvent affecter la disponibilité de la personne.

   Workfront calcule la disponibilité d’une personne en fonction des préférences de gestion des ressources dans votre zone de configuration.

   Si les préférences de gestion des ressources au niveau du système sont définies sur le planning de la personne, la valeur que vous spécifiez ici est ignorée et la personne est considérée comme étant disponible selon ce qui est spécifié dans son planning.

   Pour plus d’informations, consultez la section <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurer les préférences de gestion des ressources</a>.

   Pour plus d’informations sur la création de plannings dans Workfront, consultez la section <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Créer un planning</a>.
   </li>

   <li><b>Groupes de ressources</b> : associer l’utilisateur ou l’utilisatrice aux groupes de ressources. Pour plus d’informations, consultez la section <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associer des groupes de ressources aux utilisateurs et aux utilisatrices </a>.</li>

   <li><b>Taux de dépenses</b> : montant des dépenses par heure pour l’utilisateur ou l’utilisatrice.
      <p>Pour connaitre les taux de dépenses effectifs par date, cliquez sur <strong>Ajouter un taux</strong>. Saisissez la valeur du taux de dépenses pour la période et affectez une date de début et une date de fin, le cas échéant. Le taux de dépenses 1 n’aura pas de date de début et le dernier taux de dépenses n’aura pas de date de fin.</p><p>Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de dépenses 1 n’a pas de date de fin et que vous ajoutez le taux de dépenses 2 avec une date de début au 1er mai 2023, une date de fin au 30 avril 2023 est ajoutée au taux de dépenses 1 afin qu’il n’y ait aucune différence.</p></li>

   <li><b>Taux de facturation</b> : le montant de la facturation par heure pour l’utilisateur ou l’utilisatrice.
      <p>Pour connaître les taux de facturation effectifs par date, cliquez sur <strong>Ajouter un taux</strong>. Saisissez la valeur du taux de facturation pour la période et affectez une date de début et une date de fin, le cas échéant. Le taux de facturation 1 ne comporte pas de date de début de validité et le dernier taux de facturation n’a pas de date de fin de validité.</p> <p>Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de facturation 1 ne comporte pas de date de fin et que vous en ajoutez une seconde avec une date de début au 1er mai 2023, une date de fin au 30 avril 2023 est ajoutée au taux de facturation 1 afin qu’il n’y ait aucun trou.</p><p> <img alt="Coûts et taux de facturation des utilisateurs et utilisatrices" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulaires personnalisés</td> 
      <td><p>Associez un formulaire personnalisé existant à cet utilisateur ou cette utilisatrice. Vous devez créer un formulaire personnalisé avant de pouvoir l’associer à un utilisateur ou une utilisatrice. Seuls les formulaires personnalisés actifs sont affichés dans la liste. Les champs que vous ne pouvez pas modifier ne s’affichent pas dans un formulaire personnalisé individuel.</p> <p><strong>Remarque :</strong> Les fonctionnalités de formulaire personnalisées avancées telles que les champs de recherche externes et les champs natifs de Workfront ne sont disponibles que lorsque vous ouvrez l’enregistrement de l’utilisateur sur la page de détails, et non dans la boîte de dialogue Modifier l’utilisateur. (Dans la liste des personnes, cliquez sur un nom pour ouvrir les détails.)</p> <p>Pour plus d’informations sur la création de formulaires personnalisés, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref">Création d’un formulaire personnalisé</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Commentaire</td> 
      <td>Saisissez le commentaire à envoyer aux personnes et à la zone Mises à jour de leurs profils.</td> 
     </tr> 
    </tbody> 
   </table>
