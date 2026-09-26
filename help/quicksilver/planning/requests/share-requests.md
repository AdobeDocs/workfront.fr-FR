---
title: Demandes de partage de Planning
description: Vous pouvez partager une demande Workfront Planning avec d’autres personnes après l’avoir soumise.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 3934b1b333f86c8c700617871bfaac23d2b19213
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 7%
---
# Demandes de partage de Planning

<!--add to TOC, and miniTOC-->

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Une fois la version à prévisualiser, les mêmes fonctionnalités sont également disponibles tous les mois dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Une fois la requête Planning soumise, vous pouvez contrôler qui la voit, qui peut y travailler et les actions que chaque personne ou équipe est autorisée à entreprendre. Cela permet aux bonnes personnes de se concentrer sur les bonnes requêtes et de s’assurer qu’elles ne peuvent prendre que les actions appropriées à leur rôle.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout Workfront ou workflow avec un package Planning</p> 
Ou
<p>Toute planification Workfront lors de l’achat en tant que produit autonome</p> 
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
   <td>   <p>Autorisations d’affichage ou supérieures pour un espace de travail et un type d’enregistrement, si vous êtes un utilisateur Workfront</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant le partage de requêtes

* Vous pouvez accorder les autorisations suivantes aux utilisateurs et utilisatrices pour une requête :

  * Afficher : les utilisateurs peuvent uniquement afficher la demande.
  * Contribution : les utilisateurs et utilisatrices peuvent afficher, modifier et commenter la demande.
  * Gérer : les utilisateurs et utilisatrices peuvent afficher, modifier, commenter et supprimer la demande.

* Les demandeurs se voient automatiquement attribuer un accès en gestion aux demandes qu’ils envoient, sauf si un administrateur a configuré une autre valeur par défaut.

  Pour plus d’informations, voir [Créer un formulaire de demande](/help/quicksilver/planning/requests/create-request-form.md).

* Les administrateurs et administratrices de Workfront peuvent accéder à toutes les demandes et les gérer.
* Les utilisateurs disposant d’un accès de niveau Gérer à un type d’enregistrement héritent d’un accès de niveau Gérer au formulaire de saisie de ce type d’enregistrement et à chaque demande soumise via celui-ci.
* Toute personne disposant d’autorisations sur une demande peut partager la demande avec le même niveau d’autorisation ou avec un niveau inférieur au sien.

  Les utilisateurs disposant d’autorisations de niveau Contribution ne peuvent pas accorder d’autorisations de niveau Gérer à la demande.

* Différentes personnes et équipes peuvent détenir différents niveaux d’accès sur la même requête.
* Les autorisations peuvent être attribuées par le biais de plusieurs entités. Si un utilisateur dispose des autorisations de niveau Contribution pour accéder à une demande, mais que son groupe ou sa fonction dispose des autorisations de niveau Affichage, il conserve le niveau d&#39;autorisation le plus élevé, à savoir Contribution.
* Les requêtes héritent des autorisations de l’espace de travail et du type d’enregistrement. Vous ne pouvez pas supprimer ni modifier les autorisations héritées pour les demandes Planning.

## Partage d’une requête

Assurez-vous d’utiliser la nouvelle expérience de requête.

1. {{step1-to-requests}}
1. Recherchez une demande Planning et cliquez dessus pour l&#39;ouvrir.
1. Cliquez sur **Partager**.

   La boîte de dialogue **Partager** s’ouvre pour la requête sélectionnée.

   ![Zone de partage des demandes](assets/requests-sharing-box.png)

1. Dans le champ **Accorder l’accès à cette demande**, commencez à saisir le nom d’un utilisateur, d’une équipe, d’un rôle, d’un groupe ou d’une entreprise et cliquez dessus lorsqu’il s’affiche dans la liste.

   Seules les entités actives s&#39;affichent dans la liste.
1. Dans le menu déroulant situé à droite du nom de chaque entité, sélectionnez l’un des niveaux d’autorisation suivants :

   * Gérer
   * Contribuer
   * Afficher
1. (Facultatif) Pour chaque niveau d’autorisation, cliquez sur l’icône d’autorisation granulaire et sélectionnez ou désélectionnez les autorisations granulaires, telles que **Modifier**, **Commenter**, **Partager** ou **Supprimer**.

   ![Autorisations granulaires sur les requêtes](assets/granular-permissions-on-requests.png)
1. (Facultatif) Développez la ligne Autorisations héritées pour voir qui obtient les autorisations de l’espace de travail et le type d’enregistrement.

   >[!TIP]
   >
   >Vous ne pouvez pas supprimer ni modifier les autorisations héritées pour les demandes Planning.

1. Cliquer sur **Enregistrer**.


   La demande est partagée avec les entités que vous avez sélectionnées.


