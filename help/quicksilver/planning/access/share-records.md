---
title: Partager des enregistrements
description: Vous pouvez partager des enregistrements à l’aide du bouton Partager pour accroître la collaboration dans Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 0964ad24535bf43a23c740cd63abcf8fea705b8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 9%

---


<!--update metadata with real information at release-->

# Partager des enregistrements

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Vous pouvez ajuster les autorisations des utilisateurs aux enregistrements individuels dans un type d’enregistrement. O

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

* En tant que responsable d’espace de travail, vous pouvez partager un enregistrement avec un utilisateur qui ne fait pas partie de l’espace de travail. Dans ce cas, un avertissement s’affiche en regard de l’entité ajoutée pour l’informer qu’elle n’a pas accès à l’espace de travail. Vous pouvez accepter d’ajouter l’utilisateur à l’enregistrement et à l’espace de travail ou refuser de l’ajouter à l’espace de travail, ce qui le supprime également de l’enregistrement.

* Lorsque vous partagez un enregistrement avec des utilisateurs qui disposent d’autorisations de niveau Gérer pour l’espace de travail, ils disposent également d’autorisations de niveau Gérer pour l’enregistrement par défaut. L&#39;autorisation Afficher est grisée.

* Si vous ne disposez pas des autorisations nécessaires pour ajouter des personnes à l’espace de travail, vous verrez et ajouterez uniquement des utilisateurs, des équipes, des groupes, des rôles et des sociétés qui ont déjà été ajoutés à l’espace de travail. Vous ne pouvez pas ajouter d’autres entités qui ne font pas déjà partie de l’espace de travail.

* Vous pouvez désactiver les autorisations héritées pour un seul enregistrement, auquel cas vous pouvez leur accorder des autorisations individuelles, ou ils peuvent obtenir des autorisations s’ils appartiennent à l’option « Tout le monde dans l’espace de travail ». <!-- is this OK to say "workspace? should it be "record"??-->

* Si plusieurs autorisations de partage s’appliquent au même utilisateur ou à la même utilisatrice, il ou elle reçoit l’autorisation la plus élevée de ces autorisations.

  Par exemple, si un enregistrement est partagé avec un utilisateur disposant d&#39;autorisations d&#39;affichage et que son groupe dispose d&#39;un accès de niveau Gérer, il obtient des autorisations de niveau Gérer sur l&#39;enregistrement.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Si un champ de formule ou un champ de recherche d&#39;un enregistrement connecté est basé sur un champ d&#39;un enregistrement sur lequel vous n&#39;avez aucune autorisation, le calcul correct tient compte des facteurs de l&#39;enregistrement auxquels vous ne pouvez pas accéder autrement.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Autorisations de partage d’enregistrement

