---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Créer une épreuve pour un document
description: Vous pouvez générer un BAT pour un document au moment où vous le téléchargez vers Workfront. Vous pouvez également générer un BAT pour un document déjà téléchargé dans Adobe Workfront ou pour une nouvelle version d’un BAT déjà téléchargé dans Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 12%

---

# Créer une épreuve pour un document

<!-- Audited: 1/2024 -->

Vous pouvez générer un BAT pour un document au moment où vous le téléchargez vers Workfront.

Vous pouvez également générer un BAT pour un document déjà téléchargé dans Adobe Workfront ou pour une nouvelle version d’un BAT déjà téléchargé dans Workfront.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> 
   <p>Nouveau : Tous </p>
   <p>Actuel : Pro ou supérieur</p> <p>Formule héritée : sélectionnez ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Nouvelle : standard</p>
   <p>Actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Télécharger un document et créer un BAT

1. Accédez au projet, à la tâche ou au problème où vous souhaitez créer un BAT.
1. Cliquez sur l’onglet **Documents** .
1. Cliquez sur Documents ![](assets/document-icon.png) dans le panneau de gauche.
1. Cliquez sur **Ajouter nouveau**, puis sur **Bon à tirer** dans le menu qui s’affiche.

   >[!TIP]
   >
   >Vous pouvez activer le paramètre **Générer automatiquement des bons à tirer lors du téléchargement de documents** dans votre profil utilisateur pour automatiser ce processus. Pour plus d’informations, voir [Configuration de mes paramètres](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. Dans la page **New BAT** qui s’affiche, vous pouvez

   * [Créer un BAT avancé avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Télécharger un document et créer une version d’un BAT

1. Accédez au projet, à la tâche ou au problème où vous souhaitez créer une nouvelle version d’un BAT existant.
1. Cliquez sur l’onglet **Documents** .
1. Sélectionnez le document dans lequel vous souhaitez ajouter une nouvelle version.
1. Cliquez sur **Ajouter nouveau** > **Version** > **Bon à tirer**.
1. Dans la page **Nouvelle version de BAT** qui s’affiche, vous pouvez

   * [Créer un BAT avancé avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Utilisez le glisser-déposer pour générer un BAT simple pour une nouvelle version.

Vous pouvez faire glisser et déposer un document depuis votre système de fichiers (tel que votre bureau) pour créer un BAT ou une nouvelle version d’un BAT existant. Le BAT contient les paramètres suivants, selon que vous créez un BAT ou une nouvelle version :

* **Nouveau BAT :** Crée un BAT simple qui est partagé uniquement avec vous. Vous pouvez modifier les paramètres de partage après la création du BAT, comme décrit dans la section [Modifier les paramètres du BAT](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **Nouvelle version du BAT existant :** crée une nouvelle version avec les mêmes paramètres de BAT que la version précédente.

Pour utiliser la fonction glisser-déposer afin de générer un nouveau BAT ou une nouvelle version de BAT :

1. Assurez-vous que les bons à tirer sont configurés pour être générés automatiquement, comme décrit dans la section .
1. Passez à la  [Ajoutez des documents à Adobe Workfront à partir de votre système de fichiers](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), ce qui explique la méthode de glisser-déposer pour ajouter des documents. 

## Créer un BAT pour un document existant

1. Accédez au projet, à la tâche ou à l’emplacement où vous souhaitez obtenir le BAT, puis cliquez sur la section **Documents** .
1. Passez la souris sur le document, puis cliquez sur le lien **Créer un bon à tirer** qui apparaît sous le nom du document.

   >[!NOTE]
   >
   >Si **Générer automatiquement des bons à tirer lors du téléchargement de documents** est activé dans votre profil utilisateur, le système crée automatiquement un bon à tirer simple.

1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Bon à tirer simple</td> 
      <td>Cette option crée un BAT sans workflow associé et applique les paramètres de BAT par défaut. Vous pouvez mettre à jour les paramètres de BAT par défaut ou ajouter un workflow après avoir créé le BAT. Pour plus d’informations sur les paramètres du BAT, voir <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Modifier les paramètres du BAT</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bon à tirer avancé</td> 
      <td> <p>Cette option vous permet de configurer un workflow de base ou avancé et de modifier les paramètres du BAT que vous créez. Pour plus d’informations, voir </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Créer un BAT avancé avec un workflow de base</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Créer un BAT avancé avec un workflow automatisé</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
