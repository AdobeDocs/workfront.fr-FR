---
title: Partager des enregistrements
description: Vous pouvez partager des enregistrements à l’aide du bouton Partager pour accroître la collaboration dans Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: ba5089fd02ca099d25ce0d3c2c2c039c2c6e2fe2
workflow-type: tm+mt
source-wordcount: '1772'
ht-degree: 5%

---


<!--update metadata with real information at release-->

# Partager des enregistrements

<!--this will NOT be available in Preview ever - find a way to add this in this article that is prominent-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Vous pouvez ajuster les autorisations des utilisateurs aux enregistrements individuels dans un type d’enregistrement.

Vous pouvez partager un enregistrement Adobe Workfront Planning de différentes manières :

* Partagez un lien vers l’enregistrement.

  Pour plus d’informations, voir [Partager des enregistrements à l’aide d’un lien](/help/quicksilver/planning/records/share-records.md).

* Partagez tous les enregistrements d’un espace de travail avec d’autres utilisateurs en partageant l’espace de travail et le type d’enregistrement.

  Pour plus d’informations, voir les articles suivants :

   * [Partager un espace de travail](/help/quicksilver/planning/access/share-workspaces.md)

   * [Partager un type d’enregistrement](/help/quicksilver/planning/access/share-record-types.md)

* Partagez un enregistrement à l’aide de l’option **Partager**.

  Cet article décrit comment partager un enregistrement avec d&#39;autres utilisateurs à l&#39;aide de l&#39;option **Partager**.

>[!IMPORTANT]
>
>Les utilisateurs ayant accès à un espace de travail obtiennent automatiquement au moins des autorisations d’affichage pour tous les enregistrements de l’espace de travail.
>Le partage de vues ne donne pas aux utilisateurs l’autorisation d’accéder aux enregistrements. Seuls les espaces de travail de partage peuvent accorder aux utilisateurs des autorisations sur les types d’enregistrements et les enregistrements.
>
>Pour obtenir des informations générales sur le partage d’objets dans Workfront Planning, consultez également la section [Présentation des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).


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
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>  <p>Gérer les autorisations d’un espace de travail, d’un type d’enregistrement et de l’enregistrement</p>  
   <p><b>IMPORTANT</b></p>
   <p>Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour un espace de travail peuvent partager un enregistrement</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> Les utilisateurs disposant d'une licence light ou contributor doivent se voir attribuer un modèle de mise en page incluant Planning.
   <p>Les zones Planning sont activées par défaut pour les utilisateurs standard et les administrateurs système.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant le partage d’enregistrements

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

<!--checking on the below with Lilit-->

* Vous pouvez partager des enregistrements avec les entités suivantes : personnes, groupes, équipes, entreprises ou fonctions.
* Vous pouvez accorder les niveaux d’autorisation suivants à un enregistrement :

   * Afficher
   * Gérer
* Lorsque vous partagez un espace de travail et un type d’enregistrement avec des utilisateurs, ils reçoivent également les mêmes autorisations pour les enregistrements de l’espace de travail, par défaut.
Lorsque les utilisateurs disposent des autorisations de niveau Contribution sur un espace de travail ou un type d’enregistrement, ils reçoivent des autorisations de niveau Gestion sur les enregistrements de ce type d’enregistrement.
* Lorsque vous supprimez une entité d’un espace de travail, toutes les autorisations de partage sont supprimées des types d’enregistrements et de tous les enregistrements qu’elles contiennent.
* L’accès d’un utilisateur à l’enregistrement est déterminé par la combinaison des 3 paramètres suivants :

   * Leurs autorisations héritées du type d’enregistrement et de l’espace de travail
   * Autorisations ajoutées individuellement dans la boîte de dialogue de partage d’enregistrements
   * Les autorisations suivantes :

      * **Tout le monde dans l’espace de travail peut afficher** : l’enregistrement est ainsi visible par tous les utilisateurs dans l’espace de travail <!-- is this OK to say "workspace? should it be "record"??-->
      * **Seules les personnes invitées peuvent accéder à l&#39;enregistrement** : cette option est sélectionnée par défaut et permet de restreindre l&#39;accès à l&#39;enregistrement à des personnes spécifiques.

     >[!NOTE]
     >
     >Si vous choisissez d’accorder l’autorisation **Tout le monde dans l’espace de travail peut afficher** à un type d’enregistrement ou à un enregistrement, toutes les personnes répertoriées dans la liste de partage des autorisations de l’espace de travail disposent des mêmes autorisations sur le type d’enregistrement et l’enregistrement, même si les autorisations héritées sont désactivées.


* Lorsque vous partagez un enregistrement avec un utilisateur, ils sont ajoutés avec la même autorisation que sur le type d’enregistrement, par défaut.

  Par exemple :

   * S’ils disposent des autorisations d’affichage sur le type d’enregistrement, ils obtiennent les autorisations d’affichage sur l’enregistrement
   * S’ils disposent des autorisations de niveau Contribution ou Gérer pour le type d’enregistrement, ils obtiennent des autorisations de niveau Gérer pour l’enregistrement

* En tant que responsable d’espace de travail, vous pouvez partager un enregistrement avec un utilisateur qui ne dispose pas d’autorisations sur le type d’enregistrement ou l’espace de travail. Dans ce cas, un avertissement s’affiche en regard de l’entité ajoutée pour l’informer qu’elle n’a pas accès à l’espace de travail ou au type d’enregistrement. <!--ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too--> Vous pouvez continuer à ajouter l’utilisateur à l’enregistrement, ce qui l’ajoutera également au type d’enregistrement et à l’espace de travail, ou annuler le partage.

* Lorsque l’utilisateur dispose des autorisations de niveau Gérer ou Contribuer pour l’espace de travail et le type d’enregistrement et que vous les ajoutez aux autorisations d’enregistrement, les autorisations d’affichage sont grisées. Ils conservent les mêmes autorisations pour l’enregistrement que pour le type d’enregistrement et vous ne pouvez pas leur accorder des autorisations inférieures pour l’enregistrement. <!--Lilit is checking on this, it is not working correctly-->

  Lorsqu’ils disposent des autorisations d’affichage sur l’espace de travail ou le type d’enregistrement, ils conservent les autorisations d’affichage sur les enregistrements. Vous pouvez leur accorder des autorisations de gestion pour l’enregistrement en désactivant les autorisations héritées et en sélectionnant le paramètre Seules les personnes invitées peuvent accéder . <!-- I think this is right, but because of the above not working, I can't test-->

<!-- not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.-->

* Vous pouvez désactiver les autorisations héritées pour un seul enregistrement, auquel cas vous pouvez leur accorder des autorisations pour des enregistrements individuels, ou ils peuvent obtenir des autorisations s’ils appartiennent à l’option **Tout le monde dans l’espace de travail peut afficher**.

* Si plusieurs autorisations de partage s’appliquent au même utilisateur ou à la même utilisatrice, il ou elle reçoit l’autorisation la plus élevée de ces autorisations.

  Par exemple, si un enregistrement est partagé avec un utilisateur disposant d&#39;autorisations d&#39;affichage et que son groupe dispose d&#39;un accès de niveau Gérer, il obtient des autorisations de niveau Gérer sur l&#39;enregistrement.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Si un champ de formule ou un champ de recherche d&#39;un enregistrement connecté est basé sur un champ d&#39;un enregistrement sur lequel vous n&#39;avez aucune autorisation, le calcul correct tient compte des facteurs de l&#39;enregistrement auxquels vous ne pouvez pas accéder autrement.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Autorisations de partage d’enregistrement

En tant que gestionnaire d’espace de travail, vous pouvez ajuster les autorisations aux enregistrements individuels.

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez partager les enregistrements.
1. Cliquez sur le type d’enregistrement dont vous souhaitez partager les enregistrements.

1. Utilisez l’une des méthodes suivantes :

   * En mode Tableau, pointez sur le nom d’un enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur **Partager**.
   * En mode Tableau, sélectionnez un enregistrement, puis cliquez sur **Partager** dans la barre d’outils bleue située en bas de la liste.
   * Depuis n&#39;importe quel affichage, cliquez sur le nom d&#39;un enregistrement, puis cliquez sur **Partager** dans le coin supérieur droit de la page des détails de l&#39;enregistrement.

   La boîte **Partager** s’ouvre.

   ![Autorisations pour les enregistrements avec des autorisations héritées sur &#x200B;](assets/permissions-for-records-with-inherited-permissions-on.png)

1. (Facultatif) Dans la zone **Qui a accès**, l’option **Tout le monde dans l’espace de travail peut afficher** est sélectionnée par défaut.  Tous les utilisateurs disposant d’autorisations **Vue** ou supérieures sur l’espace de travail et le type d’enregistrement disposent des mêmes autorisations sur l’enregistrement.

1. (Facultatif) Cliquez sur le nombre d’utilisateurs sous l’option **Autorisations héritées** pour afficher les utilisateurs, les équipes, les groupes, les sociétés ou les fonctions qui héritent des autorisations de l’espace de travail.

   >[!TIP]
   >
   >Vous ne pouvez pas supprimer des entités individuelles de la liste des autorisations héritées.

1. (Facultatif et conditionnel) Si vous souhaitez partager l’enregistrement avec des entités spécifiques et leur donner un accès au type d’enregistrement différent de celui qu’elles ont déjà pour l’espace de travail, procédez comme suit :

   1. Sélectionnez **Désactiver** dans le menu déroulant **Autorisations héritées**.

   >[!TIP]
   >
   >Les responsables Workspace conservent les autorisations de niveau Gérer pour le type d’enregistrement et l’enregistrement.

   1. (Facultatif) Sélectionnez **Seules les personnes invitées peuvent accéder** dans la zone **Qui a accès**.

   1. Dans le champ **Accorder l’accès à ce type d’enregistrement**, ajoutez les utilisateurs, équipes, groupes, sociétés ou fonctions auxquels vous souhaitez accorder un niveau d’autorisation différent de celui qu’ils ont pour l’espace de travail ou le type d’enregistrement.
   1. Sélectionnez l’un des niveaux d’autorisation suivants :

      * Afficher
      * Gérer

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* Outre les équipes, les groupes, les entreprises et les fonctions, vous ne pouvez partager qu’avec des utilisateurs qui ont été ajoutés au Adobe Admin Console. Vous ne pouvez pas ajouter des utilisateurs Workfront uniquement. Pour plus d’informations, voir [Gestion des utilisateurs dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
   >* Si les utilisateurs disposent des autorisations de niveau Contribution ou Gérer sur l’espace de travail et le type d’enregistrement, ils conserveront les autorisations de niveau Gérer sur l’enregistrement. L&#39;autorisation Afficher est grisée. <!--this is not dimmed at this time, Lilit to check-->
   >* Vous ne pouvez pas accorder aux utilisateurs une autorisation inférieure à l&#39;enregistrement s&#39;ils disposent d&#39;une autorisation Contribute ou supérieure au type d&#39;enregistrement.
   > Pour plus d’informations, consultez la section [Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Pour permettre aux utilisateurs qui ne disposent pas des autorisations d’accès à l’espace de travail d’afficher un enregistrement, dans le champ **Accorder l’accès à cette vue**, commencez à saisir le nom d’un utilisateur, d’un groupe, d’une équipe, d’une entreprise ou d’une fonction, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   L&#39;entité sélectionnée est ajoutée à l&#39;enregistrement, ainsi qu&#39;au type d&#39;enregistrement et à l&#39;espace de travail avec les autorisations **Vue**.

   Les administrateurs système reçoivent toujours des autorisations de niveau Gérer pour les enregistrements partagés avec eux, et il existe une indication qu’un utilisateur est un administrateur système.

1. (Facultatif) Cliquez sur **Copier le lien** pour copier un lien vers l’enregistrement dans le presse-papiers et le partager avec d’autres personnes. Le lien ouvre la page des détails de l&#39;enregistrement.
1. Cliquer sur **Enregistrer**.

   L’enregistrement est maintenant partagé avec d’autres utilisateurs.

   Les utilisateurs avec lesquels vous avez partagé l’enregistrement reçoivent à la fois une notification in-app et une notification par e-mail concernant l’octroi d’autorisations aux entités suivantes :

   * L&#39;enregistrement
   * Le type d’enregistrement, s’ils n’avaient jamais eu d’autorisations auparavant
   * L’espace de travail , s’ils n’avaient pas les autorisations sur l’espace de travail avant que l’enregistrement ne soit partagé avec eux.

   Pour plus d’informations, voir [Notifications Adobe Workfront Planning : index d’article](/help/quicksilver/planning/notifications/notifications-information.md).

1. Partagez le lien copié avec d’autres personnes. Les utilisateurs et utilisatrices qui reçoivent le lien doivent être des utilisateurs et utilisatrices actifs et se connecter à Workfront pour pouvoir accéder à la page du type d’enregistrement et l’afficher dans la vue sélectionnée. Ils doivent disposer d’autorisations sur le type d’enregistrement pour pouvoir l’afficher. Pour plus d’informations, voir également [Partager des enregistrements à l’aide d’un lien](/help/quicksilver/planning/records/share-records.md).

## Supprimer les autorisations d’un enregistrement

Vous pouvez supprimer les autorisations des utilisateurs d’un enregistrement. Cependant, ils conserveront au moins les autorisations d’affichage pour l’espace de travail, ce qui leur donnera également au moins des autorisations d’affichage pour le type d’enregistrement. Vous devez supprimer leur accès de l’espace de travail si vous souhaitez qu’ils ne disposent d’aucune autorisation sur les types d’enregistrements ou les enregistrements de l’espace de travail.

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez arrêter le partage des enregistrements, puis cliquez sur une carte de type d’enregistrement. Cela ouvre la page du type d’enregistrement.
1. Utilisez l’une des méthodes suivantes :

   * En mode Tableau, pointez sur le nom d’un enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur **Partager**.
   * En mode Tableau, sélectionnez un enregistrement, puis cliquez sur **Partager** dans la barre d’outils bleue située en bas de la liste.
   * Depuis n&#39;importe quel affichage, cliquez sur le nom d&#39;un enregistrement, puis cliquez sur **Partager** dans le coin supérieur droit de la page des détails de l&#39;enregistrement.

   La boîte **Partager** s’ouvre.
1. Recherchez l’utilisateur, le groupe, l’équipe, la société ou la fonction dont vous souhaitez supprimer les autorisations, développez le menu déroulant des autorisations à droite de leur nom, puis cliquez sur **Supprimer**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Supprimer des autorisations sur l’enregistrement](assets/remove-option-on-record-sharing-drop-down.png)

1. Cliquer sur **Enregistrer**.

   Les personnes ne disposent plus des autorisations indiquées pour l’enregistrement. Cependant, ils disposent toujours des autorisations sur le type d’enregistrement et l’espace de travail, sauf si vous les supprimez également de ces autorisations.

   Les utilisateurs qui ont été supprimés de l’accès à l’enregistrement ne sont pas avertis qu’ils ne disposent plus de ces autorisations.
