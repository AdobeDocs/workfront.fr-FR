---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accès,modèle,entonnoir,diagramme,niveaux,autorisations
navigation-topic: access-levels
title: Niveaux d'accès intégrés (hérités)
description: 'Chacun des six niveaux d’accès intégrés actuels est conçu pour un type particulier d’utilisateur ou d’utilisatrice : administrateur et administratrice système, planificateur et planificatrice, employé et employée, réviseur et réviseuse, demandeur et demandeuse, et utilisateur et utilisatrice externes. Ces niveaux d’accès vous permettent de contrôler ce que les personnes peuvent modifier et afficher dans le système. Si vous avez besoin d’un niveau d’accès personnalisé, vous pouvez copier un niveau d’accès intégré et le modifier en fonction de la quantité d’accès que vous souhaitez autoriser pour les différents types d’objets Workfront.'
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '1656'
ht-degree: 84%

---

# Niveaux d’accès intégrés (hérités)

<!--Audited: 01/2024-->

>[!NOTE]
>
>Les informations de cet article font référence aux niveaux d’accès hérités. Pour plus d’informations sur les niveaux d’accès actuels, voir [Présentation des nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).


Chacun des six niveaux d’accès intégrés actuels est conçu pour un type particulier d’utilisateur ou d’utilisatrice. Ces niveaux d’accès vous permettent de contrôler ce que les personnes peuvent modifier et afficher dans le système.

Chacun des six niveaux d’accès intégrés est conçu pour les types d’utilisateurs et d’utilisatrices suivants :

* Administrateur ou administratrice système
* Planificateur
* Employé
* Réviseur
* Demandeur
* Utilisateur ou utilisatrice externe

Selon le niveau d’accès, jusqu’à 3 paramètres sont disponibles pour la plupart des types d’objets Workfront :

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

Si vous avez besoin d’un niveau d’accès personnalisé Planificateur ou planificatrice, Employé ou employée, Demandeur ou demandeuse ou Réviseur ou réviseuse, vous pouvez copier le niveau d’accès intégré et déterminer la quantité d’accès que vous souhaitez autoriser pour les différents types d’objets Workfront.

>[!TIP]
>
>Vous ne pouvez pas modifier les niveaux d’accès Administrateur ou administratrice système ou Utilisateur ou utilisatrice externe.

Pour plus d’informations sur la création d’un niveau d’accès personnalisé ou la modification de l’un des niveaux d’accès intégrés, voir [Créer et modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Nous vous recommandons vivement de ne pas modifier les niveaux d’accès intégrés afin que vous puissiez y faire référence après avoir configuré vos utilisateurs et utilisatrices.

Pour obtenir des informations générales sur ces niveaux d’accès, voir [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Niveau d’accès pour l’administration système

Associé à la licence de plan, le niveau d’accès Administrateur ou administratrice système intégré est conçu pour une personne chargée de l’administration du système Adobe Workfront. Vous ne pouvez pas modifier ce niveau d’accès intégré.

Les personnes disposant du niveau d’accès Administrateur ou administratrice système peuvent tout faire dans Workfront. Elles peuvent afficher et modifier tous les objets et informations Workfront saisis dans Workfront par les autres utilisateurs et utilisatrices.

Elles disposent également d’un accès complet à la zone Configuration, où elles peuvent modifier n’importe quel paramètre au niveau du système. Et ils peuvent accéder à toutes les zones du Menu principal ![icône du menu principal](assets/main-menu-icon.png) ou du Menu principal ![icône du menu principal](assets/main-menu-icon.png), le cas échéant.

Pour plus d’informations, voir [Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Niveau d’accès Planificateur ou planificatrice

Également associé à la licence de plan, le niveau d’accès Planificateur ou planificatrice est conçu pour :

* les personnes responsables de groupes, d’équipes, de projets et de ressources ;
* toute personne responsable de la planification, de la création et de la gestion des tâches, des projets, des portfolios et des programmes ;
* toute personne responsable de l’affectation du travail (tâches et problèmes) à d’autres utilisateurs et utilisatrices ;
* les utilisateurs et utilisatrices qui créent des rapports et approuvent des feuilles de temps, des tâches et des documents ;
* Les utilisateurs qui doivent accéder à toutes les zones du menu principal ![icône du menu principal](assets/main-menu-icon.png) ou du menu principal ![icône du menu principal](assets/main-menu-icon.png), le cas échéant.

Vous pouvez créer une version personnalisée du niveau d’accès intégré Planificateur ou planificatrice et déterminer la quantité d’accès autorisée pour les différents types d’objets Workfront. Pour plus d’informations, consultez [Créer et modifier des niveaux d’accès personnalisés](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Voici les paramètres d’accès les plus élevés disponibles pour les objets au niveau d’accès Planificateur ou planificatrice :

| Types d’objets Workfront | Pas d’accès | Accès en affichage | Accès en modification |
|---|---|---|---|
| Projets |   |   | ✓ |
| Tâches |   |   | ✓ |
| Problèmes |   |   | ✓ |
| Portefeuilles |   |   | ✓ |
| Programmes |   |   | ✓ |
| Rapports, tableaux de bord et calendriers |   |   | ✓ |
| Filtres, vues et regroupements |   |   | ✓ |
| Documents |   |   | ✓ |
| Utilisateurs et utilisatrices |   |   | ✓ |
| Équipes |   |   | ✓ |
| Modèles |   |   | ✓ |
| Données financières |   |   | ✓ |
| Gestion des ressources |   |   | ✓ |
| Planificateur de scénarios |   |   | ✓ (le paramètre par défaut est Aucun accès.) |
| Objectifs Workfront |   |   | ✓ (le paramètre par défaut est Aucun accès.) |

{style="table-layout:auto"}

## Niveau d’accès Employé ou employée

Associé à la licence de travail, le niveau d’accès Employé ou employée est conçu pour les personnes qui effectuent le travail dans Workfront. Elles ne planifient pas le travail, elles y participent.

Les personnes disposant de ce niveau d’accès :

* sont affectées à des tâches pour lesquelles elles peuvent apporter leur contribution et consigner le temps ;
* peuventt approuver le travail et les documents, mais pas les feuilles de temps ;
* peuvent accéder aux rapports et les partager ;
* peuvent communiquer avec d’autres personnes du système ;
* Impossible d’accéder à toutes les zones du menu principal ![icône du menu principal](assets/main-menu-icon.png) ou du menu principal ![icône du menu principal](assets/main-menu-icon.png), le cas échéant, et leur zone « Utilisateurs » est nommée Équipes. Dans la zone Équipes, les personnes disposant de ce niveau d’accès peuvent afficher uniquement les équipes auxquelles elles appartiennent, ainsi que le travail affecté à ces équipes ;
* ont une capacité limitée de créer des objets, elles ne peuvent pas créer de projets, de portfolios, de programmes ou de rapports.

Vous pouvez créer une version personnalisée du niveau d’accès intégré Employé ou employée et déterminer la quantité d’accès autorisée pour les différents types d’objets Workfront. Pour plus d’informations, consultez [Créer et modifier des niveaux d’accès personnalisés](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Voici les paramètres d’accès les plus élevés disponibles pour les objets du niveau d’accès Employé ou employée :

| Types d’objets Workfront | Pas d’accès | Accès en affichage | Accès en modification |
|---|---|---|---|
| Projets |   |   | ✓ (Limité : les utilisateurs peuvent uniquement partager le projet, y créer des tâches et des événements, et modifier les données de formulaires personnalisés déjà joints à celui-ci.) |
| Tâches |   |   | ✓ |
| Problèmes |   |   | ✓ |
| Portefeuilles |   | ✓ (le paramètre par défaut est Aucun accès.) |   |
| Programmes |   | ✓ (le paramètre par défaut est Aucun accès.) |   |
| Rapports, tableaux de bord et calendriers |   | ✓ |   |
| Filtres, vues et regroupements |   |   | ✓ |
| Documents |   |   | ✓ |
| Utilisateurs et utilisatrices |   |   | ✓ |
| Équipes |   |   | ✓ (Accès limité) |
| Modèles | ✓ |   |   |
| Données financières |   | ✓ (Le paramètre par défaut est Aucun accès. Le paramètre Vue permet à la personne de n’afficher que la zone Finance dans les détails du projet.) |   |
| Gestion des ressources |   | ✓ |   |
| Planificateur de scénarios |   |   | ✓ (le paramètre par défaut est Aucun accès.) |
| Objectifs Workfront |   |   | ✓ (le paramètre par défaut est Aucun accès.) |

{style="table-layout:auto"}

## Niveau d’accès Réviseur ou réviseuse

Associé à la licence de révision, le niveau d’accès Réviseur ou réviseuse est conçu pour les personnes cadres qui demandent du travail à d’autres personnes et qui révisent et approuvent le travail. Il ne s’agit pas des personnes propriétaires de projet ou membres d’équipe, mais ces personnes ont besoin d’accéder à Workfront pour voir les tâches qu’elles supervisent.

Par exemple, une partie prenante disposant de ce niveau d’accès peut se connecter à Workfront pour participer à une révision en cours des documents marketing, voir les mises à jour concernant le travail et consulter les documents, les approbations, les rapports et les calendriers.

Les personnes avec le niveau d’accès Réviseur ou réviseuse :

* ne peuvent pas se voir attribuer des tâches ni approuver les feuilles de temps ;
* Peut accéder aux zones Demandes et Documents du Menu principal ![icône du menu principal](assets/main-menu-icon.png) ou du Menu principal ![icône du menu principal](assets/main-menu-icon.png), le cas échéant
* ont une capacité limitée de créer des objets, elles ne peuvent pas créer de projets, de portfolios, de programmes ou de rapports.

Vous pouvez créer une version personnalisée du niveau d’accès intégré Réviseur ou réviseuse et déterminer la quantité d’accès autorisée pour les différents types d’objets Workfront. Pour plus d’informations, consultez [Créer et modifier des niveaux d’accès personnalisés](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Plus limité pour les projets et les tâches que le niveau d’accès Employé ou employée, les paramètres d’accès les plus élevés disponibles pour les objets du niveau d’accès Réviseur ou réviseuse sont les suivants :

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
   <td>✓</td> 
   <td> </td> 
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
   <td>Rapports, tableaux de bord, calendriers</td> 
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
   <td>Utilisateurs et utilisatrices</td> 
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
   <td> </td> 
   <td> <p>✓ (Le paramètre par défaut est Pas d’accès. Le paramètre Vue permet à la personne de n’afficher que la zone Finance dans les détails du projet.)</p> </td> 
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
   <td>Objectifs Workfront </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Le paramètre par défaut est Pas d’accès.)</td> 
  </tr> 
 </tbody> 
</table>

## Niveau d’accès Demandeur ou demandeuse

Associé à la licence de demande, le niveau d’accès Demandeur ou demandeuse est conçu pour les personnes qui effectuent et reçoivent des demandes de travail simples dans Workfront. Par défaut, elles sont limitées à la zone Demandes.

Par exemple, une personne peut consigner des problèmes dans la file d’attente des demandes du centre d’assistance de votre entreprise.

Les personnes disposant de ce niveau d’accès :

* peuvent effectuer des demandes et les mettre à jour ;
* peuvent charger et approuver des documents ;
* peuvent examiner le statut des problèmes qu’elles ont soumis ;
* ne peuvent pas être affectées aux éléments de travail ;
* Peut accéder aux demandes uniquement à partir de la zone Demandes du Menu principal ![Icône du menu principal](assets/main-menu-icon.png) ou du Menu principal ![Icône du menu principal](assets/main-menu-icon.png), le cas échéant. Pour plus d’informations sur les files d’attente des demandes, voir [Créer une file d’attente des demandes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Vous pouvez créer une version personnalisée du niveau d’accès intégré Demandeur ou demandeuse et déterminer la quantité d’accès autorisée pour les différents types d’objets Workfront. Pour plus d’informations, consultez [Créer et modifier des niveaux d’accès personnalisés](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Voici les paramètres d’accès les plus élevés disponibles pour les objets du niveau d’accès Demandeur ou demandeuse :

| Types d’objets Workfront | Pas d’accès | Accès en affichage | Accès en modification |
|---|---|---|---|
| Projet |   | ✓ (uniquement la page Détails du projet) |   |
| Tâche |   | ✓(uniquement la page Détails de la tâche) |   |
| Problème |   |   | ✓ |
| Portefeuilles | ✓ |   |   |
| Programmes | ✓ |   |   |
| Rapports, tableaux de bord et calendriers |   | ✓ |   |
| Filtres, vues et regroupements |   |   | ✓ |
| Documents |   |   | ✓ |
| l’utilisateur ou de l’utilisatrice |   | ✓ |   |
| Équipes |   | ✓ |   |
| Modèles | ✓ |   |   |
| Données financières | ✓ |   |   |
| Gestion des ressources | ✓ |   |   |
| Planificateur de scénarios | ✓ |   |   |
| Objectifs Workfront |   |   | ✓ (le paramètre par défaut est Aucun accès.) |

{style="table-layout:auto"}

## Niveau d’accès Utilisateur ou utilisatrice externe

Le niveau d’accès Utilisateur ou utilisatrice externe n’est pas associé à une licence Workfront payante. Il s’agit du niveau d’accès le plus restrictif, conçu principalement pour des collaborateurs et collaboratrices tels que des consultantes et consultants externes qui ne se connectent pas à Workfront, mais qui doivent parfois consulter, télécharger ou afficher des documents.

Les personnes de Workfront peuvent affecter des tâches à des utilisateurs et utilisatrices externes, même si les utilisateurs et utilisatrices externes ne peuvent pas se connecter au système. Cependant, nous ne recommandons pas d’affecter des tâches et des problèmes aux utilisateurs et utilisatrices externes, car ce travail ne serait pas résolu dans le système.

Les personnes disposant du niveau d’accès Utilisateur ou utilisatrice externe :

* peuvent afficher uniquement les documents et les rapports de calendrier partagés ;
* peuvent voir les utilisateurs et utilisatrices qui partagent des documents et des rapports de calendrier avec elles ;
* peuvent approuver les documents qui sont partagés avec elles.

Vous ne pouvez pas modifier ce niveau d’accès.

>[!IMPORTANT]
>
>Le niveau d’accès Utilisateur ou utilisatrice externe n’est disponible que si l’option « Collaborer avec des personnes sans les comptes Workfront et utilisant leur adresse e-mail » est activée dans la zone Préférences système de la section Configuration. Pour plus d’informations, voir [Configurer les préférences de sécurité système](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Bien que ces paramètres ne soient pas visibles dans la zone Niveaux d’accès pour le niveau d’accès Utilisateur ou utilisatrice externe, une personne disposant de cet accès dispose des accès les plus élevés suivants sur les types d’objets Workfront :

| Types d’objets Workfront | Pas d’accès | Accès en affichage | Accès en modification |
|---|---|---|---|
| Projet | ✓ |   |   |
| Tâche | ✓ | |   |
| Problème | ✓ |   |   |
| Portefeuilles | ✓ |   |   |
| Programmes | ✓ |   |   |
| Rapports, tableaux de bord et calendriers |   | ✓ (uniquement pour les rapports de calendrier ; pas de possibilité de partager des rapports) |   |
| Filtres, vues et regroupements | ✓ |   |   |
| Documents |   | ✓ (sans possibilité de partager des documents) |   |
| Utilisateurs et utilisatrices |   | ✓ |   |
| Équipes |   | ✓ |   |
| Modèles | ✓ |   |   |
| Données financières | ✓ |   |   |
| Gestion des ressources | ✓ |   |   |
| Planificateur de scénarios | ✓ |   |   |
| Objectifs Workfront | ✓ |   |   |
