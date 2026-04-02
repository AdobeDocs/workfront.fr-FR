---
title: Accorder l’accès aux données financières
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: En tant que personne chargée de l’administration d’Adobe Workfront, vous pouvez définir l’accès d’un utilisateur ou d’une utilisatrice aux données financières dans Workfront par le biais de son niveau d’accès.
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: dfc6344303f33a9c3c89837b759235612e54904e
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 49%

---


# Accorder l’accès aux cartes tarifaires

{{highlighted-preview-article-level}}

En tant qu’administrateur Adobe Workfront, vous pouvez définir l’accès d’un utilisateur aux cartes tarifaires par le biais de son niveau d’accès, comme expliqué dans la section [Présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Pour plus d’informations sur les cartes tarifaires, voir [Gérer les cartes tarifaires](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à l’octroi de l’accès aux cartes tarifaires

Tenez compte des points suivants lors de l’octroi de l’accès aux cartes tarifaires dans Workfront :

* Les utilisateurs doivent disposer d’un accès en modification aux cartes tarifaires, aux projets et aux données financières pour joindre une carte tarifaire à un projet.
* Les utilisateurs n’ayant pas accès aux cartes tarifaires et ayant un accès Modifier aux données financières ne peuvent pas joindre de carte tarifaire à un projet, mais ils peuvent modifier d’autres taux de facturation du projet provenant d’autres sources.

## Configurer l’accès utilisateur pour évaluer les cartes à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou à modifier le niveau d’accès, comme expliqué dans la section [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** à droite des cartes tarifaires, puis sélectionnez les capacités que vous souhaitez accorder sous **Ajuster vos paramètres**.

   ![Ajuster l’accès par carte tarifaire](assets/rate-card-access-fine-tune.png)

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et domaines dans le niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), par exemple [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’attribuer à un utilisateur ou à une utilisatrice. Pour plus d’informations, voir [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accès aux cartes à taux partagé

Vous pouvez partager une carte tarifaire avec d’autres utilisateurs en leur accordant des autorisations, comme expliqué dans la section [Partager une carte tarifaire](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md).

Lorsque vous partagez un objet avec un autre utilisateur ou une autre utilisatrice, les droits des personnes destinataires sur cet objet sont déterminés par une combinaison de deux éléments :

* Les autorisations que vous accordez à votre personne destinataire pour l’objet.
* Les paramètres du niveau d’accès des personnes destinataires pour le type d’objet.
