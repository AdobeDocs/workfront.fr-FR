---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Créer une épreuve pour un document
description: Vous pouvez générer une épreuve pour un document au moment où vous le chargez dans Workfront. Vous pouvez également générer une épreuve pour un document déjà téléchargé dans Adobe Workfront ou pour une nouvelle version d’une épreuve déjà présente dans Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 100%

---

# Créer une épreuve pour un document

<!-- Audited: 1/2024 -->

Vous pouvez générer une épreuve pour un document au moment où vous le chargez dans Workfront.

Vous pouvez également générer une épreuve pour un document déjà téléchargé dans Adobe Workfront ou pour une nouvelle version d’une épreuve déjà présente dans Workfront.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> 
   <p>Nouveau : Tous </p>
   <p>Actuel : Pro ou supérieur</p> <p>Formule héritée : Select ou Premium</p> <p>Pour plus d’informations sur la relecture de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Nouveau : Standard</p>
   <p>Actuelle : travail ou plan</p> <p>Plan hérité : n’importe lequel (la relecture doit être activée pour l’utilisateur ou l’utilisatrice)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Charger un document et créer une épreuve

1. Accédez au projet, à la tâche ou au problème pour qui vous souhaitez créer une épreuve.
1. Cliquez sur l’onglet **Documents**.
1. Cliquez sur Documents ![](assets/document-icon.png) dans le panneau de gauche.
1. Cliquez sur **Ajouter**, puis sur **Épreuve** dans le menu qui apparaît.

   >[!TIP]
   >
   >Vous pouvez activer le paramètre **Générer automatiquement des épreuves lors du chargement de documents** dans votre profil d’utilisateur ou d’utilisatrice pour automatiser ce processus. Pour plus d’informations, voir [Configurer mes paramètres](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

1. Dans la page **Nouvelle épreuve** qui s’affiche, vous pouvez effectuer ce qui suit :

   * [Créer une épreuve avancée avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Charger un document et créer une nouvelle version d’une épreuve

1. Accédez au projet, à la tâche ou au problème pour qui vous souhaitez créer une nouvelle version d’une épreuve existante.
1. Cliquez sur l’onglet **Documents**.
1. Sélectionnez le document dans lequel vous souhaitez ajouter une nouvelle version.
1. Cliquez sur **Ajouter** > **Version** > **Épreuve**.
1. Dans la page **Nouvelle version d’épreuve** qui s’affiche, vous pouvez effectuer ce qui suit :

   * [Créer une épreuve avancée avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Faire glisser et déposer pour générer une épreuve simple pour une nouvelle version

Vous pouvez faire glisser et déposer un document à partir de votre système de fichiers (comme votre bureau) pour créer une épreuve ou une nouvelle version d’une épreuve existante. L’épreuve contient les paramètres suivants, selon que vous créez une épreuve ou une nouvelle version :

* **Nouvelle épreuve :** crée une épreuve simple qui n’est partagée qu’avec vous.Vous pouvez modifier les paramètres de partage après la création de l’épreuve, comme décrit dans [Modifier les paramètres de l’épreuve](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **Nouvelle version d’une épreuve existante :** crée une nouvelle version avec les mêmes paramètres d’épreuve que la version précédente.

Pour utiliser la fonction glisser-déposer afin de générer une nouvelle épreuve ou une nouvelle version d’épreuve :

1. Assurez-vous que les épreuves sont configurées pour être générées automatiquement, comme décrit dans .
1. Passez à [Ajouter des documents à Adobe Workfront à partir de votre système de fichiers](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), dans lequel est expliqué comment ajouter des documents à l’aide de la fonction glisser-déposer.

## Créer une épreuve pour un document existant

1. Accédez au projet, à la tâche ou au problème pour qui vous souhaitez créer une épreuve, puis cliquez sur la section **Documents**.
1. Passez la souris sur le document, puis cliquez sur le lien **Créer une épreuve** qui apparaît sous le nom du document.

   >[!NOTE]
   >
   >Si vous avez activé l’option **Générer automatiquement des épreuves lors du chargement de documents** dans votre profil utilisateur, le système crée automatiquement une épreuve simple.

1. Choisissez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Épreuve simple</td> 
      <td>Cette option crée une épreuve sans workflow associé et applique les paramètres d’épreuve par défaut. Vous pouvez mettre à jour les paramètres d’épreuve par défaut ou ajouter un workflow après avoir créé l’épreuve. Pour plus d’informations sur les paramètres d’épreuve, consultez <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Modification des paramètres d’épreuve</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Épreuve avancée</td> 
      <td> <p>Cette option vous permet de configurer un workflow de base ou avancé et de modifier les paramètres de l’épreuve que vous créez. Pour plus d’informations, consultez les ressources suivantes : </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Créer une épreuve avancée avec un workflow de base</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Créer une épreuve avancée avec un workflow automatisé</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
