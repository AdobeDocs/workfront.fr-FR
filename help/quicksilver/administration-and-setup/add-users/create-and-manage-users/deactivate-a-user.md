---
title: Désactivation ou réactivation d’un utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur ou administratrice Workfront, vous pouvez désactiver ou réactiver un utilisateur ou une utilisatrice.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 99%

---

# Désactiver ou réactiver un utilisateur ou une utilisatrice

<!--Audited 2/2024-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Si un utilisateur ou une utilisatrice quitte l’entreprise, vous devrez peut-être supprimer cette personne d’Adobe Workfront. Elle ne doit pas rester active dans le système, car cela créerait une confusion pour les autres utilisateurs ou utilisatrices lorsqu’ils ou elles l’ajoutent à des mises à jour ou lui affectent du travail. Lorsque vous désactivez une personne, les autres utilisateurs ou utilisatrices ne voient plus son nom lorsqu’ils ou elles recherchent des personnes dans le système.

Les administrateurs ou administratrices peuvent voir les personnes inactives dans la zone Configuration.

Vous pouvez réactiver une personne à tout moment.

>[!IMPORTANT]
>
>Nous vous recommandons de désactiver les personnes qui ont quitté l’entreprise plutôt que de les supprimer. Si une personne est supprimée, tout l’historique associé à cette personne dans Workfront est perdu. Il s’agit de ses affectations de travail, de son association à des notes, des heures, des documents et tous les autres objets qu’elle a créés.
>
>La désactivation d’une personne dans Workfront supprime ses licences sur Workfront et la relecture numérique. En outre, cette personne ne peut plus se voir affecter de travail. Lorsqu’une personne est désactivée, sa licence Workfront et sa licence de relecture deviennent disponibles pour un autre utilisateur ou une autre utilisatrice. Toutes les autres informations du profil de la personne désactivée restent inchangées.
>
>Pour plus d’informations sur l’impact de la suppression et de la désactivation d’utilisateurs ou d’utilisatrices, voir [Supprimer des utilisateurs et utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

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
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Parmi ces deux options, si l’option <b>Administratrion des utilisateurs et utilisatrices (utilisateurs et utilisatrices du groupe)</b> est activée, vous devez être administrateur ou administratrice de groupes d’un groupe dont l’utilisateur ou l’utilisatrice est membre.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de désactiver un administrateur ou une administratrice Workfront, ou un utilisateur ou une utilisatrice de licence Standard ou Plan, vous devez associer ses objets et activités à une autre personne.

Pour plus d’informations, voir [À propos de la désactivation d’administrateurs ou d’administratrices Workfront et d’utilisateurs ou d’utilisatrices de licence Plan](#about-deactivating-workfront-administrators-and-plan-license-users) dans cet article.

## Désactiver un utilisateur ou une utilisatrice

Tenez compte des points suivants lorsque vous désactivez un utilisateur ou une utilisatrice :

* L’utilisateur ou l’utilisatrice ne pourra pas accéder au système.
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* Toutes les données associées à l’utilisateur ou à l’utilisatrice seront conservées.
* Vous pouvez attribuer la licence de l’utilisateur ou l’utilisatrice désactivé à une autre personne.

Pour désactiver un utilisateur ou une utilisatrice :

{{step-1-to-users}}

1. Sélectionnez un utilisateur ou une utilisatrice, cliquez sur l’icône **Plus** ![](assets/more-icon.png), puis sur **Désactiver**.

1. Cliquez sur **Désactiver** dans la boîte de dialogue qui apparaît.

## Planifier la désactivation d’utilisateurs ou d’utilisatrices

En tant que gestionnaire, vous pouvez marquer des utilisateurs ou utilisatrices afin de signaler leur désactivation avant qu’ils ou elles ne quittent effectivement votre entreprise. Par exemple, si vous travaillez avec une personne liée par contrat, elle est présent dans votre système pour une période limitée et vous connaissez sa date de fin de contrat. Vous pouvez planifier sa désactivation à cette date.

Les administrateurs ou administratrices Workfront et les utilisateurs ou utilisatrices de licence Plan peuvent voir la date de désactivation dans leur profil d’utilisateur ou d’utilisatrice.

Pour planifier la désactivation d’une personne :

{{step-1-to-users}}

1. Sélectionnez le nom de l’utilisateur ou l’utilisatrice.

   Ou

   (Facultatif) Sélectionnez plusieurs utilisateurs ou utilisatrices pour planifier leur désactivation en bloc.

1. Cliquez sur l’icône Modifier ![](assets/edit-icon.png).
1. Dans la boîte de dialogue Modifier l’utilisateur ou l’utilisatrice qui s’affiche, cliquez sur **Planification des ressources** pour accéder à cette zone.
1. Activez l’option **Planifier la désactivation**.

1. Dans le calendrier qui s’affiche, indiquez la date et l’heure de la **Date de désactivation planifiée**.

   >[!NOTE]
   >
   >* Dans la zone de l’heure, vous ne pouvez sélectionner que des incréments d’heures entières, et non des minutes.
   >* Si vous sélectionnez une heure pour la date du jour qui est passée, Workfront planifie la désactivation le jour suivant à 00 h 00. L’heure sélectionnée correspond au fuseau horaire de l’ordinateur de l’utilisateur ou l’utilisatrice qui planifie la désactivation.

1. Cliquez sur **Enregistrer les modifications**.

   La personne est désactivée le jour choisi, quelque temps après l’heure sélectionnée. Si vous avez sélectionné plusieurs utilisateurs ou utilisatrices à désactiver en bloc, toutes les personnes sélectionnées sont désactivées le jour choisi, quelque temps après l’heure sélectionnée.

Nous vous recommandons de créer un rapport sur les personnes dont vous avez planifié la désactivation, afin de connaître les personnes dont la désactivation est imminente. Il n’y a pas de confirmation que la désactivation a eu lieu après que les personnes ont été désactivées.

## Réactiver un utilisateur ou une utilisatrice

{{step-1-to-users}}

1. Sélectionnez une personne, cliquez sur l’icône Plus ![](assets/more-icon.png), puis sur **Activer**.

1. Affectez un nouveau **Niveau d’accès** dans le menu déroulant, puis cliquez sur **Réactiver**.
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### Impact sur la relecture lors de la réactivation d’un utilisateur ou d’une utilisatrice

Les utilisateurs et utilisatrices désactivés perdent le rôle de relecture qui leur a été affecté par défaut et leur licence de relecture (si vous disposez d’un plan Workfront Premium hérité). Si vous décidez de réactiver l’utilisateur ou l’utilisatrice, vous devez :

* Réaffecter la licence (si vous disposez d’un plan Workfront Premium hérité). Pour plus d’informations sur les plans de relecture de Workfront, voir [Accéder à la fonctionnalité de relecture dans Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Vérifiez que la personne dispose du rôle d’épreuve approprié. Les utilisateurs et utilisatrices d’épreuve réactivés se voient affecter le rôle d’épreuve par défaut (si spécifié) pour les nouveaux utilisateurs et utilisatrices. Pour plus d’informations, voir [Configurer les rôles de relecture par défaut](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md).

## À propos de la désactivation d’administrateurs et d’administratrices Workfront et d’utilisateurs et d’utilisatrices de licence Standard ou Plan

Avant de désactiver un administrateur ou une administratrice Workfront ou un utilisateur ou une utilisatrice disposant d’une licence Plan, il est important de vérifier les objets et activités Workfront impliquant cette personne, puis de les associer à un autre administrateur ou à une autre administratrice Workfront ou à un autre utilisateur ou à une autre utilisatrice de licence Plan si nécessaire.

Ces objets et activités peuvent inclure les éléments suivants :

* Tâches ou problèmes affectés à l’utilisateur ou l’utilisatrice.
* Projets appartenant à l’utilisateur ou l’utilisatrice.
* Rapports configurés pour s’exécuter avec les droits d’accès de l’utilisateur ou l’utilisatrice.
* Modèles appartenant à l’utilisateur ou l’utilisatrice.
* Projets et modèles pour lesquels la personne a été désignée comme personne gestionnaire de ressources.
* Règles de routage de la file d’attente des demandes pour lesquelles l’administrateur ou l’administratrice Workfront ou l’utilisateur ou l’utilisatrice de la licence Plan est la personne désignée par défaut.
* Processus d’approbation dont une étape inclut la personne (en particulier si elle était la seule personne approbatrice de l’étape).
* Feuilles de temps qui désignent la personne en tant que personne approbatrice.
* Profils de feuille de temps qui désignent la personne en tant que personne approbatrice.
* Workflows automatisés de relecture qui incluent l’utilisateur ou l’utilisatrice.

## Impact sur la planification des ressources lorsque vous planifiez la désactivation d’un utilisateur ou d’une utilisatrice.

Lorsque vous planifiez la désactivation d’une personne, celle-ci n’apparaît plus dans le planificateur de ressources comme étant disponible pour la budgétisation des heures. Si elle continue à faire partie des groupes de ressources, elle apparaît dans le planificateur de ressources, mais sa disponibilité est de zéro heure à partir de la date de sa désactivation planifiée.

Le planificateur de ressources prend en compte toutes les fonctions des utilisateurs et des utilisatrices, les dates d’achèvement prévues des tâches et calcule les ressources en conséquence.

Pour plus d’informations sur le planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
