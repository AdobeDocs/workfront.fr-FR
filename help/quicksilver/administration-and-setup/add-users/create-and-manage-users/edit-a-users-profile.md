---
title: Modifier le profil d’un utilisateur ou d’une utilisatrice
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer des utilisateurs et utilisatrices et gérer les profils existants.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '3298'
ht-degree: 99%

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

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer des utilisateurs et utilisatrices et gérer les profils existants. Pour plus d’informations sur la création d’utilisateurs et d’utilisatrices, voir [Ajouter des utilisateurs et utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

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
   <td> <p>Nouvelle : standard</p>
   Ou
   <p>Actuelle : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur ou administratrice système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à un utilisateur ou une utilisatrice</a>. </p> </li> 
     <li> <p>L’objet <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
     <ul><li> Administration des utilisateurs (tous les utilisateurs)</li>
     <li>Administration des utilisateurs (utilisateurs du groupe)</li></ul>
     <p>Si l’option <b>Administratrion des utilisateurs et utilisatrices (utilisateurs et utilisatrices du groupe)</b> est activée, vous devez être administrateur ou administratrice de groupes d’un groupe dont l’utilisateur ou l’utilisatrice est membre pour pouvoir modifier l’utilisateur ou l’utilisatrice.</p> 
     <p>Pour plus d’informations sur le paramètre <b>Utilisateurs et utilisatrices</b> dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Modifier le profil d’un utilisateur ou d’une utilisatrice

{{step-1-to-users}}

1. Sélectionnez un utilisateur ou une utilisatrice, puis cliquez sur l’icône **Modifier** ![](assets/edit-icon.png).

   La boîte de dialogue Modifier l’utilisateur ou l’utilisatrice s’affiche.

1. Dans la boîte de dialogue **Modifier l’utilisateur ou l’utilisatrice**, modifiez les informations suivantes, puis cliquez sur **Enregistrer les modifications** à tout moment :

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
        <li> <p><b>Adresse e-mail :</b> l’adresse e-mail d’un utilisateur ou d’une utilisatrice est également son nom d’utilisateur ou d’utilisatrice dans Workfront. Ce champ respecte la casse et doit être unique. Si un utilisateur ou une utilisatrice tente d’ajouter une adresse e-mail non unique trois fois en l’espace de 10 minutes, une réponse reCAPTCHA s’affiche.</p> <p> Sélectionnez le paramètre <b>Je ne suis pas un robot</b> avant de pouvoir continuer.</p><p>Si vous utilisez la liste autorisée d’adresses e-mail et que vous saisissez un domaine d’adresse e-mail qui ne figure pas dans la liste, l’utilisateur ou l’utilisatrice ne recevra pas de notifications par e-mail. Pour plus d’informations sur la liste autorisée, voir <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configurer votre liste autorisée d’adresses e-mail</a>.</p> </li> 
        <li> <p><b>Réinitialiser le mot de passe</b> : cliquez sur ce lien pour réinitialiser le mot de passe de l’utilisateur ou de l’utilisatrice. Vous devez saisir votre propre mot de passe avant de pouvoir réinitialiser le mot de passe d’autres utilisateurs ou utilisatrices.</p> <p>Pour réinitialiser le mot de passe d’autres utilisateurs ou utilisatrices, vous devez faire partie de l’équipe d’administration Workfront ou de groupes.</p> <p><b>NOTE</b> :  
          <ul> 
           <li> <p>Si vous faites partie de l’équipe d’administration de groupes, vous ne pouvez réinitialiser les mots de passe que pour les utilisateurs et utilisatrices des groupes pour lesquesl vous êtes administrateur ou administratrice. En outre, l’autorisation Administration des utilisateurs (utilisateurs du groupe) doit être activée dans votre niveau d’accès :</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Ce paramètre est désactivé par défaut. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </li> 
           <li> <p>Vous ne pouvez pas réinitialiser le mot de passe d’un administrateur ou d’une administratrice Workfront.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;Configuration SSO&gt; Nom d’utilisateur ou d’utilisatrice</b> : si votre administrateur ou administratrice Workfront a activé une intégration SSO avec Workfront, le nom d’utilisateur ou d’utilisatrice SSO s’affiche dans ce champ. Le type de configuration SSO activé pour votre instance Workfront est visible dans ce champ. </li> 
        <li> <p><b>OnlyAllow &lt;Configuration SSO&gt; Authentification</b> : si votre administrateur ou administratrice Workfront a activé une intégration SSO avec Workfront et mis à jour les utilisateurs et utilisatrices pour SSO, ce champ est sélectionné par défaut. Le type de configuration SSO activé pour votre instance Workfront est visible dans ce champ.</p> <p>Lorsque ce champ est sélectionné, l’utilisateur ou l’utilisatrice doit se connecter à Workfront avec ses informations d’identification SSO. Si vous la décochez, les utilisateurs et utilisatrices pourront se connecter à Workfront avec leurs informations d’identification Workfront.</p> <p>Pour plus d’informations sur la configuration de Workfront avec une solution d’authentification unique, voir <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Vue d’ensemble de l’authentification unique dans Adobe Workfront</a>.</p> <p>Pour plus d’informations sur la mise à jour des utilisateurs pour la SSO, voir <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Mettre à jour les utilisateurs et utilisatrices pour l’authentification unique</a>.</p> 
        <p><b>NOTE</b> :</p> 
        <p> Si vous êtes administrateur ou administratrice de groupe, vous pouvez modifier les champs &lt;SSO Configuration&gt; uniquement pour les personnes des groupes dans lesquels vous exercez ce rôle. En outre, votre niveau d’accès doit inclure l’autorisation d’administration des utilisateurs et utilisatrices (utilisateurs et utilisatrices du groupe).
        <p>Si vous êtes administrateur ou administratrice de groupe et que votre niveau d’accès inclut l’autorisation d’administration des utilisateurs et utilisatrices (L’ensemble des utilisateurs et utilisatrices), vous pouvez modifier les champs &lt;SSO Configuration&gt; pour l’ensemble des utilisateurs et utilisatrices.</p> </li> 
        <li><b>Infos sur le travail :</b> informations sur la tâche, comme son titre (dans le champ <b>Titre</b>) et le domaine d’expertise dont la domaine est responsable (dans le champ <b>Me parler de</b>).</li> 
        <li><p><b>Coordonnées</b> : numéro de téléphone de la personne (dans les champs <b>Numéro de téléphone, Ext.</b> et <b>Numéro portable</b>) et l’adresse (dans les champs <b>Adresse, Ville, État, Code postal et Pays</b>).</p>
        <p>Si la personne utilise Unified User Management (UUM) ou Adobe Identity Management System (IMS), le champ <b>Pays</b> de la section Coordonnées accepte uniquement les valeurs de code de pays (par exemple, US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Préférences </td> 
      <td> 
       <ul> 
      <li> <p><b>Fuseau horaire :</b> le fuseau horaire de la personne.</p> <p>Pour plus d’informations sur le travail en collaboration dans Workfront dans différents fuseaux horaires, voir <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Travailler sur plusieurs fuseaux horaires</a>.</p> </li> 
       <li><b>Paramètre local des e-mails</b> : la langue préférée de l’utilisateur ou de l’utilisatrice pour la messagerie. Cela a une incidence sur le format des nombres et des dates dans les e-mails provenant de Workfront à cette personne.</li>

   <li><b>Recevoir des e-mails à partir de cet environnement de test</b> : cochez cette option si vous souhaitez recevoir des notifications par e-mail de l’environnement dans lequel vous êtes actuellement connecté.
      <p><b>NOTE</b></p>
      <p>Cette option n’est disponible que dans les environnements de prévisualisation et de sandbox. Par défaut, les notifications par e-mail sont activées dans l’environnement de production. </p>
      </li>

   </li> 
       <li><b>Envoyer le travail que je me suis affecté dans mon onglet Travailler sur</b>: cochez cette option si vous souhaitez que tout le travail que la personne s’est affecté apparaisse directement dans la liste Travaille sur de la zone Accueil. La valeur par défaut est de répertorier tous les éléments affectés à une personne dans ses listes Prêt à démarrer ou Pas prêt dans la zone Accueil.</li> 
       <li><b>Générer automatiquement des épreuves lors du chargement de documents</b> : cochez cette option si vous souhaitez que les documents que la personne charge génèrent immédiatement une épreuve. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td> <p>Sélectionnez les notifications par e-mail qui doivent être activées pour le nouvel utilisateur ou la nouvelle utilisatrice.</p> <p>Vous pouvez sélectionner des notifications instantanées ou une synthèse des notifications quotidienne.</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurer les notifications d’événement pour tous les utilisateurs et les utilisatrices du système</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accès</td> 
      <td> 
       <ul> 
      <li><b>Est actif :</b> cochez cette case pour indiquer que la personne est active. Les utilisateurs et utilisatrices actifs utilisent une licence Workfront. L’effacement de la case désactive la personne et l’empêche de se connecter à Workfront.</li> 
       <li> <p><b>Niveau d’accès :</b> sélectionnez le niveau d’accès à attribuer à cette personne.</p> 
       <p>Lors de l’attribution d’un niveau d’accès à une personne, vous pouvez attribuer un niveau égal ou inférieur à votre propre niveau d’accès.</p>
       <p>Par exemple, si votre niveau d’accès est Plan, vous ne pouvez pas lui attribuer le niveau d’accès Administration. Cependant, vous ne pouvez pas attribuer un niveau d’accès inférieur par défaut à votre propre niveau d’accès si l’administration de Workfront a activé des autorisations autres que les autorisations par défaut au niveau d’accès qui ne sont pas également activées dans votre propre niveau d’accès. </p>
       <p>Par exemple, si vous disposez d’une licence de plan sans accès à la suppression de tâches, vous ne pouvez pas attribuer à une personne une licence de travail ayant accès à la suppression de tâches, bien que la licence de travail soit inférieure à la licence de plan. Pour plus d’informations, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>. </p> 
       <p>Pour plus d’informations sur les niveaux d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurer l’accès à Adobe Workfront</a>.</p>
       <p> <b>NOTE :</b></p> 
       <p> Si votre entreprise utilise le nouveau modèle d’accès (Standard/Léger/Contribution), vous ne pouvez pas réaffecter un utilisateur ou une utilisatrice ayant une licence standard ou léger à un niveau d’accès de contribution si cette personne a déjà atteint sa limite de décision pour le mois. </p><p>Pour plus d’informations sur le nouveau modèle d’accès, voir <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">Vue d’ensemble des nouveaux niveaux d’accès</a>. </p><p>Pour plus d’informations sur les limites de décision, voir <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Vue d’ensemble du statut de décision limitée des documents et de l’épreuve pour les utilisateurs et utilisatrices non payants</a>.</p></li> 
       <li> <p><b>Modèle de mise en page</b> : choisissez un modèle de mise en page pour les utilisateurs et les utilisatrices. Le modèle de mise en page attribué aux utilisateurs et aux utilisatrices est prioritaire sur tout modèle de mise en page affecté à leur groupe principal, à leur équipe principale ou à leur rôle principal. Pour plus d’informations sur la priorité d’affectation des modèles de mise en page, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Créer et gérer des modèles de mise en page</a>.</p> <p><b>NOTE</b> :  <p>La liste suivante présente les modèles disponibles dans ce champ en fonction de votre accès :</p> 
       <ul> 
       <li>En tant qu’administrateur ou administratrice de Workfront, vous pouvez consulter tous les modèles de mise en page au niveau du système et du groupe.</li> 
       <li>En tant qu’administrateur ou administratrice de groupe, vous pouvez voir un modèle de mise en page au niveau du système, ainsi que les modèles associés aux groupes que vous gérez.</li> 
       <li>En tant que personne disposant d’une licence de plan et d’un accès en modification pour les utilisateurs et utilisatrices, vous ne pouvez afficher que les modèles de mise en page au niveau du système.</li> 
       </ul> <p>Pour plus d’informations sur les modèles de disposition au niveau du groupe, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Créer et gérer des modèles de disposition</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisation </td> 
      <td> 
       <ul> 
      <li><b>Entreprise</b> : entreprise de l’utilisateur ou de l’utilisatrice. Les personnes ne peuvent être associées qu’à une seule entreprise. Vous devez créer une entreprise avant de pouvoir l’associer à une personne. Seules les entreprises actives sont affichées dans la liste. Pour plus d’informations sur la création d’entreprises, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Créer et modifier des entreprises</a>.</li> 
      <li><b>Rend compte à :</b> si vous avez spécifié une entreprise pour l’utilisateur ou l’utilisatrice, vous pouvez également indiquer la personne responsable direct de l’utilisateur ou de l’utilisatrice dans ce champ. Un utilisateur ou une utilisatrice ne peut avoir qu’une seule personne responsable. Ce champ ne s’affiche pas si l’utilisateur ou l’utilisatrice n’est pas d’abord associé à une entreprise. </li> 
      <li><b>Personnes subordonnées :</b> si vous avez spécifié une entreprise pour l’utilisateur ou l’utilisatrice, vous pouvez également indiquer les personnes subordonnées de l’utilisateur ou de l’utilisatrice. Un utilisateur ou une utilisatrice peut avoir plusieurs personnes subordonnées. Ce champ ne s’affiche pas si l’utilisateur ou l’utilisatrice n’est pas d’abord associé à une entreprise.</li> 
      <li><b>Équipe principale</b> : spécifiez l’équipe principale de l’utilisateur ou de l’utilisatrice. Les personnes ne peuvent avoir qu’une seule équipe principale.
L’équipe principale est importante lors de l’attribution d’un modèle de disposition ou de la définition du bouton Travailler sur ce projet pour les tâches et les problèmes affectés à l’utilisateur ou à l’utilisatrice. </li> 
      <li><b>Autres équipes</b> : les utilisateurs et utilisatrices peuvent appartenir à plusieurs équipes. Un utilisateur ou une utilisatrice peut afficher les tâches affectées à l’une de ses équipes dans sa zone d’accueil. </li> 
      <li> <p><b>Groupe principal :</b> sélectionnez un groupe approprié pour affecter l’utilisateur ou l’utilisatrice. La personne peut ainsi accéder aux objets partagés avec le groupe. Vous pouvez également partager des modèles de disposition avec le groupe principal de l’utilisateur ou de l’utilisatrice.</p> <p>Il s’agit d’un champ obligatoire. Chaque personne doit être associée à un groupe principal. Si vous n’en sélectionnez pas un, votre groupe est désigné comme groupe principal de la nouvelle personne.</p> <p><b>NOTE</b> :</p> 
      <p> Vous ne pouvez affecter un groupe à une personne que si l’une des conditions suivantes est remplie :</p>
      <ul><li>Vous êtes un administrateur ou une administratrice Workfront.</li>
      <li>Vous êtes l’administrateur ou l’administratrice de ce groupe.</li>
      <li>Ce groupe est public.</li></ul> 
      <li> <p><b>Autres groupes</b> : les personnes peuvent appartenir à plusieurs groupes. Vous ne pouvez affecter un groupe à une personne que si vous êtes administrateur ou administratice Workfront, administrateur ou administratrice du groupe, ou que le groupe est public.</p> <p><b>IMPORTANT</b> :</p> 
      <p>L’ajout d’une personne à plus de 100 groupes peut entraîner des problèmes de performances dans n’importe quelle zone de Workfront qui charge la liste des groupes.</p> <p>Pour plus d’informations sur les groupes publics, voir <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Créer un groupe</a>.</p> <p>Pour plus d’informations sur les groupes, voir <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Vue d’ensemble des groupes</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planification des ressources </td> 
      <td> 
       <ul>
       <li>
       <b>Temps de travail</b> : représente le pourcentage du temps équivalent temps plein (FTE) que la personne peut consacrer au travail effectif, hors durée supplémentaire. Le temps de travail doit être un nombre décimal inférieur ou égal à 1 et ne peut pas être égal à 0. Par exemple, une disponibilité de 20 % pour le travail effectif serait de 0,2.

   La valeur par défaut de ce champ est 1, ce qui indique que la personne consacre la totalité de son FTE au travail réel lié au projet.

   Le système utilise ce nombre pour calculer la disponibilité de la personne quant au travail réel lié au projet.

   Pour plus d’informations sur la création de plannings dans Workfront, voir <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Créer un planning</a>.

   Les exceptions au planning et les congés peuvent également affecter la capacité de la personne.

   Workfront calcule la disponibilité d’une personne en fonction des préférences de gestion des ressources dans votre zone de configuration. Pour plus d’informations, voir <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurer les préférences de gestion des ressources</a>.

   <b>CONSEIL</b>

   Définissez la valeur Temps de travail sur 1 pour indiquer que la personne est disponible pour effectuer le travail lié au projet pendant la totalité de son équivalent temps plein.
   </li> 
      <li> <b>Planifier la désactivation</b> : cochez cette case si vous souhaitez planifier la désactivation de cette personne à une certaine date et à une certaine heure. </li> 
       <li><b>Date de désactivation planifiée</b> : date et heure après lesquelles la personne est désactivée. Pour plus d’informations sur la planification de la désactivation des personnes, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Planifier la désactivation des utilisateurs et utilisatrices</a> dans <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactiver ou réactiver un utilisateur ou une utilisatrice</a>.</li> 
       <li> <p><b>Rôle principal</b> : fonction principale que la personne peut remplir dans Workfront. Chaque tâche et problème auquel la personne est affectée est également affectée à cette fonction. Les fonctions sont essentielles à la gestion des ressources. Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Plan avec un accès utilisateur administratif, ou si vous êtes un administrateur ou une administratrice Workfront. Pour plus d’informations sur la configuration des utilisateurs et utilisatrices disposant d’un accès administratif, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> <p>Seules les fonctions actives s’affichent dans la liste. </p> </li> 
       <li>Si vous avez sélectionné un <b>rôle principal</b>, le champ <b>Pourcentage de disponibilité FTE</b> s’affiche. Indiquez le pourcentage de temps du planning de la personne affectée à cette fonction. La valeur par défaut du pourcentage de disponibilité FTE pour le rôle principal est de 100 %. </li> 
       <li> <p><b>Autres rôles</b> : une personne peut avoir plusieurs fonctions dans Workfront. Les fonctions sont essentielles à la gestion des ressources. Une personne peut remplir un nombre illimité de fonctions. Toutefois, nous recommandons de ne pas affecter un nombre excessivement élevé de fonctions à une personne, car la gestion des ressources pourrait devenir trop complexe pour ces personnes.<p>Seules les fonctions actives s’affichent dans la liste. Pour plus d’informations sur les fonctions, consultez la section <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Créer et gérer des fonctions</a>.</p> <p>Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Plan avec un accès utilisateur administratif, ou si vous êtes un administrateur ou une administratrice Workfront. <br>Pour plus d’informations sur la configuration des personnes disposant d’un accès administratif, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> </li> 
       <li> <p>(Le cas échéant) Si vous avez sélectionné un ou plusieurs <b>Autres rôles</b>, le champ <b>Pourcentage de disponibilité FTE</b> s’affiche pour chaque rôle. Indiquez le pourcentage de temps du planning de la personne attribué à chaque fonction. La valeur par défaut du pourcentage de disponibilité FTE pour les autres rôles est de 0 %.</p> <p><b>NOTE</b> : si d’autres rôles ont une disponibilité FTE de 0 %, ils ne s’affichent pas dans le planificateur de ressources, sauf si ces rôles comprennent des tâches affectées à la personne.</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTE</b> : <p>La somme de tous les <b>pourcentages de disponibilité FTE</b> pour tous les rôles, doit être égale à 100 %. Chaque pourcentage de disponibilité FTE calcule les heures disponibles pour chaque rôle par personne dans le planificateur de ressources. Les heures disponibles pour chaque rôle par personne dépendent du temps disponible pour la personne.</p> <p>Le temps disponible pour la personne est calculé par Workfront en fonction de la méthode sélectionnée par l’administration Workfront pour calculer le FTE dans les préférences de gestion des ressources.</p> <p>Pour plus d’informations sur le calcul de la disponibilité de la personne, voir <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Vue d’ensemble du calcul des heures et du FTE pour les personnes et les rôles dans le planificateur de ressources</a>.</p> <p>Pour plus d’informations sur la configuration des préférences de gestion des ressources, consultez la section <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurer les préférences de gestion des ressources</a>.</p> </p>
       <span class="preview"><p>(Facultatif) Les dates d’entrée en vigueur des affectations de fonctions sont utilisées dans les calculs financiers si la fonction de la personne change au cours d’un projet.</p><p>Cliquez sur <b>Définir des rôles par date</b>, sélectionnez <b>Rôle principal</b> et <b>Autres rôles</b>, puis saisissez le pourcentage d’affectation de chaque rôle. Les rôles peuvent être identiques aux rôles existants (en utilisant différents pourcentages) ou de nouveaux rôles. Sélectionnez <b>Date de début</b> lorsque ces rôles deviennent actifs. Il peut s’agir d’une date ultérieure. Lorsque les rôles les plus récents deviennent actifs, vous pouvez cliquer sur <b>Afficher les rôles précédents</b> pour afficher les rôles précédents inactifs.</p> </li></span>
       <li> <p><b>Planning</b> : associez un planning à une personne. Le planning de la personne calcule la chronologie des tâches auxquelles la personne est affectée.</p> <p>Vous devez créer un planning avant de pouvoir l’associer à une personne. Pour plus d’informations sur la création de plannings, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Créer un planning</a>.</p> <p><b>NOTE</b> : il est recommandé que le planning que vous associez à la personne corresponde à son fuseau horaire.</p> </li> 
       <li> <p><b>Profil de feuille de temps</b> : associez un profil de feuille de temps à la personne pour vous assurer que les feuilles de temps sont générées automatiquement pour la personne</p> <p><b>NOTE</b> : la liste des profils disponibles dans ce champ dépend de votre accès :
       <ul>
       <li>En tant qu’administrateur ou administratrice Workfront, vous pouvez voir tous les profils de feuilles de temps au niveau du système et du groupe.</li>
       <li>En tant qu’administrateur ou administratrice de groupes, vous pouvez voir les profils de feuille de temps au niveau du système, ainsi que ceux associés aux groupes que vous gérez.</li>
       <li>En tant qu’utilisateur ou utilisatrice disposant d’une licence Plan et d’un accès à la modification des utilisateurs et des utilisatrices, vous ne pouvez voir que les profils de feuille de temps au niveau du système. Pour plus d’informations sur les profils de feuille de calcul au niveau du groupe, voir <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Création, modification et affectation de profils de feuille de temps</a>.</li>
      </ul></p> </li> 
       <li><b>Type d’heure par défaut</b> : sélectionnez le type d’heure par défaut pour la personne. Il s’agit du type d’heure utilisé par défaut lorsque la personne consigne des heures.</li> 
       <li><b>Types d’heure disponibles</b> : sélectionnez les types d’heures qui doivent être disponibles pour la personne. Ces types d’heure sont visibles partout dans Workfront, où la personne peut consigner l’heure. Une personne ne peut voir que les types d’heures qui sont activés au niveau du projet et au niveau de la personne. Pour plus d’informations sur les types d’heure disponibles pour les personnes, consultez la section <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Définir les types d’heure et la disponibilité des feuilles de temps</a>.</li> 
       <li><b>Temps de connexion :</b> indiquez si la personne doit se consigner les tâches en heures ou en jours. Pour plus d’informations, voir <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configurer si la durée est consignée en heures ou en jours</a>.</li>

   <li> <b>FTE</b> : il s’agit de l’équivalent temps plein de la personne. Workfront utilise ce nombre pour calculer la disponibilité de la personne en fonction du planning par défaut uniquement lorsque les préférences de gestion des ressources au niveau du système sont définies sur « Le planning par défaut ».

   <p>Le FTE indique le temps que la personne peut consacrer au travail. Cela comprend les durées supplémentaires, ainsi que le temps consacré au travail sur les projets. Par exemple, le temps passé en réunion ou en formation est également inclus dans le FTE.</p>

   Le FTE doit être un nombre décimal inférieur ou égal à 1 et ne peut pas être égal à 0. Par exemple, si la valeur du FTE est de 0,5 et que l’horaire par défaut dans Workfront est de 40 heures, la personne est disponible 20 heures par semaine.

   La valeur par défaut de ce champ est 1.

   Les exceptions de planning, les congés éventuels et la valeur du temps de travail peuvent affecter la disponibilité de la personne.

   Workfront calcule la disponibilité d’une personne en fonction des préférences de gestion des ressources dans votre zone de configuration.


   Si les préférences de gestion des ressources au niveau du système sont définies sur le planning de la personne, la valeur que vous spécifiez ici est ignorée et la personne est considérée comme étant disponible selon ce qui est spécifié dans son planning.

   Pour plus d’informations, voir <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurer les préférences de gestion des ressources</a>.

   Pour plus d’informations sur la création de plannings dans Workfront, voir <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Créer un planning</a>.
   </li>

   <li><b>Groupes de ressources</b> : associez les personnes aux groupes de ressources. Pour plus d’informations, voir <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associer des groupes de ressources aux personnes </a>.</li>

   <li><b>Taux de dépenses</b> : montant du coût par heure pour la personne.
      <p>Pou les dates d’entrée en vigueur des taux de dépenses, cliquez sur <strong>Ajouter un taux</strong>. Saisissez la valeur du taux de dépenses pour la période et attribuez une Date de début et une Date de fin, le cas échéant. Le taux de dépenses 1 n’aura pas de date de début et le dernier taux de dépenses n’aura pas de date de fin.</p><p>Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de dépenses 1 n’a pas de date de fin et que vous ajoutez le taux de dépenses 2 avec une date de début du 1er mai 2023, une date de fin du 30 avril 2023 est ajoutée au taux de dépenses 1 afin qu’il n’y ait aucune différence.</p></li>

   <li><b>Taux de facturation</b> : montant de la facturation par heure pour la personne.
      <p>Pour les dates d’entrée en vigueur du taux de facturation, cliquez sur <strong>Ajouter un taux</strong>. Saisissez la valeur du taux de facturation pour la période et attribuez une date de début et une date de fin selon vos besoins. Le taux de facturation 1 ne comporte pas de date de début et le dernier taux de facturation n’a pas de date de fin.</p> <p>Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de facturation 1 ne comporte pas de date de fin et que vous en ajoutez un second avec une date de début du 1er mai 2023, une date de fin du 30 avril 2023 est ajoutée au taux de facturation 1 afin qu’il n’y ait aucune différence.</p><p> <img alt="Taux de facturation et de dépenses des personnes" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulaires personnalisés</td> 
      <td><p>Associez un formulaire personnalisé existant à cette personne. Vous devez créer un formulaire personnalisé avant de pouvoir l’associer à un utilisateur ou une utilisatrice. Seuls les formulaires personnalisés actifs sont affichés dans la liste. Les champs que vous n’avez pas le droit de modifier ne s’affichent pas dans un formulaire personnalisé individuel.</p> <p><strong>Note :</strong> les fonctionnalités avancées de formulaire personnalisé telles que les champs de recherche externe et les champs natifs de Workfront ne sont disponibles que lorsque vous ouvrez l’enregistrement de la personne sur la page de détails, et non dans la boîte de dialogue Modifier la personne. (Dans la liste des personnes, cliquez sur un nom pour ouvrir les détails.)</p> <p>Pour plus d’informations sur la création de formulaires personnalisés, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Créer ou modifier un formulaire personnalisé</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Commentaire</td> 
      <td>Saisissez le commentaire à envoyer aux personnes et à la zone Mises à jours de leurs profils.</td> 
     </tr> 
    </tbody> 
   </table>
