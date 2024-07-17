---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Actions autorisées pour différents types d’administrateurs
description: Ce tableau compare les activités d’administration disponibles pour un administrateur Adobe Workfront gérant le système Workfront, un administrateur de groupe gérant un groupe de niveau supérieur et un administrateur de groupe gérant un sous-groupe.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f556aa0b-71c5-48a9-8a84-72f1fbb2c86e
source-git-commit: 9dcd8dbe0474bdbb1fd50bb1f2525e03cd350559
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 16%

---

# Actions autorisées pour les administrateurs de groupe

Ce tableau répertorie les activités d’administration disponibles pour :

* Un administrateur Adobe Workfront gérant le système Workfront (pour les comparaisons)
* Administrateur de groupe gérant un groupe de niveau supérieur
* Un administrateur de groupe gérant un sous-groupe

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>Administrateur Workfront </th> 
   <th>Administrateur de groupe (les actions sont limitées aux groupes gérés par l’administrateur)</th> 
   <th>Administrateur de sous-groupe (les actions sont limitées aux groupes gérés par l’administrateur)</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td>Réinitialisation du mot de passe d’un utilisateur</td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Création et modification de profils utilisateur</td> 
   <td>✓</td> 
   <td>✓*</td> 
   <td>✓*</td> 
  </tr> 
  <tr> 
   <td>Créer et gérer des sous-groupes</td>
   <td>✓ </td> 
   <td>✓***</td> 
   <td>✓***</td> 
  </tr> 
  <tr> 
   <td>Configuration des préférences de projet, de tâche et de problème au niveau du système</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Activer et désactiver les préférences de projet, de tâche et d’émission pour les groupes et les sous-groupes</td> 
   <td>✓***</td> 
   <td>✓***</td> 
   <td>✓***</td> 
  </tr> 
  <tr> 
   <td>Configuration des préférences de feuille de temps et d’heure au niveau du système</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Activation et désactivation des préférences de feuille de temps et d’heure pour les groupes et les sous-groupes </td> 
   <td>✓***</td> 
   <td>✓***</td> 
   <td>✓***</td> 
  </tr> 
  <tr> 
   <td>Configuration des emails de notification d’événement au niveau du système</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Activer et désactiver les emails de notification d’événement pour les groupes et les sous-groupes</td> 
   <td>✓*** </td> 
   <td>✓***</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Créer et gérer des formulaires personnalisés</td> 
   <td>✓ </td> 
   <td>✓**</td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td>Créer et gérer des modèles de disposition</td> 
   <td>✓ </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Créer et gérer des processus d’approbation pour un groupe</td> 
   <td>✓*** </td> 
   <td>✓***</td> 
   <td>✓***</td> 
  </tr> 
  <tr> 
   <td>Créer et gérer des équipes</td> 
   <td>✓ </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Créer et gérer des taux d’exchange</td> 
   <td>✓ </td> 
   <td>✓**</td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td>Création et gestion des types d’heures</td> 
   <td>✓ </td> 
   <td>✓**</td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td>Création et gestion des chemins de jalon</td> 
   <td>✓ </td> 
   <td>✓**</td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td>Créer et gérer des plannings</td> 
   <td>✓ </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Création et gestion des entreprises</td> 
   <td>✓ </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Créer et gérer des profils de feuille de temps</td> 
   <td>✓ </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Créer des feuilles de temps à usage unique</td> 
   <td>✓</td> 
   <td>✓**</td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td>Créer et gérer des fonctions</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Créer et gérer des priorités, des statistiques, des conditions</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Création et gestion des types de risque</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Création et gestion des états</td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Connectez-vous en tant que personne d’autre</td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Afficher et restaurer les éléments supprimés</td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Affichage et gestion des éléments restaurés</td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Afficher l’attribution de licence actuelle</td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Attribuer un nombre maximal de licences</td> 
   <td>✓*** </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher les journaux d’audit</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Importation et exportation de données à l’aide de start-up</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Au niveau d’accès de l’administrateur du groupe, **Modifier** doit être sélectionné pour le paramètre **Utilisateurs**, avec **Administrateur utilisateur (Utilisateurs de groupe)** sélectionné sous **** ![](assets/gear-icon-in-access-levels.png) pour affiner vos paramètres. Pour plus d’informations, reportez-vous à la section [Configuration de l’accès des utilisateurs à la modification des utilisateurs à l’aide d’un niveau d’accès personnalisé](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit) de l’article [Accorder l’accès aux utilisateurs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

&#42;&#42; Au niveau d’accès de l’administrateur de groupe, l’accès à cette action doit être activé. Pour plus d’informations, voir [Accorder aux utilisateurs et aux utilisatrices un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

&#42;&#42;&#42; Les activités suivantes font partie des Contrôles d’entreprise avancés et ne sont pas disponibles pour le forfait Sélectionner . Seules les organisations ayant acheté les plans Prime ou Ultimate peuvent accéder à ces fonctionnalités.  Pour plus d’informations sur les plans, consultez la [page de tarification et de package Adobe Workfront](https://business.adobe.com/products/workfront/pricing.html) . (Pour les organisations qui utilisent les plans hérités, le tableau ci-dessus montre les activités pour les administrateurs de groupes et de sous-groupes.)

* Configuration des préférences de projet, de tâche et de problème au niveau du groupe
* Configuration des préférences de feuille de temps et d’heure au niveau du groupe
* Configuration des emails de notification d’événement au niveau du groupe
* Créer et gérer des processus d’approbation spécifiques à un groupe
* Attribuer des limites de licence et afficher leur utilisation par groupe d’accueil
* Affecter des administrateurs de groupe à des sous-groupes
* Autoriser les administrateurs de groupes à créer des sous-groupes
