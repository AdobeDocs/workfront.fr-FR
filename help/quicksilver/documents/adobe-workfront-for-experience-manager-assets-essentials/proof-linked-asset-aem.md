---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Relire une ressource liée pour Experience Manager Assets ou Assets Essentials
description: Après avoir lié une ressource à partir d’Experience Manager Assets Essentials, vous pouvez créer une épreuve et affecter des personnes à la révision et à l’ajout de commentaires à la ressource.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
TQID: https://experienceleague.adobe.com/adxs5pYRdr8p6SSjnGCXnHwSNKcJl3qGZjkbp764NfM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 452
ht-degree: 79%

---

# Relire une ressource liée pour Experience Manager Assets ou Assets Essentials

Après avoir lié une ressource à partir d’Experience Manager Assets Essentials, vous pouvez créer une épreuve et affecter des personnes à la révision et à l’ajout de commentaires à la ressource.

>[!NOTE]
>
>Cette fonctionnalité n&#39;est pas disponible dans la zone des nouveaux documents.<br>
>Si votre entreprise utilise l’espace de stockage dans le cloud d’Adobe, la nouvelle zone Documents s’affiche lorsque vous accédez aux documents dans Workfront. De là, vous pouvez ajouter des ressources à partir de Experience Manager Assets et les examiner et les approuver avec la visionneuse Frame.io. Pour plus d’informations, voir [Utilisation de Adobe Experience Manager avec l’intégration Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

## Conditions d’accès

<!-- Audited: 4/2025 -->

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
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

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer :

* Votre administrateur ou administratrice Workfront doit configurer une intégration Experience Manager. Pour plus d’informations, consultez la section [Configurer l’intégration d’Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurer l’intégration d’Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

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
      <td> <p>Cette option vous permet de configurer un workflow de base ou avancé et de modifier les paramètres de l’épreuve que vous créez. Pour plus d’informations, consultez les éléments suivants : </p> 
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
