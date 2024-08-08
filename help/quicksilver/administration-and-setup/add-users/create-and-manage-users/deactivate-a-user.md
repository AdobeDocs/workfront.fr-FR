---
title: Désactivation ou réactivation d’un utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur Workfront, vous pouvez désactiver ou réactiver un utilisateur.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '1088'
ht-degree: 11%

---

# Désactivation ou réactivation d’un utilisateur

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

Si un utilisateur quitte l’entreprise, vous devrez peut-être le supprimer d’Adobe Workfront. Ils ne doivent pas rester actifs dans le système, car cela créerait une confusion pour les autres utilisateurs lorsqu’ils les ajouteraient à des mises à jour ou leur attribueraient un travail. Lorsque vous désactivez un utilisateur, son nom n’est plus visible pour les autres utilisateurs qui recherchent des personnes dans le système.

Les administrateurs peuvent voir les utilisateurs inactifs dans la zone Configuration .

Vous pouvez réactiver un utilisateur à tout moment.

>[!IMPORTANT]
>
>Nous vous recommandons de désactiver les utilisateurs qui ont quitté l’organisation plutôt que de les supprimer. Si un utilisateur est supprimé, tout l’historique de Workfront associé à cet utilisateur est perdu. Cela inclut leurs affectations de travail, leur association aux notes, heures, documents et tous les autres objets qu’ils ont créés une fois.
>
>La désactivation d’un utilisateur dans Workfront supprime les licences de l’utilisateur pour Workfront et la vérification dynamique des balises. En outre, l’utilisateur ne peut plus se voir attribuer une tâche. Lorsqu’un utilisateur est désactivé, sa licence Workfront et sa licence de vérification peuvent être utilisées par un autre utilisateur. Toutes les autres informations du profil de l’utilisateur désactivé restent inchangées.
>
>Pour plus d’informations sur l’impact de la suppression et de la désactivation des utilisateurs, voir [Suppression des utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

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
   <td>  <p>Nouvelle : standard </p> <p>Ou </p><p>Actuelle : formule </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur ou administratrice système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à un utilisateur ou une utilisatrice</a>. </p> </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Parmi ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être administrateur ou administratrice d’un groupe dont l’utilisateur est membre.</p> <p>Pour plus d’informations sur le paramètre <b>Utilisateurs et utilisatrices</b> dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Conditions préalables

Avant de désactiver un administrateur Workfront ou un utilisateur sous licence Standard ou Plan, vous devez associer ses objets et activités à un autre utilisateur.

Pour plus d’informations, voir [À propos de la désactivation des administrateurs Workfront et de la planification des utilisateurs de licence](#about-deactivating-workfront-administrators-and-plan-license-users) dans cet article.

## Désactiver un utilisateur ou une utilisatrice

Lors de la désactivation d’un utilisateur, tenez compte des points suivants :

* L’utilisateur ne pourra pas accéder au système.
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* Toutes les données associées à l’utilisateur seront conservées.
* Vous pouvez attribuer une licence d’utilisateur désactivée à un autre utilisateur.

Pour désactiver un utilisateur :

{{step-1-to-users}}

1. Sélectionnez un utilisateur, cliquez sur l&#39;icône **Plus** ![](assets/more-icon.png), puis sur **Désactiver**.

1. Cliquez sur **Désactiver** dans la zone qui s’affiche.

## Planification de la désactivation pour les utilisateurs

En tant que responsable, vous pouvez souhaiter marquer les utilisateurs pour désactivation avant qu’ils ne quittent réellement votre entreprise. Par exemple, si vous travaillez avec un utilisateur contractuellement lié, il se trouve dans votre système pendant une période limitée et vous connaissez sa date de fin. Vous pouvez programmer leur désactivation à cette date.

Les administrateurs de Workfront et les utilisateurs de la licence Plan peuvent voir la date de désactivation dans leur profil utilisateur.

Pour planifier la désactivation d’un utilisateur :

{{step-1-to-users}}

1. Sélectionnez le nom de l’utilisateur.

   Ou

   (Facultatif) Sélectionnez plusieurs utilisateurs pour les planifier en vue de leur désactivation en bloc.

1. Cliquez sur l’icône Modifier ![](assets/edit-icon.png).
1. Dans la zone Edit User qui s’affiche, cliquez sur **Resource Planning** pour accéder à cette zone.
1. Activez l’option **Planifier la désactivation** .

1. Dans le calendrier qui s’affiche, indiquez la date et l’heure de la **Date de désactivation planifiée**.

   >[!NOTE]
   >
   >* Dans la zone de temps, vous pouvez sélectionner uniquement des incréments d’une heure entière, et non des minutes.
   >* Si vous sélectionnez une heure pour le jour en cours qui s’est écoulé, Workfront programmera la désactivation pour le jour suivant à 00h00. L’heure sélectionnée correspond au fuseau horaire de l’ordinateur de l’utilisateur qui planifie la désactivation.

1. Cliquez sur **Enregistrer les modifications**.

   L’utilisateur est désactivé le jour sélectionné après l’heure sélectionnée. Si vous avez sélectionné plusieurs utilisateurs à désactiver en bloc, tous les utilisateurs sélectionnés sont désactivés le jour sélectionné après l’heure sélectionnée.

Nous vous recommandons de créer un rapport pour les utilisateurs que vous avez programmés pour la désactivation, afin de vous tenir informé des utilisateurs qui vont être désactivés. Il n’existe aucune confirmation que la désactivation s’est produite une fois les utilisateurs désactivés.

## Réactiver un utilisateur

{{step-1-to-users}}

1. Sélectionnez un utilisateur, cliquez sur l’icône Plus ![](assets/more-icon.png), puis sur **Activer**.

1. Attribuez un nouveau **niveau d&#39;accès** dans le menu déroulant, puis cliquez sur **Réactiver**.
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### Impact de la vérification lorsque vous réactivez un utilisateur

Les utilisateurs désactivés perdent leur rôle de vérification par défaut et leur licence de BAT (si vous utilisez un forfait hérité Workfront Premium). Si vous choisissez de réactiver l’utilisateur, vous devez :

* Réaffectez la licence (si vous utilisez un forfait hérité Workfront Premium). Pour plus d’informations sur les plans de vérification de Workfront, voir [Accès aux fonctionnalités de vérification dans Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Vérifiez qu’ils disposent du rôle de BAT correct. Les utilisateurs de BAT réactivés se voient attribuer le rôle de BAT par défaut spécifié pour les nouveaux utilisateurs. Pour plus d’informations, voir [Configuration des rôles de vérification par défaut](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) .

## À propos de la désactivation des administrateurs Workfront et des utilisateurs de licences Standard ou Plan

Avant de désactiver un administrateur Workfront ou un utilisateur disposant d’une licence Plan, il est important de rechercher les objets et activités Workfront qui impliquent cette personne, puis de les associer à un autre administrateur Workfront ou de planifier un utilisateur de licence selon les besoins.

Ces objets et activités peuvent inclure les éléments suivants :

* Tâches ou problèmes affectés à l’utilisateur
* Projets détenus par l’utilisateur
* Rapports configurés pour s’exécuter avec les droits d’accès de l’utilisateur
* Modèles appartenant à l’utilisateur
* Projets et modèles sur lesquels l’utilisateur a été défini comme gestionnaire de ressources
* Règles de routage de la file d’attente des demandes sur lesquelles l’administrateur Workfront ou l’utilisateur de la licence Plan est le responsable par défaut
* Processus de validation comportant une étape, y compris l’utilisateur (en particulier s’il était le seul approbateur sur l’étape)
* Feuilles de calcul qui répertorient l’utilisateur en tant qu’approbateur
* Profils de feuille de temps qui répertorient l’utilisateur en tant qu’approbateur
* Vérification des processus automatisés qui incluent l’utilisateur

## Impact de la planification des ressources lorsque vous planifiez la désactivation d’un utilisateur

Lorsque vous planifiez la désactivation d’un utilisateur, il n’apparaît plus dans le planificateur de ressources comme étant disponible pour les heures de budget. S’ils restent membres des groupes de ressources, ils apparaissent dans le planificateur de ressources, mais leur disponibilité est définie sur zéro heure à compter de la date de leur désactivation planifiée.

Le planificateur de ressources prend en compte tous les rôles de tâche des utilisateurs et les dates d’achèvement planifiées des tâches et calcule les ressources en conséquence.

Pour plus d’informations sur le planificateur de ressources, consultez la [présentation du planificateur de ressources](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
