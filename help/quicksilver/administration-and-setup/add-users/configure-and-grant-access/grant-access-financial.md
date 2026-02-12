---
title: Accorder l’accès aux données financières
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: En tant que personne chargée de l’administration d’Adobe Workfront, vous pouvez définir l’accès d’un utilisateur ou d’une utilisatrice aux données financières dans Workfront par le biais de son niveau d’accès.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: 97f5adc8811a3be7be23137a82d10d45b76ec605
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 94%

---

# Accorder l’accès aux données financières

{{highlighted-preview}}

En tant que personne chargée de l’administration d’Adobe Workfront, vous pouvez définir l’accès d’un utilisateur ou d’une utilisatrice aux éléments suivants par le biais de leur niveau d’accès, comme expliqué dans [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) :

* Informations financières sur les projets dans Workfront
* Informations sur la budgétisation des ressources dans les outils de planification des ressources

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
    <p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à l’octroi de l’accès aux données financières

Tenez compte des éléments suivants lorsque vous accordez aux utilisateurs et aux utilisatrices l’accès aux données financières dans Workfront :

* Un utilisateur dont le niveau d’accès ne permet pas d’accéder aux données financières ne peut pas accorder un accès qui permettrait à d’autres utilisateurs d’afficher les données financières. Cela inclut l’accès aux projets qui afficheraient des données financières ou la modification d’un niveau d’accès pour permettre l’affichage des données financières.
* Un utilisateur ou une utilisatrice dont le niveau d’accès ne permet pas d’accéder aux données financières ne peut pas créer de risque pour un projet. Pour plus d’informations, consultez la section [Créer et modifier les risques sur les projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* Vous pouvez également utiliser un niveau d’accès pour déterminer les activités de gestion des ressources qu’un utilisateur ou une utilisatrice peut utiliser pour budgétiser ou visualiser l’allocation des ressources. Pour plus d’informations, consultez la section [Accorder l’accès à la gestion des ressources](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Configurer l’accès des utilisateurs et des utilisatrices aux données financières à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou à modifier le niveau d’accès, comme expliqué dans la section [Créer ou modifier les niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** à droite de « Données financières », puis sélectionnez les capacités que vous souhaitez accorder dans **Ajuster vos paramètres**.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (Facultatif) Dans la zone **Autoriser l’accès administratif pour**, sélectionnez les options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Taux de change</td> 
      <td> <p>Ajouter une nouvelle devise dans Workfront</p> <p>Sans cet accès, l’utilisateur et utilisatrice peuvent uniquement ajouter une devise existante à un projet qu’ils créent.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td> <p>Afficher toutes les dépenses sur les objets dans Workfront.</p> <p>Cela ne permet pas à l’utilisateur ou utilisatrice de créer de nouveaux types de dépenses.</p> <p>Sans cet accès, l’utilisateur et l’utilisatrice ne peuvent afficher que les éléments suivants :</p> 
       <ul> 
        <li>Dépenses sur les projets, tâches ou problèmes qu’ils gèrent.</li> 
        <li>Leurs propres dépenses.</li> 
        <li>Les dépenses de leurs subordonnés.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et domaines dans le niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), par exemple [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’attribuer à un utilisateur ou à une utilisatrice. Pour plus d’informations, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accéder aux informations financières partagées

Vous pouvez partager des informations financières sur un projet, une tâche ou un problème avec d’autres utilisateurs et utilisatrices en leur accordant des autorisations, comme expliqué dans la section [Partager des autorisations financières sur un objet](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Lorsque vous partagez un objet avec un autre utilisateur ou une autre utilisatrice, les droits des personnes destinataires sur cet objet sont déterminés par une combinaison de deux éléments :

* Les autorisations que vous accordez à votre personne destinataire pour l’objet.
* Les paramètres du niveau d’accès des personnes destinataires pour le type d’objet.

## Accéder aux informations financières par type de licence

Pour plus d’informations sur ce que les utilisateurs et les utilisatrices de chaque niveau d’accès peuvent faire avec les informations financières, consultez la section [Données financières](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accéder aux informations financières par paramètre

Les informations suivantes peuvent vous aider à comprendre comment utiliser les paramètres du niveau d’accès pour contrôler l’accès des utilisateurs et des utilisatrices aux données financières.

### Pas d’accès

Un utilisateur ou une utilisatrice n’ayant pas accès aux données financières n’a pas accès aux éléments suivants :

* Section Finance sous les objets Projet et Tâche
* Business case
* Taux de facturation et enregistrements de facturation
* <span class="preview">Cartes tarifaires</span>
* Coût par heure et facturation par heure selon les préférences de l’utilisateur ou de l’utilisatrice

  Vous pouvez configurer cette fonction à l’aide de l’icône en forme d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Afficher à l’étape 4 ci-dessus.

* Coût par heure et facturation par heure pour les fonctions

  Vous pouvez configurer cette fonction à l’aide de l’icône en forme d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Afficher à l’étape 4 ci-dessus.

### Accès en affichage

Un utilisateur ou une utilisarice ayant un accès Afficher aux données financières peut afficher (et non modifier) les éléments suivants :

* Section Finance sous les objets Projet et Tâche
* Business case
* Taux de facturation et enregistrements de facturation
* Coût par heure et facturation par heure selon les préférences de l’utilisateur ou de l’utilisatrice

  Vous pouvez configurer cette fonction à l’aide de l’icône en forme d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Afficher à l’étape 4 ci-dessus.

* Coût par heure et facturation par heure pour les fonctions

  Vous pouvez configurer cette fonction à l’aide de l’icône en forme d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Afficher à l’étape 4 ci-dessus.

### Accès en modification

Un utilisateur ou une utilisatrice ayant accès à la modification des données financières peut afficher et modifier les éléments suivants :

* Section Finance sous les objets Projet et Tâche
* Business case
* Taux de facturation et enregistrements de facturation
* <span class="preview">Cartes tarifaires</span>
* Coût par heure et facturation par heure selon les préférences de l’utilisateur ou de l’utilisatrice

  Vous pouvez configurer cela en utilisant l’icône en forme d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Modifier à l’étape 4 ci-dessus.

* Coût par heure et facturation par heure pour les fonctions

  Vous pouvez configurer cela en utilisant l’icône en forme d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Modifier à l’étape 4 ci-dessus.
