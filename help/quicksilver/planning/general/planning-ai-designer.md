---
title: Prise en main d’Adobe Workfront Planning Designer
description: À l’aide du Designer Adobe Planning, vous pouvez générer un nouvel espace de travail, avec les types d’enregistrements et les champs dans Workfront Planning, ou ajouter des objets à un espace de travail, ou afficher l’historique des modifications sur les enregistrements.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bf34bfa2059d227eca3faa3d719adcf4d711e457
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 8%

---


# Prise en main d’Adobe Workfront Planning Designer

{{planning-important-intro}}

À l’aide du Designer Adobe Planning, vous pouvez générer un nouvel espace de travail, avec les types d’enregistrements et les champs dans Workfront Planning, ou ajouter des objets à un espace de travail, ou afficher l’historique des modifications sur les enregistrements.

>[!IMPORTANT]
>
>Actuellement, Planning Designer n’est disponible que pour les utilisateurs participant à l’étape bêta fermée.

## <!--edit theses--> des exigences d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Packages Adobe Workfront</p></td> 
   <td> 
<p>Tout package Workfront and Planning</p>
<p>Tout package Workflow et Planning</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer des autorisations relatives à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inscription au programme de Beta fermé pour Planning Designer

<!--edit this Or create a new article under Beta programs?? -->

Actuellement, vous pouvez demander à participer au programme Beta fermé pour Planning Designer.

## Considérations relatives à Planning Designer

<!--these are from the AI Assistant - edit these-->

* Pour utiliser Planning Designer, vous devez d’abord activer l’assistant d’IA pour votre entreprise. Les éléments suivants doivent être activés pour que l’assistant AI soit disponible pour tous les membres de votre organisation :

   * L’assistant AI doit être activé pour votre organisation avant d’être disponible pour les utilisateurs de votre entreprise. Pour plus d’informations, voir [ Présentation de l’assistant AI ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
   * Une fois que Workfront a activé l’assistant AI pour votre organisation, il est disponible pour l’administrateur Workfront principal. Pour plus d’informations, voir [Configurer les informations de base de votre système](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

   * L’administrateur Workfront doit activer l’assistant AI pour tous les autres utilisateurs. Pour plus d’informations, voir [Activer ou désactiver l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

   * L’assistant d’IA fonctionne dans le contexte de chaque page. Les requêtes que vous envoyez pour l’assistant AI doivent faire référence à la fonctionnalité disponible dans la page que vous avez ouverte.

* Pour utiliser Planning Designer, un administrateur système doit l&#39;activer dans les Préférences système de votre configuration.

* Les actions effectuées par l’assistant AI dans la zone Planning s’inscrivent dans le cadre de vos autorisations Workfront Planning et de votre niveau d’accès Workfront. Pour plus d’informations, voir les articles suivants :

   * [Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Les modifications apportées par l’assistant AI au nom de l’utilisateur sont suivies dans le panneau Historique de l’enregistrement.

* Vous pouvez utiliser des commandes pour annuler vos actions. Par exemple, vous pouvez taper « Annuler la dernière modification » pour annuler votre modification.

* Lors de la création, de la mise à jour ou de la suppression d’un objet par le biais de l’assistant AI, celui-ci affiche les actions prévues et demande confirmation. Vous pouvez ensuite confirmer ou annuler les actions.

—>

## Fonctionnalité actuellement disponible pour Planning Designer

<!--edit these- they are from the Ai Assistant: 

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted

-->

Vous pouvez utiliser Planning Designer ou l&#39;assistant AI pour effectuer l&#39;une des actions suivantes :

* Création et configuration des espaces de travail

* Créer des types d’enregistrement

* Champs de conception ou champs de formule

* Créer, supprimer, dupliquer et restaurer des enregistrements

* Modifier, mettre à jour, ajouter un champ dans un enregistrement

* Lier des enregistrements à d&#39;autres enregistrements

* Accéder à l’historique des modifications d’enregistrement

* Créer des vues personnalisées

* Créer des enregistrements en important un document. La création d&#39;enregistrements à partir d&#39;un document importé n&#39;est disponible que dans Planning Designer et non dans l&#39;assistant AI. <!--add information about supported files-->

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Recherchez le Designer Planning dans Workfront Planning

Vous pouvez accéder à Planning Designer à partir de la page principale de Workfront Planning.

<!--add screen shot-->

Vous pouvez également utiliser l&#39;assistant AI pour tirer parti des mêmes fonctionnalités que Planning Designer.

## Activation de Planning Designer pour votre organisation

En tant qu’administrateur ou administratrice Workfront, vous devez d’abord activer Planning Designer pour votre organisation.

<!--add steps here-->

## Créer ou mettre à jour des objets à l&#39;aide de Planning Designer

Sauf indication contraire, vous pouvez créer ou mettre à jour des objets dans Workfront Planning à l&#39;aide du Designer Planning ou de l&#39;assistant AI.

1. Connectez-vous à Workfront, puis cliquez sur l’icône **Menu principal** ![Menu principal Points](assets/dots-main-menu.png) dans le coin supérieur droit de l’écran, ou sur l’icône **Menu principal** ![Menu principal Lignes](assets/lines-main-menu.png) dans le coin supérieur gauche, le cas échéant.

1. Cliquez sur **Planification**. La zone Planification s’ouvre.

1. Cliquez sur **Créer à l’aide de l’IA**.

1. Dans l’espace prévu à cet effet, commencez à saisir les commandes de l’assistant d’IA, puis cliquez sur Entrée lorsque vous avez terminé.

   <!--add screen shot-->

   Par exemple, vous pouvez saisir une requête similaire à celles ci-dessous :

   * Créer et configurer un espace de travail avec cinq types d’enregistrements pour gérer les campagnes

   * Créer des campagnes marketing pour chaque mois de l’année en cours

   * Ajout d’un champ de campagne pour le statut de l’espace de travail Conception marketing

   * Supprimer tous les enregistrements dont le statut est Périmé

   * Mettre à jour toutes les campagnes Planning avec le statut Actif

   * Connecter des campagnes à des rôles dans l’espace de travail de conception marketing

   * Afficher l’historique des modifications apportées à la campagne « Saint-Valentin »

   * Créer une vue chronologique pour les campagnes dans l’espace de travail de conception marketing

   * Créer des enregistrements en important un document. La création d&#39;enregistrements à partir d&#39;un document importé n&#39;est disponible que dans Planning Designer et non dans l&#39;assistant AI.

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

   Un aperçu visuel s’affiche avec un exemple de ce que l’assistant peut créer.

1. Après avoir reçu une réponse réussie, suivez les liens fournis dans la ligne de commande pour créer, mettre à jour ou réviser l’objet de votre requête.




