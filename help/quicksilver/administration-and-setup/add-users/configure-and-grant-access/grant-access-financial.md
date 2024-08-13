---
title: Accorder l’accès aux données financières
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur Adobe Workfront, vous pouvez définir l’accès d’un utilisateur aux données financières dans Workfront par le biais de son niveau d’accès.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 9%

---

# Accorder l’accès aux données financières

{{highlighted-preview}}

En tant qu’administrateur Adobe Workfront, vous pouvez définir l’accès d’un utilisateur aux éléments suivants par le biais du niveau d’accès de l’utilisateur, comme expliqué dans la [présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) :

* Informations financières sur les projets dans Workfront
* Informations sur la budgétisation des ressources dans les outils de planification des ressources

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Considérations relatives à l’accès aux données financières

Tenez compte des points suivants lorsque vous accordez aux utilisateurs l’accès aux données financières dans Workfront :

* Un utilisateur dont le niveau d’accès n’autorise pas l’accès aux données financières ne peut pas créer de risque pour un projet. Pour plus d’informations, voir [Création et modification des risques sur les projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* Vous pouvez également utiliser un niveau d’accès pour déterminer les activités de gestion des ressources qu’un utilisateur peut utiliser pour budgéter ou afficher l’allocation des ressources. Pour plus d’informations, voir [Accorder l’accès à la gestion des ressources](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Configurer l’accès des utilisateurs aux données financières à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d&#39;accès, comme expliqué dans la section [Créer ou modifier des niveaux d&#39;accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton **Afficher** ou **Modifier** à droite des données financières, puis sélectionnez les fonctionnalités que vous souhaitez accorder sous **Ajuster vos paramètres**.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (Facultatif) Dans la zone **Autoriser l’accès administratif pour**, sélectionnez les options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Taux de change</td> 
      <td> <p>Ajoutez une nouvelle devise dans Workfront.</p> <p>Sans cet accès, l’utilisateur peut uniquement ajouter une devise existante à un projet qu’il crée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td> <p>Afficher toutes les dépenses sur les objets dans Workfront.</p> <p>Cela ne permet pas à l’utilisateur de créer de nouveaux types de dépenses.</p> <p>Sans cet accès, l'utilisateur ne peut visualiser que les éléments suivants :</p> 
       <ul> 
        <li>Dépenses sur les projets, tâches ou problèmes qu'ils gèrent</li> 
        <li>Leurs propres dépenses</li> 
        <li>Les dépenses de leurs subordonnés</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), tel que [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’affecter à un utilisateur. Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Accès aux informations financières partagées

Vous pouvez partager des informations financières sur un projet, une tâche ou un problème avec d’autres utilisateurs en leur accordant des autorisations, comme expliqué dans la section [Partager des autorisations financières sur un objet](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Lorsque vous partagez un objet avec un autre utilisateur, les droits du destinataire le concernant sont déterminés par une combinaison de deux éléments :

* Autorisations que vous accordez à votre destinataire pour l’objet
* Paramètres du niveau d&#39;accès du destinataire pour le type d&#39;objet

## Accès aux informations financières par type de licence

Pour plus d’informations sur ce que les utilisateurs de chaque niveau d’accès peuvent faire avec les informations financières, reportez-vous à la section [Données financières](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) de l’article [Fonctionnalité disponible pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accès aux informations financières en définissant

Les informations suivantes peuvent vous aider à comprendre comment utiliser les paramètres de niveau d’accès pour contrôler l’accès des utilisateurs aux données financières.

### Pas d’accès

Un utilisateur n’ayant pas accès aux données financières n’a pas accès aux éléments suivants :

* Section Finance sous Objets de projet et de tâche
* Analyse de cas
* Taux de facturation et enregistrements de facturation
* <span class="preview">Carte de taux</span>
* Coût par heure et facturation par heure selon les préférences de l’utilisateur

  Vous pouvez le configurer à l’aide de l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Afficher à l’étape 4 ci-dessus.

* Coût par heure et facturation par heure sur les rôles de tâche

  Vous pouvez le configurer à l’aide de l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Afficher à l’étape 4 ci-dessus.

### Accès aux vues

Un utilisateur disposant d’un accès en mode Affichage aux données financières peut afficher (et non modifier) les éléments suivants :

* Section Finance sous Objets de projet et de tâche
* Analyse de cas
* Taux de facturation et enregistrements de facturation
* Coût par heure et facturation par heure selon les préférences de l’utilisateur

  Vous pouvez le configurer à l’aide de l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Afficher à l’étape 4 ci-dessus.

* Coût par heure et facturation par heure sur les rôles de tâche

  Vous pouvez le configurer à l’aide de l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Afficher à l’étape 4 ci-dessus.

### Modifier l’accès

Un utilisateur disposant de l’accès Modifier aux données financières peut afficher et modifier les éléments suivants :

* Section Finance sous Objets de projet et de tâche
* Analyse de cas
* Taux de facturation et enregistrements de facturation
* <span class="preview">Carte de taux</span>
* Coût par heure et facturation par heure selon les préférences de l’utilisateur

  Vous pouvez le configurer à l’aide de l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Modifier de l’étape 4 ci-dessus.

* Coût par heure et facturation par heure sur les rôles de tâche

  Vous pouvez le configurer à l’aide de l’icône d’engrenage ![](assets/gear-icon-settings.png) sur le bouton Modifier de l’étape 4 ci-dessus.
