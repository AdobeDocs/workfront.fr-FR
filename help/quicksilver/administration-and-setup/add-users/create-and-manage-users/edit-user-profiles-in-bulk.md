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
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '2212'
ht-degree: 95%

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
     <li> <p>Niveau d’accès de l’administrateur système. </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifier des comptes d’utilisateurs et d’utilisatrices en masse

{{step-1-to-users}}

1. Sélectionnez plusieurs utilisateurs, puis cliquez sur l’icône Modifier ![icône Modifier](assets/edit-icon.png).

1. Dans la zone **Modifier l’utilisateur ou l’utilisatrice** qui s’affiche, modifiez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Préférences</td> 
      <td> 
       <ul> 
        <li><b>Fuseau horaire :</b> fuseau horaire des utilisateurs et utilisatrices.</li> 
        <li><b>Paramètre local</b> : paramètre local préféré des utilisateurs et utilisatrices. Cela affecte le format des nombres et des dates dans les e-mails envoyés par Workfront.</li> 
        <li><b>Envoyer le travail que je me suis affecté dans mon onglet Travailler sur </b> : ce paramètre fait référence à une fonctionnalité obsolète qui a été supprimée de Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Sélectionnez les notifications par e-mail qui doivent être activées pour le nouvel utilisateur ou la nouvelle utilisatrice.<p>Vous pouvez sélectionner des notifications instantanées ou une synthèse des notifications quotidienne. Toutes les synthèses de notifications quotidiennes sont envoyées peu après la même heure pour tous les utilisateurs et utilisatrices sélectionnés. Pour plus d’informations, consultez <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurer les notifications d’événements pour tous les utilisateurs et utilisatrices du système</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accès</td> 
      <td> 
       <ul> 
        <li><b>Est actif :</b> sélectionnez ce champ pour indiquer si les utilisateurs et utilisatrices sont actifs. Les utilisateurs et utilisatrices actifs utilisent une licence Workfront. La désélection du champ désactive les utilisateurs et les utilisatrices.</li> 
        <li> 
        <p><b>Niveau d’accès :</b> sélectionnez le niveau d’accès à attribuer à ces utilisateurs et ces utilisatrices. Tous les utilisateurs et utilisatrices sélectionnés disposeront du même niveau d’accès.
        </p> 
        <p>Lorsque vous attribuez un niveau d’accès à des utilisateurs et des utilisatrices, vous pouvez attribuer un niveau égal ou inférieur à votre propre niveau d’accès. (Par exemple, si votre niveau d’accès est Planificateur, vous ne pouvez pas attribuer le niveau d’accès Administrateur.) </p>
        <p>Cependant, vous ne pouvez pas attribuer un niveau d’accès inférieur au vôtre si l’administrateur ou l’administratrice Workfront a accordé des autorisations pour le niveau d’accès qui ne sont pas également activées pour le vôtre (via les paramètres d’affinage, comme décrit dans <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>).</p> 
        <p>Pour plus d’informations sur les niveaux d’accès, consultez <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurer l’accès à Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Modèle de disposition</b> : choisissez un modèle de disposition pour les utilisateurs et les utilisatrices. Le modèle de disposition attribué aux utilisateurs et aux utilisatrices est prioritaire sur tout modèle de disposition affecté à leur groupe principal, à leur équipe principale ou à leur fonction principale. Pour plus d’informations sur la priorité d’affectation des modèles de disposition, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Créer et gérer des modèles de disposition</a>.</p> 
        <p><b>NOTE</b> : la liste des modèles de disposition disponibles dans ce champ dépend de votre accès :
          <ul>
           <li>En tant qu’administrateur ou administratrice Workfront, vous pouvez consulter tous les modèles de mise en page au niveau du système et du groupe.</li>
           <li>En tant qu’administrateur ou administratrice de groupes, vous pouvez voir les modèles de disposition au niveau du système, ainsi que ceux associés aux groupes que vous gérez.</li>
           <li><p>Si vous disposez d’une licence de planification et d’un accès à la modification des utilisateurs et utilisatrices, vous ne pouvez voir que les modèles de disposition au niveau du système. </p>
           <p>Pour plus d’informations sur les modèles de disposition au niveau du groupe, voir <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Créer et gérer des modèles de disposition</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisation</td> 
      <td> 
       <ul> 
        <li><b>Entreprise</b> : entreprise des utilisateurs et utilisatrices. Les personnes ne peuvent être associées qu’à une seule entreprise. Vous devez créer une entreprise avant de pouvoir l’associer à une personne. Seules les entreprises actives sont affichées dans la liste. Pour plus d’informations sur la création d’entreprises, voir Comprendre et gérer les entreprises.</li> 
        <li><b>Équipe principale</b> : indiquez l’équipe principale des utilisateurs et utilisatrices. Les personnes ne peuvent avoir qu’une seule équipe principale. </li> 
        <li><b>Autres équipes</b> : les personnes peuvent appartenir à plusieurs équipes. </li> 
        <li> <p><b>Groupe principal :</b> sélectionnez un groupe en guise de groupe principal des personnes. La personne peut ainsi accéder aux objets partagés avec le groupe.</p> <p><b>NOTE</b> : ce champ est obligatoire. Les personnes doivent obligatoirement être associées à un groupe principal.</p> <p>Vous ne pouvez attribuer un groupe aux personnes que dans les cas suivants :</p> 
         <ul> 
          <li>Vous êtes un administrateur ou une administratrice Workfront.</li> 
          <li>Vous êtes l’administrateur ou l’administratrice de ce groupe.</li> 
          <li>Ce groupe est public.</li> 
         </ul> </li> 
        <li> <p><b>Autres groupes</b> : les personnes peuvent appartenir à plusieurs groupes. Vous ne pouvez attribuer un groupe à une personne que dans les cas suivants :</p> 
         <ul> 
          <li>Vous êtes un administrateur ou une administratrice Workfront.</li> 
          <li>Vous êtes l’administrateur ou l’administratrice de ce groupe.</li> 
          <li> <p>Ce groupe est public. </p> 
          <p>Pour plus d’informations sur les groupes publics, voir <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Créer un groupe</a>.</p> 
          <p>Pour plus d’informations sur les groupes, voir <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Vue d’ensemble des groupes</a>.</p> 
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
       <b>Temps de travail</b> : représente le pourcentage du temps équivalent temps plein (FTE) que la personne peut consacrer au travail effectif, hors durée supplémentaire. Le temps de travail doit être un nombre décimal inférieur ou égal à 1 et ne peut pas être égal à 0. Par exemple, une disponibilité de 20 % pour le travail effectif serait de 0,2.

   La valeur par défaut de ce champ est 1, ce qui indique que la personne consacre la totalité de son équivalent temps complet au travail réel lié au projet.

   Le système utilise ce nombre pour calculer la disponibilité de la personne quant au travail réel lié au projet.

   Pour plus d’informations sur la création de plannings dans Workfront, voir <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Créer un planning</a>.

   Les exceptions au planning et les congés peuvent également affecter la capacité de la personne.

   Workfront calcule la disponibilité d’une personne en fonction des préférences de gestion des ressources dans votre zone de configuration. Pour plus d’informations, voir <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurer les préférences de gestion des ressources</a>.

   <b>CONSEIL</b>

   Définissez la valeur Temps de travail sur 1 pour indiquer que la personne est disponible pour effectuer le travail lié au projet pendant la totalité de son équivalent temps complet.
   </li>

   <li><b>Planifier la désactivation</b> : cochez cette case pour programmer la désactivation des personnes après un certain temps.</li> 
       <li><b>Date de désactivation planifiée</b> : date après laquelle les personnes sont désactivées. Pour plus d’informations sur la planification de la désactivation des personnes, voir la section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Planifier la désactivation des utilisateurs et utilisatrices</a> dans <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactiver ou réactiver un utilisateur ou une utilisatrice</a>.</li> 
       <li> <p><b>Rôle principal</b> : rôle principal de la personne dans Workfront. Par défaut, l’ensemble des tâches et problèmes auxquels les personnes sont affectées sont également affectés à cette fonction. Les fonctions sont essentielles à la gestion des ressources. Pour plus d’informations sur les fonctions, voir <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Créer et gérer des fonctions</a>.</p> <p>Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Plan avec un accès utilisateur administratif, ou si vous êtes un administrateur ou une administratrice Workfront. Pour plus d’informations sur la configuration des personnes disposant d’un accès administratif, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> </li> 
       <li>(Facultatif) Si vous avez sélectionné un <b>Rôle principal</b>, le champ <b>Pourcentage de disponibilité équivalent temps complet</b> s’affiche. Spécifiez le pourcentage de temps affecté à cette fonction dans le planning des utilisateurs et utilisatrices. La valeur par défaut du pourcentage de disponibilité équivalent temps complet pour le rôle principal est de 100 %.</li> 
       <li> <p><b>Autres rôles</b> : les utilisateurs et les utilisatrices peuvent exercer plusieurs fonctions dans Workfront. Les fonctions sont essentielles à la gestion des ressources. Une personne peut remplir un nombre illimité de fonctions. Toutefois, nous recommandons de ne pas affecter un nombre excessivement élevé de fonctions à une personne, car la gestion des ressources pourrait devenir trop complexe pour ces personnes.</p> <p>Pour plus d’informations sur les fonctions, consultez la section <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Créer et gérer des fonctions</a>.</p> <p>Vous ne pouvez mettre à jour ce champ que si vous disposez d’une licence Plan avec un accès utilisateur administratif, ou si vous êtes un administrateur ou une administratrice Workfront. Pour plus d’informations sur la configuration des utilisateurs et utilisatrices disposant d’un accès administratif, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> </li> 
       <li> <p>(Facultatif) Si vous avez sélectionné un ou plusieurs <b>Autres rôles</b>, le champ <b>Pourcentage de disponibilité équivalent temps complet</b> s’affiche pour chaque rôle. Spécifiez le pourcentage de temps affecté à chaque fonction dans le planning des personnes. La valeur par défaut du pourcentage de disponibilité équivalent temps complet pour les autres rôles est de 0 %.</p> <p><b>NOTE</b> :  
       <ul> 
       <li>si d’autres rôles ont une disponibilité équivalent temps complet de 0 %, ils ne s’affichent pas dans le planificateur de ressources, sauf si ces rôles comprennent des tâches affectées à la personne.</li> 
       <li> <p>La somme de tous les pourcentages de disponibilité équivalent temps complet pour tous les rôles doit être égale à 100 %. Chaque pourcentage de disponibilité équivalent temps complet calcule les heures disponibles pour chaque rôle par personne dans le planificateur de ressources. Les heures disponibles pour chaque rôle par personne dépendent du temps disponible pour la personne.</p> <p>Le temps disponible pour la personne est calculé par Workfront en fonction de la méthode sélectionnée par l’administration Workfront pour calculer l’équivalent temps complet dans les préférences de gestion des ressources.</p> <p>Pour plus d’informations sur le calcul de la disponibilité de la personne, consultez la section <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Vue d’ensemble du calcul des heures et de l’équivalent temps complet pour les personnes et les rôles dans le planificateur de ressources</a>.</p> <p>Pour plus d’informations sur la configuration des préférences de gestion des ressources, consultez la section <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurer les préférences de gestion des ressources</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Planning</b> : associez un planning pour les utilisateurs et utilisatrices. Le planning des utilisateurs et des utilisatrices calcule la chronologie des tâches auxquelles ces personnes sont affectées.</p> <p>L’administration Workfront ou un administrateur ou une administratrice de groupes doit créer un planning avant de pouvoir l’associer à des personnes.</p> <p>Sélectionnez un planning au niveau du système ou d’un groupe pour l’affecter aux personnes sélectionnées.</p> <p>Pour plus d’informations sur les plannings au niveau du système et du groupe, consultez la section <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Créer un planning</a>.</p> <p><b>IMPORTANT</b> : Workfront utilise le planning d’une personne uniquement lorsque le paramètre « Calculer la disponibilité des ressources avec » est défini sur « Le planning de la personne ». Pour plus d’informations sur la manière dont le paramètre « Calculer la disponibilité des ressources avec » affecte le planning utilisé pour la gestion des ressources, consultez la section <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurer les préférences de la gestion des ressources</a>.</p> </li> 
       <li> <p><b>Profil de feuille de temps</b> : associez un profil de feuille de temps aux personnes. Les feuilles de temps sont ainsi générées automatiquement pour les personnes.</p> 
       <p><b>NOTE</b> :  
       <ul> 
       <li>La liste des profils de feuilles de temps disponibles dans ce champ dépend de votre accès :
       <ul>
       <li>En tant qu’administrateur ou administratrice Workfront, vous pouvez voir tous les profils de feuilles de temps au niveau du système et du groupe.</li>
       <li><p>En tant qu’administrateur ou administratrice de groupes, vous pouvez voir les profils de feuille de temps au niveau du système, ainsi que ceux associés aux groupes que vous gérez.</p></li>
       <li><p>En tant qu’utilisateur ou utilisatrice disposant d’une licence de planification et d’un accès à la modification des utilisateurs et des utilisatrices, vous ne pouvez voir que les profils de feuille de temps au niveau du système.</p></li>
       </ul></li> 
       <li>Si vous êtes administrateur ou administratrice de groupes, toutes les personnes que vous modifiez doivent être membres d’un groupe que vous gérez.</li> 
       </ul> </p> </li> 
       <li><b>Type d’heure par défaut</b> : sélectionnez le type d’heure par défaut pour les utilisateurs et les utilisatrices. Il s’agit du type d’heure utilisé par défaut lorsque les utilisateurs et les utilisatrices consignent des heures.</li> 
       <li> <p><b>Types d’heures disponibles</b> : sélectionnez les types d’heures qui doivent être disponibles pour la personne. Ces types d’heures sont visibles partout dans Workfront où les personnes peuvent consigner des heures. Une personne ne peut voir que les types d’heures qui sont activés au niveau du projet et au niveau de la personne.</p> 
       <p>Pour plus d’informations sur les types d’heures disponibles pour les utilisateurs, voir <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref"> Définir les types d’heures et la disponibilité </a>.</p> 
       </li> 
       <li> <b>Équivalent temps complet</b> : il s’agit de l’équivalent temps complet de l’utilisateur ou de l’utilisatrice. Workfront utilise ce nombre pour calculer la disponibilité de la personne en fonction du planning par défaut uniquement lorsque les préférences de gestion des ressources au niveau du système sont définies sur « Le planning par défaut ».

   <p>L’équivalent temps complet indique le temps que la personne peut consacrer au travail. Cela comprend les durées supplémentaires, ainsi que le temps consacré au travail sur les projets. Par exemple, le temps passé en réunion ou en formation est également inclus dans l’équivalent temps complet.</p>

   L’équivalent temps complet doit être un nombre décimal inférieur ou égal à 1 et ne peut pas être égal à 0. Par exemple, si la valeur de l’équivalent temps complet est de 0,5 et que l’horaire par défaut dans Workfront est de 40 heures, la personne est disponible 20 heures par semaine.

   La valeur par défaut de ce champ est 1.

   Les exceptions de planning, les congés éventuels et la valeur du temps de travail peuvent affecter la disponibilité de la personne.

   Workfront calcule la disponibilité d’une personne en fonction des préférences de gestion des ressources dans votre zone de configuration.

   Si les préférences de gestion des ressources au niveau du système sont définies sur le planning de la personne, la valeur que vous spécifiez ici est ignorée et la personne est considérée comme étant disponible selon ce qui est spécifié dans son planning.

   Pour plus d’informations, consultez la section <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurer les préférences de gestion des ressources</a>.

   Pour plus d’informations sur la création de plannings dans Workfront, voir <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Créer un planning</a>.
   </li> 
       <li> <p><b>Groupes de ressources</b> : associez les utilisateurs et utilisatrices aux groupes de ressources.</p> <p><b>NOTE</b> : seuls les groupes de ressources communs à tous les utilisateurs et utilisatrices sélectionnés apparaissent dans ce champ. Si les utilisateurs et utilisatrices sélectionnés n’ont pas de groupes de ressources partagés, ce champ est vide. Si ce champ est vide, les groupes de ressources que vous spécifiez ici remplaceront leurs groupes de ressources individuels.</p> 
       <p>Pour plus d’informations sur les groupes de ressources, voir <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">Vue d’ensemble des groupes de ressources</a>.</p> </li> 
       <li><b>Coûts par heure</b> : le montant des coûts par heure pour l’utilisateur ou l’utilisatrice. </li> 
       <li><b>Facturation par heure</b> : le montant de la facturation par heure pour l’utilisateur ou l’utilisatrice.</li> 
       <li><b>Formulaires personnalisés</b> : associez un formulaire personnalisé existant aux utilisateurs et utilisatrices. Vous devez créer un formulaire personnalisé avant de pouvoir l’associer à un utilisateur ou une utilisatrice. Seuls les formulaires personnalisés actifs sont affichés dans la liste. Pour plus d’informations sur la création de formulaires personnalisés, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Créer un formulaire personnalisé</a>.</li> 
       <li><b>Commenter</b> : saisissez un commentaire dans le champ prévu à cet effet. Tous les utilisateurs et utilisatrices sélectionnés recevront une notification in-app ainsi qu’une notification par e-mail contenant votre commentaire. Le commentaire s’affiche dans l’onglet Mises à jour du profil des utilisateurs et utilisatrices.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Dans la section **Formulaires personnalisés**, sélectionnez l’option **Recalculer les expressions personnalisées** pour vous assurer que tous les champs personnalisés calculés des formulaires personnalisés associés aux utilisateurs et utilisatrices sélectionnés sont à jour.

1. Cliquez sur **Enregistrer les modifications**.
