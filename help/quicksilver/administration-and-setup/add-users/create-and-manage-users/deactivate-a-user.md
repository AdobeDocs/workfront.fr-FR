---
title: Désactiver ou réactiver un utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur ou administratrice Workfront, vous pouvez désactiver ou réactiver un utilisateur ou une utilisatrice.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: 0c2a54406ceb690e638cdc0376a3dc01a7c2df76
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 62%

---

# Désactiver ou réactiver un utilisateur ou une utilisatrice

<!--Audited 5/2025-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Si un utilisateur ou une utilisatrice quitte l’organisation, il est recommandé de le désactiver dans le système afin d’éviter toute confusion pour les autres utilisateurs et utilisatrices lors de son ajout à des mises à jour ou de son affectation à des tâches. Lorsque vous désactivez une personne, les autres utilisateurs ou utilisatrices ne voient plus son nom lorsqu’ils ou elles recherchent des personnes dans le système.

Les administrateurs ou administratrices peuvent voir les personnes inactives dans la zone Configuration.

Vous pouvez réactiver une personne à tout moment.

>[!IMPORTANT]
>
>* Nous vous recommandons de désactiver les personnes qui ont quitté l’entreprise plutôt que de les supprimer. Si une personne est supprimée, tout l’historique associé à cette personne dans Workfront est perdu. Il s’agit de ses affectations de travail, de son association à des notes, des heures, des documents et tous les autres objets qu’elle a créés.
>
>* La désactivation d’une personne dans Workfront supprime ses licences sur Workfront et la relecture numérique. En outre, cette personne ne peut plus se voir affecter de travail. Lorsqu’une personne est désactivée, sa licence Workfront et sa licence de relecture deviennent disponibles pour un autre utilisateur ou une autre utilisatrice. Toutes les autres informations du profil de la personne désactivée restent inchangées.
>
>* La désactivation d’un utilisateur dans Workfront ne le supprime pas du profil de produit Workfront dans Adobe Admin Console. Pour plus d’informations, voir [Supprimer des utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

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
     <li> <p>Utilisateurs paramétrant votre niveau d’accès en Modifier l’accès, avec Créer et au moins l’une des deux options d’administration des utilisateurs activées sous Ajuster vos paramètres <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De ces deux options, si l’option Administration des utilisateurs (utilisateurs du groupe) est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
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

1. Sélectionnez un utilisateur dans la liste des utilisateurs.
1. Cliquez sur l’icône **Plus** ![Icône Plus](assets/more-icon.png), puis sur **Désactiver**.

1. Dans la boîte de dialogue **Désactiver l’utilisateur**, cliquez sur **Désactiver**.

## Planifier la désactivation d’utilisateurs ou d’utilisatrices

En tant que gestionnaire, vous pouvez marquer des utilisateurs ou utilisatrices afin de signaler leur désactivation avant qu’ils ou elles ne quittent effectivement votre entreprise. Par exemple, si vous travaillez avec un utilisateur lié par contrat, il est présent dans votre système pendant une période limitée et vous connaissez sa date de résiliation. Vous pouvez planifier sa désactivation à cette date.

Les administrateurs ou administratrices Workfront et les utilisateurs ou utilisatrices de licence Plan peuvent voir la date de désactivation dans leur profil d’utilisateur ou d’utilisatrice.

Pour planifier la désactivation d’une personne :

{{step-1-to-users}}

1. Sélectionnez l’utilisateur dans la liste des utilisateurs.

   Ou

   (Facultatif) Sélectionnez plusieurs utilisateurs ou utilisatrices pour planifier leur désactivation en bloc.

1. Cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png).
1. Dans le panneau de gauche de la zone **Modifier l’utilisateur**, cliquez sur **Planification des ressources**.
1. Cochez la case **Planifier la désactivation**.

1. Sélectionnez la date et l’heure de la **Date de désactivation planifiée**.

   >[!NOTE]
   >
   >* Dans la zone de l’heure, vous ne pouvez sélectionner que des incréments d’heures entières, et non des minutes.
   >* Si vous sélectionnez une heure pour le jour en cours qui s’est écoulé, Workfront planifie la désactivation le lendemain à 00 h 00.
   >* L’heure sélectionnée correspond au fuseau horaire de l’ordinateur de l’utilisateur ou l’utilisatrice qui planifie la désactivation.

1. Cliquez sur **Enregistrer les modifications**.

La personne est désactivée le jour choisi, quelque temps après l’heure sélectionnée. Si vous avez sélectionné plusieurs utilisateurs ou utilisatrices à désactiver en bloc, toutes les personnes sélectionnées sont désactivées le jour choisi, quelque temps après l’heure sélectionnée.

Nous vous recommandons de créer un rapport pour les utilisateurs dont la désactivation a été planifiée, afin de les tenir informés des utilisateurs qui vont bientôt être désactivés. Rien ne confirme que la désactivation a eu lieu une fois les utilisateurs désactivés.

## Réactiver un utilisateur ou une utilisatrice

{{step-1-to-users}}

1. Sélectionnez un utilisateur, cliquez sur l’icône **Plus** ![Icône Plus](assets/more-icon.png), puis sur **Activer**.

1. Dans la boîte de dialogue **Réactiver l&#39;utilisateur**, sélectionnez un nouveau **Niveau d&#39;accès** dans le menu déroulant, puis cliquez sur **Réactiver**.
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

* Tâches ou événements affectés à l&#39;utilisateur.
* Projets appartenant à l’utilisateur.
* Rapports configurés pour s’exécuter avec les droits d’accès de l’utilisateur.
* Modèles appartenant à l’utilisateur.
* Projets et modèles pour lesquels l’utilisateur a été défini comme gestionnaire de ressources.
* Règles de routage de file d’attente de demandes l’administrateur Workfront ou l’utilisateur de licence de plan est le cessionnaire par défaut.
* Processus d’approbation comportant une étape incluant l’utilisateur (en particulier s’il était le seul approbateur de l’étape).
* Feuilles de temps qui répertorient l’utilisateur comme approbateur/approbatrice.
* Profils de feuille de temps qui répertorient l’utilisateur en tant qu’approbateur.
* Relecture des workflows automatisés qui incluent l’utilisateur.

## Impact sur la planification des ressources lorsque vous planifiez la désactivation d’un utilisateur ou d’une utilisatrice.

Lorsque vous planifiez la désactivation d’une personne, celle-ci n’apparaît plus dans le planificateur de ressources comme étant disponible pour la budgétisation des heures. Si elle continue à faire partie des groupes de ressources, elle apparaît dans le planificateur de ressources, mais sa disponibilité est de zéro heure à partir de la date de sa désactivation planifiée.

Le planificateur de ressources prend en compte toutes les fonctions des utilisateurs et des utilisatrices, les dates d’achèvement prévues des tâches et calcule les ressources en conséquence.

Pour plus d’informations sur le planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
