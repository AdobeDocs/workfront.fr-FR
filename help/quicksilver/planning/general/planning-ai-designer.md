---
title: Prise en main d’Adobe Workfront Planning Designer
description: Vous pouvez utiliser Adobe Planning Designer optimisé par l’IA pour configurer facilement vos espaces de travail et vos structures de données. Planning Designer prend en charge de nombreux éléments, de la création et la configuration des espaces de travail à la définition de champs et de formules, la gestion des enregistrements, la révision de l'historique des modifications et la création de vues personnalisées. Utilisé directement ou par l’intermédiaire de l’assistant d’IA, Planning Designer offre un environnement flexible et puissant pour créer et maintenir des informations structurées et connectées.
recommendations: noDisplay, noCatalog
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
source-git-commit: b52c188d767ee37699ead71ed90642458d9889fa
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 4%

---


# Prise en main d’Adobe Workfront Planning Designer

>[!IMPORTANT]
>
>Planning Designer est actuellement disponible uniquement pour les utilisateurs participant au programme de Beta fermé.
>
>Les informations de cet article font référence à Adobe Workfront Planning, une fonctionnalité supplémentaire d’Adobe Workfront.
>
>Pour obtenir la liste des conditions requises pour accéder à Workfront Planning, consultez [Présentation de l&#39;accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Pour obtenir des informations générales sur Workfront Planning, voir [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Vous pouvez utiliser Adobe Planning Designer optimisé par l’IA pour configurer facilement vos espaces de travail et vos structures de données. Planning Designer prend en charge de nombreux éléments, de la création et la configuration des espaces de travail à la définition de champs et de formules, la gestion des enregistrements, la révision de l&#39;historique des modifications et la création de vues personnalisées.

Utilisé directement ou par l’intermédiaire de l’assistant d’IA, Planning Designer offre un environnement flexible et puissant pour créer et maintenir des informations structurées et connectées.

Pour plus d’informations sur Workfront Planning, consultez les articles suivants :

* [Informations générales sur Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Présentation de l’accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)


## &#x200B;<!--edit theses??--> des exigences d’accès

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

## S’inscrire au programme Beta fermé pour Planning Designer

Actuellement, vous pouvez demander à participer au programme de Beta fermé pour Planning Designer en nous envoyant un e-mail à sargism@adobe.com.

Une fois l’e-mail reçu, notre équipe d’ingénieurs active Planning Designer dans votre instance Workfront.

>[!IMPORTANT]
>
>Votre société doit d&#39;abord accepter le contrat d&#39;assistant AI avant que Planning Designer ne soit disponible dans votre système.

## Envoyer des commentaires sur Planning Designer

Vous pouvez envoyer des commentaires sur Planning Designer au cours du programme bêta.

1. Connectez-vous à Workfront, puis cliquez sur l’icône **Menu principal** ![Menu principal Lignes](assets/lines-main-menu.png) dans le coin supérieur gauche, puis cliquez sur **Planning**.

   La zone **Planification** s’ouvre.

1. Cliquez sur **Créer avec l’IA**. <!--update this tag name when they change it-->

   La zone **Configuration de Workspace** de la fenêtre **Planning Designer** s&#39;ouvre. <!--replace shot below when they rename the area to Planning Designer-->

1. Cliquez sur **Soumettre des commentaires ici** au bas de la page.
1. Ajoutez vos commentaires dans l&#39;espace prévu à cet effet, puis cliquez sur **Envoyer**.
Vos commentaires sont envoyés aux équipes d’ingénierie et de produit.

## Considérations relatives à Planning Designer

* Pour utiliser Planning Designer, vous devez d’abord activer l’assistant d’IA pour votre entreprise. Les éléments suivants doivent être en place pour que l’assistant AI soit disponible pour tous les membres de votre organisation :

   * Workfront doit rendre l’assistant d’IA disponible pour votre organisation.

     Pour plus d’informations, consultez [Conditions préalables pour l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).
   * Une fois que Workfront a rendu l’assistant d’IA disponible pour votre organisation, l’administrateur Workfront principal peut y accéder.

     Pour plus d’informations, voir [Configurer les informations de base de votre système](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).
   * L’administrateur Workfront doit accepter le contrat d’assistant AI, puis activer l’assistant AI pour tous les autres utilisateurs.

     Pour plus d’informations, voir [Activer ou désactiver l’assistant AI](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).
* Une fois que l’administrateur système a activé l’assistant AI pour votre organisation, Planning Designer est disponible par défaut pour tous les utilisateurs et utilisatrices, s’il a été mis à disposition pour votre organisation.
* Les actions effectuées par le Designer Planning peuvent également l&#39;être par l&#39;assistant AI, lorsque vous l&#39;utilisez dans la zone Planning.
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
  >Bien que nous prenions en charge les types de fichiers .XLSX et .CSV, ils ne peuvent pas être utilisés pour l&#39;importation d&#39;enregistrements à grande échelle via Planning Designer.
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

1. Cliquez sur **Créer avec l’IA**. <!--update this when they change it-->

   La zone **Configuration de Workspace** de la fenêtre **Planning Designer** s&#39;ouvre. <!--replace shot below when they rename the area to Planning Designer-->

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
1. Ouvrez l&#39;espace de travail que vous avez modifié à l&#39;aide de Planning Designer et apportez d&#39;autres modifications à ses objets.

## Désactiver Planning Designer pour votre organisation

Une fois que votre administrateur Workfront a accepté le contrat d’assistant AI, Planning Designer est activé par défaut pour tous les membres de votre organisation.

Pour le désactiver :

1. Connectez-vous à Workfront en tant qu’administrateur système.
1. Cliquez sur **Menu principal** ![Icône du menu principal](assets/main-menu-shell.png) dans le coin supérieur gauche de l’écran, puis cliquez sur **Configuration**.
1. Cliquez sur **Système** > dans le panneau de gauche, puis accédez à la zone **Préférences IA**.
1. Désactivez le paramètre **Planification de l’intégration**. <!--add new screen shot with info icon and new name of the toggle; ensure you don't show the AI Reviewer if it is not in Prod yet-->

   ![Paramètre Planning Designer dans les Préférences système](assets/planning-designer-toggle-in-system-preferences.png)
1. Cliquer sur **Enregistrer**.

   Cela supprime Planning Designer pour tous les utilisateurs du système.






