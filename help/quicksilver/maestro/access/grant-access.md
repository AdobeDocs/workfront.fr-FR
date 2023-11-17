---
title: Accorder l’accès à Adobe Maestro
description: Découvrez comment accorder l’accès et partager des informations dans Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 937498a68a994d19b0005d518d7e313c48961672
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Accorder l’accès à Adobe Maestro

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe Workfront.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients. Vous devez être un client Workfront pour avoir accès à Maestro.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Tous les utilisateurs de votre entreprise peuvent avoir accès à Maestro, si les conditions préalables suivantes sont réunies :

<!--the first requisite will be removed when we go to GA-->

* Votre entreprise est inscrite au programme bêta fermé Adobe Maestro.
* En tant qu’administrateur système, vous devez ajouter la zone Maestro au menu principal à l’aide d’un modèle de mise en page.

  Maestro ne s’affiche par défaut dans le menu principal pour aucun utilisateur, y compris les administrateurs système.

  Pour plus d’informations, voir [Personnalisation du menu principal à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

<!-- take out the note below when we release permissions-->

>[!NOTE]
>
>Aucun niveau d’accès ou autorisation n’est associé aux utilisateurs ou aux informations dans Maestro. Tous les utilisateurs pour lesquels Maestro est activé dans leur environnement peuvent afficher, modifier et supprimer toutes les informations ajoutées à Maestro par un autre utilisateur.

## Partage de la zone Maestro dans le menu principal avec d’autres

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

Une fois que votre entreprise a été inscrite au programme bêta Maestro, vous pouvez ajouter la zone Maestro au menu principal de tous les utilisateurs à l’aide d’un modèle de mise en page.

1. Connexion à **Workfront** en tant qu’administrateur Workfront.

1. Ajoutez la variable **Maestro** icon ![](assets/maestro-icon.png) à la fonction **Menu Principal** en utilisant une **Modèle de mise en page**.

   Pour plus d’informations, voir [Personnalisation du menu principal à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Attribuez le modèle de mise en page aux utilisateurs auxquels vous souhaitez accéder à Maestro.

   Pour plus d’informations, voir [Affecter des utilisateurs à un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Tous les utilisateurs affectés au modèle peuvent désormais accéder à Maestro dans leur menu principal.

   Les utilisateurs peuvent commencer à créer des espaces de travail, des types d’enregistrements, des enregistrements et des champs.

<!--

## Share permissions to a workspace

Only system administrators can access all workspaces in Maestro. As a system administrator, you must share a workspace with other users for them to view, manage, or contribute to it. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu at the right of a user or group name, then click **Remove**. 
    
    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 
1. Click **Save**.

-->