---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Ajouter des utilisateurs
description: En tant qu’administrateur ou administratrice de Workfront ou personne disposant d’un accès administratif intégral, vous pouvez ajouter des utilisateurs et utilisatrices dans Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: c71c5c4a545f9256ecce123ae3513d01a7251ad7
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 75%

---

# Ajouter des utilisateurs

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>* **Vous devez créer des administrateurs système via Adobe Admin Console.**
>
>   Pour obtenir des instructions sur la création d’administrateurs système dans Adobe Admin Console, voir [Gérer les utilisateurs dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>   Les administrateurs de groupe peuvent utiliser cette procédure pour créer des utilisateurs et soumettre l’utilisateur pour approbation administrative.
>
>* **Si votre entreprise utilise l’authentification unique (SSO)** nous vous recommandons de créer des utilisateurs et de les affecter à Workfront dans Adobe Admin Console. La création de ces utilisateurs dans Workfront est possible, mais il peut y avoir des problèmes de transfert de ces informations vers Adobe Admin Console, en fonction de la configuration d’Admin Console dans votre organisation.
>  >   Après avoir créé l’utilisateur dans le Adobe Admin Console, vous pouvez configurer ses informations dans Workfront, telles que l’attribution de rôles, de groupes, d’équipes et de niveaux d’accès.
>* **Si votre entreprise n’utilise pas l’authentification unique (SSO)** vous pouvez ajouter des utilisateurs qui ne sont pas administrateurs système directement dans Workfront. Vous pouvez ajouter des utilisateurs et utilisatrices dans Adobe Admin Console, mais les ajouter dans Workfront permet de définir leur niveau d’accès lors de leur création, ce qui peut vous faire gagner du temps.



Vous pouvez ajouter des utilisateurs dans Adobe Workfront en créant des utilisateurs individuels à partir de zéro ou en copiant des utilisateurs existants.

Pour plus d’informations sur l’importation simultanée de plusieurs utilisateurs, voir [Importer des utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
—>

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
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant d’ajouter une personne, rassemblez les informations sur elle énumérées ci-dessous et déterminez les informations que vous souhaitez associer à cette personne :

* Quelles sont les informations personnelles de la personne ? Il vous faut au minimum les éléments suivants :

   * Nom complet
   * Nom d’utilisateur ou d’utilisatrice
   * Mot de passe par défaut
   * Adresse e-mail

  >[!NOTE]
  >
  >Vous pouvez déterminer si les personnes peuvent voir les coordonnées d’autres personnes en affinant le paramètre Vue utilisateurs et utilisatrices lors de la spécification des niveaux d’accès pour les objets Workfront. Pour plus d’informations, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Quelle est la position de la nouvelle personne au sein de l’entreprise ? Cette personne a-t-elle des personnes subordonnées directes ? À qui cette personne rend-elle compte ?
* Quelle est la fonction de la personne ? Cette fonction existe-t-elle dans Workfront ? Y a-t-il une limite au nombre de personnes pouvant occuper cette fonction ? Pour plus d’informations sur la création de fonctions, voir [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* Quel doit être le niveau d’accès de la personne ? Existe-t-il déjà ou faut-il en créer un ? Pour plus d’informations, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* Dans quel groupe principal cette personne doit-elle se trouver ? La personne doit-elle faire partie de plusieurs groupes ? Pour plus d’informations sur les groupes, voir [Vue d’ensemble des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* Dans quelle équipe interne cette personne doit-elle se trouver ? La personne doit-elle faire partie de plusieurs équipes ? Pour plus d’informations sur les équipes, voir [Vue d’ensemble des équipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Quelles informations personnalisées devez-vous associer à cette personne ?

  Si les informations sur les personnes sont capturées dans des champs personnalisés que vous avez créés, vous devez disposer d’un formulaire personnalisé lors de la création d’un utilisateur ou d’une utilisatrice. Pour plus d’informations sur les formulaires personnalisés, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Créer entièrement une personne

{{step-1-to-users}}

1. Cliquez sur **Nouvel utilisateur ou utilisatrice > Nouvel utilisateur ou utilisatrice** pour ajouter une nouvelle personne à Workfront.

   Ou

   Cliquez sur **Nouvel utilisateur ou utilisatrice > Importer des utilisateurs et utilisatrices** pour ajouter des personnes en chargeant un fichier d’import de feuille de calcul.

   Si vous importez des personnes, vous n’avez pas besoin de suivre ces étapes. Pour plus d’informations, voir [Importer des personnes](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. Dans la boîte **Nouvel utilisateur ou utilisatrice** qui s’affiche, cliquez sur **Afficher les options avancées**, puis configurez les options disponibles pour saisir les informations relatives à la personne.

   Pour plus d’informations sur ces options, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Utilisez l’une des méthodes suivantes :

   * Gardez l’option **Envoyer un e-mail d&#39;invitation à cette personne** activée. Dans ce cas, la personne reçoit un e-mail dans lequel elle peut suivre un lien pour créer son propre mot de passe pour Workfront. Les personnes qui n’acceptent pas l’invitation par e-mail et ne créent pas de mot de passe Workfront sont répertoriées comme non enregistrées dans Workfront.
   * Désactivez **Envoyez un e-mail d’invitation à cette personne**, puis saisissez un **Mot de passe** pour la personne et confirmez-le dans la boîte **Confirmer le mot de passe**. Vous devrez partager ce mot de passe avec la personne en dehors de Workfront.

   >[!NOTE]
   >
   >* Si votre administrateur ou administratrice de Workfront a activé une intégration SSO avec Workfront, le champ Autoriser l’authentification &lt;SSO Configuration> uniquement est masqué si vous désactivez l’invitation par e-mail. Le champ ID de fédération ou nom d’utilisateur ou d’utilisatrice &lt;SSO Configuration> reste visible.
   >
   >* Si votre organisation a été intégrée à Admin Console et que vous ajoutez une personne via Workfront, vous n’avez pas la possibilité d’envoyer une invitation par e-mail.
   >
   >   Pour les utilisateurs et utilisatrices d’Adobe existants, l’utilisateur ou l’utilisatrice peut recevoir ou non un e-mail sur la disponibilité de Workfront. Il s’agit d’une préférence contrôlée par l’administrateur ou l’administratrice d’Adobe pour le produit.

1. Cliquez sur **Ajouter cette personne**.

   Ou

   Cliquez sur **Ajouter une personne et en créer une autre** pour enregistrer la nouvelle personne et en ajouter un autre.

   >[!NOTE]
   >
   >* Si vous êtes un administrateur de groupes qui ajoute un utilisateur, les options de cette étape sont **Soumettre l’utilisateur à l’approbation de l’administrateur** et **Soumettre à approbation et en démarrer un autre**. L’utilisateur est créé avec le statut Désactivé et Approbation en attente .
   > 
   >* Si l’utilisateur ne quitte pas le statut Désactivé et Approbation en attente dans les minutes qui suivent, et qu’une actualisation d’écran ne supprime pas le badge Approbation en attente , vous pouvez approuver l’utilisateur manuellement.
   >
   >   1. Accédez à Configuration > Utilisateurs.
   >   1. Sélectionnez la ou les personnes dans la liste Utilisateurs et utilisatrices.
   >   1. Cliquez sur le menu à trois points dans l’en-tête de la liste.
   >   1. Sélectionnez **Approuver**.
   >   1. Après quelques minutes, actualisez la page.


## Copier une personne existante pour créer un nouvel utilisateur ou une nouvelle utilisatrice

Vous pouvez créer une personne en copiant une personne existante.

>[!NOTE]
>
>Lorsque vous créez une personne en procédant ainsi, toutes les informations sont copiées à partir de la personne d’origine vers la personne nouvellement créée, à l’exception des éléments suivants :
>
>* Les informations contenues dans la section « Informations personnelles ».
>* Lors de la connexion, l’onglet de destination par défaut pour le niveau d’accès.
>* Rapports directs
>

Pour créer une nouvelle personne en copiant une personne existante, procédez comme suit :

{{step-1-to-users}}

1. Sélectionnez l’utilisateur à copier, puis cliquez sur l’icône Copier ![icône Copier](assets/copy-icon.png).
1. Dans la boîte **Copier l’utilisateur ou l’utilisatrice** qui s’affiche, modifiez les champs disponibles pour la nouvelle personne.

   Pour plus d’informations sur tous les champs associés à une personne, voir [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Cliquez sur **Ajouter cette personne**.

   Ou

   Cliquez sur **Ajouter une personne et en créer une autre** pour enregistrer la nouvelle personne et en ajouter un autre.

Cela crée un nouveau compte dans Workfront pour l’utilisateur ou l’utilisatrice.

Si vous avez sélectionné l’option d&#39;envoi d’une invitation à la personne, celle-ci devrait recevoir un e-mail dans lequel elle pourra suivre un lien de création de mot de passe pour Workfront.

>[!NOTE]
>
>Si votre organisation a été intégrée à Admin Console et que vous ajoutez une personne via Workfront, vous n’avez pas la possibilité d’envoyer une invitation par e-mail.
>
>Pour les utilisateurs et utilisatrices d’Adobe existants, l’utilisateur ou l’utilisatrice peut recevoir ou non un e-mail sur la disponibilité de Workfront. Il s’agit d’une préférence contrôlée par l’administrateur ou l’administratrice d’Adobe pour le produit.
