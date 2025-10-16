---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Relire une ressource liée pour Experience Manager Assets ou Assets Essentials
description: Après avoir lié une ressource à partir d’Experience Manager Assets Essentials, vous pouvez créer une épreuve et affecter des personnes à la révision et à l’ajout de commentaires à la ressource.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 81%

---

# Relire une ressource liée pour Experience Manager Assets ou Assets Essentials

Après avoir lié une ressource à partir d’Experience Manager Assets Essentials, vous pouvez créer une épreuve et affecter des personnes à la révision et à l’ajout de commentaires à la ressource.

## Conditions d’accès

<!-- Audited: 4/2025 -->

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront</td> 
   <td> 
   <p>Standard</p>
   <p>Travail ou supérieur</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produits supplémentaires</td> 
   <td>Vous devez disposer d’Experience Manager as a Cloud Service ou d’Assets Essentials, et quelqu’un doit vous ajouter au produit en tant qu’utilisateur ou utilisatrice dans l’Admin Console. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux documents</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher accès ou version ultérieure</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer :

* Votre administrateur ou administratrice Workfront doit configurer une intégration Experience Manager. Pour plus d’informations, voir [Configurer l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurer l’intégration Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Créer une épreuve

Vous pouvez créer des épreuves statiques, vidéo ou interactives.

Pour créer une épreuve :

1. Accédez au projet, à la tâche ou au problème pour lequel vous souhaitez créer une épreuve, puis cliquez sur la section **Documents**.
1. Passez la souris sur le document, puis cliquez sur le lien **Créer une épreuve** qui apparaît sous le nom du document.

   >[!NOTE]
   >
   >Si vous avez activé l’option **Générer automatiquement des épreuves lors du chargement de documents** dans votre profil utilisateur, le système crée automatiquement une épreuve simple.

1. Sélectionnez l’une des options suivantes dans la liste déroulante :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Épreuve simple</strong></td> 
      <td>Cette option crée une épreuve sans workflow associé et applique les paramètres d’épreuve par défaut. Vous pouvez mettre à jour les paramètres par défaut de l’épreuve ou ajouter un workflow après avoir créé l’épreuve. Pour plus d’informations sur les paramètres d’épreuve, consultez <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Modification des paramètres d’épreuve</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Épreuve avancée</strong></td> 
      <td> <p>Cette option vous permet de configurer un workflow de base ou avancé et de modifier les paramètres de l’épreuve que vous créez. Pour plus d’informations, voir : </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Créer une épreuve avancée avec un workflow de base</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Créer une épreuve avancée avec un workflow automatisé</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Gérer une épreuve existante

Une fois que vous avez créé une épreuve, vous pouvez effectuer les opérations suivantes :

* Afficher l’activité de l’étape actuelle
* Mettre à jour les personnes réviseuses et les échéances
* Modifier le workflow

Pour plus d’informations sur la gestion d’une épreuve existante, voir [Gestion des épreuves dans Adobe Workfront : index d’article](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Vérifier une épreuve

Les réviseurs affectés peuvent effectuer les opérations suivantes :

* Afficher la ressource et ajouter des commentaires
* Ajouter des actions aux commentaires
* Comparer les versions
* Approuver ou refuser l’épreuve

Pour plus d’informations sur ce que vous pouvez faire avec l’outil de relecture, voir [Révision de BAT dans Adobe Workfront : index d’article](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
