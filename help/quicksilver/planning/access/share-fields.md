---
title: Partager les champs de planification Workfront
description: Vous pouvez partager le champ d’un enregistrement Workfront Planning avec d’autres utilisateurs afin d’assurer la collaboration lors de l’utilisation d’Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 2d26437c69b3c36366938952d426532934f55c52
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 3%

---


# Partager les champs de planification Workfront

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

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
* L’accès à un champ est obtenu en combinant les paramètres suivants :

  * **Autorisations héritées** : par défaut, un champ hérite du même accès qu’une personne sur le type d’enregistrement (les autorisations de type Afficher un enregistrement donnent à un utilisateur les autorisations d’afficher les valeurs de champ ; les autorisations de type Contribuer ou Gérer un enregistrement donnent à un utilisateur les autorisations de gérer les valeurs de champ). Vous pouvez désactiver les autorisations héritées et donner aux utilisateurs un accès au champ inférieur à celui dont ils disposent pour le type d’enregistrement.
  * La sélection **Tout le monde dans l’espace de travail peut afficher** ou **Seules les personnes invitées peuvent accéder**. Vous pouvez autoriser toutes les personnes disposant d’autorisations sur l’espace de travail à afficher le champ ou n’accorder des autorisations qu’à des entités individuelles.

  Si plusieurs règles s’appliquent à la même personne, elles reçoivent l’autorisation la plus élevée disponible de la part de l’une des règles.

* Seuls les propriétaires et les responsables d’espace de travail peuvent ajuster les autorisations de champ. Les responsables d’espace de travail conservent toujours un accès de niveau Gérer à tous les champs. Ceci ne peut pas être réduit.
* Le partage de champ contrôle l’accès aux valeurs, et non les paramètres de champ. Seuls les gestionnaires d’espace de travail peuvent modifier la configuration d’un champ.
* L’ajout d’une personne à la liste de partage d’un champ ne lui accorde pas d’accès à l’espace de travail ou de type enregistrement. S’il ne dispose pas de cet accès, une icône d’avertissement indique que l’autorisation ne prendra effet qu’une fois qu’il aura été ajouté au type d’enregistrement.
* Les champs système (par exemple, Créé par, ID d’enregistrement) et les champs principaux ne peuvent pas faire l’objet d’un partage limité.
* Les champs restreints sont appliqués partout où le champ s’affiche. Cela inclut tous les affichages, les pages de détails des enregistrements, les formulaires de demande, les connexions et champs de recherche, les tableaux de bord de zone de travail, l’API et les outils de MCP.
* Les champs de recherche héritent des autorisations de leur champ source.
* Les vues publiques restent entièrement visibles et en lecture seule pour toute personne qui peut y accéder.
* Lorsque vous dupliquez un enregistrement, les valeurs restreintes ne sont pas copiées dans les nouveaux enregistrements.
* Les modifications de valeurs de champ restreintes ne sont pas enregistrées dans l’Historique d’un enregistrement.
* Les modifications des autorisations pour les champs ne déclenchent pas de notifications.
* Pour les types d’enregistrements globaux, les autorisations de champ s’appliquent à tous les espaces de travail secondaires et ne peuvent pas être ajustées localement.


De Claude :
Autorisations supplémentaires pour les champs : ajoutez éventuellement ceci à l’article Présentation pour l’ensemble du partage?? - help/quicksilver/planning/access/sharing-permissions-overview.md

Voici comment le type d’enregistrement/l’accès à l’espace de travail mappe à l’accès au niveau du champ dans le document :

Niveaux d&#39;autorisation de champ (deux seulement, plus aucun) :

Aucun accès - le champ est complètement masqué
Afficher les valeurs de champ : peut voir la valeur, ne peut pas la modifier
Gérer les valeurs de champ : peut afficher et modifier.

Héritage par défaut à partir du rôle de type d’enregistrement

Type d’enregistrement/accès à l’espace de travail Autorisation de champ par défaut
Afficher les valeurs de champ
Valeurs de champ Gérer de Contribute
Gérer (gestionnaire d’espace de travail) Gérer les valeurs de champ (verrouillé — ne peut pas être réduit)

Par défaut, un champ reflète simplement le rôle que quelqu’un a dans le type d’enregistrement : les observateurs sont en lecture seule, les contributeurs et les responsables ont des droits de modification. Les gestionnaires de Workspace constituent un cas particulier : lorsqu&#39;ils sont ajoutés à la liste de partage d&#39;un champ, l&#39;option « Gérer les valeurs de champ » est présélectionnée et l&#39;option « Afficher les valeurs de champ » est désactivée, car leur accès en modification ne peut jamais être supprimé.

Paramètre de caractère générique (secours)
En dehors de l’héritage, chaque champ comporte une valeur par défaut sous forme de caractère générique :

Tout le monde dans l’espace de travail peut afficher (par défaut)
Accessible par les personnes invitées uniquement

Méthode de calcul de l’autorisation finale

Si les autorisations héritées sont activées : accès d’une personne = le plus élevé de (hérité du type d’enregistrement, caractère générique, autorisation accordée individuellement).
Si les autorisations héritées sont désactivées : accès d’une personne = le plus élevé de (caractère générique, autorisation accordée individuellement) - le rôle de type d’enregistrement n’est plus pris en compte.
Si l’héritage est désactivé, le caractère générique est « Seules les personnes invitées peuvent accéder à » et la personne n’est pas ajoutée individuellement → elle n’a pas accès.

Autres notes d’autorisation

Accorder individuellement l’accès à une personne ne lui accorde pas l’accès de type espace de travail/enregistrement . Celui-ci reste simplement inactif (avec une icône d’avertissement) jusqu’à ce qu’elle soit ajoutée séparément à l’espace de travail.
Pour les types d’enregistrements globaux, les autorisations sur les champs sont définies une fois et s’appliquent à tous les espaces de travail secondaires. Les responsables des espaces de travail secondaires/d’équipe ne peuvent pas les remplacer localement.

## Champs de partage

