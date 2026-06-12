---
title: Partager des enregistrements
description: Vous pouvez partager des enregistrements à l’aide du bouton Partager pour accroître la collaboration dans Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 9ffad1aa-3c96-40fa-9c62-7a3e00699f18
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/NTytTWD-zq3PVhXn4n-GHinvQxna1wfnAXjaeYBgTEY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 95859f692efbd6ce12238cc03e23e1cecbd99956
workflow-type: tm+mt
source-wordcount: 1713
ht-degree: 8%

---

<!--update metadata with real information at release-->

# Partager des enregistrements

<!--
this will NOT be available in Preview ever - find a way to add this in this article that is prominent
-->

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>\
<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Vous pouvez ajuster les autorisations des utilisateurs aux enregistrements individuels dans un type d’enregistrement dans Adobe Workfront Planning.

Vous pouvez partager un enregistrement Adobe Workfront Planning de différentes manières :

* Partagez un lien vers l’enregistrement.

  Pour plus d’informations, voir [Partager des enregistrements à l’aide d’un lien](/help/quicksilver/planning/records/share-records.md).

* Partagez tous les enregistrements d’un espace de travail avec d’autres utilisateurs en partageant l’espace de travail et le type d’enregistrement.

  Pour plus d’informations, voir les articles suivants :

   * [Partager un espace de travail](/help/quicksilver/planning/access/share-workspaces.md)

   * [Partager un type d’enregistrement](/help/quicksilver/planning/access/share-record-types.md)

* Partagez un enregistrement individuel ou partagez plusieurs enregistrements en bloc à l’aide de l’option **Partager**.

  Cet article décrit comment partager des enregistrements avec d&#39;autres utilisateurs à l&#39;aide de l&#39;option **Partager**.

>[!IMPORTANT]
>
>* Les utilisateurs ayant accès à un espace de travail obtiennent automatiquement au moins des autorisations d’affichage pour tous les enregistrements de l’espace de travail.
>* Le partage de vues ne donne pas aux utilisateurs l’autorisation d’accéder aux enregistrements. Seuls les espaces de travail de partage peuvent accorder aux utilisateurs des autorisations sur les types d’enregistrements et les enregistrements.
>
>Pour obtenir des informations générales sur le partage d’objets dans Workfront Planning, consultez également la section [Présentation des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

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
<p>Tout package Workfront and Planning</p> 
Ou
<p>Tout package Workflow et Planning</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Tous</p> 
   <p><b>NOTE</b></p>
   <p>Seules les personnes disposant d’une licence Standard peuvent se voir accorder des autorisations de gestion des enregistrements. Toutes les autres licences ne peuvent avoir que des autorisations d’affichage et l’option Gérer est grisée pour celles-ci.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>  <p>Gérer les autorisations d’un espace de travail, d’un type d’enregistrement et de l’enregistrement</p>  
   <p><b>IMPORTANT</b></p>
   <p>Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour un espace de travail peuvent partager un enregistrement</p></td> 
  </tr>
</tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant le partage d’enregistrements

<!--
maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information
-->

<!--checking on the below with Lilit-->

* Vous pouvez partager des enregistrements avec les entités suivantes : personnes, groupes, équipes, entreprises ou fonctions.
* Les restrictions suivantes existent :

   * Impossible de partager plus de 100 enregistrements à la fois.
   * Vous ne pouvez pas partager d&#39;enregistrements avec plus de 100 entités.
* Si vous limitez les autorisations à un enregistrement, les utilisateurs ne verront plus cet enregistrement et les valeurs de ses champs de recherche où que ce soit dans le système où cet enregistrement s’affiche.
* Workfront vérifie les autorisations d’enregistrement dans les connexions jusqu’à 5 enregistrements, en s’assurant que les utilisateurs voient uniquement les enregistrements partagés avec eux.
* Vous pouvez accorder les niveaux d’autorisation suivants à un enregistrement :

   * Afficher
   * Gérer
* Lorsque vous partagez un espace de travail et un type d’enregistrement avec des utilisateurs, ils reçoivent également les mêmes autorisations pour les enregistrements de l’espace de travail, par défaut.
Lorsque les utilisateurs disposent des autorisations de niveau Contribution sur un espace de travail ou un type d’enregistrement, ils reçoivent des autorisations de niveau Gestion sur les enregistrements de ce type d’enregistrement.
* Lorsque vous supprimez une entité d’un espace de travail, toutes les autorisations de partage sont supprimées des types d’enregistrements et de tous les enregistrements qu’elles contiennent.
* Vous ne pouvez pas partager un enregistrement avec un utilisateur qui ne dispose pas d’autorisations sur l’espace de travail ou sur le type d’enregistrement.

  Si vous partagez un enregistrement avec une personne qui ne se trouve pas dans l’espace de travail, elle est automatiquement ajoutée à l’espace de travail.
* L’accès d’un utilisateur à l’enregistrement est déterminé par la combinaison des 3 paramètres suivants :

   * Leurs autorisations héritées du type d’enregistrement et de l’espace de travail
   * Autorisations ajoutées individuellement dans la zone de partage d’enregistrements
   * Le paramètre **Tout le monde peut voir** dans l’espace de travail.

     Ainsi, l’enregistrement est visible par tous dans l’espace de travail

     <!--
      Cannot do this on a record: 
      * **Only invited people can access**: This is selected by default and allows restricting access to the record to specific people. 
      -->

* Lorsque vous partagez un enregistrement avec un utilisateur, ils sont ajoutés avec la même autorisation que sur le type d’enregistrement, par défaut.

  Par exemple :

   * S’ils disposent des autorisations d’affichage sur le type d’enregistrement, ils obtiennent les autorisations d’affichage sur l’enregistrement
   * S’ils disposent des autorisations de niveau Contribution ou Gérer pour le type d’enregistrement, ils obtiennent des autorisations de niveau Gérer pour l’enregistrement

* Lorsque l’utilisateur dispose des autorisations de niveau Gérer ou Contribuer pour l’espace de travail et le type d’enregistrement et que vous les ajoutez aux autorisations d’enregistrement, les autorisations d’affichage sont grisées. Ils conservent les mêmes autorisations pour l’enregistrement que pour le type d’enregistrement et vous ne pouvez pas leur accorder des autorisations inférieures pour l’enregistrement.

* Vous pouvez désactiver les autorisations héritées pour un seul enregistrement, auquel cas vous pouvez donner à certains utilisateurs des autorisations pour des enregistrements individuels, ou ils peuvent obtenir des autorisations s’ils appartiennent à l’espace de travail, grâce à l’option **Tout le monde dans l’espace de travail peut afficher**.

* Si plusieurs autorisations de partage s’appliquent au même utilisateur ou à la même utilisatrice, ils ou elles reçoivent le niveau le plus élevé de ces autorisations.

  Par exemple, si un enregistrement est partagé avec un utilisateur disposant d&#39;autorisations d&#39;affichage et avec son groupe disposant d&#39;un accès de niveau Gérer, ce dernier reçoit des autorisations de niveau Gérer pour l&#39;enregistrement.

* Si un champ de formule ou un champ de recherche d&#39;un enregistrement connecté est basé sur un champ d&#39;un enregistrement sur lequel vous n&#39;avez aucune autorisation, le calcul correct tient compte des facteurs de l&#39;enregistrement auxquels vous ne pouvez pas accéder autrement.

  <!--
   Not possible: 
   * As a workspace manager, you can share a record with a user that does not have permissions to the record type or the workspace. In this case, there is a warning next to the added entity notifying you that they don't have access to the workspace or the record type.  You can continue adding the user to the record which will also add them to the record type and workspace, or cancel the sharing.
   -->

  <!--
   ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too
   -->

<!--
Lilit is checking on this, it is not working correctly
-->

<!--
   check on this: I cannot disable inherited permissions when this setting is ON and this documented in a TIP below: When they have View permissions to the workspace or the record type, they retain View permissions to the records. You can grant them Manage permissions to the record by disabling Inherited permissions and selecting the Only invited people can access setting.
   -->

<!-- 
   not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.
   -->

<!--
   Too granular??
   If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 
   If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions 
   -->

<!--
   not sure if any of the Share record types points might match here - ask Lilit??
   -->

## Partager des enregistrements

En tant que gestionnaire d’espace de travail, vous pouvez ajuster les autorisations aux enregistrements individuels.

{{step1-to-planning}}

1. Ouvrez l’espace de travail, puis le type d’enregistrement dont vous souhaitez partager les enregistrements.

1. Utilisez l’une des méthodes suivantes :

   * En mode Tableau, pointez sur le nom d’un enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur **Partager**.
   * En mode Tableau, sélectionnez un ou plusieurs enregistrements, puis cliquez sur **Partager** dans la barre d’outils bleue située en bas de la liste.
   * Depuis n&#39;importe quel affichage, cliquez sur le nom d&#39;un enregistrement, puis cliquez sur **Partager** dans le coin supérieur droit de la page des détails de l&#39;enregistrement.

   La boîte **Partager** s’ouvre.

   ![Autorisations pour les enregistrements avec des autorisations héritées sur &#x200B;](assets/permissions-for-records-with-inherited-permissions-on.png)

   >[!WARNING]
   >
   >Vous ne pouvez pas partager des autorisations sur des enregistrements ajoutés dans différents espaces de travail. Lorsque vous partagez des enregistrements en bloc, les enregistrements doivent tous être créés dans le même espace de travail.

1. (Facultatif) Dans la zone **Qui a accès**, l’option **Tout le monde dans l’espace de travail peut afficher** est sélectionnée par défaut.  Tous les utilisateurs disposant d’autorisations **Vue** ou supérieures sur l’espace de travail et le type d’enregistrement disposent des mêmes autorisations sur l’enregistrement.

1. (Facultatif) Cliquez sur les avatars d’utilisateurs sous l’option **Autorisations héritées de** pour afficher les utilisateurs, les équipes, les groupes, les sociétés ou les fonctions qui héritent des autorisations de l’espace de travail. <!--logged bug to move "Permissions" to lowercase-->

   Les autorisations de l’utilisateur sur le type d’enregistrement s’affichent lorsque vous développez les autorisations héritées.

   >[!TIP]
   >
   >Vous ne pouvez pas supprimer des entités individuelles de la liste des autorisations héritées. Les utilisateurs des équipes, des groupes, des sociétés ou des fonctions sont répertoriés au lieu des entités auxquelles ils étaient associés lorsque l’espace de travail et le type d’enregistrement ont été partagés avec eux.

1. (Facultatif et conditionnel) Si vous souhaitez partager l’enregistrement avec des entités spécifiques et leur donner un accès au type d’enregistrement différent de celui qu’elles ont déjà pour l’espace de travail, procédez comme suit :

   1. Désélectionnez l’option **Activé** dans **Autorisations héritées**. Elle est sélectionnée par défaut.

      L’option devient **Désactivé**.

      >[!TIP]
      >
      >Les responsables Workspace et les créateurs d’enregistrements disposent toujours des autorisations de niveau Gérer pour le type d’enregistrement et l’enregistrement.

      <!-- 
      This is no longer possible for a record: 
      (Optional) Select **Only invited people can access** from the **Who has access** area. You must indicate individual users, groups, teams, or companies to share the records with. 
      >[!TIP]
      >
      >You cannot disable or enable Inherited permissions when this setting is selected.
      -->

   1. Dans le champ **Accorder l’accès à cet enregistrement**, ajoutez les utilisateurs, équipes, groupes, sociétés ou fonctions auxquels vous souhaitez accorder un niveau d’autorisation différent de celui dont ils disposent pour l’espace de travail ou le type d’enregistrement.

      Lorsque vous partagez un enregistrement avec un utilisateur, sa fonction principale et son adresse e-mail s’affichent également dans le champ. Le paramètre Afficher les informations de contact doit être activé pour que l’objet Utilisateurs de votre niveau d’accès puisse afficher l’e-mail de l’utilisateur.

   1. Sélectionnez l’un des niveaux d’autorisation suivants :

      * Afficher
      * Gérer

      >[!IMPORTANT]
      >
      >* Si les utilisateurs disposent des autorisations de niveau Contribution ou Gérer sur l’espace de travail et le type d’enregistrement, vous pouvez leur accorder des autorisations de niveau Gérer sur l’enregistrement. L&#39;autorisation Afficher est grisée.
      >* Vous ne pouvez pas accorder aux utilisateurs une autorisation inférieure à l&#39;enregistrement s&#39;ils disposent d&#39;une autorisation Contribute ou supérieure au type d&#39;enregistrement.
      >Pour plus d’informations, consultez la section [Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
      >* Vous ne pouvez pas accorder d’autorisations aux utilisateurs qui ne se trouvent pas dans l’espace de travail. Les utilisateurs qui ne disposent pas d’autorisations sur l’espace de travail et le type d’enregistrement ne peuvent accéder à aucun des enregistrements.

   <!--   
   Not possible:
   1. To give users who do not have permissions to the workspace access to view a record, in the **Grant access to this view** field, start typing the name of a user, a group, team, company, or job role, then click it when it displays in the list. 
      The entity you selected is added to the record and also to the record type and the workspace with **View** permissions. 
      System administrators always receive Manage permissions to records shared with them, and there is an indication that a user is a System administrator.
   -->

1. (Facultatif) Cliquez sur **Copier le lien** pour copier un lien vers l’enregistrement dans le presse-papiers et le partager avec d’autres personnes. Le lien ouvre la page des détails de l&#39;enregistrement.
1. Cliquer sur **Enregistrer**.

   L’enregistrement est maintenant partagé avec d’autres utilisateurs.

   Les utilisateurs avec lesquels vous avez partagé l’enregistrement reçoivent à la fois une notification in-app et une notification par e-mail concernant l’octroi d’autorisations pour l’enregistrement.

   <!--
   not possible anymore: 
   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them.
   -->

   Pour plus d’informations, voir [Notifications Adobe Workfront Planning : index d’article](/help/quicksilver/planning/notifications/notifications-information.md).


1. (Facultatif) Partagez le lien copié avec d’autres personnes.

   Les utilisateurs et utilisatrices qui reçoivent le lien doivent être des utilisateurs et utilisatrices actifs et se connecter à Workfront pour pouvoir accéder à la page du type d’enregistrement et l’afficher dans la vue sélectionnée.

   Ils doivent disposer d’autorisations sur le type d’enregistrement pour pouvoir l’afficher.

   Pour plus d’informations, voir également [Partager des enregistrements à l’aide d’un lien](/help/quicksilver/planning/records/share-records.md).


## Supprimer les autorisations d’un enregistrement

Vous pouvez supprimer les autorisations des utilisateurs d’un enregistrement. Cependant, ils conserveront au moins les autorisations d’affichage pour l’espace de travail, ce qui leur donnera également au moins des autorisations d’affichage pour le type d’enregistrement.

Vous devez supprimer leur accès de l’espace de travail si vous souhaitez qu’ils ne disposent d’aucune autorisation sur les types d’enregistrements ou les enregistrements de l’espace de travail.

Vous ne pouvez pas supprimer un utilisateur des autorisations héritées.

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez arrêter le partage des enregistrements, puis cliquez sur une carte de type d’enregistrement. Cela ouvre la page du type d’enregistrement.
1. Utilisez l’une des méthodes suivantes :

   * En mode Tableau, pointez sur le nom d’un enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur **Partager**.
   * Dans la vue Tableau, sélectionnez un ou plusieurs enregistrements, puis cliquez sur **Partager** dans la barre d’outils bleue en bas de la liste.

     Vous devez sélectionner les enregistrements qui ont été créés dans le même espace de travail.
   * Depuis n&#39;importe quel affichage, cliquez sur le nom d&#39;un enregistrement, puis cliquez sur **Partager** dans le coin supérieur droit de la page des détails de l&#39;enregistrement.

   La boîte **Partager** s’ouvre.
1. Recherchez l’utilisateur, le groupe, l’équipe, la société ou la fonction dont vous souhaitez supprimer les autorisations, développez le menu déroulant des autorisations à droite de leur nom, puis cliquez sur **Supprimer**.

   ![Supprimer des autorisations sur l’enregistrement](assets/remove-option-on-record-sharing-drop-down.png)

1. Cliquer sur **Enregistrer**.

   Les personnes ne disposent plus des autorisations indiquées pour l’enregistrement. Cependant, ils disposent toujours des autorisations sur le type d’enregistrement et l’espace de travail, sauf si vous les supprimez également de ces autorisations.

   Les utilisateurs qui ont été supprimés de l’accès à l’enregistrement ne sont pas avertis qu’ils ne disposent plus de ces autorisations.
