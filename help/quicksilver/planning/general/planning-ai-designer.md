---
title: Prise en main d’Adobe Workfront Planning Designer
description: Vous pouvez utiliser Adobe Planning Designer optimisé par l’IA pour configurer facilement vos espaces de travail et vos structures de données. Planning Designer prend en charge de nombreux éléments, de la création et la configuration des espaces de travail à la définition de champs et de formules, la gestion des enregistrements, la révision de l'historique des modifications et la création de vues personnalisées. Utilisé directement ou par l’intermédiaire de l’assistant d’IA, Planning Designer offre un environnement flexible et puissant pour créer et maintenir des informations structurées et connectées.
recommendations: noDisplay, noCatalog
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
exl-id: ba7a4b04-5faa-41b6-86d0-4d0ce946ad1e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YZRzcl8ymUo85jplCgKOx-qI83Gqa4CUI6saxfijtec
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 184cff4f2ebf8a1343d784936f10c902e350c134
workflow-type: tm+mt
source-wordcount: 1386
ht-degree: 7%

---

# Prise en main d’Adobe Workfront Planning Designer

<!--remove the Beta tags in the screen shots on this page when this is released to GA - maybe March 2, 2026-->

>[!IMPORTANT]
>
>Planning Designer est actuellement disponible pour tous les clients disposant d’un statut Beta.
>
>Les informations de cet article se rapportent à Adobe Workfront Planning, une nouvelle fonctionnalité d’Adobe Workfront.
>
>Pour obtenir la liste des conditions requises pour accéder à Workfront Planning, consultez [Vue d’ensemble de l’accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Pour obtenir des informations générales sur Workfront Planning, voir [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Vous pouvez utiliser Adobe Planning Designer optimisé par l’IA pour configurer facilement vos espaces de travail et vos structures de données. Planning Designer prend en charge de nombreux éléments, de la création et la configuration des espaces de travail à la définition de champs et de formules, la gestion des enregistrements, la révision de l&#39;historique des modifications et la création de vues personnalisées.

Utilisé directement ou par l’intermédiaire de l’assistant d’IA, Planning Designer offre un environnement flexible et puissant pour créer et maintenir des informations structurées et connectées.

Pour plus d’informations sur Workfront Planning, consultez les articles suivants :

* [Index des informations générales et des articles pour Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Commencer à utiliser Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Vue d’ensemble de l’accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)


## <!--edit theses??--> des exigences d’accès

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
   <p>L'administrateur système doit activer Planning Designer pour votre organisation</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer des autorisations relatives à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  
   </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Activation de Planning Designer pour votre organisation

En tant qu’administrateur système, vous pouvez activer Planning Beta pour votre organisation. Une fois ce paramètre activé, chaque personne de votre instance Workfront peut afficher les fonctionnalités de Designer Planning dans sa zone Planning.

1. Connectez-vous en tant qu’administrateur Workfront dans Workfront.
1. Cliquez sur l&#39;icône **Menu principal** ![Icône du menu principal](assets/main-menu-shell.png), puis sur **Configuration**.
1. Accédez à **Système** > **Préférences** > **Préférences AI**.
1. Activez **Activer l’IA**<!--and ensure you have a signed Gen AI Agreement with Adobe-->.
   <!--1. Turn on the **Opt in to AI Beta** setting.-->
1. Activez le paramètre **Planning Designer**.
   <!-- add new screenshot-->
   ![Paramètre Planning Designer dans les Préférences système](assets/planning-designer-toggle-in-system-preferences.png)

1. Cliquer sur **Enregistrer**.

   Les fonctionnalités de Planning Designer pour la création ou la modification d&#39;espaces de travail sont désormais disponibles pour tous les utilisateurs de votre organisation qui peuvent accéder à Planning.

<!--

## Turn off the Planing Designer for your organization

After your Workfront administrator accepts the AI Assistant agreement, the Planning Designer is turned on for everyone in your organization, by default. 

To turn it off: 

1. Log in to Workfront as a System Administrator. 
1. Click **Main Menu** ![Main menu icon](assets/main-menu-shell.png) in the upper-left corner of the screen, then click **Setup**.
1. Click **System** >  in the left panel, then go to the **AI preferences** area.
1. Turn off the **Planning Onboarding** setting.
1. Click **Save**.

    This removes the Planning Designer for all users in the system.

-->

<!--

## Enroll in the Closed Beta program for the Planning Designer

Currently, you can request to participate in the Closed Beta program for the Planning Designer by sending us an email to sargism@adobe.com.

After we receive the email, our Engineering team will turn on the Planning Designer in your Workfront instance. 

>[!IMPORTANT]
>
>Your company must first accept the AI Assistant agreement before the Planning Designer is available in your system. 

-->

## Envoyer des commentaires sur Planning Designer

Vous pouvez envoyer des commentaires sur Planning Designer au cours du programme bêta.

1. Connectez-vous à Workfront, puis cliquez sur l’icône **Menu principal** ![Menu principal Lignes](assets/lines-main-menu.png) dans le coin supérieur gauche, puis cliquez sur **Planning**.

   La zone **Planification** s’ouvre.

1. Cliquez sur **Créer avec l’IA**. <!--update this tag name when they change it-->

   La fenêtre **Planning Designer** s&#39;ouvre.

1. Cliquez sur **Soumettre des commentaires ici** au bas de la page.
1. Ajoutez vos commentaires dans l&#39;espace prévu à cet effet, puis cliquez sur **Envoyer**.
Vos commentaires sont envoyés aux équipes d’ingénierie et de produit.

## Considérations relatives à Planning Designer

* Il n’est pas nécessaire d’activer le contrat d’IA avant de pouvoir accéder à Planning Designer.

<!--* You must sign the Beta agreement to access the Planning Designer.-->

<!--
Sargis and Ashot  said these are not required: 

* To use the Planning Designer, you first need to enable AI for your organization. The following must be in place for the AI features to be available to everyone in your organization:

    * Workfront must make the AI features available for your organization.

        For details, see [Prerequisites to AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).
    * After Workfront makes the AI features available for your organization, the main Workfront administrator can access it. 

        For information, see [Configure basic information for your system](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md). 
    * The Workfront administrator must accept the Gen AI agreement, and then turn on AI and the Planning Designer for your organization. 

        For more information, see [Enable or disable AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md). 

-->

* L’administrateur Workfront doit activer le Designer Planning de votre organisation. Ensuite, Planning Designer est disponible par défaut pour tous les utilisateurs.
* Les actions effectuées par le Designer Planning peuvent également l&#39;être par l&#39;assistant AI, lorsque vous l&#39;utilisez dans la zone Planning, si votre entreprise a signé l&#39;accord AI.
* Les actions effectuées par l&#39;assistant AI dans la zone Planning ou celles effectuées par le Designer Planning s&#39;inscrivent dans le cadre de vos autorisations Workfront Planning et de votre niveau d&#39;accès Workfront.

  Pour plus d’informations, voir les articles suivants :

  * [Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Les modifications apportées par l&#39;assistant AI ou Planning Designer pour le compte de l&#39;utilisateur sont suivies dans le panneau Historique de l&#39;enregistrement.

* Les actions effectuées par le Designer de planification sont permanentes et peuvent être irréversibles. Par exemple, la suppression d’un champ est irréversible. Passez en revue toutes les actions proposées par le Designer avant de les accepter.

  >[!IMPORTANT]
  >
  >Lors de la création, de la mise à jour ou de la suppression d&#39;un objet par le biais de Planning Designer, l&#39;invite ne demande confirmation que pour les actions irréversibles. Par exemple, la suppression d’un type d’enregistrement ou d’un espace de travail est irréversible. La suppression d’un enregistrement ne l’est pas. Planning Designer ne demande une confirmation que lorsqu&#39;il tente de supprimer un type d&#39;enregistrement ou un espace de travail.

* Lorsque vous créez des espaces de travail et des types d&#39;enregistrements à l&#39;aide de Planning Designer, les vues et les champs sont également créés automatiquement.

## Fonctionnalité actuellement disponible pour Planning Designer

Vous pouvez utiliser Planning Designer ou l&#39;assistant AI pour effectuer l&#39;une des actions suivantes :

* Création et configuration des espaces de travail

<!--On March 2: * Edit workspaces-->

* Créer des types d’enregistrements, notamment en définissant et en ajoutant des types d’enregistrements globaux aux espaces de travail

* Champs de conception ou champs de formule

* Créer, supprimer, dupliquer et restaurer des enregistrements

* Modifier, mettre à jour, ajouter un champ dans un enregistrement

* Lier des enregistrements à d&#39;autres enregistrements

* Accéder à l’historique des modifications d’enregistrement

* Créer des vues personnalisées

* Créer des enregistrements en important un document

  Par exemple, vous pouvez charger l&#39;image d&#39;un organigramme hiérarchique de votre société et Planning Designer peut créer un espace de travail à partir de cette image.

  La création d&#39;objets à partir d&#39;un document importé n&#39;est disponible que dans Planning Designer et non dans l&#39;assistant AI.

  >[!IMPORTANT]
  >
  >Bien que nous prenions en charge les types de fichiers .XLSX, ils ne peuvent pas être utilisés pour l&#39;importation d&#39;enregistrements à grande échelle via Planning Designer.
  >Si vous devez importer un nombre important d&#39;enregistrements à ce stade, nous vous recommandons de le faire en utilisant les fonctions manuelles disponibles dans Planning.
  >
  >Pour plus d’informations, voir [Créer des enregistrements en important des informations à partir d’un fichier CSV ou Excel](/help/quicksilver/planning/records/import-file-to-create-records.md).
  >Pour les limitations de type de fichier, reportez-vous à la section « Obtenir des suggestions basées sur un document que vous téléchargez » de l’[Utilisation du remplissage de formulaire optimisé par l’IA pour remplir une demande à l’aide d’invites ou de documents](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Créer ou mettre à jour des objets à l&#39;aide de Planning Designer

Sauf indication contraire, vous pouvez créer ou mettre à jour des objets dans Workfront Planning à l&#39;aide du Designer Planning ou de l&#39;assistant AI.

1. Connectez-vous à Workfront, puis cliquez sur l’icône **Menu principal** ![Menu principal Lignes](assets/lines-main-menu.png) dans le coin supérieur gauche, puis cliquez sur **Planning**.

   La zone **Planification** s’ouvre. <!--update screen shot when they change the name of the button-->

   ![Bouton Créer avec IA sur la page Espaces de travail](assets/design-with-ai-button-on-workspaces-page.png)

1. Cliquez sur **Créer avec l’IA** ou sur **Créer un espace de travail**, puis utilisez la fenêtre d’invite en haut pour indiquer le type d’espace de travail que vous souhaitez créer. <!--update this when they change it to Generate with AI-->

   La fenêtre **Planning Designer** s&#39;ouvre. <!--remove the Beta tag here when this removes from Beta-->

   ![Fenêtre Planning Designer](assets/planning-designer-window.png)

1. Dans l’espace prévu à cet effet, commencez à saisir des invites pour l’assistant AI, puis cliquez sur Entrée lorsque vous avez terminé.

   <!--add screen shot-->

   Par exemple, vous pouvez saisir des invites similaires à celles ci-dessous :

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

   Vous pouvez afficher les espaces de travail, les types d’enregistrements, les champs, les vues et les enregistrements dans la zone de prévisualisation à droite de l’invite.

   >[!TIP]
   >
   >Certains objets sont créés immédiatement, sans avoir besoin d’être confirmés.

1. (Facultatif) Saisissez des invites supplémentaires pour modifier davantage vos objets.
1. (Facultatif) Cliquez sur l’icône **Afficher ou masquer l’écran de prévisualisation** ![Masquer ou afficher l’icône de l’écran de prévisualisation](assets/hide-show-preview-screen-in-planning-designer.png) pour ouvrir ou fermer l’écran de prévisualisation à droite.
1. Cliquez sur l’icône **Ouvrir l’espace de travail dans un nouvel onglet** ![Ouvrir l’espace de travail dans un nouvel onglet](assets/open-workspace-on-new-tab-icon.png) pour ouvrir l’espace de travail que vous mettez à jour dans un nouvel onglet.
1. Cliquez sur l’icône **Fermer** **X** pour fermer Planning Designer et ouvrir la zone Espaces de travail.
1. (Facultatif) Pour modifier un espace de travail, effectuez l’une des opérations suivantes :

   * Ouvrez l’espace de travail et apportez-y des modifications manuellement. Pour plus d’informations, voir [Modifier les espaces de travail](/help/quicksilver/planning/architecture/edit-workspaces.md).
   * Cliquez sur **Modifier avec l’IA**. Vous ouvrez ainsi Planning Designer. Répétez les étapes ci-dessus pour utiliser l’IA et apporter d’autres modifications à l’espace de travail.


