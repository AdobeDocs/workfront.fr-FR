---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Modification en masse des profils utilisateur
description: En tant qu’administrateur Adobe Workfront, vous pouvez modifier les comptes d’utilisateurs en bloc.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: 18dfb67626982d73ad33871b8afce4a3f0d4cdb3
workflow-type: tm+mt
source-wordcount: '2247'
ht-degree: 0%

---

# Modification en masse des profils utilisateur

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Vous pouvez modifier les comptes d’utilisateurs par lot. Lors de la modification en masse d’utilisateurs, seuls les champs que vous sélectionnez spécifiquement sont mis à jour avec les mêmes informations pour tous les utilisateurs sélectionnés. Tous les autres champs non sélectionnés restent identiques pour chaque utilisateur, même s’ils sont différents pour chaque utilisateur.

>[!NOTE]
>
>* Vous ne pouvez pas modifier en masse la section Informations personnelles des profils des utilisateurs, car ces informations doivent être uniques pour chaque utilisateur.
>* Pour garantir la précision des données et des performances optimales, nous vous recommandons de ne sélectionner pas plus de 2 000 utilisateurs à la fois pour une modification en masse.
>

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez disposer de l’une des options suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
     <li> <p><b>Utilisateurs</b> paramètre de votre niveau d’accès configuré sur <b>Modifier</b> accès, avec <b>Créer</b> et au moins l’une des deux <b>Administration des utilisateurs</b> options activées sous <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>de ces deux options, si Utilisateur <b>Administration (utilisateurs de groupe)</b> est activé, vous devez être administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> <p>Pour plus d’informations sur la variable <b>Utilisateurs</b> paramétrer un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Modification en masse des comptes d’utilisateurs

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Utilisateurs** ![](assets/users-icon-in-main-menu.png).

1. Sélectionnez plusieurs utilisateurs, puis cliquez sur l’icône Modifier ![](assets/edit-icon.png).

1. Dans le **Modifier l’utilisateur** qui s’affiche, modifiez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Préférences</td> 
      <td> 
       <ul> 
        <li><b>Fuseau horaire :</b> Fuseau horaire des utilisateurs.</li> 
        <li><b>Paramètres régionaux</b>: paramètres régionaux préférés des utilisateurs. Cela affecte le format des nombres et des dates dans les emails provenant de Workfront.</li> 
        <li><b>Envoyer le travail que je m’assigne à mon onglet Travail</b>: cochez cette option si vous souhaitez que tout ce que les utilisateurs se voient attribuer apparaisse directement dans l’onglet Travail . La valeur par défaut est de répertorier tous les éléments affectés à un utilisateur dans son onglet Demande de travail .</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Sélectionnez les notifications électroniques qui doivent être activées pour le nouvel utilisateur.<p>Vous pouvez sélectionner des notifications instantanées ainsi que des notifications de résumé quotidiennes. Toutes les notifications de résumé quotidien sont diffusées parfois après la même heure pour tous les utilisateurs sélectionnés. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configuration des notifications d’événement pour tous les membres du système</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accès</td> 
      <td> 
       <ul> 
        <li><b>Est actif :</b> Sélectionnez ce champ pour indiquer si les utilisateurs sont actifs. Les utilisateurs actifs utilisent une licence Workfront. La désélection du champ désactive les utilisateurs.</li> 
        <li> 
        <p><b>Niveau d’accès :</b> Sélectionnez le niveau d’accès à affecter à ces utilisateurs. Tous les utilisateurs sélectionnés auront le même niveau d’accès.
        </p> 
        <p>Lorsque vous attribuez un niveau d’accès aux utilisateurs, vous pouvez attribuer un niveau égal ou inférieur à votre propre niveau d’accès. (Par exemple, si votre niveau d’accès est Planificateur, vous ne pouvez pas attribuer le niveau d’accès Administrateur.) </p>
        <p>Cependant, vous ne pouvez pas attribuer un niveau d’accès inférieur au vôtre si l’administrateur Workfront a activé des autorisations au niveau d’accès qui ne sont pas également activées dans le vôtre (via les paramètres d’optimisation, comme décrit dans la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>).</p> 
        <p>Pour plus d’informations sur les niveaux d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurer l’accès à Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Modèle de mise en page</b>: choisissez un modèle de mise en page pour les utilisateurs. Le modèle de mise en page affecté aux utilisateurs est prioritaire par rapport à tout modèle de mise en page affecté à leur groupe d’accueil, à leur équipe d’accueil ou à leur rôle de tâche principale. Pour plus d’informations sur la priorité d’attribution du modèle de mise en page, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Création et gestion des modèles de mise en page</a>.</p> 
        <p><b>REMARQUE</b>: la liste des modèles de mise en page disponibles dans ce champ dépend de votre accès :
          <ul>
           <li>En tant qu’administrateur Workfront, vous pouvez consulter tous les modèles de mise en page au niveau du système et du groupe.</li>
           <li>En tant qu’administrateur de groupe, vous pouvez afficher les modèles de mise en page au niveau du système, ainsi que ceux associés aux groupes que vous gérez.</li>
           <li><p>En tant qu’utilisateur disposant d’une licence de planificateur et ayant accès à la modification des utilisateurs, vous ne pouvez afficher que les modèles de mise en page au niveau du système. </p>
           <p>Pour plus d’informations sur les modèles de mise en page au niveau du groupe, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Création et gestion des modèles de mise en page</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisation</td> 
      <td> 
       <ul> 
        <li><b>Société</b>: entreprise des utilisateurs. Les utilisateurs ne peuvent être associés qu’à une seule entreprise. Vous devez créer une société avant de pouvoir l’associer à un utilisateur. Seules les entreprises actives s’affichent dans la liste. Pour plus d’informations sur la création d’entreprises, voir Présentation et gestion des entreprises.</li> 
        <li><b>Équipe Accueil</b>: spécifiez l’équipe d’accueil des utilisateurs. Les utilisateurs ne peuvent avoir qu’une seule équipe d’accueil. </li> 
        <li><b>Autres équipes</b>: les utilisateurs peuvent appartenir à plusieurs équipes. </li> 
        <li> <p><b>Groupe d’accueil :</b> Sélectionnez un groupe approprié pour affecter les utilisateurs en tant que groupe d’accueil. Cela permet à l’utilisateur d’accéder aux objets partagés avec le groupe.</p> <p><b>REMARQUE</b>: il s’agit d’un champ obligatoire. Les utilisateurs ne peuvent pas être associés à un groupe d’accueil.</p> <p>Vous ne pouvez affecter un groupe aux utilisateurs que dans les cas suivants :</p> 
         <ul> 
          <li>Vous êtes administrateur Workfront.</li> 
          <li>Vous êtes l’administrateur de ce groupe.</li> 
          <li>Le groupe est public.</li> 
         </ul> </li> 
        <li> <p><b>Autres groupes</b>: les utilisateurs peuvent appartenir à plusieurs groupes. Vous ne pouvez affecter un groupe à un utilisateur que dans les cas suivants :</p> 
         <ul> 
          <li>Vous êtes administrateur Workfront.</li> 
          <li>Vous êtes l’administrateur de ce groupe.</li> 
          <li> <p>Le groupe est public. </p> 
          <p>Pour plus d’informations sur les groupes publics, voir <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Création d’un groupe</a>.</p> 
          <p>Pour plus d’informations sur les groupes, voir <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Présentation des groupes</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planification des ressources</td> 
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

   <li><b>Planifier la désactivation</b>: cochez cette case si vous souhaitez planifier la désactivation des utilisateurs au bout d’un certain temps.</li> 
       <li><b>Date planifiée de désactivation</b>: date à laquelle les utilisateurs sont désactivés. Pour plus d’informations sur la planification de la désactivation des utilisateurs, voir la section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Planification de la désactivation pour les utilisateurs</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactivation ou réactivation d’un utilisateur</a>.</li> 
       <li> <p><b>Rôle de Principal</b>: il s’agit du rôle de tâche principal d’un utilisateur dans Workfront. Par défaut, chaque tâche et problème auquel les utilisateurs sont affectés est également affecté à ce rôle de tâche. Les rôles de tâche sont essentiels dans la gestion des ressources. Pour plus d’informations sur les rôles de tâche, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Création et gestion des rôles de tâche</a></p> <p>Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Plan avec accès administrateur ou si vous êtes administrateur Workfront. Pour plus d’informations sur la configuration des utilisateurs disposant d’un accès administrateur, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
       <li>(Conditionnel) Si vous avez sélectionné une <b>Rôle de Principal</b>, la variable <b>Pourcentage de disponibilité de l’éditeur de texte enrichi</b> s’affiche. Indiquez le pourcentage de temps alloué aux plannings des utilisateurs à ce rôle de tâche. La valeur par défaut du pourcentage de disponibilité de l’éditeur de texte enrichi pour le rôle de Principal est de 100 %.</li> 
       <li> <p><b>Autres rôles</b>: les utilisateurs peuvent avoir plusieurs rôles de tâche dans Workfront. Les rôles de tâche sont essentiels dans la gestion des ressources. Le nombre de rôles de tâche qu’un utilisateur peut remplir n’est pas limité. Cependant, nous vous recommandons de ne pas affecter un utilisateur à un trop grand nombre de rôles de tâche, car la gestion des ressources peut devenir trop complexe pour ces utilisateurs.</p> <p>Pour plus d’informations sur les rôles de tâche, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Création et gestion des rôles de tâche</a>.</p> <p>Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Plan avec accès administrateur ou si vous êtes administrateur Workfront. Pour plus d’informations sur la configuration des utilisateurs disposant d’un accès administrateur, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
       <li> <p>(Conditionnel) Si vous avez sélectionné une ou plusieurs <b>Autres rôles</b>, la variable <b>Pourcentage de disponibilité de l’éditeur de texte enrichi</b> s’affiche pour chaque rôle. Indiquez le pourcentage de temps alloué aux plannings des utilisateurs à chaque rôle de tâche. La valeur par défaut pour le pourcentage de disponibilité de l’éditeur de texte enrichi pour les autres rôles est de 0 %.</p> <p><b>REMARQUE</b>:  
       <ul> 
       <li>Si d’autres rôles ont une disponibilité de l’éditeur de texte enrichi de 0 %, ils ne s’affichent pas dans le planificateur de ressources, sauf si les utilisateurs sont affectés à des tâches dans ces rôles.</li> 
       <li> <p>La somme de tous les pourcentages de disponibilité de l’éditeur de texte enrichi pour tous les rôles doit être égale à 100 %. Chaque pourcentage de disponibilité de l’éditeur de texte enrichi calcule les heures disponibles pour chaque rôle par utilisateur dans le planificateur de ressources. Les Heures disponibles pour chaque rôle par utilisateur dépendent de l’heure disponible pour l’utilisateur.</p> <p>L’heure disponible pour l’utilisateur est calculée par Workfront selon la méthode sélectionnée par l’administrateur Workfront pour calculer l’éditeur de texte enrichi dans les préférences de gestion des ressources.</p> <p>Pour plus d’informations sur le calcul de la disponibilité de l’utilisateur, voir <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Présentation du calcul des heures et de l’éditeur de texte enrichi pour les utilisateurs et les rôles dans le planificateur de ressources</a>.</p> <p>Pour plus d’informations sur la configuration des préférences de gestion des ressources, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configuration des préférences de gestion des ressources</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Planification</b>: associez une planification aux utilisateurs. Le planning des utilisateurs calcule la chronologie des tâches auxquelles les utilisateurs sont affectés.</p> <p>Un administrateur Workfront ou un administrateur de groupe doit créer un planning avant qu’il puisse être associé aux utilisateurs.</p> <p>Sélectionnez une planification au niveau du système ou d’un groupe pour l’affecter aux utilisateurs sélectionnés.</p> <p>Pour plus d’informations sur les planifications au niveau du système et des groupes, voir <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Création d’un planning</a>.</p> <p><b>IMPORTANT</b>: Workfront utilise le planning d’un utilisateur uniquement lorsque le paramètre Calculer la disponibilité de la ressource avec est défini sur la Planification de l’utilisateur. Pour plus d’informations sur la manière dont le paramètre Calculer la disponibilité des ressources à l’aide du paramètre affecte le planning utilisé pour la gestion des ressources, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configuration des préférences de gestion des ressources</a>.</p> </li> 
       <li> <p><b>Profil de feuille de calcul</b>: associez un profil de feuille de temps aux utilisateurs. Cela garantit que les feuilles de temps sont générées automatiquement pour les utilisateurs.</p> 
       <p><b>REMARQUE</b>:  
       <ul> 
       <li>La liste des profils de feuille de temps disponibles dans ce champ dépend de votre accès :
       <ul>
       <li>En tant qu’administrateur Workfront, vous pouvez consulter tous les profils de feuille de temps au niveau du système et du groupe.</li>
       <li><p>En tant qu’administrateur de groupe, vous pouvez consulter les profils de feuille de temps au niveau du système, ainsi que ceux associés aux groupes que vous gérez.</p></li>
       <li><p>En tant qu’utilisateur disposant d’une licence de planificateur et ayant accès à la modification des utilisateurs, vous ne pouvez afficher que les profils de feuille de temps au niveau du système.</p></li>
       </ul></li> 
       <li>Si vous êtes administrateur de groupe, tous les utilisateurs que vous modifiez doivent appartenir à un groupe que vous administrez.</li> 
       </ul> </p> </li> 
       <li><b>Type d’heure par défaut</b>: sélectionnez le type d’heure par défaut pour les utilisateurs. Il s’agit du type d’heure utilisé par défaut lorsque l’utilisateur consigne l’heure.</li> 
       <li> <p><b>Types d’heure disponibles</b>: sélectionnez les types d’heures qui doivent être disponibles pour l’utilisateur. Ces types d’heure sont visibles partout dans Workfront où les utilisateurs peuvent consigner l’heure. Un utilisateur peut uniquement afficher les types d’heures activés au niveau du projet ainsi qu’au niveau de l’utilisateur.</p> 
       <p>Pour plus d’informations sur les types d’heures disponibles pour les utilisateurs, voir <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Définition des types d’heures et de la disponibilité des feuilles de temps</a>.</p> 
       </li> 
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
       <li> <p><b>Pools de ressources</b>: associez les utilisateurs aux pools de ressources.</p> <p><b>REMARQUE</b>: seuls les pools de ressources communs à tous les utilisateurs sélectionnés apparaissent dans ce champ. Si les utilisateurs sélectionnés n’ont aucun pool de ressources partagé, ce champ est vide. Si ce champ est vide, les pools de ressources que vous spécifiez ici remplaceront leurs pools de ressources individuels.</p> 
       <p>Pour plus d’informations sur les pools de ressources, voir <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Présentation des pools de ressources </a>.</p> </li> 
       <li><b>Coût par heure</b>: montant du coût par heure pour l’utilisateur. </li> 
       <li><b>Facturation par heure</b>: montant de la facturation par heure pour l’utilisateur.</li> 
       <li><b>Forms personnalisée</b>: associez un formulaire personnalisé utilisateur existant aux utilisateurs. Vous devez créer un formulaire personnalisé pour pouvoir l’associer à un utilisateur. Seuls les formulaires personnalisés actifs s’affichent dans la liste. Pour plus d’informations sur la création de formulaires personnalisés, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Création ou modification d’un formulaire personnalisé</a>.</li> 
       <li><b>Commentaire</b>: saisissez un commentaire dans le champ fourni. Tous les utilisateurs sélectionnés recevront une notification in-app ainsi qu’une notification par e-mail avec votre commentaire. Le commentaire s’affiche dans l’onglet Mises à jour du profil des utilisateurs.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Dans la variable **Forms personnalisée** , sélectionnez **Recalculer des expressions personnalisées** pour vous assurer que tous les champs personnalisés calculés des formulaires personnalisés joints aux utilisateurs sélectionnés sont à jour.

1. Cliquez sur **Enregistrer les modifications**.
