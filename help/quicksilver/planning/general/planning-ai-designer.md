---
title: Prise en main d’Adobe Workfront Planning Designer
description: À l’aide du Designer Adobe Planning, vous pouvez générer un nouvel espace de travail, avec les types d’enregistrements et les champs dans Workfront Planning, ajouter des objets à un espace de travail ou afficher l’historique des modifications sur les enregistrements.
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 866b237db5d109b0a435145119a6412e41d960ab
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 6%

---


<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# Prise en main d’Adobe Workfront Planning Designer

{{planning-important-intro}}

Vous pouvez utiliser Adobe Planning Designer optimisé par l’IA pour générer un nouvel espace de travail, ajouter des objets à un espace de travail (types d’enregistrements, enregistrements, vues ou champs) ou afficher l’historique des modifications sur les enregistrements.

>[!IMPORTANT]
>
>Planning Designer est actuellement disponible uniquement pour les utilisateurs participant au programme de Beta fermé.

Pour plus d’informations sur Workfront Planning, consultez les articles suivants :

* [Informations générales sur Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Présentation de l’accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)


## Conditions d’accès

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

* Pour utiliser Planning Designer, votre entreprise doit répondre aux exigences requises pour utiliser l’assistant d’IA Workfront.

  Pour plus d’informations, consultez [Conditions préalables pour l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

* Pour utiliser Planning Designer, un administrateur système doit l&#39;activer dans les Préférences système de votre configuration.

* Vous pouvez utiliser des invites pour créer des objets Planning à l&#39;aide de l&#39;assistant IA dédiée à Workfront de la zone Planning ou à l&#39;aide du Designer Planning.

* Les actions effectuées par l&#39;assistant AI dans la zone Planning ou celles effectuées par le Designer Planning s&#39;inscrivent dans le cadre de vos autorisations Workfront Planning et de votre niveau d&#39;accès Workfront.

  Pour plus d’informations, voir les articles suivants :

   * [Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Les modifications apportées par Planning Designer pour le compte de l&#39;utilisateur sont suivies dans le panneau Historique de l&#39;enregistrement.

* Vous pouvez utiliser des commandes pour annuler vos actions. Par exemple, vous pouvez taper « Annuler la dernière modification » pour annuler votre modification.

* Lors de la création, de la mise à jour ou de la suppression d&#39;un objet par le biais de Planning Designer, les actions prévues sont affichées et une confirmation est demandée. Vous pouvez ensuite confirmer ou annuler les actions.

* Lorsque vous créez des espaces de travail et des types d&#39;enregistrements à l&#39;aide de Planning Designer, les vues et les champs sont également créés automatiquement.

## Fonctionnalité actuellement disponible pour Planning Designer

Vous pouvez utiliser Planning Designer ou l&#39;assistant AI pour effectuer l&#39;une des actions suivantes :

* Création et configuration des espaces de travail

* Créer des types d’enregistrement

* Champs de conception ou champs de formule

* Créer, supprimer, dupliquer et restaurer des enregistrements

* Modifier, mettre à jour, ajouter un champ dans un enregistrement

* Lier des enregistrements à d&#39;autres enregistrements

* Accéder à l’historique des modifications d’enregistrement

* Créer des vues personnalisées

* Créer des enregistrements en important un document.

  La création d&#39;enregistrements à partir d&#39;un document importé n&#39;est disponible que dans Planning Designer et non dans l&#39;assistant AI.

  Pour plus d’informations sur les types et tailles de fichiers acceptés, consultez la section « Mécanismes de sécurisation du document » de l’article [Utiliser le remplissage de formulaire optimisé par l’IA pour remplir une demande à l’aide d’invites ou de documents](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Activation de Planning Designer pour votre organisation

En tant qu’administrateur ou administratrice Workfront, vous devez d’abord activer Planning Designer pour votre organisation.

<!--add steps here-->

1. Connectez-vous à Workfront en tant qu’administrateur système.
1. Cliquez sur **Menu principal** ![Icône du menu principal](assets/main-menu-shell.png) dans le coin supérieur gauche de l’écran, puis cliquez sur **Configuration**.
1. Cliquez sur **Système** > dans le panneau de gauche, puis accédez à la zone **Préférences IA**.
1. Activez les paramètres suivants :
   * **Activer AI**
   * **S’inscrire aux versions bêta de l’IA**
   * **Planning Designer**

   ![Paramètre Planning Designer dans les Préférences système](assets/planning-designer-toggle-in-system-preferences.png)
1. Cliquer sur **Enregistrer**.

   Tous les utilisateurs du système qui disposent d’une licence Standard peuvent désormais voir le bouton **Concevoir avec l’IA** sur la page principale Espaces de travail de la zone Planning. <!--check screen shot-->

   ![Bouton Conception avec IA sur la page Espaces de travail](assets/design-with-ai-button-on-workspaces-page.png)

   Tous les utilisateurs peuvent désormais démarrer et utiliser Planning Designer pour créer et mettre à jour des objets Workfront Planning.

## Créer ou mettre à jour des objets à l&#39;aide de Planning Designer

Sauf indication contraire, vous pouvez créer ou mettre à jour des objets dans Workfront Planning à l&#39;aide du Designer Planning ou de l&#39;assistant AI.

1. Connectez-vous à Workfront, puis cliquez sur l’icône **Menu principal** ![Menu principal Lignes](assets/lines-main-menu.png) dans le coin supérieur gauche.

1. Cliquez sur **Planification**. La zone Planification s’ouvre.

1. Cliquez sur **Créer à l’aide de l’IA**.

   La fenêtre **Planning Designer** s&#39;ouvre.

   ![Fenêtre Planning Designer](assets/planning-designer-window.png)

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

1. Après avoir reçu une réponse réussie, suivez les liens fournis dans la zone d’invite pour créer, mettre à jour ou réviser l’objet de votre requête.

   Lorsque vous acceptez de créer vos objets, vos modifications s&#39;affichent à droite de la zone d&#39;invite.

   Vous pouvez vérifier les espaces de travail, les types d’enregistrements, les champs, les vues et les enregistrements dans la zone d’aperçu à droite de l’invite.
1. (Facultatif) Saisissez des invites supplémentaires pour modifier davantage vos objets.
1. (Facultatif) Cliquez sur l’icône **Activer/désactiver l’écran d’aperçu d’AI Workspace** ![Masquer ou afficher l’icône de l’écran d’aperçu](assets/hide-show-preview-screen-in-planning-designer.png) pour ouvrir ou fermer l’écran d’aperçu à droite.
1. Cliquez sur l’icône **Ouvrir l’espace de travail dans un nouvel onglet** ![Ouvrir l’espace de travail dans un nouvel onglet](assets/open-workspace-on-new-tab-icon.png) pour ouvrir l’espace de travail que vous mettez à jour dans un nouvel onglet.
1. Cliquez sur l’icône **Fermer** **X** pour fermer Planning Designer et ouvrir la zone Espaces de travail.
1. Ouvrez l&#39;espace de travail que vous avez modifié à l&#39;aide de Planning Designer et apportez d&#39;autres modifications à ses objets.




