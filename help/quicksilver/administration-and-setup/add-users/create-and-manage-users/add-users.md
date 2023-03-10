---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Ajouter des utilisateurs
description: En tant qu’administrateur Workfront ou utilisateur disposant d’un accès administrateur complet, vous pouvez ajouter des utilisateurs dans Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# Ajouter des utilisateurs

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées au Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, vous devez effectuer cette action via Adobe Admin Console.
>
>Pour plus d’informations sur l’ajout d’un utilisateur dans Adobe Admin Console :
>
>* Voir [Création d’utilisateurs dans Workfront avec Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
>* Voir la section &quot;Ajouter des utilisateurs&quot; de l’article [Gérer les utilisateurs individuellement](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contactez votre administrateur Adobe Admin Console.
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Admin Console, reportez-vous à la section [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Vous pouvez ajouter des utilisateurs dans Adobe Workfront en créant des utilisateurs individuels à partir de zéro ou en copiant des utilisateurs existants.

Pour plus d’informations sur l’importation simultanée de plusieurs utilisateurs, voir [Importer des utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
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

## Conditions préalables

Avant d’ajouter un utilisateur, rassemblez les informations sur l’utilisateur répertoriées ci-dessous et déterminez les informations à associer à cet utilisateur :

* Quelles sont les informations personnelles de l’utilisateur ? Vous avez besoin au minimum des éléments suivants :

   * Nom complet
   * Un nom d’utilisateur
   * Mot de passe par défaut
   * Adresse e-mail

   >[!NOTE]
   >
   >Vous pouvez déterminer si les utilisateurs peuvent afficher les coordonnées d’autres utilisateurs en affinant le paramètre Affichage utilisateur lors de la spécification des niveaux d’accès aux objets Workfront. Pour plus d’informations, voir [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Quelle est la position du nouvel utilisateur au sein de l’entreprise ? Cette personne a-t-elle des rapports directs ? À qui cette personne se rapporte-t-elle ?
* Quel est le rôle de la personne ? Ce rôle de tâche existe-t-il dans Workfront ? Y a-t-il une limite au nombre de personnes qui peuvent remplir ce rôle d’employé ? Pour plus d’informations sur la création de rôles de tâche, voir [Création et gestion des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* Quel niveau d’accès doit avoir l’utilisateur ? Existe-t-il déjà ou devez-vous en créer un nouveau ? Pour plus d’informations, voir [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* Dans quel groupe d’accueil cet utilisateur doit-il se trouver ? La personne doit-elle appartenir à plusieurs groupes ? Pour plus d’informations sur les groupes, voir [Présentation des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* Dans quelle équipe d’accueil cet utilisateur doit-il se trouver ? La personne doit-elle faire partie de plusieurs équipes ? Pour plus d’informations sur les équipes, voir [Présentation des équipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Quelles informations personnalisées devez-vous associer à cet utilisateur ?

   Si des informations sur les utilisateurs sont capturées dans des champs personnalisés que vous avez créés, un formulaire personnalisé doit être prêt lors de la création d’un utilisateur. Pour plus d’informations sur les formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Création d’un utilisateur à partir de zéro

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Utilisateurs** ![](assets/users-icon-in-main-menu.png).

1. Cliquez sur **Nouvel utilisateur > Nouvel utilisateur** pour ajouter un utilisateur qui n’a pas encore été ajouté à Workfront.

   Ou

   Cliquez sur **Nouvel utilisateur > Importer des utilisateurs** pour ajouter des utilisateurs en chargeant un fichier d’importation de feuille de calcul.

   Si vous importez des utilisateurs, vous n’avez pas besoin de poursuivre cette procédure. Pour plus d’informations, voir [Importer des utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. Dans le **Nouvel utilisateur** s’affiche, cliquez sur **Afficher les options avancées**, puis configurez les options disponibles pour saisir les informations de la personne.

   Pour plus d’informations sur ces options, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Utilisez l’une des méthodes suivantes :

   * Laissez tomber **Envoyer un courrier électronique d’invitation à cette personne** activée. Dans ce cas, l’utilisateur reçoit un courrier électronique lui permettant de suivre un lien afin de créer son propre mot de passe pour Workfront. Les utilisateurs qui n’acceptent pas l’invitation par courrier électronique et ne créent pas de mot de passe Workfront sont répertoriés comme Non enregistrés dans Workfront.
   * Désactiver **Envoyer un courrier électronique d’invitation à cette personne**, puis saisissez une **Mot de passe** pour la personne et confirmez-la dans le **Confirmer le mot de passe** de la boîte. Vous devrez partager ce mot de passe avec l’utilisateur en dehors de Workfront.

   >[!NOTE]
   >
   >Si votre administrateur Workfront a activé une intégration SSO avec Workfront, alors l’option Autoriser uniquement &lt;sso configuration=&quot;&quot;> Le champ d’authentification est masqué si vous désactivez l’invitation par courrier électronique. L’ID de fédération ou &lt;sso configuration=&quot;&quot;> Le champ Nom d’utilisateur reste visible.

   >[!NOTE]
   Si votre entreprise a été intégrée au Admin Console et que vous ajoutez un utilisateur via Workfront, vous n’avez pas la possibilité d’envoyer une invitation par courrier électronique.
   Les nouveaux utilisateurs d’Adobe sont ajoutés au Admin Console et le Admin Console leur envoie un courrier électronique pour les inviter à terminer le processus d’enregistrement. Tous les utilisateurs doivent terminer le processus d’enregistrement pour accéder à n’importe quel système d’Adobe.
   Pour les utilisateurs d’Adobe existants, l’utilisateur peut recevoir ou non un e-mail sur la disponibilité de Workfront. Il s’agit d’une préférence contrôlée par l’administrateur d’Adobe pour le produit.

1. Cliquez sur **Ajouter Cet Utilisateur**.

   Ou

   Cliquez sur **Ajout d’un utilisateur et démarrage d’une autre personne** pour enregistrer le nouvel utilisateur et en ajouter un autre.

## Copier un utilisateur pour en créer un nouveau

Vous pouvez créer un utilisateur en copiant un utilisateur existant.

>[!NOTE]
Lorsque vous créez un utilisateur de cette manière, toutes les informations sont copiées de l’utilisateur d’origine vers l’utilisateur nouvellement créé, à l’exception des informations suivantes :
* Informations de la section Informations personnelles .
* Lorsque je me connecte, affichez : L&#39;onglet d&#39;entrée par défaut pour le niveau d&#39;accès est sélectionné dans cette zone.
* Rapports directs
>


Pour créer un utilisateur en copiant un utilisateur existant :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Utilisateurs** ![](assets/users-icon-in-main-menu.png).
1. Sélectionnez l’utilisateur à copier, puis cliquez sur l’icône Copier . ![](assets/copy-icon.png).
1. Dans le **Nouvel utilisateur** qui s’affiche, modifiez les champs disponibles pour le nouvel utilisateur.

   Pour plus d’informations sur tous les champs associés à un utilisateur, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Cliquez sur **Ajouter Cet Utilisateur**.

   Ou

   Cliquez sur **Ajout d’un utilisateur et démarrage d’une autre personne** pour enregistrer le nouvel utilisateur et en ajouter un autre.

Un nouveau compte est ainsi créé dans Workfront pour l’utilisateur.

Si vous avez sélectionné l’option permettant d’envoyer une invitation à l’utilisateur, celui-ci doit recevoir un e-mail lui permettant de suivre un lien pour créer son mot de passe Workfront.

>[!NOTE]
Si votre entreprise a été intégrée au Admin Console et que vous ajoutez un utilisateur via Workfront, vous n’avez pas la possibilité d’envoyer une invitation par courrier électronique.
Les nouveaux utilisateurs d’Adobe sont ajoutés au Admin Console et le Admin Console leur envoie un courrier électronique pour les inviter à terminer le processus d’enregistrement. Tous les utilisateurs doivent terminer le processus d’enregistrement pour accéder à n’importe quel système d’Adobe.
Pour les utilisateurs d’Adobe existants, l’utilisateur peut recevoir ou non un e-mail sur la disponibilité de Workfront. Il s’agit d’une préférence contrôlée par l’administrateur d’Adobe pour le produit.
