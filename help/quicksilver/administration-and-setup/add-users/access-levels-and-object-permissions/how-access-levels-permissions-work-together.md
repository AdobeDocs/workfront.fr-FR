---
title: Fonctionnement des niveaux d’accès et des autorisations
user-type: administrator
content-type: reference
product-area: system-administration
keywords: accès,modèle,entonnoir,diagramme,niveaux,autorisations
navigation-topic: access-levels
description: L’équipe d’administration d’Adobe Workfront détermine le niveau d’accès de chaque personne. Ce niveau d’accès définit ce que les personnes peuvent voir et faire avec les types d’objets et les zones du système.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 96%

---

# Fonctionnement des niveaux d’accès et des autorisations

>[!NOTE]
>
>Les informations de cet article font référence aux niveaux d’accès hérités. Pour plus d’informations sur les nouveaux niveaux d’accès, voir [Présentation des nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

L’équipe d’administration d’Adobe Workfront détermine le niveau d’accès de chaque personne. Ce niveau d’accès définit ce que les personnes peuvent voir et faire avec les types d’objets et les zones du système.

Les utilisateurs et utilisatrices ont également accès à des objets individuels lorsque d’autres personnes partagent et accordent certaines autorisations sur ces objets.


![Hiérarchie des modèles de sécurité](assets/security-model-hierachy.png)

Par exemple, si votre niveau d’accès indique que vous pouvez créer des tâches, mais que les autorisations que vous recevez sur un projet spécifique ne vous permettent pas d’y ajouter des tâches, vous ne pourrez pas ajouter de tâches dans le projet, mais uniquement ailleurs dans Workfront.

Cet article explique comment fonctionne cette combinaison.

## Niveau d’accès

Le niveau d’accès affecté à chaque personne par une équipe d’administration Workfront est nécessaire pour se connecter à Workfront.

Les niveaux d’accès par défaut sont les suivants :

* Administration système (joint à la licence Plan)
* Planification (joint à la licence Plan)
* Travail (joint à la licence Travail)
* Révision (joint à la licence Révision)
* Demande (joint à la licence Demande)
* Utilisateur ou utilisatrice externe (attaché à la licence E-mail externe)

La licence Workfront pour chaque niveau d’accès par défaut détermine ce qui est disponible et configurable dans le niveau d’accès. Pour plus d’informations sur les licences Workfront, voir la section [Vue d’ensemble des licences Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Pour les personnes qui y sont affectées, un niveau d’accès définit ce qu’elles peuvent voir et faire avec les types d’objets et les zones suivants dans Workfront :

* Projets
* Tâches
* Problèmes
* Portefeuilles
* Rapports, tableaux de bord et calendriers
* Filtres, vues et regroupements
* Documents
* Autres utilisateurs et utilisatrices
* Modèles
* Données financières
* Gestion des ressources
* Planificateur de scénarios
* Objectifs Workfront

Dans un niveau d’accès personnalisé, vous pouvez configurer les paramètres de ces objets et zones afin de modifier l’accès qu’auront les utilisateurs et utilisatrices à ces derniers. En fonction de la licence associée au niveau d’accès, ainsi que du type d’objet ou de zone, vous pouvez configurer le niveau d’accès de manière à ce qu’il n’autorise aucun accès, un accès en affichage ou un accès en modification à un objet ou à une zone.

>[!IMPORTANT]
>
>Nous vous recommandons vivement de ne pas modifier les niveaux d’accès intégrés afin que vous puissiez y faire référence après avoir configuré vos utilisateurs et utilisatrices. Pour personnaliser un niveau d’accès, copiez le niveau d’accès par défaut et modifiez la copie. (Vous pouvez procéder ainsi pour chaque niveau d’accès, à l’exception de l’administrateur ou administratrice système et de l’utilisateur ou l’utilisatrice externe.)

Pour une explication détaillée de chacun des niveaux d’accès par défaut, voir la section [Niveaux d’accès intégrés](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Pour savoir comment affecter un niveau d’accès à un utilisateur ou une utilisatrice, voir la section [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Autorisations

Lors du partage d’un objet avec une autre personne dans le système, un utilisateur ou une utilisatrice peut accorder à la personne destinataire l’une des autorisations suivantes sur l’objet.

* **Afficher** : ce niveau d’autorisation permet à la personne destinataire de partager l’objet de l’une des manières suivantes :

   * à l’échelle du système afin que l’ensemble des utilisateurs et utilisatrices puissent le voir (non disponible pour tous les objets) ;
   * avec les utilisateurs et utilisatrices externes qui n’ont pas de licence Workfront (non disponible pour tous les objets) ;
   * Avec une adresse e-mail (disponible uniquement pour les documents)

* **Contribuer** : (non disponible pour tous les objets)
* **Gérer** : lorsqu’une personne partage un objet, les droits de la personne destinataire sur l’objet sont déterminés par une combinaison de ses niveau d’accès et des autorisations accordées par la personne responsable du partage. Le niveau d’accès le plus bas disponible dans cette combinaison détermine ce que la personne destinataire peut faire avec l’objet.

  >[!INFO]
  >
  >**Exemple :** si le niveau d’accès de la personne destinataire n’autorise pas la modification du projet, cette personne ne peut ni modifier ni supprimer un projet, même si la personne à l’origine du partage lui a accordé des autorisations pour le gérer.
  >
  >Ou, si le niveau d’accès de la personne destinataire autorise la modification de projet, mais que la personne responsable accorde des autorisations de lecture seule à un projet, l’utilisateur ou l’utilisatrice ne peut pas modifier ou supprimer le projet.

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

>[!NOTE]
>
>* Si un utilisateur ou une utilisatrice partage un objet avec certaines autorisations et que cet objet a des objets enfants en dessous, la personne destinataire hérite des mêmes autorisations pour ces objets enfants.
>* Si un niveau d’accès restreint les utilisateurs et utilisatrices de supprimer certains objets, cela ne les empêche pas de supprimer les objets enfants qu’ils contiennent.
>

## Plus d’exemples de scénarios

Quand Olivia partage un projet Workfront avec Tony, l’accès de Tony à ce projet est déterminé par une combinaison de deux éléments :

* le niveau d’accès de Tony, attribué par l’administrateur ou l’administratrice Workfront ;
* les autorisations de Tony pour le projet, spécifiées par Olivia.

Les actions de Tony sur le projet peuvent être limitées davantage au projet, mais la limitation ne peut pas être outrepassée conformément à ce qui est autorisé à son niveau d’accès :

* Si le niveau d’accès de Tony ne lui permet pas de créer des tâches, il ne peut pas ajouter de tâches au projet, même si Olivia lui a donné l’autorisation d’y ajouter des tâches.
* Si le niveau d’accès de Tony lui permet de créer des tâches, mais qu’Olivia n’a pas accordé d’autorisation pour ajouter des tâches au projet, il ne peut pas ajouter de tâches à ce projet, mais il peut ajouter des tâches à d’autres projets pour lesquels il a reçu l’autorisation de le faire.
