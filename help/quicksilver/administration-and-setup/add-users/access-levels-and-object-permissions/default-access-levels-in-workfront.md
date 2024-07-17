---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accès,modèle,entonnoir,diagramme,niveaux,autorisations
navigation-topic: access-levels
title: Niveaux d’accès intégrés
description: Chacun des six niveaux d’accès intégrés actuels est conçu pour un type particulier d’utilisateur, y compris l’administrateur système, le planificateur, le responsable de traitement, le réviseur, le demandeur et l’utilisateur externe. Ces niveaux d’accès vous permettent de contrôler ce que les utilisateurs peuvent modifier et afficher dans le système. Si vous avez besoin d’un niveau d’accès personnalisé, vous pouvez copier un niveau d’accès intégré et le modifier en fonction de la quantité d’accès que vous souhaitez lui permettre pour les différents types d’objets Workfront.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 9d2165cdc9399273a4f79b90d4049f50097cadee
workflow-type: tm+mt
source-wordcount: '1685'
ht-degree: 13%

---

# Niveaux d’accès intégrés

<!--Audited: 01/2024-->

>[!NOTE]
>
>Cet article décrit les niveaux d’accès intégrés actuels dans Adobe Workfront. Pour plus d’informations sur les nouveaux niveaux d’accès intégrés, consultez la [Présentation des nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).


Chacun des six niveaux d’accès intégrés actuels est conçu pour un type particulier d’utilisateur. Ces niveaux d’accès vous permettent de contrôler ce que les utilisateurs peuvent modifier et afficher dans le système.

Chacun des six niveaux d’accès intégrés est conçu pour les types d’utilisateurs suivants :

* Administrateur ou administratrice système
* Planificateur
* Employé
* Réviseur
* Demandeur
* Utilisateur ou utilisatrice externe

Selon le niveau d’accès, jusqu’à 3 paramètres sont disponibles pour la plupart des types d’objets Workfront :

<table style="table-layout:auto">
    <tr>
        <td>Modifier</td>
        <td>Les utilisateurs peuvent créer, modifier, supprimer et partager l’objet Workfront.</td>
    </tr>
    <tr>
        <td>Afficher</td>
        <td>Les utilisateurs peuvent examiner et partager l’objet Workfront</td>
    </tr>
    <tr>
        <td>Pas d’accès
</td>
        <td>Les utilisateurs ne peuvent pas accéder à l’objet Workfront</td>
    </tr>
</table>

Si vous avez besoin d’un niveau d’accès personnalisé pour le planificateur, le traitement, le demandeur ou le réviseur, vous pouvez copier le niveau d’accès intégré et déterminer la quantité d’accès que vous souhaitez lui permettre pour les différents types d’objets Workfront.

>[!TIP]
>
>Vous ne pouvez pas modifier les niveaux d’accès Administrateur système ou Utilisateur externe.

Pour plus d’informations sur la création d’un niveau d’accès personnalisé ou la modification de l’un des niveaux d’accès intégrés, voir [ Créer et modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Nous vous recommandons vivement de ne pas modifier les niveaux d’accès intégrés afin que vous puissiez y faire référence après avoir configuré vos utilisateurs.

Pour obtenir des informations générales sur ces niveaux d’accès, voir [Présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Niveau d’accès administrateur système

Associé à la licence Plan, le niveau d’accès Administrateur système intégré est conçu pour un utilisateur chargé de l’administration du système Adobe Workfront. Vous ne pouvez pas modifier ce niveau d’accès intégré.

Les utilisateurs disposant du niveau d’accès Administrateur système peuvent tout faire dans Workfront. Ils peuvent afficher et modifier tous les objets et informations Workfront saisis dans Workfront par tous les autres utilisateurs.

Ils disposent également d’un accès complet à la zone Configuration, où ils peuvent modifier n’importe quel paramètre au niveau du système. Et ils peuvent accéder à toutes les zones du menu principal ![](assets/main-menu-icon.png) ou du menu principal ![](assets/lines-main-menu.png), si disponible.

Pour plus d’informations, voir [Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Niveau d’accès du planificateur

Également joint à la licence Plan, le niveau d’accès du planificateur est conçu pour :

* Chargés de groupes, d’équipes, de projets et de ressources
* Toute personne responsable de la planification, de la création et de la gestion des tâches, des projets, des portefeuilles et des programmes.
* Toute personne responsable de l’affectation du travail (tâches et problèmes) à d’autres utilisateurs
* Utilisateurs qui créent des rapports et approuvent des feuilles de temps, des tâches et des documents
* Utilisateurs qui doivent accéder à toutes les zones du menu principal ![](assets/main-menu-icon.png) ou du menu principal ![](assets/lines-main-menu.png), le cas échéant

Vous pouvez créer une version personnalisée du niveau d’accès intégré du planificateur et déterminer la quantité d’accès qu’il permet aux différents types d’objets Workfront. Pour plus d’informations, consultez [Créer et modifier des niveaux d’accès personnalisés](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Voici les paramètres d’accès les plus élevés disponibles pour les objets au niveau d’accès du planificateur :

| Type d’objet Workfront | Pas d’accès | Accès aux vues | Modifier l’accès |
|---|---|---|---|
| Projets |   |   | ✓ |
| Tâches |   |   | ✓ |
| Problèmes |   |   | ✓ |
| Portefeuilles |   |   | ✓ |
| Programmes |   |   | ✓ |
| Rapports, tableaux de bord et calendriers |   |   | ✓ |
| Filtres, vues et regroupements |   |   | ✓ |
| Documents |   |   | ✓ |
| Utilisateurs |   |   | ✓ |
| Équipes |   |   | ✓ |
| Modèles |   |   | ✓ |
| Données financières |   |   | ✓ |
| Gestion des ressources |   |   | ✓ |
| Planificateur de scénarios |   |   | ✓ (Le paramètre par défaut est No Access.) |
| Objectifs Workfront |   |   | ✓ (Le paramètre par défaut est No Access.) |

{style="table-layout:auto"}

## Niveau d’accès du traitement

Associé à la licence Work, le niveau d’accès Worker est conçu pour les utilisateurs qui effectuent le travail dans Workfront. Ils ne planifient pas le travail, ils le terminent.

Utilisateurs disposant de ce niveau d&#39;accès :

* sont affectées à des tâches où ils peuvent contribuer et consigner le temps ;
* Peut approuver le travail et les documents, mais pas les feuilles de temps
* Peut accéder aux rapports et les partager
* Peut communiquer avec d’autres utilisateurs du système
* Impossible d&#39;accéder à toutes les zones du menu principal ![](assets/main-menu-icon.png) ou du menu principal ![](assets/lines-main-menu.png), le cas échéant, et leur zone &quot;Utilisateurs&quot; est nommée Équipes. Dans la zone Équipes, les utilisateurs disposant de ce niveau d’accès peuvent afficher uniquement les équipes auxquelles ils appartiennent, ainsi que le travail affecté à ces équipes.
* La possibilité de créer des objets est limitée : ils ne peuvent pas créer de projets, de portefeuilles, de programmes ou de rapports.

Vous pouvez créer une version personnalisée du niveau d’accès intégré au traitement et déterminer la quantité d’accès qu’il permet pour les différents types d’objets Workfront. Pour plus d’informations, consultez [Créer et modifier des niveaux d’accès personnalisés](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Voici les paramètres d’accès les plus élevés disponibles pour les objets du niveau d’accès Worker :

| Type d’objet Workfront | Pas d’accès | Accès aux vues | Modifier l’accès |
|---|---|---|---|
| Projets |   |   | ✓ (Limité : les utilisateurs peuvent uniquement partager le projet, créer des tâches et des problèmes et modifier les données dans des formulaires personnalisés qui y sont déjà associés.) |
| Tâches |   |   | ✓ |
| Problèmes |   |   | ✓ |
| Portefeuilles |   | ✓ (Le paramètre par défaut est No Access.) |   |
| Programmes |   | ✓ (Le paramètre par défaut est No Access.) |   |
| Rapports, tableaux de bord et calendriers |   | ✓ |   |
| Filtres, vues et regroupements |   |   | ✓ |
| Documents |   |   | ✓ |
| Utilisateurs |   |   | ✓ |
| Équipes |   |   | ✓ (accès limité) |
| Modèles | ✓ |   |   |
| Données financières |   | ✓ (Le paramètre par défaut est No Access. Le paramètre Afficher permet à l’utilisateur de n’afficher que la zone Finance   dans Détails du projet.) |   |
| Gestion des ressources |   | ✓ |   |
| Planificateur de scénarios |   |   | ✓ (Le paramètre par défaut est No Access.) |
| Objectifs Workfront |   |   | ✓ (Le paramètre par défaut est No Access.) |

{style="table-layout:auto"}

## Niveau d’accès des réviseurs

Associé à la licence de révision, le niveau d’accès Réviseur est conçu pour les cadres qui demandent du travail à d’autres utilisateurs et qui révisent et approuvent le travail. Il ne s’agit pas de propriétaires de projet ou de membres d’équipe, mais ils ont besoin d’accéder à Workfront pour voir les tâches qu’ils supervisent.

Par exemple, une partie prenante disposant de ce niveau d’accès peut se connecter à Workfront pour participer à une révision constante des documents marketing, voir les mises à jour de travail et consulter les documents, les approbations, les rapports et les calendriers.

Utilisateurs avec le niveau d’accès Réviseur :

* Impossible d’attribuer des tâches ou d’approuver les feuilles de temps
* Peuvent accéder aux zones Requêtes et Documents dans le menu principal ![](assets/main-menu-icon.png) ou le menu principal ![](assets/lines-main-menu.png), le cas échéant.
* La possibilité de créer des objets est limitée : ils ne peuvent pas créer de projets, de portefeuilles, de programmes ou de rapports.

Vous pouvez créer une version personnalisée du niveau d’accès intégré du réviseur et déterminer la quantité d’accès qu’il permet pour les différents types d’objets Workfront. Pour plus d’informations, consultez [Créer et modifier des niveaux d’accès personnalisés](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Plus limité pour les projets et les tâches que le niveau d’accès Worker, les paramètres d’accès les plus élevés disponibles pour les objets du niveau d’accès Reviseur sont les suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type d’objet Workfront</th> 
   <th>Pas d’accès</th> 
   <th>Accès aux vues</th> 
   <th>Modifier l’accès</th> 
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
   <td>✓ (Le paramètre par défaut est No Access.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programmes</td> 
   <td> </td> 
   <td>✓ (Le paramètre par défaut est No Access.)</td> 
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
   <td> </td> 
   <td> <p>✓ (Le paramètre par défaut est No Access. Le paramètre Afficher permet à l’utilisateur de n’afficher que la zone Finance   dans Détails du projet.)</p> </td> 
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
   <td>✓ (Le paramètre par défaut est No Access.)</td> 
  </tr> 
  <tr> 
   <td>Objectifs Workfront </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Le paramètre par défaut est No Access.)</td> 
  </tr> 
 </tbody> 
</table>

## Niveau d’accès du demandeur

Associé à la licence Request , le niveau d’accès Requestor est conçu pour les utilisateurs qui effectuent et reçoivent des demandes de travail simples dans Workfront. Par défaut, elles sont limitées à la zone Demandes .

Par exemple, un utilisateur peut consigner des problèmes dans la file d’attente des demandes du service d’assistance de votre entreprise.

Utilisateurs disposant de ce niveau d&#39;accès :

* Peut effectuer des requêtes et les mettre à jour
* Peut télécharger et approuver des documents
* Peuvent examiner l’état des problèmes qu’ils ont envoyés.
* Ne peut pas être affecté aux tâches
* Les demandes ne peuvent accéder qu’à partir de la zone Demandes du menu principal ![](assets/main-menu-icon.png) ou du menu principal ![](assets/lines-main-menu.png), le cas échéant. Pour plus d’informations sur les files d’attente de requête, voir [Création d’une file d’attente de requête](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Vous pouvez créer une version personnalisée du niveau d’accès intégré du demandeur et déterminer la quantité d’accès qu’il permet pour les différents types d’objets Workfront. Pour plus d’informations, consultez [Créer et modifier des niveaux d’accès personnalisés](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Voici les paramètres d’accès les plus élevés disponibles pour les objets du niveau d’accès du demandeur :

| Type d’objet Workfront | Pas d’accès | Accès aux vues | Modifier l’accès |
|---|---|---|---|
| Projet |   | ✓ (Page Détails du projet uniquement) |   |
| Tâche |   | ✓(Page Détails de la tâche uniquement) |   |
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
| Objectifs Workfront |   |   | ✓ (Le paramètre par défaut est No Access.) |

{style="table-layout:auto"}

## Niveau d’accès des utilisateurs externes

Le niveau d’accès Utilisateur externe n’est pas associé à une licence Workfront payante. Il s’agit du niveau d’accès le plus restrictif, conçu principalement pour les collaborateurs tels que les consultants externes qui ne se connectent pas à Workfront, mais qui doivent parfois consulter, télécharger ou afficher des documents.

Les utilisateurs de Workfront peuvent affecter des tâches à des utilisateurs externes, même s’ils ne peuvent pas se connecter au système. Cependant, nous ne recommandons pas d’affecter des tâches et des problèmes aux utilisateurs externes, car ce travail ne serait pas résolu dans le système.

Utilisateurs disposant du niveau d’accès Utilisateur externe :

* Peuvent afficher uniquement les documents et les rapports de calendrier partagés avec eux.
* peuvent voir les utilisateurs qui partagent des documents et des rapports de calendrier avec eux ;
* Peut approuver les documents qui sont partagés avec eux

Vous ne pouvez pas modifier ce niveau d&#39;accès.

>[!IMPORTANT]
>
>L’option Utilisateur externe n’est disponible que si l’option &quot;Collaborer avec des personnes sans compte Workfront à l’aide de leur adresse électronique&quot; est activée dans la zone Préférences système de la section Configuration. Pour plus d’informations, voir [Configuration des préférences de sécurité du système](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Bien que ces paramètres ne soient pas visibles dans la zone Niveaux d’accès pour le niveau d’accès Utilisateur externe , un utilisateur disposant de cet accès dispose des droits d’accès suivants sur les types d’objets Workfront :

| Type d’objet Workfront | Pas d’accès | Accès aux vues | Modifier l’accès |
|---|---|---|---|
| Projet | ✓ |   |   |
| Tâche | ✓ | |   |
| Problème | ✓ |   |   |
| Portefeuilles | ✓ |   |   |
| Programmes | ✓ |   |   |
| Rapports, tableaux de bord et calendriers |   | ✓ (Uniquement pour les rapports de calendrier ; impossible de partager les rapports) |   |
| Filtres, vues et regroupements | ✓ |   |   |
| Documents |   | ✓ (sans possibilité de partager des documents) |   |
| Utilisateurs |   | ✓ |   |
| Équipes |   | ✓ |   |
| Modèles | ✓ |   |   |
| Données financières | ✓ |   |   |
| Gestion des ressources | ✓ |   |   |
| Planificateur de scénarios | ✓ |   |   |
| Objectifs Workfront | ✓ |   |   |
