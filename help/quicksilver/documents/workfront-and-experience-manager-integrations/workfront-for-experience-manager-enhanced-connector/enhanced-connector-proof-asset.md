---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Épreuve d’une ressource liée avec le connecteur amélioré
description: Après avoir lié une ressource d’Experience Manager Assets, vous pouvez créer une épreuve et affecter des utilisateurs et des utilisatrices à la révision et l’ajout de commentaires à la ressource.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 98%

---

# Épreuve d’une ressource liée avec le connecteur amélioré

Après avoir lié une ressource d’Experience Manager Assets, vous pouvez créer une épreuve et affecter des utilisateurs et des utilisatrices à la révision et l’ajout de commentaires à la ressource. Les épreuves créées à partir de ressources liées sont comptabilisées dans votre quota de stockage d’épreuves.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Standard</p>
   <p>Travail ou supérieur</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produits supplémentaires</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès en lecture ou supérieur à un document</p> </td> 
  </tr> 
 </tbody> 
</table>


Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer, vous devez

* installer le connecteur amélioré Workfront pour Experience Manager.

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

## Gérer une épreuve existante

Une fois que vous avez créé une épreuve, vous pouvez effectuer certaines actions, telles que les suivantes :

* Afficher l’activité de l’étape actuelle
* Mettre à jour les personnes réviseuses et les échéances
* Modifier le workflow

Pour plus d’informations sur la gestion d’une épreuve existante, consultez [Gestion des épreuves dans Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Vérifier une épreuve

Les réviseurs et réviseuses affectés peuvent effectuer certaines opérations, telles que les suivantes :

* Afficher la ressource et ajouter des commentaires
* Ajouter des actions aux commentaires
* Comparer les versions
* Approuver ou refuser l’épreuve

Pour plus d’informations sur ce que vous pouvez faire avec l’outil de relecture, consultez [Révision des épreuves dans Adobe Workfront](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
