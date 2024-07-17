---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Relire une ressource liée avec le connecteur amélioré
description: Après avoir lié une ressource de Experience Manager Assets, vous pouvez créer un BAT et affecter des utilisateurs à la révision et à l’ajout de commentaires à la ressource.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 25%

---

# Relire une ressource liée avec le connecteur amélioré

Après avoir lié une ressource de Experience Manager Assets, vous pouvez créer un BAT et affecter des utilisateurs à la révision et à l’ajout de commentaires à la ressource. Les bons à tirer créés à partir de ressources liées sont pris en compte dans votre quota de stockage de BAT.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p> N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Travail ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer de Experience Manager Assets Essentials.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès ou version ultérieure</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Avant de commencer, vous devez

* Installation de Workfront pour Experience Manager Enhanced Connector

## Créer un BAT

Vous pouvez créer des BAT statiques, vidéo ou interactifs.

Pour créer un BAT :

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

## Gérer un BAT existant

Une fois que vous avez créé un BAT, vous pouvez faire des choses comme

* Afficher l’activité de l’étape actuelle
* Mettre à jour les validants et les échéances
* Modifier le workflow

Pour plus d’informations sur la gestion d’un BAT existant, voir [Gestion des BAT dans Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Vérifier une épreuve

Les réviseurs affectés peuvent effectuer des opérations telles que

* Afficher la ressource et effectuer des commentaires
* Ajout d’actions aux commentaires
* Comparaison de versions
* Approuver ou refuser le BAT

Pour plus d’informations sur ce que vous pouvez faire avec l’outil de vérification, voir [Vérification des bons à tirer dans Adobe Workfront](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
