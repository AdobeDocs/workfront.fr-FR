---
title: Fonctionnement des niveaux d’accès et des autorisations
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,model,funnel,diagramme,levels,permissions
navigation-topic: access-levels
description: L’administrateur Adobe Workfront détermine le niveau d’accès que chaque utilisateur doit avoir. Ce niveau d’accès définit ce que les utilisateurs peuvent voir et faire avec les types d’objets et les zones du système.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: 1bd454246419e199e5cfd0d8d1d73cd30c0b13b1
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 1%

---

# Fonctionnement des niveaux d’accès et des autorisations hérités

L’administrateur Adobe Workfront détermine le niveau d’accès que chaque utilisateur doit avoir. Ce niveau d’accès définit ce que les utilisateurs peuvent voir et faire avec les types d’objets et les zones du système.

En outre, les utilisateurs ont accès à des objets individuels lorsque d’autres utilisateurs partagent et accordent certaines autorisations sur ces objets.

Ainsi, les activités qu’un utilisateur peut effectuer avec un objet sont définies par une combinaison de leur niveau d’accès et des autorisations qui leur sont accordées pour ce projet.

![](assets/security-model-hierachy.png)

Par exemple, si votre niveau d’accès indique que vous pouvez créer des tâches, mais que les autorisations que vous recevez sur un projet spécifique ne vous permettent pas d’y ajouter des tâches, vous ne pouvez pas ajouter de tâches sur le projet même si vous pouvez créer des tâches ailleurs dans Workfront.

Cet article explique le fonctionnement de cette combinaison.

## Niveau d’accès hérité

Le niveau d’accès attribué à chaque utilisateur par un administrateur Workfront est requis pour se connecter à Workfront.

Les niveaux d’accès hérités par défaut sont les suivants :

* Administrateur système (joint à la licence Plan)
* Planificateur (joint à la licence Plan)
* Worker (joint à la licence de travail)
* Réviseur (joint à la licence de révision)
* Demandeur (joint à la licence de demande)
* Utilisateur externe (joint à la licence de courrier électronique externe)

La licence Workfront pour chaque niveau d’accès par défaut détermine ce qui est disponible et configurable au niveau d’accès. Pour plus d’informations sur les licences Workfront, voir [Présentation des licences Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Pour les utilisateurs qui y sont affectés, un niveau d’accès définit ce qu’ils peuvent voir et faire avec les types d’objets et zones suivants dans Workfront :

* Projets
* Tâches
* Événements
* Portefeuilles
* Rapports, tableaux de bord et calendriers
* Filtres, vues et regroupements
* Documents
* Autres utilisateurs
* Modèles
* Données financières
* Gestion des ressources
* Planificateur de scénarios
* Objectifs Workfront

Dans un niveau d’accès personnalisé, vous pouvez configurer les paramètres de ces objets et zones afin de modifier le niveau d’accès des utilisateurs à ces objets. En fonction de la licence associée au niveau d’accès, ainsi que du type de l’objet ou de la zone, vous pouvez configurer le niveau d’accès pour ne pas autoriser l’accès, l’affichage ou la modification de l’accès à un objet ou à une zone.

>[!IMPORTANT]
>
>Nous vous recommandons vivement de ne pas modifier les niveaux d’accès intégrés afin que vous puissiez y faire référence après avoir configuré vos utilisateurs. Pour personnaliser un niveau d&#39;accès, copiez le niveau d&#39;accès par défaut et modifiez la copie. (Vous pouvez le faire pour chaque niveau d’accès, à l’exception de l’administrateur système et de l’utilisateur externe.)

Pour une explication détaillée de chacun des niveaux d’accès par défaut, voir [Niveaux d’accès intégrés dans Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Pour obtenir des instructions sur l’attribution d’un niveau d’accès à un utilisateur, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Autorisations

Lors du partage d’un objet avec une personne du système, un utilisateur peut accorder au destinataire l’une des autorisations suivantes sur l’objet.

* **Affichage**: Ce niveau d&#39;autorisation permet au destinataire de partager l&#39;objet de l&#39;une des manières suivantes :

   * à l’échelle du système afin que tous les utilisateurs puissent le voir (non disponible pour tous les objets) ;
   * Avec les utilisateurs externes qui n’ont pas de licence Workfront (non disponible pour tous les objets)
   * Avec une adresse électronique (disponible uniquement pour les documents)

* **Contribution**: (non disponible pour tous les objets)
* **Gérer**: Lorsqu’une personne partage un objet, les droits du destinataire sur l’objet sont déterminés par une combinaison du niveau d’accès du destinataire et des autorisations accordées par le responsable du partage. Le niveau d’accès le plus bas disponible dans cette combinaison détermine ce que le destinataire peut faire avec l’objet.

   >[!INFO]
   >
   >**Exemple :** Si le niveau d’accès du destinataire n’autorise pas la modification de projet, cette personne ne peut pas modifier ni supprimer un projet, même si le responsable du partage lui a accordé des autorisations pour le gérer.
   >
   >Ou, si le niveau d’accès du destinataire autorise la modification de projet, mais que le responsable accorde des autorisations d’affichage uniquement à un projet, l’utilisateur ne peut pas modifier ou supprimer le projet.

Le tableau suivant compare l’accès général d’un utilisateur aux objets (défini par le niveau d’accès de l’utilisateur) aux autorisations d’un objet partagé spécifique :

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
   <td>Accordée par un administrateur Workfront au niveau d’accès d’un utilisateur</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Accordée par un utilisateur partageant un objet au niveau de l’objet</td> 
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
>* Si un utilisateur partage un objet avec certaines autorisations et que cet objet a des objets enfants en dessous, le destinataire hérite des mêmes autorisations pour ces objets enfants.
>* Si un niveau d’accès limite la suppression de certains objets par les utilisateurs, cela ne les empêche pas de supprimer les objets enfants qu’ils contiennent.
>


## Autres scénarios d’exemple

Quand Olivia partage un projet Workfront avec Tony, l&#39;accès de Tony à ce projet est déterminé par une combinaison de deux éléments :

* Niveau d’accès de Tony, attribué par l’administrateur Workfront
* Autorisations de Tony pour le projet, spécifiées par Olivia

Les actions de Tony sur le projet peuvent être limitées davantage au projet, mais elles ne peuvent pas être illimitées au-delà de ce qui est autorisé à son niveau d&#39;accès :

* Si le niveau d&#39;accès de Tony ne lui permet pas de créer des tâches, il ne peut pas ajouter de tâches au projet, même si Olivia lui a donné l&#39;autorisation d&#39;y ajouter des tâches.
* Si le niveau d’accès de Tony lui permet de créer des tâches, mais qu’Olivia n’a pas accordé d’autorisation pour ajouter des tâches au projet, il ne peut pas ajouter de tâches à ce projet, mais il peut ajouter des tâches à d’autres projets pour lesquels il a reçu l’autorisation de le faire.
