---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Ajouter des utilisateurs
description: En tant qu’administrateur Workfront ou utilisateur disposant d’un accès administrateur complet, vous pouvez ajouter des utilisateurs dans Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 198129edd8690393e3214f5041b183b5516617a7
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 21%

---

# Ajouter des utilisateurs

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>Si votre entreprise a été intégrée à Adobe Admin Console, vous devez créer des administrateurs système via Adobe Admin Console.
>
>Pour plus d’informations sur la création d’administrateurs système dans Adobe Admin Console, voir [Gestion des administrateurs système dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Les administrateurs de groupe des organisations intégrées à Adobe Admin Console peuvent suivre cette procédure pour créer des utilisateurs et envoyer l’utilisateur pour approbation par l’administrateur.
>
>Pour obtenir une liste de procédures qui varient selon que votre organisation a été intégrée ou non à Adobe Admin Console, voir [Différences d’administration en fonction de la plateforme (Adobe Workfront Fusion/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Vous pouvez ajouter des utilisateurs dans Adobe Workfront en créant des utilisateurs individuels à partir de zéro ou en copiant des utilisateurs existants.

Pour plus d’informations sur l’importation simultanée de plusieurs utilisateurs, voir [Importation d’utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Conditions d’accès

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
   <td><p>Nouvelle : standard</p><p>Ou</p><p>Actuelle : formule</p></td> 
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

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Avant d’ajouter un utilisateur, rassemblez les informations sur l’utilisateur répertoriées ci-dessous et déterminez les informations à associer à cet utilisateur :

* Quelles sont les informations personnelles de l’utilisateur ? Vous avez besoin au minimum des éléments suivants :

   * Nom complet
   * Un nom d’utilisateur
   * Mot de passe par défaut
   * Adresse e-mail

  >[!NOTE]
  >
  >Vous pouvez déterminer si les utilisateurs peuvent afficher les coordonnées d’autres utilisateurs en affinant le paramètre Affichage utilisateur lors de la spécification des niveaux d’accès aux objets Workfront. Pour plus d’informations, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Quelle est la position du nouvel utilisateur au sein de l’entreprise ? Cette personne a-t-elle des rapports directs ? À qui cette personne se rapporte-t-elle ?
* Quel est le rôle de la personne ? Ce rôle de tâche existe-t-il dans Workfront ? Y a-t-il une limite au nombre de personnes qui peuvent remplir ce rôle d’employé ? Pour plus d’informations sur la création de rôles de tâche, voir [Création et gestion de rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* Quel niveau d’accès doit avoir l’utilisateur ? Existe-t-il déjà ou devez-vous en créer un nouveau ? Pour plus d’informations, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* Dans quel groupe d’accueil cet utilisateur doit-il se trouver ? La personne doit-elle appartenir à plusieurs groupes ? Pour plus d’informations sur les groupes, voir [Présentation des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* Dans quelle équipe d’accueil cet utilisateur doit-il se trouver ? La personne doit-elle faire partie de plusieurs équipes ? Pour plus d’informations sur les équipes, voir [Présentation des équipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Quelles informations personnalisées devez-vous associer à cet utilisateur ?

  Si des informations sur les utilisateurs sont capturées dans des champs personnalisés que vous avez créés, un formulaire personnalisé doit être prêt lors de la création d’un utilisateur. Pour plus d’informations sur les formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Création d’un utilisateur à partir de zéro

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Utilisateurs** ![](assets/users-icon-in-main-menu.png).

1. Cliquez sur **Nouvel utilisateur > Nouvel utilisateur** pour ajouter un utilisateur qui n’a pas encore été ajouté à Workfront.

   Ou

   Cliquez sur **Nouvel utilisateur > Importer des utilisateurs** pour ajouter des utilisateurs en chargeant un fichier d’importation de feuille de calcul.

   Si vous importez des utilisateurs, vous n’avez pas besoin de poursuivre cette procédure. Pour plus d’informations, voir [Importer des utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. Dans la zone **New User** qui s’affiche, cliquez sur **Afficher les options avancées**, puis configurez les options disponibles pour saisir les informations de la personne.

   Pour plus d’informations sur ces options, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Utilisez l’une des méthodes suivantes :

   * Laissez **Envoyer un courrier électronique d’invitation à cette personne** activé. Dans ce cas, l’utilisateur reçoit un courrier électronique lui permettant de suivre un lien afin de créer son propre mot de passe pour Workfront. Les utilisateurs qui n’acceptent pas l’invitation par courrier électronique et ne créent pas de mot de passe Workfront sont répertoriés comme Non enregistrés dans Workfront.
   * Désactivez **Envoyer un courrier électronique d’invitation à cette personne**, puis tapez un **mot de passe** pour la personne et confirmez-le dans la zone **Confirmer le mot de passe**. Vous devrez partager ce mot de passe avec l’utilisateur en dehors de Workfront.

   >[!NOTE]
   >
   >* Si votre administrateur Workfront a activé une intégration SSO avec Workfront, le champ Autoriser uniquement l’authentification &lt;configuration SSO> est masqué si vous désactivez l’invitation par courrier électronique. Le champ ID de fédération ou &lt;Configuration SSO> Nom d’utilisateur reste visible.
   >
   * Si votre organisation a été intégrée à l’Admin Console et que vous ajoutez un utilisateur via Workfront, vous n’avez pas la possibilité d’envoyer une invitation par courrier électronique.
   >
   Pour les utilisateurs et les utilisatrices d’Adobe existants, l’utilisateur ou l’utilisatrice peut recevoir ou non un e-mail sur la disponibilité de Workfront. Il s’agit d’une préférence contrôlée par l’administrateur ou l’administratrice d’Adobe pour le produit.

1. Cliquez sur **Ajouter cette personne**.

   Ou

   Cliquez sur **Ajouter une personne et démarrer une autre** pour enregistrer le nouvel utilisateur et en ajouter un autre.

   >[!NOTE]
   >
   Si vous êtes administrateur de groupe et que vous ajoutez un utilisateur à une organisation qui a été intégrée à Adobe Admin Console, les options de cette étape sont **Submit user for Admin Approval** et **Submit for Approval &amp; Start Other**. L’utilisateur est créé dans un état Désactivé et En attente d’approbation . Un administrateur Workfront doit approuver l’utilisateur, qui l’active dans Workfront et l’ajoute à Adobe Admin Console.

## Copier un utilisateur pour en créer un nouveau

Vous pouvez créer un utilisateur en copiant un utilisateur existant.

>[!NOTE]
>
Lorsque vous créez un utilisateur de cette manière, toutes les informations sont copiées de l’utilisateur d’origine vers l’utilisateur nouvellement créé, à l’exception des informations suivantes :
>
* Les informations de la section Informations personnelles .
* Lorsque je me connecte, affichez : l&#39;onglet d&#39;entrée par défaut du niveau d&#39;accès est sélectionné dans cette zone.
* Rapports directs
>

Pour créer un utilisateur en copiant un utilisateur existant :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Utilisateurs** ![](assets/users-icon-in-main-menu.png).
1. Sélectionnez l’utilisateur à copier, puis cliquez sur l’icône Copier ![](assets/copy-icon.png).
1. Dans la zone **Copier l’utilisateur** qui s’affiche, modifiez les champs disponibles pour le nouvel utilisateur.

   Pour plus d’informations sur tous les champs associés à un utilisateur, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Cliquez sur **Ajouter cette personne**.

   Ou

   Cliquez sur **Ajouter une personne et démarrer une autre** pour enregistrer le nouvel utilisateur et en ajouter un autre.

Un nouveau compte est ainsi créé dans Workfront pour l’utilisateur.

Si vous avez sélectionné l’option permettant d’envoyer une invitation à l’utilisateur, celui-ci doit recevoir un e-mail lui permettant de suivre un lien pour créer son mot de passe Workfront.

>[!NOTE]
>
Si votre organisation a été intégrée à l’Admin Console et que vous ajoutez un utilisateur via Workfront, vous n’avez pas la possibilité d’envoyer une invitation par courrier électronique.
>
Pour les utilisateurs et les utilisatrices d’Adobe existants, l’utilisateur ou l’utilisatrice peut recevoir ou non un e-mail sur la disponibilité de Workfront. Il s’agit d’une préférence contrôlée par l’administrateur ou l’administratrice d’Adobe pour le produit.
