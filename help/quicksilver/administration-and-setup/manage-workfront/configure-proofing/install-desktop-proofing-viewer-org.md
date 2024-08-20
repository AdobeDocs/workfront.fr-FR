---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Installation de la visionneuse de vérification de l’appli de bureau pour votre organisation
description: La visionneuse de vérification de l’appli de bureau, conçue principalement pour la vérification du contenu interactif, est une application qui doit être installée sur l’ordinateur local de chaque utilisateur. En tant qu’administrateur Adobe Workfront ou administrateur Workfront Proof, vous pouvez effectuer cette installation.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 17%

---

# Installation de la visionneuse de vérification de l’appli de bureau pour votre entreprise

<!--Audited: 05/2024-->

La visionneuse de vérification de l’appli de bureau, conçue principalement pour la vérification du contenu interactif, est une application qui doit être installée sur l’ordinateur local de chaque utilisateur. En tant qu’administrateur Adobe Workfront ou administrateur Workfront Proof, vous pouvez effectuer cette installation.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>Formule actuelle : Pro ou supérieure</p> <p>ou</p> <p>Formule héritée : Premium ou Sélectionner</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>L’administrateur doit être sélectionné dans votre profil d’autorisation de BAT. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configuration de l’accès de vérification de l’utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuration requise

La visionneuse de vérification de l’appli de bureau est prise en charge sur les systèmes d’exploitation suivants :

* Windows 7 et versions ultérieures, 32 bits et 64 bits
* Mac OS X 10.9 et versions supérieures, 64 bits

## Conditions préalables

Pour permettre aux utilisateurs d’utiliser la visionneuse de vérification de l’appli de bureau, vous devez configurer le système afin qu’il lance la visionneuse de vérification de l’appli de bureau en tant que vue par défaut pour les bons à tirer interactifs avant l’installation.

## Configuration de la visionneuse de vérification de l’appli de bureau comme valeur par défaut pour les BAT interactifs

Après avoir installé la visionneuse de vérification de l’appli de bureau pour votre entreprise, vous pouvez la définir comme visionneuse par défaut pour les bons à tirer interactifs.

{{step1-to-proofing}}

1. Cliquez sur **Paramètres du compte** près du coin supérieur droit de Workfront Proof, puis cliquez sur l’onglet **Paramètres** .

1. Sous **Valeurs par défaut du BAT**, à la fin de la ligne **Visionneuse de vérification de l’appli de bureau pour la vérification interactive**, cliquez sur **Configuration**.

   ![Valeurs par défaut du bon à tirer](assets/proof-defaults.png)

1. Cliquez sur **Activé et par défaut**, puis sur **Enregistrer**.

## Installation de la visionneuse de vérification de l’appli de bureau pour vos utilisateurs

* [Installation de la visionneuse de vérification de l’appli de bureau sur Mac](#installing-the-desktop-proofing-viewer-on-mac)
* [Installation de la visionneuse de vérification de l’appli de bureau sous Windows](#installing-the-desktop-proofing-viewer-on-windows)

### Installation de la visionneuse de vérification de l’appli de bureau sur Mac {#installing-the-desktop-proofing-viewer-on-mac}

1. Sur l’ordinateur de l’utilisateur, effectuez l’une des opérations suivantes pour télécharger l’application :

   * Si vous utilisez l’environnement de production, cliquez sur [Téléchargement de production Mac pour la visionneuse de vérification de l’appli de bureau](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg).
   * Si vous utilisez l’environnement de prévisualisation, cliquez sur [Téléchargement de prévisualisation Mac pour la visionneuse de vérification de l’appli de bureau](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg).

1. Ouvrez le fichier que vous venez de télécharger pour démarrer l’installation.
1. Dans la boîte d&#39;installation qui s&#39;affiche, cliquez sur **Continuer**, puis sur **Installer**.

   ![Boîte d’installation](assets/install-wf-proof-box.png)

1. Assurez-vous que chaque utilisateur termine l’installation en ouvrant un BAT interactif à partir de la zone Documents de Workfront.

### Installation de la visionneuse de vérification de l’appli de bureau sous Windows {#installing-the-desktop-proofing-viewer-on-windows}

1. Sur l’ordinateur de l’utilisateur, effectuez l’une des opérations suivantes pour télécharger l’application :

   * Dans l’environnement de production, cliquez sur [Téléchargement de production Windows pour la visionneuse de vérification de l’appli de bureau](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe).
   * Dans l’environnement Aperçu, cliquez sur [Téléchargement de l’aperçu Windows pour la visionneuse de vérification de l’appli de bureau](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. Ouvrez le fichier que vous venez de télécharger pour démarrer l’installation.
1. Dans la zone d&#39;avertissement de sécurité qui s&#39;affiche, cliquez sur **Exécuter**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   La visionneuse de vérification de l’appli de bureau installe et s’exécute.

1. (Le cas échéant) Si vous installez l’application à l’aide d’Internet Explorer, actualisez la page de lancement dans le navigateur après l’installation de l’application.
1. Assurez-vous que chaque utilisateur termine l’installation en ouvrant un BAT interactif à partir de la zone Documents de Workfront.
