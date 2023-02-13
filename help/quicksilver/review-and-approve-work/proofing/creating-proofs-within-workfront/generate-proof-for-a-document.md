---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Création d’un BAT pour un document
description: Vous pouvez générer un BAT pour un document au moment où vous le téléchargez vers Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Création d’un BAT pour un document

Vous pouvez générer un BAT pour un document au moment où vous le téléchargez vers Workfront.

Vous pouvez également générer un BAT pour un document déjà téléchargé dans Adobe Workfront ou pour une nouvelle version d’un BAT déjà téléchargé dans Workfront.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou version ultérieure</p> <p>ou</p> <p>Plan hérité : Sélectionner ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Travail ou plan</p> <p>Plan hérité : N’importe quel (la vérification doit être activée pour l’utilisateur)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront BAT.

## Télécharger un document et créer un BAT

1. Accédez au projet, à la tâche ou à l’emplacement où vous souhaitez créer un BAT.
1. Cliquez sur le bouton **Documents** .
1. Cliquez sur Documents ![](assets/document-icon.png) dans le panneau de gauche.
1. Cliquez sur **Ajouter**, puis cliquez sur **Bon à tirer** dans le menu qui s’affiche.

   >[!TIP]
   >
   >Vous pouvez activer la variable **Générer automatiquement des bons à tirer lors du téléchargement de documents** dans votre profil utilisateur pour automatiser ce processus. Pour plus d’informations, voir [Configurer mes paramètres](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. Dans le **Nouveau BAT** qui s’affiche, vous pouvez

   * [Créer un BAT avancé avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Créer un BAT avancé avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Télécharger un document et créer une version d’un BAT

1. Accédez au projet, à la tâche ou au problème où vous souhaitez créer une nouvelle version d’un BAT existant.
1. Cliquez sur le bouton **Documents** .
1. Sélectionnez le document dans lequel vous souhaitez ajouter une nouvelle version.
1. Cliquez sur **Ajouter** > **Version** > **Bon à tirer**.
1. Dans le **Nouvelle version du BAT** qui s’affiche, vous pouvez

   * [Créer un BAT avancé avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Créer un BAT avancé avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Utilisez le glisser-déposer pour générer un BAT simple pour une nouvelle version.

Vous pouvez faire glisser et déposer un document à partir de votre système de fichiers (tel que votre bureau) pour créer un BAT ou une nouvelle version d’un BAT existant. Le BAT contient les paramètres suivants, selon que vous créez un BAT ou une nouvelle version :

* **Nouveau BAT :** Crée un BAT simple qui est partagé uniquement avec vous. Vous pouvez modifier les paramètres de partage une fois le BAT créé, comme décrit dans la section [Modification des paramètres du BAT](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **Nouvelle version du BAT existant :** Crée une version avec les mêmes paramètres de BAT que la version précédente.

Pour utiliser la fonction glisser-déposer afin de générer un nouveau BAT ou une nouvelle version de BAT :

1. Assurez-vous que les bons à tirer sont configurés pour être générés automatiquement, comme décrit dans la section .
1. Passez à la  [Ajout de documents à Adobe Workfront à partir de votre système de fichiers](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), qui explique la méthode de glisser-déposer d’ajout de documents. 

## Créer un BAT pour un document existant

1. Accédez au projet, à la tâche ou au problème pour lequel vous souhaitez obtenir le BAT, puis cliquez sur le bouton **Documents** .
1. Passez la souris sur le document, puis cliquez sur l’icône **Créer un bon à tirer** lien qui apparaît sous le nom du document.

   >[!NOTE]
   >
   >Si vous avez **Générer automatiquement des bons à tirer lors du téléchargement de documents** activé dans votre profil utilisateur, le système crée automatiquement un BAT simple.

1. Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Bon à tirer simple</td> 
      <td>Cette option crée un BAT sans workflow associé et applique les paramètres de BAT par défaut. Vous pouvez mettre à jour les paramètres de BAT par défaut ou ajouter un workflow après avoir créé le BAT. Pour plus d’informations sur les paramètres du BAT, voir <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Modification des paramètres du BAT</a>.</td> 
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
