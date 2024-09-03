---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Relire une ressource liée pour Experience Manager Assets ou Assets Essentials
description: Après avoir lié une ressource à partir d’Experience Manager Assets Essentials, vous pouvez créer une épreuve et affecter des personnes à la révision et à l’ajout de commentaires à la ressource.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: b87839d6c6dbfe978a3e14ef4b448560742f95c3
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 100%

---

# Relire une ressource liée pour Experience Manager Assets ou Assets Essentials

Après avoir lié une ressource à partir d’Experience Manager Assets Essentials, vous pouvez créer une épreuve et affecter des personnes à la révision et à l’ajout de commentaires à la ressource.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Travail ou supérieur</p>
   <p>La relecture doit être activée pour votre utilisateur ou utilisatrice.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer d’Experience Manager as a Cloud Service ou d’Assets Essentials, et quelqu’un doit vous ajouter au produit en tant qu’utilisateur ou utilisatrice dans l’Admin Console. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher accès ou version ultérieure</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Conditions préalables

Avant de commencer

* Votre administrateur ou administratrice Workfront doit configurer une intégration Experience Manager. Pour plus d’informations, voir [Configurer l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurer l’intégration Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Créer une épreuve

Vous pouvez créer des épreuves statiques, vidéo ou interactives.

Pour créer une épreuve :

1. Accédez au projet, à la tâche ou au problème pour lequel vous souhaitez créer une épreuve, puis cliquez sur la section **Documents**.
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
      <td role="rowheader"><strong>Épreuve simple</strong></td> 
      <td>Cette option crée une épreuve sans workflow associé et applique les paramètres d’épreuve par défaut. Vous pouvez mettre à jour les paramètres d’épreuve par défaut ou ajouter un workflow après avoir créé l’épreuve. Pour plus d’informations sur les paramètres d’épreuve, consultez <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Modification des paramètres d’épreuve</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Épreuve avancée</strong></td> 
      <td> <p>Cette option vous permet de configurer un workflow de base ou avancé et de modifier les paramètres de l’épreuve que vous créez. Pour plus d’informations, consultez les ressources suivantes : </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Créer une épreuve avancée avec un workflow de base</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Créer une épreuve avancée avec un workflow automatisé</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Gérer une épreuve existante

Une fois que vous avez créé une épreuve, vous pouvez effectuer certaines actions, telles que les suivantes :

* Afficher l’activité de l’étape actuelle
* Mettre à jour les personnes réviseuses et les échéances
* Modifier le workflow

Pour plus d’informations sur la gestion d’une épreuve existante, consultez [Gestion des épreuves dans Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Vérifier une épreuve

Les réviseurs et réviseuses affectés peuvent effectuer certaines opérations, telles que les suivantes :

* Afficher la ressource et ajouter des commentaires
* Ajouter des actions aux commentaires
* Comparer les versions
* Approuver ou refuser l’épreuve

Pour plus d’informations sur ce que vous pouvez faire avec l’outil de relecture, consultez [Révision des épreuves dans Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
