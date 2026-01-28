---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accès,modèle,entonnoir,diagramme,niveaux,autorisations
navigation-topic: access-levels
title: Fonctionnalité disponible pour chaque type d’objet pour différents niveaux d’accès (hérité)
description: Les tableaux suivants répertorient les fonctionnalités disponibles pour chaque type d’objet dans les différents niveaux d’accès.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 92%

---

# Fonctionnalité disponible pour chaque type d’objet pour différents niveaux d’accès (hérité)

{{highlighted-preview}}

>[!NOTE]
>
>Les informations de cet article font référence aux niveaux d’accès hérités. Pour plus d’informations sur les niveaux d’accès actuels, voir [Présentation des nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

Les tableaux suivants répertorient les fonctionnalités disponibles pour chaque type d’objet dans les différents niveaux d’accès.

Ils indiquent également les actions que les administrateurs et administratrices Workfront peuvent désactiver ou activer à l’aide d’un niveau d’accès.

>[!NOTE]
>
>Cet article décrit les fonctionnalités disponibles pour les niveaux d’accès dans le modèle de package Workfront actuel. Pour connaître les fonctionnalités disponibles dans le nouveau modèle de package, consultez [Fonctionnalité disponible pour chaque type d’objet pour les nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md).

## Projets

Seuls les personnes disposant d’une licence Plan peuvent bénéficier d’un accès complet aux projets.

| Action | Planificateur | Employé | Réviseur | Demandeur | Utilisateur ou utilisatrice externe |
|---|---|---|---|---|---|
| Créer | ✓&#42; |  |  |  |  |
| Copier | ✓&#42; |  |  |  |  |
| Supprimer | ✓&#42; |  |  |  |  |
| Partager | ✓&#42; | ✓&#42; |  |  |  |
| Partager sur le système | ✓&#42; |  |  |  |  |
| Afficher | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Ajouter un formulaire personnalisé | ✓ |  |  |  |  |
| Mettre à jour des champs personnalisés | ✓ | ✓ |  |  |  |
| Ajouter un processus d’approbation | ✓ |  |  |  |  |
| Approuver un projet | ✓ | ✓ | ✓ |  |  |
| Ajouter un document | ✓ | ✓ | ✓ |  |  |
| Ajouter un problème | ✓ | ✓ |  |  |  |
| Ajouter des tâches | ✓ | ✓ |  |  |  |
| Envoyer des mises à jour/commentaires | ✓ | ✓ | ✓ |  |  |
| Modifier le statut | ✓ |  |  |  |  |
| Consigner les heures | ✓ | ✓ |  |  |  |
| Modifier les affectations | ✓ | ✓ |  |  |  |
| Gérer un niveau de référence | ✓ |  |  |  |  |
| Gérer les risques | ✓ |  |  |  |  |
| Gérer les finances | ✓ |  |  |  |  |
| Ajouter/modifier des dépenses | ✓ | ✓ |  |  |  |
| Joindre des modèles | ✓ |  |  |  |  |
| Enregistrer en tant que modèle | ✓ |  |  |  |  |
| Ajouter/modifier un business case | ✓ |  |  |  |  |
| Modifier des détails du projet | ✓ |  |  |  |  |
| Modifier le personnel | ✓ |  |  |  |  |
| Exporter vers MS Project | ✓ | ✓ | ✓ |  |  |
| Recalculer les finances / la chronologie | ✓ |  |  |  |  |
| Définir des propriétés de file d’attente | ✓ |  |  |  |  |



&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Tâches

| Action | Planificateur | Employé | Réviseur | Demandeur | Utilisateur ou utilisatrice externe |
|---|---|---|---|---|---|
| Créer | ✓&#42; | ✓&#42; |  |  |  |
| Supprimer | ✓&#42; | ✓&#42; |  |  |  |
| Partager | ✓&#42; | ✓&#42; |  |  |  |
| Partager sur le système | ✓&#42; |  |  |  |  |
| Afficher | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Ajouter des tâches antérieures | ✓ | ✓ |  |  |  |
| Ajouter des problèmes | ✓ | ✓ |  |  |  |
| Modifier une tâche (à l’exception du statut) | ✓ | ✓ |  |  |  |
| Modifier le statut de la tâche | ✓ | ✓ |  |  |  |
| Ajouter des documents | ✓ | ✓ | ✓ |  |  |
| Copier une tâche | ✓ | ✓ |  |  |  |
| Déplacer une tâche | ✓ | ✓ |  |  |  |
| Consigner les heures | ✓ | ✓ |  |  |  |
| Accepter une affectation | ✓ | ✓ |  |  |  |
| Créer une affectation | ✓ | ✓ | Modification en ligne uniquement | Modification en ligne uniquement |  |
| Joindre un formulaire personnalisé | ✓ | ✓ |  |  |  |
| Modifier les champs personnalisés | ✓ | ✓ |  |  |  |
| Créer un processus d’approbation | ✓ | ✓ |  |  |  |
| Approuver une tâche | ✓ | ✓ | ✓ |  |  |
| Modifier des finances | ✓ |  |  |  |  |
| Ajouter/modifier des dépenses | ✓ | ✓ |  |  |  |
| Afficher Finance | ✓ | ✓ | ✓ |  |  |
| Mises à jour / commentaires | ✓ | ✓ | ✓ |  |  |

{style="table-layout:auto"}

&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Problèmes

| Action | Planificateur | Employé | Réviseur | Demandeur | Utilisateur ou utilisatrice externe |
|---|---|---|---|---|---|
| Créer | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Modifier | ✓ | ✓ | ✓ | ✓ |  |
| Supprimer | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Partager | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Partager sur le système | ✓&#42; |  |  |  |  |
| Afficher | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Joindre des formulaires personnalisés | ✓ | ✓ | ✓ | ✓ |  |
| Modifier les champs personnalisés | ✓ | ✓ | ✓ | ✓ |  |
| Approuver des problèmes | ✓ | ✓ | ✓ | ✓ |  |
| Ajouter un processus d’approbation | ✓ | ✓ | ✓ | ✓ |  |
| Ajouter des documents | ✓ | ✓ | ✓ | ✓ |  |
| Copier les problèmes | ✓ | ✓ | ✓ | ✓ |  |
| Déplacer les problèmes | ✓ | ✓ | ✓ | ✓ |  |
| Consigner les heures | ✓ | ✓ |  |  |  |
| Convertir un problème en projet | ✓ | ✓ |  |  |  |
| Convertir un problème en tâche | ✓ |  |  |  |  |
| Accepter des affectations | ✓ | ✓ |  |  |  |
| Créer des affectations | ✓ | ✓ |  |  |  |
| Ajouter des mises à jour et des commentaires | ✓ | ✓ | ✓ | ✓ |  |



&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Portefeuilles

Seuls les utilisateurs et utilisatrices disposant d’une licence Plan peuvent avoir un accès complet aux portfolios.

| Action | Planificateur | Employé | Réviseur | Demandeur | Utilisateur ou utilisatrice externe |
|---|---|---|---|---|---|
| Créer | ✓&#42; |  |  |  |  |
| Supprimer | ✓&#42; |  |  |  |  |
| Partager | ✓&#42; |  |  |  |  |
| Partager sur le système | ✓&#42; |  |  |  |  |
| Afficher | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Modifier les détails | ✓ |  |  |  |  |
| Joindre des formulaires personnalisés | ✓ |  |  |  |  |
| Modifier les champs personnalisés | ✓ |  |  |  |  |
| Ajouter et supprimer des projets | ✓ |  |  |  |  |
| Approuver des projets | ✓ |  |  |  |  |
| Optimisation du portfolio | ✓ |  |  |  |  |
| Ajouter des documents | ✓ | ✓ | ✓ |  |  |
| Ajouter des mises à jour et des commentaires | ✓ | ✓ | ✓ |  |  |



&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Programmes

Seuls les personnes disposant d’une licence Plan peuvent avoir un accès complet aux programmes.

| Action | Planificateur | Employé | Réviseur | Demandeur | Utilisateur ou utilisatrice externe |
|---|---|---|---|---|---|
| Créer | ✓&#42; |  |  |  |  |
| Supprimer | ✓&#42; |  |  |  |  |
| Partager | ✓&#42; |  |  |  |  |
| Partager sur le système | ✓&#42; |  |  |  |  |
| Afficher | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Modifier les détails | ✓ |  |  |  |  |
| Joindre des formulaires personnalisés | ✓ |  |  |  |  |
| Modifier les champs personnalisés | ✓ |  |  |  |  |
| Ajouter et supprimer des projets | ✓ |  |  |  |  |
| Approuver des projets | ✓ |  |  |  |  |
| Optimisation du portfolio | ✓ |  |  |  |  |
| Ajouter des documents | ✓ | ✓ | ✓ |  |  |
| Ajouter des mises à jour et des commentaires | ✓ | ✓ | ✓ |  |  |



&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Rapports, tableaux de bord et calendriers

Les utilisateurs et utilisatrices disposant d’une licence Plan peuvent avoir un accès complet aux rapports. Tous les autres niveaux d’accès disposent d’un accès en affichage aux rapports.

| Action | Planificateur | Employé | Réviseur | Demande | Utilisateur ou utilisatrice externe |
|---|---|---|---|---|---|
| Créer | ✓&#42; |  |  |  |  |
| Supprimer | ✓&#42; |  |  |  |  |
| Afficher les rapports intégrés | ✓&#42; |  |  |  |  |
| Partager | ✓&#42; | ✓ | ✓ |  |  |
| Partager publiquement des calendriers et des rapports | ✓&#42; |  |  |  |  |
| Partager sur le système | ✓&#42; |  |  |  |  |
| Afficher | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Modifier | ✓ |  |  |  |  |
| Copier | ✓ |  |  |  |  |

{style="table-layout:auto"}

&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

>[!NOTE]
>
>Les demandeurs et demandeuses ne peuvent afficher que les rapports qui ont été partagés avec eux.

## Filtres, vues et regroupements

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Action</p> </th> 
   <th> <p>Planificateur</p> </th> 
   <th> <p>Employé</p> </th> 
   <th> <p>Réviseur</p> </th> 
   <th> <p>Demandeur</p> </th> 
   <th>Utilisateur ou utilisatrice externe<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Créer</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Partager</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Partager sur le système</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifier</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Documents

| Action | Planificateur | Employé | Réviseur | Demandeur | Utilisateur ou utilisatrice externe |
|---|---|---|---|---|---|
| Créer | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Supprimer (documents et dossiers) | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Partager | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Partager publiquement (en externe) | ✓&#42; |  |  |  |  |
| Partager sur le système | ✓&#42; | ✓&#42; |  |  |  |
| Afficher | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Modifier les détails | ✓ | ✓ | ✓ | ✓ |  |
| Téléchargement | ✓ | ✓ | ✓ | ✓ | ✓ |
| Passage en caisse | ✓ | ✓ | ✓ | ✓ |  |
| Ajouter des approbateurs et approbatrices | ✓ | ✓ | ✓ | ✓ |  |
| Approuver des documents | ✓ | ✓ | ✓ | ✓ | ✓ |
| Joindre des formulaires personnalisés | ✓ | ✓ | ✓ | ✓ |  |
| Modifier les champs personnalisés | ✓ | ✓ | ✓ | ✓ |  |
| Déplacer vers (objet) | ✓ | ✓ | ✓ | ✓ |  |
| Envoyer à (intégration) | ✓ | ✓ | ✓ | ✓ |  |
| Ajouter des mises à jour et des commentaires | ✓ | ✓ | ✓ | ✓ |  |
| Charger une nouvelle version | ✓ | ✓ | ✓ | ✓ |  |
| Supprimer une version | ✓ | ✓ | ✓ | ✓ |  |
| Aperçu | ✓ | ✓ | ✓ | ✓ | ✓ |
| Épreuve | ✓ | ✓ | ✓ | ✓ |  |
| Créer une épreuve | ✓ | ✓ |  |  |  |
| Supprimer l’épreuve | ✓ | ✓ | ✓ | ✓ |  |
| Ajouter/Supprimer&#42;&#42; | ✓ | ✓ | ✓ | ✓ |  |
| Renommer&#42;&#42; | ✓ | ✓ | ✓ | ✓ |  |
| Lier (avec intégration) | ✓ | ✓ | ✓ | ✓ |  |
| Annuler le lien (avec intégration) | ✓ | ✓ | ✓ | ✓ |  |

{style="table-layout:auto"}

&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Disponible uniquement pour les dossiers de documents, et non pour les documents

## Utilisateurs et utilisatrices

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Action</p> </th> 
   <th> <p>Planificateur</p> </th> 
   <th>Employé</th> 
   <th> <p>Réviseur</p> </th> 
   <th> <p>Demandeur</p> </th> 
   <th> <p>Utilisateur ou utilisatrice externe**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Créer</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifier, supprimer, désactiver, se connecter en tant que ou réinitialiser le mot de passe d’un utilisateur ou d’une utilisatrice</td> 
   <td>✓*<p><b>REMARQUE </b> : vous ne pouvez pas vous connecter en tant qu'utilisateur administrateur système.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifier, supprimer, désactiver, se connecter en tant que ou réinitialiser le mot de passe d’un utilisateur ou d’une utilisatrice d’un groupe sous son administration</td> 
   <td>✓*<p><b>REMARQUE </b> : vous ne pouvez pas vous connecter en tant qu'utilisateur administrateur système.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher les utilisateurs et utilisatrices</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher les coordonnées</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Les utilisateurs et utilisatrices externes ne peuvent rechercher que d’autres utilisateurs et utilisatrices.

## Équipes

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Action</p> </th> 
   <th> <p>Planificateur</p> </th> 
   <th>Employé</th> 
   <th> <p>Réviseur</p> </th> 
   <th> <p>Demandeur</p> </th> 
   <th> <p>Utilisateur ou utilisatrice externe*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Créer</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Supprimer</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifier les équipes auxquelles la personne appartient.</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifier les équipes dans les groupes que la personne gère.</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher toutes les équipes</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Afficher les équipes associées aux groupes de la personne</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Modèles

| Action | Planificateur | Employé | Réviseur | Demandeur | Utilisateur ou utilisatrice externe |
|---|---|---|---|---|---|
| Créer | ✓&#42; |  |  |  |  |
| Supprimer | ✓&#42; |  |  |  |  |
| Partager | ✓&#42; |  |  |  |  |
| Partager sur le système | ✓&#42; |  |  |  |  |
| Afficher | ✓&#42; |  |  |  |  |
| Copier | ✓ |  |  |  |  |
| Modifier les détails du modèle | ✓ |  |  |  |  |

{style="table-layout:auto"}

&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Données financières

Seuls les utilisateurs et utilisatrices disposant d’une licence Plan peuvent avoir un accès complet aux données financières.

Les types de licence Demande et Utilisateur ou utilisatrice externe ne sont pas inclus ici car ils n’ont pas accès à ces objets et zones.

| Action | Planificateur | Employé | Réviseur |
|---|---|---|---|
| Modifier les taux de facturation et de coûts du rôle | ✓&#42; |  |  |
| Modifier les taux de facturation et de coûts de la personne | ✓&#42; |  |  |
| Afficher les taux de facturation et de coûts du rôle | ✓&#42; |  |  |
| Afficher les taux de facturation et de coûts de la personne | ✓&#42; |  |  |
| Gérer des enregistrements de facturation | ✓ |  |  |
| Gérer les dépenses | ✓ | ✓ |  |
| Afficher les données financières | ✓&#42; | ✓&#42; | ✓&#42; |
| <span class="preview">Gérer les cartes tarifaires</span> | ✓ |  |  |
| Afficher des informations par coût dans les outils de planification des ressources | ✓ |  |  |
| Budgéter les ressources dans les outils de planification des ressources&#42;&#42; | ✓ |  |  |
| Afficher l’affectation des ressources dans les outils de planification des ressources&#42; | ✓ | ✓ | ✓ |
| Créer des risques sur les projets | ✓ |  |  |
| Afficher les risques sur les projets | ✓ | ✓ | ✓ |

{style="table-layout:auto"}

&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Nécessite un accès supplémentaire à la gestion des ressources.

## Gestion des ressources

Seuls les utilisateurs et utilisatrices disposant d’une licence Plan peuvent avoir un accès complet pour [sélectionner un objet ou une zone]. D’autres types de licence peuvent avoir un accès limité ou non à la gestion des ressources dans Workfront.

| Action | Planificateur | Employé | Réviseur | Demandeur | Utilisateur ou utilisatrice externe |
|---|---|---|---|---|---|
| Modifier les priorités et les heures budgétées dans le Planificateur | ✓&#42; |  |  |  |  |
| Créer, modifier et supprimer des groupes de ressources&#42;&#42; | ✓&#42; |  |  |  |  |
| Mettez à jour les heures prévues dans l’équilibreur de charge de travail&#42;&#42;&#42; | ✓* |  |  |  |  |
| Afficher les priorités du projet dans le planificateur de ressources | ✓&#42; |  |  |  |  |
| Afficher l’allocation des ressources dans les outils de planification des ressources | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Afficher les groupes de ressources | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Budgéter les ressources dans les outils de planification des ressources&#42;&#42; | ✓ |  |  |  |  |
| Joindre des groupes de ressources à des projets, modèles et utilisateurs et utilisatrices | ✓ |  |  |  |  |

{style="table-layout:auto"}

&#42; Avec un niveau d’accès, les administrateurs et administratrices Workfront peuvent désactiver ou activer cette fonctionnalité. Pour plus d’informations, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Nécessite un accès supplémentaire aux données financières et des autorisations pour les finances du projet. Si vous accordez l’accès à la gestion des ressources à une personne du planificateur qui n’a pas accès aux données financières, cette personne peut toujours voir les affectations horaires dans le planificateur de ressources, mais elle ne peut pas passer à la vue des coûts ou afficher le business case. Pour plus d’informations, voir [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) et [Partager des autorisations financières sur un objet](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;Nécessite l’autorisation de contribuer à l’objet, avec l‘option Créer des affectations activée sous Paramètres avancés. Pour plus d’informations, voir la section [Comprendre les autorisations héritées et la hiérarchie des objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) dans l’article [Vue d’ensemble des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Zone Planificateur de scénarios

| Action | Planificateur | Employé | Réviseur | Demandeur | Utilisateur ou utilisatrice externe |
|---|---|---|---|---|---|
| Créer/modifier des plans et initiatives existants | ✓ | ✓ | ✓ |  |  |
| Ajouter ou modifier des informations sur les fonctions dans les plans et les initiatives&#42; | ✓ | ✓ | ✓ |  |  |
| Ajouter ou modifier des informations sur les coûts des plans et des initiatives&#42; | ✓ | ✓ | ✓ |  |  |
| Supprimer des plans et des initiatives | ✓ | ✓ | ✓ |  |  |
| Afficher les scénarios dans le menu principal ![icône du planificateur de scénarios](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ | |  |
| Afficher les plans et initiatives créés par l’utilisateur ou l’utilisatrice&#42; | ✓ | ✓ | ✓ |  |  |

{style="table-layout:auto"}

>[!NOTE]
>
>Les utilisateurs et utilisatrices peuvent afficher un plan créé par une autre personne uniquement si un lien vers le plan est partagé avec eux.

&#42; Pour que les utilisateurs et utilisatrices puissent afficher les données financières dans un plan ou une initiative, ils doivent avoir accès aux données financières. Pour plus d’informations, voir [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Zone Objectifs Workfront

| Actions | Afficher | Modifier |
|---|---|---|
| Créer |  | ✓ |
| Modifier/supprimer tous les objectifs |  | ✓ |
| Afficher Objectifs dans le menu principal | ✓ | ✓ |
| Afficher la zone Objectifs à partir d’un lien partagé | ✓ | ✓ |
| Afficher tous les objectifs du système | ✓ | ✓ |
| Activer/désactiver/fermer tous les objectifs |  | ✓ |
| Créer/modifier/supprimer des activités |  | ✓ |
| Créer/modifier/supprimer des résultats |  | ✓ |
| Ajouter un objectif aligné |  | ✓ |
| Mettre à jour la progression d’un résultat ou d’une activité |  | ✓ |
| Posséder un objectif, un résultat ou une activité | ✓ | ✓ |
| Commenter un objectif | ✓ | ✓ |
| Copier des objectifs |  | ✓ |
| Afficher la section Liste des objectifs dans le panneau de gauche | ✓ | ✓ |
| Afficher la section Graphiques dans le panneau de gauche | ✓ | ✓ |
| Afficher la section Alignement des objectifs dans le panneau de gauche | ✓ | ✓ |


