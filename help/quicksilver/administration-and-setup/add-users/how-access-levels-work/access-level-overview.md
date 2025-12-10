---
title: Présentation des nouveaux niveaux d'accès
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accès,niveau,système,administrateur,administratrice,standard,léger,contributeur,contributrice
navigation-topic: access-levels
description: Chaque utilisateur ou utilisatrice doit disposer d’un niveau d’accès pour se connecter et travailler dans Workfront. Vous utilisez le niveau d’accès pour définir ce qu’un utilisateur ou une utilisatrice peut voir et effectuer avec certains objets et zones Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '1720'
ht-degree: 91%

---

# Vue d’ensemble des nouveaux niveaux d’accès

>[!NOTE]
>
>Les informations de cet article se rapportent aux niveaux d’accès actuels. Pour plus d&#39;informations sur les niveaux d&#39;accès hérités, voir [Présentation des niveaux d&#39;accès](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

En tant qu’administrateur ou administratrice Adobe Workfront, vous attribuez un niveau d’accès à un utilisateur ou une utilisatrice à deux fins :

* Chaque utilisateur ou utilisatrice doit disposer d’un niveau d’accès pour se connecter et travailler dans Workfront.
* Vous utilisez le niveau d’accès pour définir ce qu’un utilisateur ou une utilisatrice peut voir et effectuer avec certains objets et zones Workfront.

## Nouveaux niveaux d’accès intégrés dans Adobe Workfront {#built-in-access}

Workfront dispose de 5 nouveaux niveaux d’accès intégrés :

* Administrateur ou administratrice système
* Standard
* Léger
* Contributeur
* Externe

Selon le niveau d’accès, jusqu’à 3 autorisations sont disponibles pour la plupart des types d’objets Workfront :

<table style="table-layout:auto">
    <tr>
        <td>Modifier</td>
        <td>Les utilisateurs et utilisatrices peuvent créer, modifier, supprimer et partager l’objet Workfront.</td>
    </tr>
    <tr>
        <td>Afficher</td>
        <td>Les utilisateurs et utilisatrices peuvent réviser et partager l’objet Workfront.</td>
    </tr>
    <tr>
        <td>Pas d’accès</td>
        <td>Les utilisateurs et utilisatrices ne peuvent pas accéder à l’objet Workfront.</td>
    </tr>
</table>

Si vous avez besoin d’un niveau d’accès personnalisé, vous pouvez copier le niveau d’accès intégré et ajuster la quantité d’accès que vous souhaitez qu’il autorise pour les différents types d’objets Workfront. Pour plus d’informations sur la création d’un niveau d’accès personnalisé, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Nous vous recommandons vivement de ne pas modifier les niveaux d’accès intégrés afin que vous puissiez y faire référence après avoir configuré vos utilisateurs et utilisatrices.

### Niveau d’accès pour l’administration système

Associé à la licence Standard, ce niveau d’accès intégré est conçu pour un utilisateur ou une utilisatrice responsable de l’administration du système Adobe Workfront. Vous ne pouvez pas modifier ce niveau d’accès intégré.

Les personnes disposant du niveau d’accès Administrateur ou administratrice système peuvent tout faire dans Workfront. Elles peuvent afficher et modifier tous les objets et informations Workfront saisis dans Workfront par les autres utilisateurs et utilisatrices.

Elles ont également accès à la zone Configuration complète, dans laquelle elles peuvent modifier n’importe quel paramètre au niveau du système, et elles peuvent accéder à toutes les zones du menu principal.

Pour plus d’informations, consultez [Accorder à un utilisateur ou à une utilisatrice un accès d’administration complet](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Niveau d’accès standard

Également associé à la licence standard, ce niveau d’accès est conçu pour les utilisateurs et utilisatrices pour effectuer les opérations suivantes :

* Planifier, créer et effectuer un suivi de tous les projets au même endroit
* Automatiser les processus de routine
* Gérer les ressources
* Effectuer un suivi et collaborer sur les requêtes
* Effectuer un suivi et générer des rapports sur les finances du projet
* Démarrer des requêtes de travail entrantes
* Collaborer sur des projets, tâches et problèmes

>[!NOTE]
>
>Vous pouvez créer une version personnalisée du niveau d’accès standard intégré et ajuster la quantité d’accès autorisée pour les différents types d’objets Workfront. Pour plus d’informations sur la création d’un niveau d’accès personnalisé, voir [Créer ou modifier les niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Détails de l’accès**

Voici les paramètres d’accès les plus élevés disponibles pour les objets au niveau d’accès standard :

| Types d’objets Workfront | Pas d’accès | Accès en affichage | Accès en modification |
|---|---|---|---|
| Projets |   |   | ✓ |
| Tâches |   |   | ✓ |
| Problèmes |   |   | ✓ |
| Portefeuilles |   |   | ✓ |
| Programmes |   |   | ✓ |
| Rapports (y compris les tableaux de bord et les rapports de calendrier) |   |   | ✓ |
| Filtres, vues et regroupements |   |   | ✓ |
| Documents |   |   | ✓ |
| Utilisateurs |   |   | ✓ |
| Modèles |   |   | ✓ |
| Données financières |   |   | ✓ |
| Gestion des ressources |   |   | ✓ |
| Planificateur de scénarios |   |   | ✓ (le paramètre par défaut est Aucun accès.) |
| Objectifs |   |   | ✓ |

{style="table-layout:auto"}

### Niveau d’accès Light

Attaché à la licence Light, ce niveau d’accès est conçu pour les utilisateurs et les utilisatrices pour effectuer les opréations suivantes :

* Afficher tous les éléments et mises à jour liés au travail
* Approuver les projets, les tâches et les problèmes
* Afficher des tableaux de bord et des rapports
* Suivre les heures pour les tâches et les événements et approuver les feuilles de temps
* Créer et gérer des problèmes

Ce qui suit est vrai pour les utilisateurs et utilisatrices avec le niveau d’accès Light :

* Ils peuvent se voir attribuer des tâches, mais ne peuvent pas les terminer.
* Ils peuvent accéder aux demandes et aux documents dans le menu principal.
* ont une capacité limitée de créer des objets, elles ne peuvent pas créer de projets, de portfolios, de programmes ou de rapports.

>[!NOTE]
>
>Vous pouvez créer une version personnalisée du niveau d’accès Light intégré et ajuster l’étendue de l’accès qu’il permet aux différents types d’objets Workfront. Pour plus d’informations sur la création d’un niveau d’accès personnalisé, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Détails de l’accès**

Voici les paramètres d’accès les plus élevés disponibles pour les objets de niveau d’accès Light :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Types d’objets Workfront</th> 
   <th>Pas d’accès</th> 
   <th>Accès en affichage</th> 
   <th>Accès en modification</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projets</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tâches</td> 
   <td> </td> 
   <td></td> 
   <td>✓ (limité)</td> 
  </tr> 
  <tr> 
   <td>Problèmes</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Portefeuilles</td> 
   <td> </td> 
   <td>✓ (Le paramètre par défaut est Pas d’accès.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programmes</td> 
   <td> </td> 
   <td>✓ (Le paramètre par défaut est Pas d’accès.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rapports (y compris les tableaux de bord et les rapports de calendrier)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filtres, vues et regroupements</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Utilisateurs</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
    <tr> 
   <td>Équipes</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr>
  <tr> 
   <td>Modèles</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Données financières</td> 
   <td></td> 
   <td> <p>✓ (le paramètre par défaut est Aucun accès)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gestion des ressources</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Planificateur de scénarios </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Le paramètre par défaut est Pas d’accès.)</td> 
  </tr>

<tr>   
   <td>Objectifs </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (le paramètre par défaut est Aucun accès)</td> 
 </tbody> 
</table>

### Niveau d’accès Contribution

Attaché à la licence Contribution, ce niveau d’accès est conçu pour les utilisateurs et les utilisatrices pour effectuer les opérations suivantes :

* Soumettre des demandes
* Effectuer un suivi des demandes
* Mettre à jour et examiner les demandes
* Approuver les demandes

Ce qui suit est vrai pour les utilisateurs et utilisatrices disposant de ce niveau d’accès intégré :

* peuvent effectuer des demandes et les mettre à jour ;
* peuvent charger et approuver des documents ;
* peuvent approuver des projets, des tâches et des problèmes ;

  >[!NOTE]
  >
  >Les contributeurs peuvent participer aux validations mais ne peuvent pas accéder à l&#39;onglet Validations pour afficher ou gérer les processus de validation.

* peuvent examiner le statut des problèmes qu’elles ont soumis ;
* Ils peuvent être affectés à des tâches, mais ne peuvent pas les terminer.
* Ils ne peuvent accéder aux demandes qu’à partir du menu principal. Pour plus d’informations sur les files d’attente des demandes, voir [Créer une file d’attente des demande](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Vous pouvez créer une version personnalisée du niveau d’accès intégré Contribution et ajuster l’étendue de l’accès qu’il permet pour les différents types d’objets Workfront. Pour plus d’informations sur la création d’un niveau d’accès personnalisé, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Détails de l’accès**

Voici les paramètres d’accès les plus élevés disponibles pour les objets du niveau d’accès Contribution :

| Types d’objets Workfront | Pas d’accès | Accès en affichage | Accès en modification |
|---|---|---|---|
| Projet |   | ✓ (limité) |   |
| Tâche |   | ✓(limité) |   |
| Problème |   |   | ✓ |
| Portefeuilles |   | ✓ |   |
| Programmes |   | ✓ |   |
| Rapports (y compris les tableaux de bord et les rapports de calendrier) |   | ✓ (onglet Détails uniquement) |   |
| Filtres, vues et regroupements |   |   | ✓ |
| Document |   |   | ✓ |
| l’utilisateur ou de l’utilisatrice |   | ✓ |   |
| Équipes |   | ✓ |   |
| Modèles | ✓ |   |   |
| Données financières | ✓ |   |   |
| Gestion des ressources | ✓ |   |   |
| Planificateur de scénarios | ✓ |   |   |
| Objectifs |   |   | ✓ (le paramètre par défaut est Aucun accès) |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>À compter de la version 24.7, les contributeurs ont un accès en affichage aux programmes et aux portefeuilles par défaut.
>
> 
>Les contributeurs intégrés avant la version 24.7 n’auront toujours pas accès aux programmes et portefeuilles par défaut. Vous pouvez mettre à jour leur accès pour l’afficher manuellement si nécessaire.

### Niveau d’accès Utilisateur ou utilisatrice externe

Ce niveau d’accès n’est pas associé à une licence Workfront payante. Il s’agit du niveau d’accès le plus restrictif, conçu principalement pour des collaborateurs et collaboratrices tels que des consultantes et consultants externes qui ne se connectent pas à Workfront, mais qui doivent parfois consulter, télécharger ou afficher des documents.

Les personnes disposant du niveau d’accès Utilisateur ou utilisatrice externe :

* peuvent afficher uniquement les documents et les rapports de calendrier partagés ;
* peuvent afficher les personnes qui partagent des documents et des rapports de calendrier avec elles ;
* peuvent approuver les documents qui sont partagés avec elles.

Les utilisateurs externes ne peuvent pas être affectés à des tâches.

Vous ne pouvez pas modifier ce niveau d’accès.

>[!IMPORTANT]
>
>Le niveau d’accès Utilisateur ou utilisatrice externe n’est disponible que si l’option « Collaborer avec des personnes sans les comptes Workfront et utilisant leur adresse e-mail » est activée dans la zone Préférences système de la section Configuration. Pour plus d’informations, voir [Configurer les préférences de sécurité système](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **Détails de l’accès**

Voici les paramètres d’accès les plus élevés disponibles pour les objets du niveau d’accès Utilisateur ou utilisatrice externe.

| Types d’objets Workfront | Pas d’accès | Accès en affichage | Accès en modification |
|---|---|---|---|
| Projet | ✓ |   |   |
| Tâche | ✓ |   |   |
| Problème | ✓ |   |   |
| Portefeuilles | ✓ |   |   |
| Programmes | ✓ |   |   |
| Rapports (y compris les tableaux de bord et les rapports de calendrier) |   | ✓ (uniquement pour les rapports de calendrier ; pas de possibilité de partager des rapports) |   |
| Filtres, vues et regroupements | ✓ |   |   |
| Document |   | ✓ (pas de possibilité de partager des documents) |   |
| l’utilisateur ou de l’utilisatrice |   | ✓ |   |
| Équipes | ✓ |   |   |
| Modèles | ✓ |   |   |
| Données financières | ✓ |   |   |
| Gestion des ressources | ✓ |   |   |
| Planificateur de scénarios | ✓ |   |   |
| Objectifs | ✓ |   |   |


## Fonctionnement des niveaux d’accès et des autorisations

Les niveaux d’accès définissent ce que les utilisateurs et utilisatrices peuvent voir et faire avec les types d’objets généraux et les zones du système tels que les projets, les tâches et les problèmes. Les autorisations définissent ce à quoi vous avez accès sur des objets spécifiques créés par d’autres personnes dans le système, comme un projet créé pour exécuter une campagne marketing.

Le tableau suivant compare l’accès général d’un utilisateur ou d’une utilisatrice aux objets (défini par le niveau d’accès de l’utilisateur ou l’utilisatrice) aux autorisations d’un objet partagé spécifique :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>Niveau d’accès </th> 
   <th>Autorisations </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Accordé par un administrateur ou une administratrice Workfront au niveau d’accès d’un utilisateur ou d’une utilisatrice</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Accordé par un utilisateur ou une utilisatrice partageant un objet au niveau de l’objet</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Hérité d’un objet partagé de rang supérieur 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Les activités qu’un utilisateur ou une utilisatrice peut réaliser avec un objet sont définies par une combinaison de leur niveau d’accès et des autorisations qui leur sont accordées.

![Hiérarchie des modèles de sécurité](assets/security-model-hierachy-copy.png)

### Accorder des autorisations via le partage d’objets

Les utilisateurs et utilisatrices accèdent à des objets individuels lorsque d’autres utilisateurs et utilisatrices partagent et accordent certaines autorisations sur ces objets.

>[!NOTE]
>
>* Si un utilisateur ou une utilisatrice partage un objet avec certaines autorisations et que cet objet a des objets enfants en dessous, la personne destinataire hérite des mêmes autorisations pour ces objets enfants.
>* Si un niveau d’accès restreint les utilisateurs et utilisatrices de supprimer certains objets, cela ne les empêche pas de supprimer les objets enfants qu’ils contiennent.

Un utilisateur ou une utilisatrice peut accorder à la personne destinataire l’une des autorisations suivantes à l’objet individuel :

* **Afficher** : ce niveau d’autorisation permet à la personne destinataire de partager l’objet de l’une des manières suivantes :

   * à l’échelle du système afin que l’ensemble des utilisateurs et utilisatrices puissent le voir (non disponible pour tous les objets) ;
   * avec les utilisateurs et utilisatrices externes qui n’ont pas de licence Workfront (non disponible pour tous les objets) ;
   * avec une adresse e-mail (disponible uniquement pour les documents et les calendriers).

* **Contribuer** : (non disponible pour tous les objets).
* **Gérer** : lorsqu’une personne partage un objet, les droits de la personne destinataire sur l’objet sont déterminés par une combinaison de ses niveau d’accès et des autorisations accordées par la personne responsable du partage. Le niveau d’accès le plus bas disponible dans cette combinaison détermine ce que la personne destinataire peut faire avec l’objet.

### Exemples de scénarios

#### **Scénario 1**

Si le niveau d’accès de la personne destinataire n’autorise pas la modification de projet, cette personne ne peut pas modifier ni supprimer un projet, même si la personne responsable du partage lui a accordé des autorisations pour le gérer.

Ou, si le niveau d’accès de la personne destinataire autorise la modification de projet, mais que la personne responsable accorde des autorisations de lecture seule à un projet, l’utilisateur ou l’utilisatrice ne peut pas modifier ou supprimer le projet.

#### **Scénario 2**

Quand Olivia partage un projet Workfront avec Tony, l’accès de Tony à ce projet est déterminé par une combinaison de deux éléments :

* le niveau d’accès de Tony, attribué par l’administrateur ou l’administratrice Workfront ;
* les autorisations de Tony pour le projet, spécifiées par Olivia.

Les actions de Tony sur le projet peuvent être limitées davantage au projet, mais la limitation ne peut pas être outrepassée conformément à ce qui est autorisé à son niveau d’accès :

* Si le niveau d’accès de Tony ne lui permet pas de créer des tâches, il ne peut pas ajouter de tâches au projet, même si Olivia lui a donné l’autorisation d’y ajouter des tâches.
* Si le niveau d’accès de Tony lui permet de créer des tâches, mais qu’Olivia n’a pas accordé d’autorisation pour ajouter des tâches au projet, il ne peut pas ajouter de tâches à ce projet, mais il peut ajouter des tâches à d’autres projets pour lesquels il a reçu l’autorisation de le faire.
