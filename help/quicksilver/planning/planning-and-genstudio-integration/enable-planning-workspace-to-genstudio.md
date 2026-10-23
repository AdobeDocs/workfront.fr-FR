---
title: Activation d’un Workspace Workfront Planning vers GenStudio for Performance Marketing
description: Si vous disposez déjà d’un espace de travail dans Adobe Workfront Planning, vous pouvez l’activer pour GenStudio for Performance Marketing au lieu de recréer vos données.
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 0bcb6ef2abbf3789339af27119422ef413cd6eef
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 2%
---
# Activer un espace de travail Workfront Planning vers GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--
Better metadata, at publishing:
---
title: Promote a Workfront Planning workspace to GenStudio
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can promote a Workfront Planning workspace to GenStudio and have its information visible and updated from both systems.
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->
Outre Workfront Planning, si votre société a également acheté Adobe GenStudio for Performance Marketing, l’espace de travail GenStudio est disponible dans Adobe Workfront Planning lorsque votre instance de Workfront est intégrée à l’instance de GenStudio de votre société.

Si vous disposez déjà d’un espace de travail dans Workfront Planning, vous pouvez l’activer pour GenStudio au lieu de recréer vos données.

L’activation d’un espace de travail le lie à un projet de stockage Adobe et mappe ses types d’enregistrements et ses champs au schéma de l’espace de travail GenStudio. Une fois la configuration terminée, vous pouvez ouvrir les enregistrements de l’espace de travail dans GenStudio.

Tenez compte des points suivants :

* Vous devez avoir accès à Workfront Planning et à GenStudio for Performance Marketing.
* Vous devez disposer d’un projet d’espace de stockage Adobe pour effectuer la liaison à l’espace de travail. Un administrateur d’organisation peut en créer un dans le Adobe Admin Console.

  Pour plus d’informations, voir [Gérer le stockage Adobe](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html). <!--ensure this site still works-->


## Activer un espace de travail Workfront Planning vers GenStudio

1. Dans Workfront Planning, ouvrez l’espace de travail à activer.
1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’espace de travail, puis cliquez sur **Activer GenStudio**.

   La zone **Activer pour Workspace GenStudio** s’ouvre avec les étapes suivantes :

   1. **Projet ACPC** : sélectionnez le **Projet ACPC** (projet d&#39;espace de stockage Adobe) que vous souhaitez synchroniser avec cet espace de travail, puis cliquez sur **Suivant**. Les utilisateurs accèdent à l’espace de travail dans GenStudio par l’intermédiaire de ce projet.

      ![Activer Workspace GenStudio - Étape du projet ACPC](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **Types d’enregistrement** : mappez les types d’enregistrement de l’espace de travail aux six types d’enregistrement requis par GenStudio :

      * Campagnes
      * Produits
      * Personas
      * Canaux
      * Régions
      * Activations

      Pour chacun, ouvrez la liste et sélectionnez le type d&#39;enregistrement Planning correspondant, ou sélectionnez **Ajouter** pour le créer, puis cliquez sur **Suivant**.

      ![Activation de Workspace GenStudio - Étape Types d’enregistrement](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **Champs** : mappez les champs de chaque type d’enregistrement. Utilisez les onglets situés en haut de la boîte de dialogue pour passer d’un type d’enregistrement à un autre. Pour chaque champ, sélectionnez le champ Planning correspondant ou sélectionnez **Ajouter** pour le créer.

      Répétez la configuration des champs pour tous les types d’enregistrements.

      ![Activation de Workspace GenStudio - Étape Champs &#x200B;](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. Examinez et traitez tous les avertissements.

      Par exemple, un nouveau champ peut devenir le champ principal pour le type d’enregistrement ou un alias de champ déjà utilisé est renommé (si vous avez déjà un champ nommé « Régions », celui importé peut devenir « Régions 2 »).

      Le mappage d’un champ **Statut** ajoute les options requises.

   1. Cliquez sur **Publier**.

      Un message de confirmation s’affiche lorsque l’espace de travail est activé. Les types d’enregistrements mappés sont marqués dans l’espace de travail.

      Les types d’enregistrements mappés pour être accessibles depuis GenStudio comportent une nouvelle icône **Adobe** sur leurs cartes.

      ![Type d’enregistrement des campagnes avec icône Adobe](assets/campaigns-record-type-card-with-adobe-icon.png)

1. Ouvrez GenStudio, sélectionnez **Campagnes**, puis cliquez sur le **projet ACPC** que vous avez initialement configuré pour cette configuration dans le coin inférieur gauche de l’écran. Examinez les types d’enregistrements et les champs importés.

   >[!TIP]
   >
   >Vous ne voyez que les enregistrements autorisés par votre appartenance à un projet CCAM.
