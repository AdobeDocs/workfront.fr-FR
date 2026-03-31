---
product-area: requests
navigation-topic: create-requests
title: Supprimer une demande envoyée ou un brouillon de demande
description: Vous pouvez supprimer des demandes envoyées ou des brouillons de demandes dans Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 26%

---

# Supprimer une requête envoyée ou un brouillon de requête

Vous pouvez supprimer les demandes envoyées par Adobe Workfront ou Adobe Workfront Planning ou les brouillons de demandes que vous avez créés ou pour lesquels vous disposez d’autorisations de niveau Gérer.

Les administrateurs Workfront et les responsables de l’espace de travail Workfront Planning peuvent également supprimer les demandes et demander les brouillons qu’ils n’ont pas créés.

Vous ne pouvez pas afficher les demandes Planning dans l’expérience des demandes héritées.

Cet article décrit comment supprimer des brouillons de demandes dans la nouvelle expérience de demande. La suppression de demandes Workfront et Planning ou de leurs brouillons est identique.

Pour plus d’informations, voir :

* [Créer et soumettre des demandes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [Créer des demandes à partir de brouillons](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)
* [Envoyer des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tout package de Workfront ou de workflow</p>

<p>Tout package Workfront Planning permettant de gérer les demandes Planning </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Contributeur ou supérieur</p>
   <p>Requête ou supérieure</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront ou un responsable d'espace de travail Planning pour supprimer les requêtes que vous n'avez pas créées.</p><p>Vous devez disposer d'un accès en modification aux événements.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Vous devez avoir créé la demande ou le brouillon pour la supprimer dans la nouvelle expérience de demande, ou être un administrateur Workfront ou un responsable de l’espace de travail Planning pour supprimer les brouillons des demandes que vous n’avez pas envoyées.
   </p><p>Vous devez disposer d’autorisations de modification pour les événements que vous supprimez.</p>  </td> 
  </tr>

</tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Supprimer des requêtes ou des brouillons de requêtes dans la nouvelle expérience de requête

Vous pouvez supprimer des requêtes et des brouillons dans les zones suivantes :

* Dans la zone Demandes de Workfront
* Dans le widget Mes requêtes de l’Accueil
* À partir d’une page de requête

Les utilisateurs suivants peuvent supprimer des brouillons de demande :

* Les administrateurs Workfront peuvent supprimer les demandes et les brouillons qu’ils ou d’autres personnes ont envoyés.
* Les gestionnaires de l&#39;espace de travail Planning de Workfront peuvent supprimer des demandes et des brouillons dans l&#39;espace de travail Planning qu&#39;ils administrent.
* Les utilisateurs peuvent supprimer les demandes et les brouillons qu’ils ont envoyés.

### Supprimez une demande ou un brouillon de la zone des Demandes ou du widget Mes demandes dans l’Accueil.

{{step1-to-requests}}

1. Pour accéder au widget **Mes requêtes** dans **Accueil** :

   {{step1-to-home}}

   1. Recherchez le widget **Mes requêtes**.

      Pour plus d’informations sur le widget **Mes requêtes**, voir [Utiliser le widget Mes requêtes](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Dans la liste **Demandes** ou le widget **Mes demandes** de l’**Accueil**, pointez sur la demande ou le brouillon à supprimer, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png)

1. Cliquez sur **Supprimer**

   Ou

   Cliquez avec le bouton droit sur la demande sélectionnée, puis cliquez sur **Supprimer**.

   >[!TIP]
   >
   >Lorsque vous n’avez pas accès à la création des problèmes, vous recevez un avertissement indiquant que votre administrateur ou administratrice vous a interdit de créer des demandes.

1. Dans la boîte de dialogue qui s’ouvre, cliquez sur **Supprimer**.

   La demande ou le brouillon est supprimé.

   Les demandes supprimées sont enregistrées dans la corbeille et un administrateur Workfront peut les récupérer pendant 30 jours au maximum. Impossible de récupérer les brouillons.

### Supprimer en bloc des requêtes d’une liste

{{step1-to-requests}}

1. Pour accéder au widget **Mes requêtes** dans **Accueil** :

   {{step1-to-home}}

   1. Recherchez le widget **Mes requêtes**.

      Pour plus d’informations sur le widget Mes requêtes, voir [Utiliser le widget Mes requêtes](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Dans la liste **Demandes** ou le widget **Mes demandes**, cliquez sur la case à gauche de chaque demande à supprimer.
1. Dans la barre bleue située en bas de la page, cliquez sur **Supprimer**.

   >[!NOTE]
   >
   >Si l’option **Supprimer** n’est pas visible dans la barre bleue, vous n’êtes pas autorisé à supprimer une ou plusieurs des requêtes sélectionnées.

### Conditions préalables à la suppression des brouillons de demande

Vous devez effectuer les opérations suivantes avant de pouvoir supprimer un brouillon de demande :

* Commencez à créer une demande. Cette opération enregistre automatiquement la demande sous forme de brouillon dans la section Brouillons.

  Pour plus d’informations sur la création de demandes, voir la section [Créer et envoyer des demandes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Supprimer les brouillons de demande dans l’expérience de demande héritée

Vous pouvez supprimer des demandes rédigées après qu’elles ont été enregistrées en tant que brouillons si vous ne les trouvez plus pertinentes. Vous ne pouvez pas récupérer les brouillons de demande supprimés.

Vous ne pouvez pas accéder aux demandes Planning ou à leurs brouillons à partir de l’expérience de demande héritée.

{{step1-to-requests}}

1. Cliquez sur **Brouillons** dans le panneau de gauche.

   Tous les brouillons de toutes les files d’attente des demandes s’affichent dans cette liste.

1. Sélectionnez un brouillon dans la liste, puis cliquez sur **Supprimer** en haut de la liste.
1. Cliquez sur **Oui, supprimer**.

   Le brouillon est supprimé et ne peut pas être récupéré.






