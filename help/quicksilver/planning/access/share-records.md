---
title: Partager des enregistrements
description: Vous pouvez partager des enregistrements à l’aide du bouton Partager pour accroître la collaboration dans Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: e6fc6def1553df3faa8e1200f7ec2ca2bb97eb04
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 6%

---


<!--update metadata with real information at release-->

# Partager des enregistrements

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


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
* Lorsque vous partagez un espace de travail avec des utilisateurs, ils reçoivent également les mêmes autorisations pour les enregistrements de l’espace de travail, par défaut.
* Lorsque vous supprimez une entité d’un espace de travail, toutes les autorisations de partage sont supprimées des types d’enregistrements et de tous les enregistrements qu’elles contiennent.
* L’accès d’un utilisateur à l’enregistrement est déterminé par la combinaison des 3 paramètres suivants :

   * Leurs autorisations héritées du type d’enregistrement et de l’espace de travail
   * Autorisations ajoutées individuellement dans la boîte de dialogue de partage d’enregistrements
   * Les autorisations suivantes :

      * **Tout le monde dans l’espace de travail peut afficher** : l’enregistrement est ainsi visible par tous les utilisateurs dans l’espace de travail <!-- is this OK to say "workspace? should it be "record"??-->
      * **Seules les personnes invitées peuvent accéder à l&#39;enregistrement** : cette option est sélectionnée par défaut et permet de restreindre l&#39;accès à l&#39;enregistrement à des personnes spécifiques.

* Vous pouvez accorder les niveaux d’autorisation suivants à un enregistrement :

   * Afficher
   * Gérer

* Lorsque vous partagez un enregistrement avec un utilisateur, ils sont ajoutés avec la même autorisation que sur le type d’enregistrement, par défaut.

  Par exemple :

   * S’ils disposent des autorisations d’affichage sur le type d’enregistrement, ils obtiennent les autorisations d’affichage sur l’enregistrement
   * S’ils disposent des autorisations de niveau Contribution ou Gérer pour le type d’enregistrement, ils obtiennent des autorisations de niveau Gérer pour l’enregistrement

* En tant que responsable d’espace de travail, vous pouvez partager un enregistrement avec un utilisateur qui ne fait pas partie de l’espace de travail. Dans ce cas, un avertissement s’affiche en regard de l’entité ajoutée pour l’informer qu’elle n’a pas accès à l’espace de travail. Vous pouvez continuer à ajouter l’utilisateur à l’enregistrement, ce qui l’ajoutera également à l’espace de travail, ou arrêter de l’ajouter à l’enregistrement, ce qui ne l’ajoutera pas non plus à l’espace de travail.

* Lorsque vous partagez un enregistrement avec des utilisateurs qui disposent d’autorisations de niveau Gérer pour l’espace de travail, ils disposent également d’autorisations de niveau Gérer pour l’enregistrement par défaut. L&#39;autorisation Afficher est grisée.

* Si vous ne disposez pas des autorisations nécessaires pour ajouter des personnes à l’espace de travail, vous verrez et ajouterez uniquement des utilisateurs, des équipes, des groupes, des rôles et des sociétés qui ont déjà été ajoutés à l’espace de travail. Vous ne pouvez pas ajouter d’autres entités qui ne font pas déjà partie de l’espace de travail.

* Vous pouvez désactiver les autorisations héritées pour un seul enregistrement, auquel cas vous pouvez leur accorder des autorisations pour des enregistrements individuels, ou ils peuvent obtenir des autorisations s’ils appartiennent à l’option **Tout le monde dans l’espace de travail peut afficher**. <!-- is this OK to say "workspace? should it be "record"??-->

* Si plusieurs autorisations de partage s’appliquent au même utilisateur ou à la même utilisatrice, il ou elle reçoit l’autorisation la plus élevée de ces autorisations.

  Par exemple, si un enregistrement est partagé avec un utilisateur disposant d&#39;autorisations d&#39;affichage et que son groupe dispose d&#39;un accès de niveau Gérer, il obtient des autorisations de niveau Gérer sur l&#39;enregistrement.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Si un champ de formule ou un champ de recherche d&#39;un enregistrement connecté est basé sur un champ d&#39;un enregistrement sur lequel vous n&#39;avez aucune autorisation, le calcul correct tient compte des facteurs de l&#39;enregistrement auxquels vous ne pouvez pas accéder autrement.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Autorisations de partage d’enregistrement

Vous pouvez ajuster les autorisations sur des enregistrements individuels, si vous disposez de l’autorisation Gérer sur l’espace de travail.

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez partager les enregistrements.
1. Cliquez sur le type d’enregistrement dont vous souhaitez partager les enregistrements.

1. Utilisez l’une des méthodes suivantes :

   * En mode Tableau, pointez sur le nom d’un enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png), puis sur **Partager**.
   * Depuis n&#39;importe quel affichage, cliquez sur le nom d&#39;un enregistrement, puis cliquez sur **Partager** dans le coin supérieur droit de la page des détails de l&#39;enregistrement.

   La boîte **Partager** s’ouvre.

   ![Autorisations pour les enregistrements avec des autorisations héritées sur &#x200B;](assets/permissions-for-records-with-inherited-permissions-on.png)

1. (Facultatif) Dans la zone **Qui a accès**, l’option **Tout le monde dans l’espace de travail peut afficher** est sélectionnée par défaut.  Tous les utilisateurs disposant d’autorisations de niveau Affichage ou supérieur sur l’espace de travail et le type d’enregistrement peuvent afficher l’enregistrement.

1. (Facultatif) Cliquez sur le nombre d’utilisateurs sous l’option **Autorisations héritées** pour afficher les utilisateurs, les équipes, les groupes, les sociétés ou les fonctions qui héritent des autorisations de l’espace de travail.

   >[!TIP]
   >
   >Vous ne pouvez pas supprimer des entités individuelles de la liste des autorisations héritées.

1. (Facultatif et conditionnel) Si vous souhaitez partager le type d’enregistrement avec des entités spécifiques et leur donner un accès au type d’enregistrement différent de celui qu’elles ont déjà pour l’espace de travail, procédez comme suit :

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
   >* Si les utilisateurs disposent des autorisations de niveau Contribution ou Gérer sur l’espace de travail et le type d’enregistrement, ils conserveront les autorisations de niveau Gérer sur l’enregistrement. L&#39;autorisation Afficher est grisée
   >* Vous ne pouvez pas accorder aux utilisateurs une autorisation inférieure à l&#39;enregistrement s&#39;ils disposent de Contribute ou d&#39;une autorisation supérieure.
   > Pour plus d’informations, consultez la section [Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Pour permettre aux utilisateurs qui ne disposent pas des autorisations d’accès à l’espace de travail d’afficher un enregistrement, dans le champ **Accorder l’accès à cette vue**, commencez à saisir le nom d’un utilisateur, d’un groupe, d’une équipe, d’une entreprise ou d’une fonction, puis cliquez dessus lorsqu’il s’affiche dans la liste.

   L&#39;entité sélectionnée est ajoutée à l&#39;enregistrement et à l&#39;espace de travail avec les autorisations **Vue**.

   Les administrateurs système reçoivent toujours des autorisations de niveau Gérer pour les enregistrements partagés avec eux, et il existe une indication qu’un utilisateur est un administrateur système.

1. (Facultatif) Cliquez sur **Copier le lien** pour copier un lien vers l’enregistrement dans le presse-papiers et le partager avec d’autres personnes. Le lien ouvre la page des détails de l&#39;enregistrement.
1. Cliquer sur **Enregistrer**.

   L’enregistrement est maintenant partagé avec d’autres utilisateurs.
   <!--Checking with Lilit on this: The users you shared the record with receive both an in-app and email notification about having given permissions to the following entities:

   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them. -->

1. Partagez le lien copié avec d’autres personnes. Les utilisateurs et utilisatrices qui reçoivent le lien doivent être des utilisateurs et utilisatrices actifs et se connecter à Workfront pour pouvoir accéder à la page du type d’enregistrement et l’afficher dans la vue sélectionnée. Ils doivent disposer d’autorisations sur le type d’enregistrement pour pouvoir l’afficher. Pour plus d’informations, voir également [Partager des enregistrements à l’aide d’un lien](/help/quicksilver/planning/records/share-records.md).

## Supprimer des autorisations d’un enregistrement (**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B; CECI A ÉTÉ COPIÉ À PARTIR DES TYPES D’ENREGISTREMENTS, IL DOIT ÊTRE MODIFIÉ POUR LES ENREGISTREMENTS, MAIS ATTENDEZ LA RÉPONSE SLACK DE LA LISTE &#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**)

Vous pouvez supprimer les autorisations des utilisateurs d’un enregistrement. Cependant, ils conserveront au moins les autorisations d’affichage sur l’espace de travail d’enregistrement, qui leur donnent également au moins les autorisations d’affichage sur le type d’enregistrement. Vous devez supprimer leur accès de l’espace de travail si vous souhaitez qu’ils ne disposent d’aucune autorisation sur les types d’enregistrements de l’espace de travail.

{{step1-to-planning}}

1. Ouvrez l’espace de travail dont vous souhaitez arrêter le partage des types d’enregistrements, puis cliquez sur une carte de type d’enregistrement. Cela ouvre la page du type d’enregistrement.

1. Dans l’onglet d’un affichage, cliquez sur **Partager** dans le coin supérieur droit du type d’enregistrement.
1. Cliquez sur **Partager le type d’enregistrement**.

   La boîte **Partager** s’ouvre.
1. Recherchez l’utilisateur, le groupe, l’équipe, la société ou la fonction dont vous souhaitez supprimer les autorisations, développez le menu déroulant des autorisations à droite de leur nom, puis cliquez sur **Supprimer**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Option de suppression dans le menu déroulant Partage de type d’enregistrement](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Cliquer sur **Enregistrer**.

   Les personnes ne disposent plus des autorisations indiquées pour le type d’enregistrement. Toutefois, ils disposent toujours des autorisations pour l’espace de travail, sauf si vous les supprimez également des autorisations d’espace de travail.

   Les utilisateurs qui ont été supprimés de l’accès à l’affichage ne sont pas avertis qu’ils ne disposent plus de cet accès.
