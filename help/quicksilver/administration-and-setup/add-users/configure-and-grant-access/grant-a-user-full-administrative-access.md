---
title: Octroi d’un accès administratif complet à un utilisateur
description: Vous pouvez accorder aux utilisateurs un accès d’administration complet à Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 1%

---

# Octroi d’un accès administratif complet à un utilisateur

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées au Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, vous devez effectuer cette action via Adobe Admin Console.
>
>Pour obtenir des instructions sur l’octroi d’un accès administrateur complet dans Adobe Admin Console :
>
>* Voir [Création d’administrateurs système dans Workfront avec Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create2)
>* Consultez la section &quot;Modifier les détails de l’utilisateur&quot; de l’article [Gérer les utilisateurs individuellement](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) dans la documentation de Adobe Admin Console.
>* Contactez votre administrateur Adobe Admin Console.
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Admin Console, reportez-vous à la section [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

En tant qu’administrateur Adobe Workfront, vous pouvez créer un autre administrateur Workfront en lui affectant le niveau d’accès Administrateur système. Un utilisateur disposant de ce niveau d’accès dispose d’un accès d’administration complet à tous les éléments de Workfront, y compris les éléments qu’il n’a pas créés lui-même.

>[!NOTE]
>
>Cela diffère de l’utilisation d’un niveau d’accès pour accorder aux utilisateurs un accès administratif à certaines zones du système. Pour plus d’informations, voir :
>
>* [Octroi aux utilisateurs un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Accès d’un administrateur Workfront et accès d’un utilisateur Plan disposant de droits d’administration](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) dans cet article
>


## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td> <p>Vous devez être un administrateur Workfront. Pour plus d’informations, voir <a href="#" class="MCXref xref selected">Octroi d’un accès administratif complet à un utilisateur</a>.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Octroi d’un accès administrateur système complet à un utilisateur unique

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Utilisateurs** ![](assets/users-icon-in-main-menu.png).

1. Cliquez sur le nom de l’utilisateur auquel vous souhaitez accorder des droits d’administrateur.
1. Cliquez sur le menu Plus ![](assets/more-icon.png), puis cliquez sur **Modifier**.

1. Sur le **Modifier la personne** s’affiche, cliquez sur **Accès**.

1. Dans le **niveau d&#39;accès** , sélectionnez la liste déroulante **Administrateur système** niveau d’accès.

   Selon les modifications apportées à votre système, le nom de ce niveau d’accès peut avoir changé.

1. Cliquez sur **Enregistrez les modifications.**

   L’utilisateur dispose désormais de droits d’administrateur système complets dans le système.

## Accès d’un administrateur Workfront et accès d’un utilisateur Plan disposant de droits d’administration  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

Les deux tableaux ci-dessous montrent la différence entre les droits d’accès d’un utilisateur disposant d’un niveau d’accès administrateur Workfront et ceux d’un utilisateur disposant d’une licence Plan avec certains droits d’administration.

Les administrateurs de Workfront peuvent afficher tous les objets du système (indépendamment de l’utilisateur qui les a créés), en créer de nouveaux et modifier ou supprimer les objets existants. Ils disposent d’un accès complet à tous les objets du système.

Les utilisateurs disposant d’une licence Plan qui peuvent modifier les fonctionnalités d’une zone disposent d’un accès complet aux fonctionnalités de cette zone.

>[!NOTE]
>
>Les utilisateurs disposant d’une licence Plan qui sont désignés comme administrateurs de groupe peuvent effectuer certaines des actions autorisées pour les administrateurs Workfront. Ils sont autorisés à effectuer ces actions uniquement pour les groupes qu’ils administrent, leurs sous-groupes et les utilisateurs de ces groupes et sous-groupes. Pour plus d’informations, voir [Administrateurs de groupe](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Accès à la zone Configuration](#access-to-the-setup-area)
* [Accès aux objets](#access-to-objects)

### Accès à la zone Configuration {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zone/objet</th> 
   <th>Administrateur Workfront </th> 
   <th>Utilisateur avec une licence Plan et certains droits d’administration</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Préférences du projet : Projets</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Préférences du projet : Tâches et problèmes</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Préférences du projet : Statuts</td> 
   <td>Accès complet</td> 
   <td> <p>Accès interdit</p> </td> 
  </tr> 
  <tr> 
   <td>Préférences du projet : Priorités</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Préférences du projet : Gravités</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Préférences du projet : Taux de change</td> 
   <td>Accès complet</td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>Traitements : Approbations</td> 
   <td> <p>Accès complet</p> </td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>Traitements : Chemins Milestone</td> 
   <td>Accès complet</td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>Formulaires personnalisés</td> 
   <td>Accès complet</td> 
   <td> <p>Gérez les formulaires personnalisés qu’ils ont créés ou les formulaires personnalisés partagés avec eux.</p> <p>Joindre des formulaires personnalisés qu’ils ont créés ou des formulaires personnalisés partagés avec eux à des objets auxquels ils ont des autorisations de gestion ou de contribution.</p> </td> 
  </tr> 
  <tr> 
   <td>Corbeille : Récemment supprimés</td> 
   <td>Accès complet</td> 
   <td> <p>Les utilisateurs qui sont administrateurs de groupes peuvent restaurer les projets affectés aux groupes qu’ils gèrent, ainsi que les tâches, problèmes ou documents associés à ces projets.</p> </td> 
  </tr> 
  <tr> 
   <td>Corbeille : Récemment restaurés</td> 
   <td>Accès complet</td> 
   <td>Les utilisateurs qui sont des administrateurs de groupe peuvent voir les éléments qu’ils ont récemment restaurés.</td> 
  </tr> 
  <tr> 
   <td>Fonctions</td> 
   <td>Accès complet</td> 
   <td> <p>Modifiez mais ne supprimez pas les rôles de tâche existants.</p> <p>Ajoutez de nouveaux rôles de tâche.</p> </td> 
  </tr> 
  <tr> 
   <td>Équipes</td> 
   <td>Accès complet</td> 
   <td> <p>Accès interdit à la création d’équipes.</p> <p>Ajoutez des équipes existantes aux utilisateurs lors de la création ou de la modification d’utilisateurs.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupes</td> 
   <td>Accès complet</td> 
   <td> <p>Accès à la création de groupes.</p> <p>Seuls les administrateurs de groupe peuvent gérer l’appartenance à un groupe, les sous-groupes et les états au niveau du groupe pour les groupes qu’ils gèrent. </p> </td> 
  </tr> 
  <tr> 
   <td>Entreprises</td> 
   <td>Accès complet</td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>Connexion en tant que</td> 
   <td>Accès complet </td> 
   <td> <p>Si l’accès administratif de leur groupe est activé à son niveau d’accès et s’il est désigné comme administrateur de groupe, il peut se connecter en tant qu’utilisateurs du groupe qu’il administre et de leurs sous-groupes. Ils ne peuvent pas se connecter en tant qu’administrateur système.<br>Pour plus d’informations sur l’activation de l’accès administratif de groupe pour les utilisateurs, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Planifications</td> 
   <td>Accès complet</td> 
   <td> <p>Accès à la modification des planifications.</p> <p>Accès pour ajouter des plannings existants à d’autres utilisateurs, au niveau de l’utilisateur. </p> </td> 
  </tr> 
  <tr> 
   <td>Frise chronologique et heures : Profils de feuille de temps</td> 
   <td>Accès complet</td> 
   <td> <p>Accès pour affecter des profils de feuille de temps existants aux utilisateurs, au niveau de l’utilisateur.</p> <p>Les utilisateurs qui sont administrateurs de groupes peuvent créer des profils de feuille de temps pour les groupes qu’ils gèrent et leurs sous-groupes. </p> </td> 
  </tr> 
  <tr> 
   <td>Frise chronologique et heures : Types d’heure</td> 
   <td>Accès complet</td> 
   <td> <p>Accès pour attribuer des types d’heure aux utilisateurs, au niveau de l’utilisateur.</p> </td> 
  </tr> 
  <tr> 
   <td>Frise chronologique et heures : Préférences</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Email : Notifications : Notifications d’événement</td> 
   <td>Activer/Désactiver tout</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Email : Notifications : Notifications de rappel</td> 
   <td>Accès complet</td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>Email : Notifications : Modèles de courrier électronique</td> 
   <td>Accès complet</td> 
   <td> <p>Aucun accès pour modifier les modèles d’email.</p> <p>Accès pour ajouter des modèles de courrier électronique existants aux notifications de rappel.</p> </td> 
  </tr> 
  <tr> 
   <td>Email : Reminders automatiques</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Email : Invitations</td> 
   <td>Accès complet</td> 
   <td> <p>Accès à la modification des invitations par courrier électronique.</p> <p>Accès pour envoyer des invitations par courrier électronique à des utilisateurs non enregistrés uniquement à partir de l’onglet Personnes.</p> </td> 
  </tr> 
  <tr> 
   <td>Email : Configuration</td> 
   <td>Accès complet</td> 
   <td> <p>Accès interdit</p> </td> 
  </tr> 
  <tr> 
   <td>Cartes de score</td> 
   <td>Accès complet</td> 
   <td> <p>Accès complet</p> </td> 
  </tr> 
  <tr> 
   <td>Types de dépenses</td> 
   <td>Accès complet</td> 
   <td> <p>Accès interdit</p> </td> 
  </tr> 
  <tr> 
   <td>Types de risques</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Niveaux d'accès</td> 
   <td> <p>Accès complet pour modifier tous les niveaux d'accès.</p> <p>Par défaut, les niveaux d’accès Administrateur système et Utilisateur externe ne peuvent pas être modifiés.</p> </td> 
   <td> <p>Aucun accès pour modifier les niveaux d’accès.</p> <p>Attribuez un niveau d’accès à d’autres utilisateurs inférieur ou égal au leur au niveau de l’utilisateur.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : Modèles de mise en page</td> 
   <td>Accès complet</td> 
   <td> <p>Accès pour affecter des modèles de mise en page existants à d’autres utilisateurs, au niveau de l’utilisateur. </p> <p>Les utilisateurs désignés comme administrateurs de groupe peuvent créer des modèles de mise en page pour les groupes et les sous-groupes qu’ils gèrent.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : Mise à jour de flux</td> 
   <td>Accès complet</td> 
   <td> <p>Aucun accès pour modifier les flux de mise à jour.</p> <p>Accès à l’ajout de champs à suivre dans les flux de mise à jour lors de la modification du Forms personnalisé.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : Filtres</td> 
   <td>Accès complet</td> 
   <td> <p>Accès à la création de filtres dans la zone Configuration .</p> <p>Accès pour créer de nouveaux filtres dans une liste d’objets.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : Vues</td> 
   <td>Accès complet</td> 
   <td> <p>Aucun accès à la création d’affichages dans la zone Configuration.</p> <p>Accès pour créer de nouvelles vues dans une liste d’objets.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : Groupements</td> 
   <td>Accès complet</td> 
   <td> <p>Accès à la création de groupes dans la zone Configuration .</p> <p>Accès pour créer de nouveaux regroupements dans une liste d’objets.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : Contrôles de liste</td> 
   <td>Accès complet</td> 
   <td> <p>Accès interdit</p> </td> 
  </tr> 
  <tr> 
   <td>Documents : Fournisseurs cloud</td> 
   <td>Accès complet</td> 
   <td> <p>Aucun accès pour configurer les fournisseurs cloud.</p> <p>Accès aux documents vers et depuis l’onglet Documents pour les fournisseurs cloud après l’intégration des fournisseurs cloud à Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents : Mappage des métadonnées</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Documents : Intégration SharePoint</td> 
   <td>Accès complet</td> 
   <td> <p>Accès interdit pour configurer une intégration SharePoint.</p> <p>Accès aux documents vers et depuis SharePoint à partir de l’onglet Documents , une fois l’intégration de SharePoint à Workfront configurée.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents : Intégration personnalisée</td> 
   <td>Accès complet</td> 
   <td> <p>Aucun accès pour configurer une intégration personnalisée.</p> <p>Accès à des documents vers et depuis des fournisseurs tiers à partir de l’onglet Documents , une fois les fournisseurs tiers intégrés à Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Système : Marques</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Système : Informations sur le client</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Système : Authentification unique (SSO)</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Système : Mise à jour des utilisateurs pour SSO</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Système : Démarrages</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Système : Diagnostics</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
  <tr> 
   <td>Système : Préférences</td> 
   <td>Accès complet</td> 
   <td>Accès interdit</td> 
  </tr> 
 </tbody> 
</table>

### Accès aux objets {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zone/objet</th> 
   <th>Administrateur Workfront </th> 
   <th>Utilisateur avec une licence Plan et certains droits d’administration</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendriers</td> 
   <td>Accès complet</td> 
   <td>Gérez les calendriers qu’ils créent et les calendriers partagés avec eux.</td> 
  </tr> 
  <tr> 
   <td>Tableaux de bord</td> 
   <td>Accès complet</td> 
   <td>Gérez les tableaux de bord qu’ils créent et les tableaux de bord partagés avec eux.</td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>Accès complet</td> 
   <td>Gérez les documents qu’ils téléchargent ou les documents partagés avec eux.</td> 
  </tr> 
  <tr> 
   <td>Événements</td> 
   <td>Accès complet</td> 
   <td>Gérez les problèmes qu’ils créent ou les problèmes partagés avec eux.</td> 
  </tr> 
  <tr> 
   <td>Portefeuilles</td> 
   <td>Accès complet</td> 
   <td>Gérez les portefeuilles qu’ils créent ou les portefeuilles partagés avec eux. </td> 
  </tr> 
  <tr> 
   <td>Programmes</td> 
   <td>Accès complet</td> 
   <td>Gérez les programmes qu’ils créent ou les programmes partagés avec eux.</td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Accès complet</td> 
   <td>Gérez les projets qu’ils créent ou les projets partagés avec eux.</td> 
  </tr> 
  <tr> 
   <td>Rapports</td> 
   <td>Accès complet</td> 
   <td>Gérez les rapports qu’ils créent ou les rapports partagés avec eux. Affichez, copiez et modifiez les rapports système.</td> 
  </tr> 
  <tr> 
   <td>Tâches</td> 
   <td>Accès complet</td> 
   <td>Gérer les tâches qu’ils créent ou les tâches partagées avec</td> 
  </tr> 
  <tr> 
   <td>Modèles</td> 
   <td>Accès complet</td> 
   <td>Gérer les modèles qu’ils créent ou les modèles partagés avec eux</td> 
  </tr> 
  <tr> 
   <td>Feuilles de temps</td> 
   <td>Accès complet</td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>Utilisateurs</td> 
   <td>Accès complet</td> 
   <td> <p>Accès limité</p> <p>Ils ne peuvent pas affecter de groupes à des utilisateurs pour lesquels ils ne sont pas administrateurs de groupe ou à des groupes qui ne sont pas publics.</p> <p>Ils ne peuvent pas attribuer un niveau d’accès aux utilisateurs qui est supérieur à leur niveau d’accès.</p> <p>Si l’accès administratif de leur groupe est activé à son niveau d’accès et s’il est désigné comme administrateur de groupe dans un groupe, il peut réinitialiser le mot de passe et se connecter en tant qu’utilisateurs du groupe qu’il administre et de leurs sous-groupes. Ils ne peuvent pas réinitialiser le mot de passe ou se connecter en tant qu’administrateur système.<br>Pour plus d’informations sur l’activation de l’accès administratif de groupe pour les utilisateurs, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
