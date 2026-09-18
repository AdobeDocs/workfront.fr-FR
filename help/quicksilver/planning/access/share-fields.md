---
title: Partager les champs de planification Workfront
description: Vous pouvez partager le champ d’un enregistrement Workfront Planning avec d’autres utilisateurs afin d’assurer la collaboration lors de l’utilisation d’Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: ac94936cc4dc9dc4f2d56b3f1221f71a405c5c65
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 4%
---

# Partager les champs de planification Workfront

{{planning-important-intro}}

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Une fois la version à prévisualiser, les mêmes fonctionnalités sont également disponibles tous les mois dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Vous pouvez partager le champ d’un enregistrement Workfront Planning avec d’autres utilisateurs afin d’assurer la collaboration lors de l’utilisation d’Adobe Workfront Planning.

Le partage de champ permet aux administrateurs de Workspace de contrôler l’accès à un champ individuel. Chaque champ d’un type d’enregistrement possède sa propre boîte de dialogue de partage dans laquelle l’accès peut être défini sur Aucun accès, Afficher les valeurs de champ ou Gérer les valeurs de champ.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout Workfront ou workflow avec un package Planning</p> 
Ou
<p>Tout package de produit autonome Workfront Planning</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Tous</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Planning</p></td> 
   <td><p>Tous</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Vous devez ajouter un workflow et un type de licence Planning au niveau d'accès lorsque vous disposez à la fois d'un workflow et d'un package Planning</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td><p>Gérer les autorisations sur un champ pour modifier les valeurs du champ</p>  
   <p>Autorisations de niveau Contribution ou supérieur à un type d’enregistrement pour hériter des autorisations de niveau Gérer pour le champ</p>  
   </td> 
  </tr>
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives au partage de champs

* Vous pouvez partager des champs avec des utilisateurs, des fonctions, des groupes, des équipes ou des sociétés.
* Vous ne pouvez partager des champs qu’à partir de la vue Tableau d’un type d’enregistrement.
* Les types de champs suivants ne peuvent pas être partagés :

  * Champs système (par exemple, Créé par, ID d’enregistrement)
  * Champs principaux
  * Champs de recherche. Ils héritent toujours des autorisations de leurs champs d’objet source.
* L’accès à un champ est obtenu en combinant les paramètres suivants :

  * **Autorisations héritées** : par défaut, un champ hérite du même accès qu’une personne dispose au type d’enregistrement. Vous pouvez désactiver les autorisations héritées et donner aux utilisateurs un accès au champ inférieur à celui dont ils disposent pour le type d’enregistrement.
  * La sélection **Toute personne ayant accès au type d’enregistrement peut afficher** ou **Seules les personnes invitées peuvent accéder**. Vous pouvez autoriser toutes les personnes disposant d’autorisations sur l’espace de travail à afficher le champ ou n’accorder des autorisations qu’à des entités individuelles.

  Si plusieurs règles s’appliquent à la même personne, elles reçoivent l’autorisation la plus élevée disponible de la part de l’une des règles.

* Pour rendre un champ en lecture seule accessible à tous dans un espace de travail, vérifiez que la configuration suivante existe :

  * Désactiver les autorisations héritées
  * Conservez le paramètre **Toute personne ayant accès au type d’enregistrement peut afficher**
  * N’ajoutez aucune entité individuelle.

* Selon les autorisations de type d’enregistrement, les utilisateurs peuvent recevoir les autorisations de champ suivantes :

  * Les autorisations de type d’enregistrement d’affichage permettent à un utilisateur d’afficher les valeurs de champ
  * Les autorisations de type Contribuer ou Gérer des enregistrements donnent à un utilisateur les autorisations de gérer les valeurs de champ

* Seuls les propriétaires et les responsables d’espace de travail peuvent ajuster les autorisations de champ. Les responsables Workspace conservent toujours un accès de niveau Gérer à tous les champs, une fonction qui ne peut pas être réduite.
* Le partage de champ contrôle l’accès aux valeurs, et non les paramètres de champ. Seuls les gestionnaires d’espace de travail peuvent modifier la configuration d’un champ.
* L’ajout d’une personne à la liste de partage d’un champ ne lui accorde pas d’accès à l’espace de travail ou de type enregistrement. S’il ne dispose pas de cet accès, une icône d’avertissement indique que l’autorisation ne prendra effet qu’une fois qu’il aura été ajouté au type d’enregistrement.
* Les champs avec des autorisations restreintes sont appliqués partout où le champ s’affiche. Cela inclut tous les affichages, les pages de détails des enregistrements, les formulaires de demande, les connexions et champs de recherche, les tableaux de bord de zone de travail, l’API et les outils de MCP.
* Les vues publiques restent entièrement visibles et en lecture seule pour toute personne qui peut y accéder.
  <!--Not sure if this is right - right now, it allows me to duplicate with the values in the new record - checking with Lilit: * When you duplicate a record, the restricted values are not copied to the new records.-->
* Les modifications de valeurs de champ restreintes ne sont pas enregistrées dans l’Historique d’un enregistrement.
* Les modifications des autorisations pour les champs ne déclenchent pas de notifications.
* Pour les types d’enregistrements globaux, les autorisations de champ s’appliquent à tous les espaces de travail secondaires et ne peuvent pas être ajustées localement.

<!--
From Claude: 
Additional permissions for fields - maybe add this to the Overview article for all of the sharing?? - help/quicksilver/planning/access/sharing-permissions-overview.md 

Here's how record type / workspace access maps to field-level access in the document:

Field permission levels (only two, plus none):

No Access – field is completely hidden
View field values – can see the value, can't edit
Manage field values – can view and edit

Default inheritance from record type role

Record type / workspace access    Default field permission
View    View field values
Contribute    Manage field values
Manage (workspace manager)    Manage field values (locked — cannot be reduced)

So by default, a field simply mirrors whatever role someone has on the record type — Viewers get read-only, Contributors and Managers get edit rights. Workspace managers are a special case: whenever they're added to a field's sharing list, "Manage field values" is pre-selected and the "View field values" option is disabled, since their edit access can never be taken away.

Wildcard (fallback) setting
Separate from inheritance, each field has a wildcard default:

Everyone in the workspace can view (default)
Only invited people can access

How the final permission is calculated

If inherited permissions are enabled: a person's access = the highest of (inherited from record type, wildcard, individually granted permission).
If inherited permissions are disabled: a person's access = the highest of (wildcard, individually granted permission) — record type role no longer factors in.
If inheritance is disabled, wildcard is "Only invited people can access," and the person isn't individually added → they get No Access.

Other permission notes

Individually granting access to someone doesn't grant them workspace/record-type access — it just sits inactive (with a warning icon) until they're separately added to the workspace.
For Global Record Types, field permissions are set once and apply to all secondary workspaces; secondary/team workspace managers cannot override them locally.

-->

## Champs de partage

En tant que responsable d’espace de travail, vous pouvez ajuster les autorisations sur des champs individuels.

{{step1-to-planning}}

1. Ouvrez l’espace de travail, puis le type d’enregistrement dont vous souhaitez partager les champs.

1. Dans la vue Tableau, passez la souris sur le nom de l’en-tête de colonne d’un champ, cliquez sur le menu **Plus** ![Menu Plus](assets/more-menu.png), puis cliquez sur **Partager le champ**.

   La boîte **Partager** s’ouvre.

1. (Facultatif) Dans la zone **Accorder l’accès**, l’option **Toute personne ayant accès au type d’enregistrement peut consulter** est sélectionnée par défaut. Tous les utilisateurs disposant d’autorisations d’**Affichage** ou supérieures pour l’espace de travail et le type d’enregistrement disposent des mêmes autorisations pour le champ .

1. (Facultatif) Cliquez sur les avatars d’utilisateurs sous l’option **Autorisations héritées de** pour afficher les utilisateurs, les équipes, les groupes, les sociétés ou les fonctions qui héritent des autorisations de l’espace de travail.

   Les autorisations de l’utilisateur sur le type d’enregistrement s’affichent lorsque vous développez les autorisations héritées.

   >[!TIP]
   >
   >Vous ne pouvez pas supprimer des entités individuelles de la liste des autorisations héritées. Les utilisateurs des équipes, des groupes, des sociétés ou des fonctions sont répertoriés au lieu des entités auxquelles ils étaient associés lorsque l’espace de travail et le type d’enregistrement ont été partagés avec eux.

1. (Facultatif et conditionnel) Si vous souhaitez partager le champ avec des entités spécifiques et leur donner un accès au champ différent de celui qu’elles ont déjà pour le type d’enregistrement, procédez comme suit :

   1. Désélectionnez l’option **Activé** dans **Autorisations héritées**. Elle est sélectionnée par défaut.

      L’option devient **Désactivé**.

      >[!TIP]
      >
      >Les responsables Workspace conservent les autorisations de niveau Gérer pour le type d’enregistrement et le champ.

   1. (Facultatif) Cliquez sur le menu déroulant **Toute personne ayant accès au type d’enregistrement peut afficher** et sélectionnez **Seules les personnes invitées peuvent accéder**.

      >[!IMPORTANT]
      >
      >Cette modification, ainsi que la désactivation des **autorisations héritées** suppriment l’accès pour toutes les personnes qui peuvent afficher le type d’enregistrement et ne donnent accès qu’aux personnes désignées. Les responsables et les administrateurs de Workspace auront toujours accès à tous les champs.


   1. Dans la zone **Accorder l’accès**, ajoutez les utilisateurs, équipes, groupes, sociétés ou fonctions auxquels vous souhaitez accorder un niveau d’autorisation différent de celui dont ils disposent pour l’espace de travail ou le type d’enregistrement.

      Lorsque vous partagez un champ avec un utilisateur, sa fonction principale et son adresse e-mail s’affichent également dans le champ. Le paramètre Afficher les informations de contact doit être activé pour que l’objet Utilisateurs de votre niveau d’accès puisse afficher l’e-mail de l’utilisateur.

   1. Sélectionnez l’un des niveaux d’autorisation suivants :

      * Afficher les valeurs des champs
      * Gérer les valeurs des champs

      >[!IMPORTANT]
      >
      ><!-- * If users have Contribute or Manage permissions to the workspace and the record type, you can give them Manage permissions to the field. The View permission is dimmed.-->
      >* Vous ne pouvez pas accorder aux utilisateurs une autorisation moindre sur le champ s&#39;ils disposent d&#39;une autorisation Contribute ou supérieure au type d&#39;enregistrement.
      >
      >* Vous ne pouvez pas accorder d’autorisations aux utilisateurs qui ne se trouvent pas dans l’espace de travail. Les utilisateurs qui ne disposent pas d’autorisations sur l’espace de travail et le type d’enregistrement ne peuvent accéder à aucun des champs. Ils pourront accéder aux champs lorsqu&#39;ils obtiendront des autorisations sur l&#39;espace de travail et les types d&#39;enregistrements.

1. Cliquer sur **Enregistrer**.

   Le champ est maintenant partagé avec d’autres utilisateurs.

   <!--
    Not possible for fields: 
    The users you shared the field with receive both an in-app and email notification about having been given permissions to the field.
    For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md).
    -->

## Supprimer les autorisations d’un champ

Vous pouvez supprimer les autorisations des utilisateurs d’un champ. Cependant, ils conserveront au moins les autorisations d’affichage pour l’espace de travail et le type d’enregistrement, ce qui leur donnera au moins les autorisations d’affichage pour le champ.

Vous devez supprimer leur accès de l’espace de travail si vous souhaitez qu’ils ne disposent d’aucune autorisation sur les types d’enregistrements ou les champs de l’espace de travail.

Vous ne pouvez pas supprimer un utilisateur des autorisations héritées.

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez arrêter le partage des champs, puis cliquez sur une carte de type enregistrement. La page du type d’enregistrement s’affiche.
1. Dans la vue Tableau, passez la souris sur le nom de l’en-tête de colonne d’un champ, cliquez sur le menu **Plus** ![Menu Plus](assets/more-menu.png), puis cliquez sur **Partager le champ**.

   La boîte **Partager** s’ouvre.
1. Recherchez l’utilisateur, le groupe, l’équipe, la société ou la fonction dont vous souhaitez supprimer les autorisations, développez le menu déroulant des autorisations à droite de leur nom, puis cliquez sur **Supprimer**.

1. Cliquer sur **Enregistrer**.

   Les personnes ne disposent plus des autorisations indiquées pour le champ . Cependant, ils disposent toujours des autorisations sur le type d’enregistrement et l’espace de travail, sauf si vous les supprimez également de ces autorisations.

   Les utilisateurs qui ont été supprimés de l’accès au champ ne reçoivent aucune notification indiquant qu’ils ne disposent plus de ces autorisations.
