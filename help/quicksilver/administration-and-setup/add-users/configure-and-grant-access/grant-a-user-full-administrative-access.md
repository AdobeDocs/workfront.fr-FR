---
title: Octroi d’un accès administratif complet à un utilisateur
description: Vous pouvez accorder aux utilisateurs et aux utilisatrices un accès administratif complet à Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: eb68357ed4fd8f323707aa4a54a0f946253bf4e0
workflow-type: tm+mt
source-wordcount: '1550'
ht-degree: 93%

---

# Accorder à un utilisateur ou à une utilisatrice un accès administratif complet

<!--Audited: 12/2024-->

>[!IMPORTANT]
>
>La procédure décrite sur cette page ne s’applique qu’aux entreprise qui n’ont pas encore été intégrées à l’Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, vous devez effectuer cette action via Adobe Admin Console.
>
>Pour obtenir des instructions sur l’octroi d’un accès administrateur complet dans Adobe Admin Console, voir [Gérer les utilisateurs dans Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Pour obtenir une liste des procédures qui diffèrent selon que votre organisation a été intégrée ou non à Adobe Admin Console, consultez la section [Différences d’administration en fonction de la plateforme (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

En tant que personne membre de l’administration Adobe Workfront, vous pouvez créer un autre administrateur ou une autre administratrice Workfront en lui attribuant un niveau d’accès administratif au système. Un utilisateur ou une utilisatrice ayant ce niveau d’accès dispose d’un accès administratif complet à tout ce qui se trouve dans Workfront, y compris aux éléments non créés par ses soins.

>[!NOTE]
>
>Cette approche diffère de l’utilisation d’un niveau d’accès pour accorder aux utilisateurs et aux utilisatrices des droits d’administration pour des sections spécifiques du système. Pour plus d’informations, consultez les sections suivantes :
>
>* [Accorder un accès administratif à certaines zones aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* Consulter dans cet article [Accès d’une personne membre de l’administration Workfront par rapport à l’accès d’un utilisateur ou d’une utilisatrice disposant d’une licence Plan et ayant des droits d’administration](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights)
>

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
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard</p>
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront. </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Accorder un accès administratif complet au système à un utilisateur ou à une utilisatrice unique

{{step-1-to-users}}

1. Cliquez sur le nom de l’utilisateur ou de l’utilisatrice à qui vous souhaitez accorder des droits d’administration.
1. Cliquez sur le ![](assets/more-icon.png) de menu **Plus** à droite du nom d’utilisateur, puis cliquez sur **Modifier**.

   La zone **Modifier la personne** s’affiche.
1. Cliquez sur **Accéder** dans le panneau de gauche.
1. Dans la liste déroulante **Niveau d&#39;accès**, sélectionnez le niveau d&#39;accès **Administrateur système**.

   En fonction des modifications apportées à votre système, le nom de ce niveau d’accès peut avoir changé.

1. Cliquez sur **Enregistrer les modifications.**

   L’utilisateur ou l’utilisatrice dispose désormais de tous les droits d’administration du système.

## Accès d’un administrateur ou d’une administratrice Workfront par rapport à l’accès d’un utilisateur ou d’une utilisatrice disposant d’une licence Plan et ayant des droits d’administration  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

Les deux tableaux ci-dessous montrent la différence entre les droits d’accès d’un utilisateur disposant d’un niveau d’accès d’administrateur système Workfront et ceux d’un utilisateur disposant d’une licence de plan avec certains droits d’administration.

Les administrateurs et les administratrices de Workfront peuvent visualiser tous les objets du système (quelle que soit la personne qui les a créés), en créer de nouveaux et modifier ou supprimer des objets existants. Un accès complet à tous les objets du système leur est accordé.

Les utilisateurs et les utilisatrices disposant d’une licence Plan qui peuvent modifier les fonctionnalités d’un domaine ont un accès complet aux fonctionnalités de ce domaine.

>[!NOTE]
>
>Les utilisateurs et les utilisatrices disposant d’une licence Plan qui font aussi partie de l’adiministration de groupes peuvent effectuer certaines des actions d’administration autorisées dans Workfront. Ces personnes sont autorisées à effectuer ces actions uniquement pour les groupes qu’elles administrent, leurs sous-groupes et les utilisateurs et utilisatrices de ces groupes et sous-groupes. Pour plus d’informations, consultez la section [Administrateurs et administrratrices de groupes](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Accès à la zone de configuration](#access-to-the-setup-area)
* [Accès aux objets](#access-to-objects)

### Accès à la zone de configuration {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Zone/objet</th> 
   <th>Administrateur ou administratrice Workfront </th> 
   <th>Utilisateur ou utilisatrice disposant d’une licence Plan et de certains droits d’administration</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Préférences du projet : projets</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Préférences du projet : tâches &amp; problèmes</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Préférences du projet : statuts</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès</p> </td> 
  </tr> 
  <tr> 
   <td>Préférences du projet : priorités</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Préférences du projet : gravités</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Préférences du projet : taux de change</td> 
   <td>Accès complet</td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>Processus : approbations</td> 
   <td> <p>Accès complet</p> </td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>Processus : chemins jalonnés</td> 
   <td>Accès complet</td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>Formulaires personnalisés</td> 
   <td>Accès complet</td> 
   <td> <p>Gérer les formulaires personnalisés créés par ces personnes ou les formulaires personnalisés partagés avec elles.</p> <p>Joindre les formulaires personnalisés qu’elles ont créés ou qui sont partagés avec elles à des objets pour lesquels elles ont des droits de gestion et de contribution.</p> </td> 
  </tr> 
  <tr> 
   <td>Corbeille : récemment supprimé</td> 
   <td>Accès complet</td> 
   <td> <p>Les utilisateurs et les utilisatrices qui sont aussi responsables de l’administration de groupes peuvent restaurer les projets assignés aux groupes dont la gestion leur est accordée, ainsi que les tâches, les problèmes ou les documents associés à ces projets.</p> </td> 
  </tr> 
  <tr> 
   <td>Corbeille : récemment restauré</td> 
   <td>Accès complet</td> 
   <td>Les utilisateurs et les utilisatrices qui sont aussi responsables de l’administration de groupes peuvent voir les éléments récemment restaurés par leur soins.</td> 
  </tr> 
  <tr> 
   <td>Fonctions</td> 
   <td>Accès complet</td> 
   <td> <p>Modifier les fonctions existantes mais pas les supprimer.</p> <p>Ajouter de nouvelles fonctions.</p> </td> 
  </tr> 
  <tr> 
   <td>Équipes</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès pour créer des équipes.</p> <p>Ajouter des équipes existantes aux utilisateurs et aux utilisatrices lors de la création ou de la modification d’utilisateurs et d’utilisatrices.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupes</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès à la création de groupes.</p> <p>Seuls les administrateurs et les administratrices de groupes peuvent gérer l’appartenance à un groupe, aux sous-groupes et les statuts au niveau du groupe pour les groupes dont la gestion leur est affectée. </p> </td> 
  </tr> 
  <tr> 
   <td>Entreprises</td> 
   <td>Accès complet</td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>Se connecter en tant que</td> 
   <td>Accès complet </td> 
   <td> <p>Si l’accès administratif de groupes des utilisateurs et des utilisatrices est activé à leur niveau d’accès et que la fonction d’administration de groupes leur est aussi affectée, la connexion en tant qu’utilisateurs ou utilisatrices du groupe administré et de ses sous-groupes leur est accordée. Par contre l’administration système ne leur est pas accordée.<br>Pour plus d’informations sur l’activation de l’accès administratif de groupes pour les utilisateurs et les utilisatrices, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et aux utilisatrices</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Planifications</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès à la modification des plannings.</p> <p>Accès à l’ajout de plannings existants à d’autres personnes, au niveau de l’utilisateur ou de l’utilisatrice. </p> </td> 
  </tr> 
  <tr> 
   <td>Feuille de temps et heures : profils de feuilles de temps</td> 
   <td>Accès complet</td> 
   <td> <p>Accès à l’attribution de profils de feuilles de temps existants aux utilisateurs et aux utilisatrices, au niveau de l’utilisateur ou de l’utilisatrice.</p> <p>Les utilisateurs et les utilisatrices qui ont la responsabilité de la gestion de groupes peuvent créer des profils de feuilles de temps pour les groupes administrés par leur soins et leurs sous-groupes. </p> </td> 
  </tr> 
  <tr> 
   <td>Feuille de temps et heures : types d’heures</td> 
   <td>Accès complet</td> 
   <td> <p>Accès à l’attribution de types d’heures aux utilisateurs ou aux utilisatrices, au niveau de l’utilisateur ou de l’utilisatrice.</p> </td> 
  </tr> 
  <tr> 
   <td>Feuille de temps et heures : préférences</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>E-mail : notifications : notifications d’événements</td> 
   <td>Activer/Désactiver tout</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>E-mail : notifications : notifications de rappel</td> 
   <td>Accès complet</td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>E-mail : notifications : modèles d’e-mails</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès à la modification des modèles d’e-mails.</p> <p>Accès à l’ajout de modèles d’e-mails existants aux notifications de rappel.</p> </td> 
  </tr> 
  <tr> 
   <td>E-mail : rappels automatiques</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>E-mail : invitations</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès à la modification des invitations par e-mail.</p> <p>L’accès au renvoi d’invitations par e-mail aux utilisateurs et aux utilisatrices dont l’enregistrement n’a pas été effectué, se fait uniquement à partir de l’onglet « Personnes ».</p> </td> 
  </tr> 
  <tr> 
   <td>E-mail : configuration</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès</p> </td> 
  </tr> 
  <tr> 
   <td>Cartes de score</td> 
   <td>Accès complet</td> 
   <td> <p>Accès complet</p> </td> 
  </tr> 
  <tr> 
   <td>Types de dépenses</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès</p> </td> 
  </tr> 
  <tr> 
   <td>Types de risques</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Niveaux d'accès</td> 
   <td> <p>Accès complet pour modifier tous les niveaux d’accès.</p> <p>Par défaut, les niveaux d’accès des membres de l’administration système et des utilisateurs et utilisatrices externes ne peuvent pas être modifiés.</p> </td> 
   <td> <p>Pas d’accès à la modification des niveaux d’accès.</p> <p>Attribuer aux autres utilisateurs et aux autres utilisatrices un niveau d’accès qui ne dépasse pas leur propre niveau.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : modèles de mise en page</td> 
   <td>Accès complet</td> 
   <td> <p>Accès à l’attribution de modèles de mise en page existants à d’autres utilisateurs et utilisatrices, au niveau de la personne. </p> <p>Les personnes désignées comme administrateurs ou administratrices de groupes peuvent créer des modèles de mise en page pour les groupes et les sous-groupes qu’elles gèrent.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : flux de mise à jour</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès à la modification des flux de mise à jour.</p> <p>Accès à l’ajout de champs à suivre dans les flux de mise à jour lors de la modification de formulaires personnalisés.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : filtres</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès à la création de filtres dans la zone de configuration.</p> <p>Accès à la création de nouveaux filtres dans une liste d’objets.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : vues</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès à la création de vues dans la zone de configuration.</p> <p>Accès à la création de nouvelles vues dans une liste d’objets.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : regroupements</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès à la création de regroupements dans la zone de configuration.</p> <p>Accès permettant de créer de nouveaux regroupements dans une liste d’objets.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface : contrôles de listes</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès</p> </td> 
  </tr> 
  <tr> 
   <td>Documents : fournisseurs cloud</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès à la configuration des fournisseurs cloud.</p> <p>Accès à la liaison de documents vers et depuis les fournisseurs cloud à partir de l’onglet Documents, une fois que les fournisseurs cloud ont été intégrés à Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents : mappage des métadonnées</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Documents : intégration SharePoint</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès à la configuration d’une intégration SharePoint.</p> <p>Accès à la liaison de documents vers et depuis SharePoint à partir de l’onglet Documents, après que l’intégration SharePoint avec Workfront ait été configurée.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents : intégration personnalisée</td> 
   <td>Accès complet</td> 
   <td> <p>Pas d’accès à la configuration d’une intégration personnalisée.</p> <p>Accès à la liaison de documents vers et depuis des fournisseurs tiers à partir de l’onglet Documents, une fois que les fournisseurs tiers ont été intégrés à Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Système : branding</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Système : Infos client</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Système : authentification unique (SSO)</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Système : mettre à jour les utilisateurs et utilisatrices pour SSO</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Système : Kickstart</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Système : diagnostics</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
  </tr> 
  <tr> 
   <td>Système : préférences</td> 
   <td>Accès complet</td> 
   <td>Pas d’accès</td> 
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
   <th>Administrateur ou administratrice Workfront </th> 
   <th>Utilisateur ou utilisatrice disposant d’une licence Plan et de certains droits d’administration</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendriers</td> 
   <td>Accès complet</td> 
   <td>Gérer les calendriers que les personnes créent et les calendriers partagés avec elles.</td> 
  </tr> 
  <tr> 
   <td>Tableaux de bord</td> 
   <td>Accès complet</td> 
   <td>Gérer les tableaux de bord que les personnes créent et les tableaux de bord partagés avec elles.</td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>Accès complet</td> 
   <td>Gérer les documents que les personnes chargent ou les documents partagés avec elles.</td> 
  </tr> 
  <tr> 
   <td>Problèmes</td> 
   <td>Accès complet</td> 
   <td>Gérer les problèmes que les personnes créent ou les problèmes partagés avec elles.</td> 
  </tr> 
  <tr> 
   <td>Portefeuilles</td> 
   <td>Accès complet</td> 
   <td>Gérer les portfolios que les personnes créent ou les portfolios partagés avec elles. </td> 
  </tr> 
  <tr> 
   <td>Programmes</td> 
   <td>Accès complet</td> 
   <td>Gérer les programmes que les personnes créent ou les programmes partagés avec elles.</td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Accès complet</td> 
   <td>Gérer les projets que les personnes créent ou les projets partagés avec elles.</td> 
  </tr> 
  <tr> 
   <td>Rapports</td> 
   <td>Accès complet</td> 
   <td>Gérer les rapports que les personnes créent ou les rapports partagés avec elles. Afficher, copier et modifier les rapports du système.</td> 
  </tr> 
  <tr> 
   <td>Tâches</td> 
   <td>Accès complet</td> 
   <td>Gérer les tâches que les personnes créent ou les tâches partagées avec elles.</td> 
  </tr> 
  <tr> 
   <td>Modèles</td> 
   <td>Accès complet</td> 
   <td>Gérer les modèles que les personnes créent ou les modèles partagés avec elles.</td> 
  </tr> 
  <tr> 
   <td>Feuilles de temps</td> 
   <td>Accès complet</td> 
   <td>Accès complet</td> 
  </tr> 
  <tr> 
   <td>Utilisateurs</td> 
   <td>Accès complet</td> 
   <td> <p>Accès limité</p> <p>Les groupes ne sont pas attribués à des personnes dont ils ne sont pas administrateurs ou administratrices de groupes ou à des groupes qui ne sont pas publics.</p> <p>Un niveau d’accès supérieur à leur propre niveau d’accès ne peut pas être attribué aux utilisateurs et aux utilisatrices.</p> <p>Si l’accès d’administration de groupes est activé pour leur niveau d’accès et que l’administration de groupes leur est attribuée pour un groupe, les droits de réinitialisation du mot de passe et de connexion des utilisateurs et des utilisatrices de ce groupe et de ses sous-groupes leur sont accordés La réinitialisation du mot de passe et la connexion en tant qu’administrateur ou administratrice système n’est pas disponible.<br>Pour plus d’informations sur l’activation de l’accès administratif de groupes pour les utilisateurs et les utilisatrices, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et aux utilisatrices</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
