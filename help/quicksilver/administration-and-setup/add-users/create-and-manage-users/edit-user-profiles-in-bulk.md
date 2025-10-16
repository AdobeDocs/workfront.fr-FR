---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Modifier les profils utilisateur en bloc
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez modifier les comptes des utilisateurs et des utilisatrices en masse.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: 72d0b8e0e190f774c7e3f14a78904fb1dd3f2b14
workflow-type: tm+mt
source-wordcount: '2587'
ht-degree: 64%

---

# Modifier en masse des profils d’utilisateurs et d’utilisatrices

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Vous pouvez modifier les comptes des utilisateurs et utilisatrices en masse. Lors de la modification en masse d’utilisateurs et d’utilisatrices, seuls les champs que vous sélectionnez spécifiquement sont mis à jour avec les mêmes informations pour tous les utilisateurs et utilisatrices sélectionnés. Tous les autres champs non sélectionnés restent identiques pour chaque utilisateur ou utilisatrice, même s’ils sont différents pour chaque utilisateur ou utilisatrice.

>[!NOTE]
>
>* Vous ne pouvez pas modifier en masse la section Informations personnelles des profils des utilisateurs et des utilisatrices, car ces informations doivent être uniques pour chaque personne.
>* Pour garantir la précision des données et des performances optimales, nous vous recommandons de ne pas sélectionner plus de 2 000 utilisateurs et utilisatrices à la fois lors d’une modification en masse.
>

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès de l’administrateur système. </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier des comptes d’utilisateurs et d’utilisatrices en masse

{{step-1-to-users}}

1. Sélectionnez plusieurs utilisateurs, puis cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png).

1. Dans la zone **Modifier l’utilisateur**, modifiez les informations de l’une des sections, puis cliquez sur **Enregistrer** à tout moment.

### Préférences

* **Fuseau horaire** : fuseau horaire de l’utilisateur.

  Pour plus d’informations sur l’aide apportée aux utilisateurs et utilisatrices par le biais de Workfront dans les différents fuseaux horaires, voir [Utilisation des fuseaux horaires](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

* **Locale d’e-mail** : paramètres régionaux d’e-mails préférés des utilisateurs et utilisatrices. Cela affecte le format des nombres et des dates dans les e-mails envoyés par Workfront à cet utilisateur ou cette utilisatrice.

  >[!NOTE]
  >
  >Lorsque votre organisation utilise l’expérience unifiée Adobe, les préférences linguistiques de l’utilisateur sont stockées dans son profil Adobe et les paramètres régionaux des e-mails ne sont pas utilisés. Pour plus d’informations sur l’accès à ces préférences, voir [Expérience unifiée Adobe pour Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

### Notifications

Sélectionnez les notifications par e-mail qui doivent être activées pour les utilisateurs.

Vous pouvez sélectionner des notifications instantanées ou une synthèse des notifications quotidienne. Toutes les notifications de résumés quotidiens sont diffusées après la même heure pour tous les utilisateurs que vous avez sélectionnés.

Pour plus d’informations, voir [Configurer les notifications d’événements pour tous les utilisateurs et utilisatrices du système](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

### Accès

* **L’utilisateur est actif** : activez cette option pour indiquer que les utilisateurs sont actifs. Les utilisateurs et utilisatrices actifs utilisent une licence Workfront. La désactivation du champ désactive les utilisateurs et les empêche de se connecter à Workfront.

* **Niveau d’accès** : sélectionnez le niveau d’accès à affecter à ces utilisateurs. Tous les utilisateurs sélectionnés auront le même niveau d&#39;accès.

  Lorsque vous attribuez un niveau d’accès aux utilisateurs et utilisatrices, vous pouvez attribuer un niveau égal ou inférieur à votre propre niveau d’accès. (Par exemple, si votre niveau d&#39;accès est Standard, vous ne pouvez pas attribuer le niveau d&#39;accès Administrateur.)

  Cependant, vous ne pouvez pas attribuer un niveau d’accès inférieur par défaut à votre propre niveau d’accès si l’administrateur ou l’administratrice Workfront a activé des autorisations autres que les autorisations par défaut au niveau d’accès qui ne sont pas également activées dans votre propre niveau d’accès.

  Par exemple, si vous possédez une licence Standard sans accès pour supprimer des tâches, vous ne pouvez pas attribuer à quelqu&#39;un une licence light avec accès pour supprimer des tâches, bien que la licence light soit inférieure à la licence standard. Pour plus d’informations, voir la section [Créer ou modifier des niveaux d’accès personnalisés](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Pour plus d’informations sur les niveaux d’accès, voir [Configurer l’accès à Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  >[!NOTE]
  >
  >Si votre entreprise utilise le nouveau modèle d’accès (Standard/Light/Contributeur ou Contributrice), vous ne pouvez pas réaffecter un utilisateur Standard ou Light à un niveau d’accès Contributeur ou Contributrice si cet utilisateur ou cette utilisatrice a déjà atteint sa limite de décision pour le mois.
  >
  >Pour plus d’informations sur le nouveau modèle d’accès, voir [Vue d’ensemble des nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).
  >
  >Pour plus d’informations sur les limites de décision, voir [Vue d’ensemble du statut de décision limitée des documents et de l’épreuve pour les utilisateurs et utilisatrices non payants](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

* **Modèle de mise en page** : choisissez un modèle de mise en page pour les utilisateurs et les utilisatrices. ce modèle de mise en page est prioritaire sur tout modèle de mise en page affecté à son groupe principal, à son équipe interne ou à son rôle de Principal. Pour plus d’informations sur la priorité d’affectation des modèles de mise en page, voir [Création et gestion des modèles de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

  La liste suivante décrit la manière dont la liste des modèles disponibles dans ce champ dépend de votre accès :

   * En tant qu’administrateur ou administratrice Workfront, vous pouvez consulter tous les modèles de mise en page au niveau du système et du groupe.
   * En tant qu’administrateur ou administratrice de groupes, vous pouvez voir le modèle de mise en page au niveau du système, ainsi que ceux associés aux groupes que vous gérez.
   * Les utilisateurs disposant d’une licence Standard ou Plan et ayant accès à la modification d’utilisateurs ne peuvent afficher que des modèles de mise en page au niveau du système.

     Pour plus d’informations sur les modèles de mise en page au niveau du groupe, voir [Création et modification de modèles de mise en page d’un groupe](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

### Organisation

* **Entreprise** : entreprise des utilisateurs et utilisatrices. Les personnes ne peuvent être associées qu’à une seule entreprise. Vous devez créer une entreprise avant de pouvoir l’associer à une personne. Seules les entreprises actives sont affichées dans la liste. Pour plus d’informations sur la création d’entreprises, voir [Créer et modifier des entreprises](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* **Équipe principale** : indiquez l’équipe principale des utilisateurs et utilisatrices. Les personnes ne peuvent avoir qu’une seule équipe principale.
* **Autres équipes** : les personnes peuvent appartenir à plusieurs équipes.
* **Groupe principal actuel** : sélectionnez un groupe approprié pour affecter les utilisateurs. Cela permet aux utilisateurs d’accéder aux objets partagés avec le groupe. Vous pouvez également partager des modèles de mise en page avec un groupe principal.

  Champ obligatoire. Chaque utilisateur et utilisatrice doit être associé à un groupe principal. Si vous ne sélectionnez pas de groupe principal, celui-ci est affecté comme groupe principal.

  Vous ne pouvez affecter un groupe à une personne que si l’une des conditions suivantes est vraie :

   * Vous êtes un administrateur ou une administratrice Workfront.
   * Vous êtes l’administrateur ou l’administratrice du groupe.
   * le groupe est public

* **Autres groupes** : les personnes peuvent appartenir à plusieurs groupes. Vous ne pouvez affecter un groupe à un utilisateur ou une utilisatrice que si vous êtes un administrateur ou une administratrice Workfront, que si vous êtes administrateur ou administratrice du groupe ou que si le groupe est public.

  >[!IMPORTANT]
  >
  >L’ajout d’une personne à plus de 100 groupes peut entraîner des problèmes de performances dans n’importe quelle zone de Workfront qui charge la liste des groupes.

  Pour plus d’informations sur les groupes publics, voir [Créer un groupe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

  Pour plus d’informations sur les groupes, voir [Vue d’ensemble des groupes](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md).

### Planification des ressources

* **Temps de travail** : représente le pourcentage du temps équivalent temps plein (ETP) que les utilisateurs sont disponibles pour le travail réel, sans compter les frais généraux. Le temps de travail doit être un nombre décimal inférieur ou égal à 1 et ne peut pas être égal à 0. Par exemple, une disponibilité de 20 % pour le travail effectif serait de 0,2.

  La valeur par défaut de ce champ est 1, ce qui indique que la personne consacre la totalité de son équivalent temps complet au travail réel lié au projet.

  Le système utilise ce nombre pour calculer la disponibilité de la personne quant au travail réel lié au projet.

  Pour plus d’informations sur la création de plannings dans Workfront, voir [Créer un planning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  Les exceptions au planning et les congés peuvent également affecter la capacité de la personne.

  Workfront calcule la disponibilité d’une personne en fonction des préférences de gestion des ressources dans votre zone de configuration. Pour plus d’informations, voir [Configurer les préférences de gestion des ressources](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  >[!TIP]
  >
  >Définissez la valeur Temps de travail sur 1 pour indiquer que la personne est disponible pour effectuer le travail lié au projet pendant la totalité de son équivalent temps plein.

* **Définir la date de désactivation** : cliquez sur ce bouton si vous souhaitez planifier la désactivation de ces utilisateurs à une certaine date et à une certaine heure.
* **Date de désactivation** : date et heure de désactivation des utilisateurs. Pour plus d’informations sur la planification de la désactivation d’utilisateurs, voir [&#x200B; Planification de la désactivation d’utilisateurs &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation) dans [&#x200B; Désactiver ou réactiver un utilisateur &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
* **Rôle de Principal** : il s’agit de la fonction principale que les utilisateurs peuvent remplir dans Workfront. Chaque tâche et événement affecté aux utilisateurs est également affecté à cette fonction. Les fonctions sont essentielles à la gestion des ressources. Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Standard ou Plan avec un accès utilisateur administratif ou si vous êtes un administrateur Workfront. Pour plus d’informations sur la configuration des utilisateurs et des utilisatrices disposant d’un accès d’administration, consultez la section [Accorder un accès aux utilisateurs et aux utilisatrices](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

  Seules les fonctions actives s’affichent dans la liste.

* (Facultatif) Si vous avez sélectionné un **Rôle principal**, le champ **Pourcentage de disponibilité équivalent temps complet** s’affiche. Spécifiez le pourcentage de temps affecté à cette fonction dans le planning des utilisateurs et utilisatrices. La valeur par défaut du pourcentage de disponibilité équivalent temps complet pour le rôle principal est de 100 %.
* **Autres rôles** : les utilisateurs et les utilisatrices peuvent exercer plusieurs fonctions dans Workfront. Les fonctions sont essentielles à la gestion des ressources. Une personne peut remplir un nombre illimité de fonctions. Toutefois, nous recommandons de ne pas affecter un nombre excessivement élevé de fonctions à une personne, car la gestion des ressources pourrait devenir trop complexe pour ces personnes.

  Seules les fonctions actives s’affichent dans la liste. Pour plus d’informations sur les fonctions, consultez la section [Créer et gérer des fonctions](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

  Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Standard ou Plan avec un accès utilisateur administratif ou si vous êtes un administrateur Workfront.

  Pour plus d’informations sur la configuration des utilisateurs et utilisatrices disposant d’un accès administratif, consultez la section [Accorder l’accès aux utilisateurs et utilisatrices](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

* (Facultatif) Si vous avez sélectionné un ou plusieurs **Autres rôles**, le champ **Pourcentage de disponibilité équivalent temps complet** s’affiche pour chaque rôle. Spécifiez le pourcentage de temps affecté à chaque fonction dans le planning des personnes. La valeur par défaut du pourcentage de disponibilité équivalent temps complet pour les autres rôles est de 0 %.

  si d’autres rôles ont une disponibilité équivalent temps complet de 0 %, ils ne s’affichent pas dans le planificateur de ressources, sauf si ces rôles comprennent des tâches affectées à la personne.

  La somme de tous les **pourcentages de disponibilité de l’équivalent temps complet** pour toutes les fonctions, doit être égale à 100 %. Chaque pourcentage de disponibilité équivalent temps complet calcule les heures disponibles pour chaque rôle par personne dans le planificateur de ressources. Les heures disponibles pour chaque rôle par personne dépendent du temps disponible pour la personne.

  Le temps disponible pour la personne est calculé par Workfront en fonction de la méthode sélectionnée par l’administration Workfront pour calculer l’équivalent temps complet dans les préférences de gestion des ressources.

  Pour plus d’informations sur le calcul de la disponibilité de l’utilisateur ou de l’utilisatrice, consultez la section [Vue d’ensemble du calcul des heures et de l’équivalent temps complet pour les utilisateurs et les utilisatrices et les fonctions dans le planificateur de ressources](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

  Pour plus d’informations sur la configuration des préférences de gestion des ressources, consultez la section [Configurer les préférences de gestion des ressources](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Planning** : associez un planning pour les utilisateurs et utilisatrices. Le planning des utilisateurs et des utilisatrices calcule la chronologie des tâches auxquelles ces personnes sont affectées.

  Vous devez créer un planning avant de pouvoir l’associer aux utilisateurs. Pour plus d’informations sur la création de plannings, voir [Créer un planning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  >[!IMPORTANT]
  >
  >Workfront utilise la planification d’un utilisateur uniquement lorsque le paramètre **Calculer la disponibilité des ressources à l’aide de** est défini sur **Planification de l’utilisateur**. Pour plus d&#39;informations sur l&#39;impact de ce paramètre sur la planification utilisée pour la gestion des ressources, voir [Configurer les préférences de gestion des ressources](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Profil de feuille de temps** : associez un profil de feuille de temps aux utilisateurs pour vous assurer que les feuilles de temps sont générées automatiquement.

  La liste des profils disponibles dans ce champ dépend de votre accès :

   * En tant que membre de l’équipe d’administration de Workfront, vous pouvez consulter tous les profils de feuille de temps au niveau du système et de tous les groupes.
   * En tant qu’administrateur ou administratrice de groupes, vous pouvez voir les profils de feuille de temps au niveau du système, ainsi que ceux associés aux groupes que vous gérez.
   * Les utilisateurs disposant d&#39;une licence Standard ou Plan et ayant accès à la modification d&#39;utilisateurs ne peuvent afficher que les profils de feuilles de temps au niveau du système. Pour plus d’informations sur les profils de feuille de temps au niveau du groupe, consultez la section [Créer, modifier et affecter des profils de feuille de temps](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Type d’heure par défaut** : sélectionnez le type d’heure par défaut pour les utilisateurs et les utilisatrices. Il s’agit du type d’heure utilisé par défaut lorsque les utilisateurs et les utilisatrices consignent des heures.
* **Types d’heures disponibles** : sélectionnez les types d’heures qui doivent être disponibles pour les utilisateurs. Ces types d’heures sont visibles partout dans Workfront où les personnes peuvent consigner des heures. Les utilisateurs peuvent uniquement voir les types d’heures activés au niveau du projet ainsi qu’au niveau de l’utilisateur. Pour plus d’informations sur les types d’heures disponibles pour les utilisateurs, voir [&#x200B; Définir les types d’heures et la disponibilité &#x200B;](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
* **ETP** : il s’agit de l’équivalent temps plein des utilisateurs. Workfront utilise ce nombre pour calculer la disponibilité des utilisateurs en fonction de la planification par défaut uniquement lorsque les préférences de gestion des ressources au niveau du système sont définies sur la planification par défaut.

  L’équivalent temps complet indique le temps que les utilisateurs peuvent passer au travail. Cela comprend les durées supplémentaires, ainsi que le temps consacré au travail sur les projets. Par exemple, le temps passé en réunion ou en formation est également inclus dans l’équivalent temps complet.

  L’équivalent temps complet doit être un nombre décimal inférieur ou égal à 1 et ne peut pas être égal à 0. Par exemple, si la valeur d’équivalent temps complet est 0,5 et que la planification par défaut dans Workfront est de 40 heures, les utilisateurs sont disponibles 20 heures par semaine.

  La valeur par défaut de ce champ est 1.

  Les exceptions d&#39;horaire, les congés et la valeur du temps de travail peuvent affecter la disponibilité des utilisateurs.

  Workfront calcule la disponibilité d’une personne en fonction des préférences de gestion des ressources dans votre zone de configuration.

  Si les préférences de gestion des ressources au niveau du système sont définies sur le planning de la personne, la valeur que vous spécifiez ici est ignorée et la personne est considérée comme étant disponible selon ce qui est spécifié dans son planning.

  Pour plus d’informations, consultez la section [Configurer les préférences de gestion des ressources](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  Pour plus d’informations sur la création de plannings dans Workfront, consultez la section [Créer un planning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Pools de ressources** : associez les utilisateurs aux pools de ressources.

  >[!NOTE]
  >
  >Seuls les groupes de ressources communs à tous les utilisateurs et utilisatrices sélectionnés apparaissent dans ce champ. Si les utilisateurs sélectionnés n&#39;ont pas de pools de ressources partagés, ce champ est vide. Si ce champ est vide, les groupes de ressources que vous spécifiez ici remplaceront leurs groupes de ressources individuels.

  Pour plus d&#39;informations sur les pools de ressources, voir [Associer des pools de ressources à des utilisateurs](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

* **Taux de dépenses** : montant des dépenses par heure pour l’utilisateur ou l’utilisatrice.

  Pour connaitre les taux de dépenses effectifs par date, cliquez sur **Ajouter un taux**. Saisissez la valeur du taux de dépenses pour la période et affectez une date de début et une date de fin, le cas échéant. Le taux de dépenses 1 n’aura pas de date de début et le dernier taux de dépenses n’aura pas de date de fin.

  Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de dépenses 1 n’a pas de date de fin et que vous ajoutez le taux de dépenses 2 avec une date de début au 1er mai 2023, une date de fin au 30 avril 2023 est ajoutée au taux de dépenses 1 afin qu’il n’y ait aucune différence.

* **Taux de facturation** : le montant de la facturation par heure pour l’utilisateur ou l’utilisatrice.

  Pour connaître les taux de facturation effectifs par date, cliquez sur **Ajouter un taux**. Saisissez la valeur du taux de facturation pour la période et affectez une date de début et une date de fin, le cas échéant. Le taux de facturation 1 ne comporte pas de date de début de validité et le dernier taux de facturation n’a pas de date de fin de validité.

  Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de facturation 1 ne comporte pas de date de fin et que vous en ajoutez une seconde avec une date de début au 1er mai 2023, une date de fin au 30 avril 2023 est ajoutée au taux de facturation 1 afin qu’il n’y ait aucun trou.

### Formulaires personnalisés

Associez un formulaire personnalisé d’utilisateur existant aux utilisateurs. Vous devez créer un formulaire personnalisé avant de pouvoir l’associer à un utilisateur ou une utilisatrice. Seuls les formulaires personnalisés actifs sont affichés dans la liste. Les champs que vous ne pouvez pas modifier ne s’affichent pas dans un formulaire personnalisé individuel.

>[!NOTE]
>
>Les fonctionnalités avancées des formulaires personnalisés, telles que les champs de recherche externe et les champs natifs de Workfront, ne sont disponibles que lorsque vous ouvrez l’enregistrement de l’utilisateur ou de l’utilisatrice sur la page de détails, et non dans la boîte de dialogue Modifier l’utilisateur . (Dans la liste des personnes, cliquez sur un nom pour ouvrir les détails.)

Vous pouvez éventuellement sélectionner l’option **Recalculer les expressions personnalisées** pour vous assurer que tous les champs personnalisés calculés des formulaires personnalisés joints aux utilisateurs sélectionnés sont à jour.

Pour plus d’informations sur la création de formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Commentaire

Saisissez le commentaire à envoyer aux personnes et à la zone Mises à jour de leurs profils.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
       <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->

