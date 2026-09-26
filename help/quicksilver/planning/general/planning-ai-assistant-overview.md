---
title: Présentation de l’assistant IA Planification d’Adobe Workfront
description: Vous pouvez utiliser l’assistant d’IA pour générer, mettre à jour ou supprimer des enregistrements en fonction du contexte de page et de la structure d’enregistrement actuels. Les commandes de l’utilisateur et l’exécution par l’IA de ces commandes fonctionnent ensemble pour s’assurer que les modifications apportées par l’IA sont reflétées avec précision dans votre environnement.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/3I5y7eTZml-nkAiAYnBFuaw72DyXgNG12D-EVYVourA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 9%
---
# Vue d’ensemble de l’assistant IA Adobe Workfront Planning



<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Une fois la version à prévisualiser, les mêmes fonctionnalités sont également disponibles tous les mois dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>



{{planning-important-intro}}

Vous pouvez utiliser l’assistant AI pour apporter des modifications ou des mises à jour aux enregistrements et à d’autres objets dans Adobe Workfront Planning en fonction du contexte de la page active.

Les commandes de l’utilisateur et l’exécution par l’IA de ces commandes fonctionnent ensemble pour s’assurer que les modifications apportées par l’IA sont reflétées avec précision dans votre environnement.

>[!IMPORTANT]
>
><span class="preview">Dans certaines organisations, l’assistant AI a été remplacé par le CX Coworker. Pour plus d’informations, voir [Présentation d’Adobe Workfront Planning CX Coworker](/help/quicksilver/planning/general/planning-cx-coworker-overview.md).</span>

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
<p>Tout Workfront ou workflow avec un package Planning</p>
Ou
<p>Tout package Planning lorsqu’il est acheté en tant que produit autonome</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licence Adobe Planning</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td>  
     <p>Votre administrateur doit effectuer les opérations suivantes pour autoriser l’accès à l’assistant AI :</p>
   <ul>
   <li><p>Ajoutez des types de licence Workflow et Planning à votre niveau d'accès lorsque vous disposez à la fois d'un package Workflow et Planning</p></li>
   <li><p>Désélectionnez Désactiver le paramètre Assistant Workfront AI dans votre niveau d’accès</p></li></ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer des autorisations relatives à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Paramètres système</p></td> 
   <td>   <p>Votre administrateur Workfront doit sélectionner le paramètre Activer l’IA dans les Préférences système de la Configuration et signer l’IA pour avoir accès à l’assistant IA</p>  
    </td> 
  </tr> 
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considérations relatives à l’assistant d’IA

* L’assistant AI doit être activé pour votre organisation avant d’être disponible pour les utilisateurs de votre entreprise.

  Pour plus d’informations, voir [ Présentation de l’assistant AI ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

* Une fois que Workfront a activé l’agent pour votre organisation, il est disponible pour l’administrateur Workfront principal. Pour plus d’informations, voir [ Configuration des préférences système ](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* L’administrateur Workfront doit activer l’assistant AI pour tous les autres utilisateurs. Pour plus d’informations, voir [Activer ou désactiver l’assistant IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* L’assistant d’IA fonctionne dans le contexte de chaque page. Les requêtes que vous envoyez pour l’assistant AI doivent faire référence à la fonctionnalité disponible dans la page que vous avez ouverte.

* Les actions effectuées par l’assistant AI dans la zone Planning s’inscrivent dans le cadre de vos autorisations Workfront Planning et de votre niveau d’accès Workfront. Pour plus d’informations, voir les articles suivants :

  * [Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Les modifications apportées par l’assistant AI au nom de l’utilisateur sont suivies dans le panneau Historique de l’enregistrement.

* Les actions effectuées par l’assistant d’IA sont permanentes et peuvent être irréversibles. Par exemple, la suppression d’un champ est irréversible. Examinez toutes les actions proposées par l’assistant AI avant de les accepter.

* Lors de la création, de la mise à jour ou de la suppression d’un objet par le biais de l’assistant AI, celui-ci affiche les actions prévues et demande confirmation. Vous pouvez ensuite confirmer ou annuler les actions.

## Fonctionnalité actuellement disponible pour l’assistant d’IA

Actuellement, l’assistant AI est disponible dans la zone Planification de Workfront pour les pages suivantes :

* Page Workspace
* Page Type d’enregistrement
* Page Enregistrement

Vous pouvez utiliser l’assistant d’IA pour effectuer les actions suivantes à ce stade :

* Rechercher des enregistrements. Vous pouvez effectuer une recherche en fonction des informations contenues dans n’importe quel champ d’enregistrement.
* Créer des enregistrements. Un identifiant avec un lien vers le nouvel enregistrement s’affiche une fois l’enregistrement créé. Vous pouvez spécifier les champs que vous souhaitez mettre à jour pendant le processus de création, tels que les dates ou la description.
* Créez des enregistrements basés sur un document que vous téléchargez. Workfront prend en charge les formats de document suivants pour l’assistant AI :

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT et la plupart des formats d’image
* Mettre à jour les champs des enregistrements affichés à l’écran
* Supprimer des enregistrements
* Restaurer les enregistrements que vous venez de supprimer


## Recherchez l’assistant AI dans Workfront Planning.

>[!NOTE]
>
><span class="preview">Si votre organisation a reçu l’accès au CX Coworker, la localisation du CX Coworker est similaire à la localisation de l’assistant AI. Pour plus d’informations, voir [Présentation d’Adobe Workfront Planning CX Coworker](/help/quicksilver/planning/general/planning-cx-coworker-overview.md).</span>


L’assistant d’IA se trouve dans les zones suivantes de Workfront Planning :

* La barre de navigation principale, dans le coin supérieur droit de l’écran.
* Dans la zone des détails d&#39;un enregistrement, après avoir ouvert l&#39;enregistrement dans l&#39;aperçu ou après avoir ouvert la page de l&#39;enregistrement.

### Accéder à l’assistant d’IA dans la zone Planification

1. Connectez-vous à Workfront, puis cliquez sur l’icône **Menu principal** ![Menu principal Lignes](assets/lines-main-menu.png) dans le coin supérieur gauche, puis cliquez sur **Planning**.

   La zone Planification s’ouvre.

1. Cliquez sur une carte **espace de travail**.

1. (Facultatif) Cliquez sur une carte **type d’enregistrement**.

1. (Facultatif) Cliquez sur un **enregistrement** pour ouvrir la page **Détails** de l’enregistrement.

1. Cliquez sur l’icône **Assistant IA** dans le coin supérieur droit de l’écran dans la barre de navigation globale ou dans le coin supérieur droit de l’aperçu ou de la page de l’enregistrement.

   ![Icône de l’assistant AI](assets/ai-assistant-icon-highlighted.png)

1. Dans l’espace prévu à cet effet, commencez à saisir les commandes de l’assistant d’IA, puis cliquez sur Entrée lorsque vous avez terminé.

   ![Panneau Assistant IA avec zone de commande vide](assets/ai-assistant-panel-with-empty-command-box.png)

   Par exemple, vous pouvez saisir l’une des valeurs suivantes :

   * Créez une campagne dont la date de début est le 4 juillet et la date de fin le 30 juillet
   * Mettez à jour le champ Description de l’enregistrement Campagne d’été avec une date à déterminer
   * Supprimer le dernier enregistrement
   * Restaurer l’enregistrement

   Un indicateur visuel s’affiche pendant que l’assistant AI traite les commandes, définissant les attentes en matière de temps de réponse.

   Après avoir reçu une réponse réussie, suivez les liens fournis ou notez les modifications sur la gauche.



