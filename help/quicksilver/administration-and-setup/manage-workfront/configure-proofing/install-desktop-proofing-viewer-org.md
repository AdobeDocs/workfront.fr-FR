---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Installation de la visionneuse de vérification de l’appli de bureau pour votre entreprise
description: La visionneuse de vérification de l’appli de bureau, conçue principalement pour la vérification du contenu interactif, est une application qui doit être installée sur l’ordinateur local de chaque utilisateur. En tant qu’administrateur Adobe Workfront ou administrateur Workfront BAT, vous pouvez effectuer cette installation.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 58f976d9f4245e528a4ddf23d39b92d9fa405311
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# Installation de la visionneuse de vérification de l’appli de bureau pour votre entreprise

La visionneuse de vérification de l’appli de bureau, conçue principalement pour la vérification du contenu interactif, est une application qui doit être installée sur l’ordinateur local de chaque utilisateur. En tant qu’administrateur Adobe Workfront ou administrateur Workfront BAT, vous pouvez effectuer cette installation.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou version ultérieure</p> <p>ou</p> <p>Plan hérité : Premium ou Select</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Travail ou plan</p> <p>Plan hérité : N’importe quel (la vérification doit être activée pour l’utilisateur)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>L’administrateur doit être sélectionné dans votre profil d’autorisation de BAT. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configuration de l’accès de vérification de l’utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Configuration requise

La visionneuse de vérification de l’appli de bureau est prise en charge sur les systèmes d’exploitation suivants :

* Windows 7 et versions ultérieures, 32 et 64 bits
* Mac OS X 10.9 et versions ultérieures, 64 bits

## Conditions préalables

Pour permettre aux utilisateurs d’utiliser la visionneuse de vérification de l’appli de bureau, vous devez

* Configurez le système pour lancer la visionneuse de vérification de l’appli de bureau en tant que vue par défaut pour les bons à tirer interactifs avant l’installation.

## Configuration de la visionneuse de vérification de l’appli de bureau comme valeur par défaut pour les BAT interactifs

Après avoir installé la visionneuse de vérification de l’appli de bureau pour votre entreprise, vous pouvez la définir comme visionneuse par défaut pour les bons à tirer interactifs.

1. Dans Workfront, cliquez sur le menu principal ![](assets/main-menu-icon.png), puis cliquez sur Vérification. ![](assets/proofing-in-main-menu.png) pour accéder au BAT Workfront.

1. Cliquez sur **Paramètres du compte** près du coin supérieur droit du BAT Workfront, puis cliquez sur le bouton **Paramètres**.

1. Sous **Valeurs par défaut des BAT**, à la fin de la variable **Visionneuse de vérification de l’appli de bureau pour la vérification interactive** ligne, cliquez sur **Configuration**.

   ![](assets/proof-defaults-350x265.png)

1. Cliquez sur **Activé et par défaut**, puis cliquez sur **Enregistrer**.

## Installation de la visionneuse de vérification de l’appli de bureau pour vos utilisateurs

* [Installation de la visionneuse de vérification de l’appli de bureau sur Mac](#installing-the-desktop-proofing-viewer-on-mac)
* [Installation de la visionneuse de vérification de l’appli de bureau sous Windows](#installing-the-desktop-proofing-viewer-on-windows)

### Installation de la visionneuse de vérification de l’appli de bureau sur Mac {#installing-the-desktop-proofing-viewer-on-mac}

1. Sur l’ordinateur de l’utilisateur, effectuez l’une des opérations suivantes pour télécharger l’application :

   * Si vous utilisez l’environnement de production, cliquez sur  [Téléchargement de production Mac pour la visionneuse de vérification de l’appli de bureau.](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg)
   * Si vous utilisez l’environnement de prévisualisation, cliquez sur  [Téléchargement de l’aperçu Mac pour la visionneuse de vérification de l’appli de bureau.](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg)
)

1. Ouvrez le fichier que vous venez de télécharger pour lancer l’installation.
1. Dans la boîte d’installation qui s’affiche, cliquez sur **Continuer**, puis cliquez sur **Installer**.

   ![00000776.png](assets/00000776-350x244.png)

1. Assurez-vous que chaque utilisateur termine l’installation en ouvrant un BAT interactif à partir de la zone Documents de Workfront.

### Installation de la visionneuse de vérification de l’appli de bureau sous Windows {#installing-the-desktop-proofing-viewer-on-windows}

1. Sur l’ordinateur de l’utilisateur, effectuez l’une des opérations suivantes pour télécharger l’application :

   * Dans l’environnement de production, cliquez sur [Téléchargement de production Windows pour la visionneuse de vérification de l’appli de bureau.](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe)
   * Dans l’environnement Aperçu, cliquez sur [Téléchargement de l’aperçu Windows pour la visionneuse de vérification de l’appli de bureau](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. Ouvrez le fichier que vous venez de télécharger pour lancer l’installation.
1. Dans la boîte d’avertissement de sécurité qui s’affiche, cliquez sur **Exécuter**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   La visionneuse de vérification de l’appli de bureau installe et s’exécute.

1. (Conditionnel) Si vous installez l’application à l’aide d’Internet Explorer, actualisez la page de lancement dans le navigateur après l’installation de l’application.
1. Assurez-vous que chaque utilisateur termine l’installation en ouvrant un BAT interactif à partir de la zone Documents de Workfront.
