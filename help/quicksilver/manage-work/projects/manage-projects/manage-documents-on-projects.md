---
product-area: projects
navigation-topic: manage-projects
title: Présentation de la gestion des documents pour les projets et les objets associés
description: Selon que votre administrateur Workfront choisit votre préférence de stockage par défaut, vous pouvez stocker des documents sur un stockage Workfront hérité ou un stockage d’entreprise Adobe. Cet article décrit comment gérer des documents pour des projets, des portfolios, des programmes, des modèles, des tâches et des événements.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 5c4ffeabf710374b14a2335b47342be4c393a7c8
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# Présentation de la gestion des documents pour les projets et les objets associés

Votre administrateur Adobe Workfront peut définir la valeur par défaut de la préférence de stockage de votre organisation pour indiquer où les documents doivent être stockés dans Workfront.

L’administrateur Workfront peut choisir l’une des options suivantes :

* Stockage Workfront
* Stockage d’entreprise Adobe

Cette préférence permet de stocker automatiquement les documents joints aux objets Workfront dans l’un des emplacements de stockage disponibles.

>[!IMPORTANT]
>
>Tous les clients n’ont pas accès à la fois au stockage Workfront et Adobe. Certains clients n’ont accès qu’à Workfront, tandis que d’autres n’ont accès qu’au stockage Adobe Enterprise par défaut. Aucune configuration n’est nécessaire pour les clients sans accès au stockage Workfront.

L’administrateur Workfront peut effectuer l’une des opérations suivantes :

* Choisissez l’une des deux options de stockage par défaut pour votre entreprise
* Permet de choisir le stockage à utiliser lors de la création de l&#39;un des objets suivants :

   * Projets
   * Portefeuilles
   * Modèles

Pour plus d’informations sur la définition des préférences de stockage pour Workfront, voir [Activer le stockage d’entreprise Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

Cet article décrit comment gérer des documents pour des projets, des portfolios, des programmes, des tâches, des événements, des modèles et des tâches de modèles.

<!--

Not sure we need these since this became an overview article: 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Light or higher</p>
   <p>Review or higher</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the objects you want to add documents to:</p>
   <ul><li>Projects</li>
   <li>Portfolios</li>
<li>Programs</li>
<li>Templates</li> 
<li>Tasks</li> 
<li>Issues</li> </ul>  
   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the objects you want to add documents to:</p>

<ul><li>A project</li>
   <li>A portfolio</li>
<li>A program</li>
<li>A template</li> 
<li>A task</li> 
<li>An issue</li> </ul>    
   
</td> 
  </tr> 
 </tbody> 
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

-->

## Présentation de l’espace de stockage de documents

Les clients peuvent avoir accès à l’une des fonctionnalités de stockage de documents suivantes :

* Uniquement le stockage Workfront. La zone Préférences de stockage dans les Préférences système n&#39;existe pas.
* Uniquement le stockage Adobe Enterprise. La zone Préférences de stockage dans les Préférences système n&#39;existe pas.
* Stockage Workfront et stockage Adobe Enterprise. L’administrateur Workfront peut choisir entre les options suivantes :

   * Sélectionne un environnement de stockage par défaut pour la gestion future des documents.
   * Permet aux utilisateurs de choisir le stockage qu’ils choisissent lorsqu’ils créent les objets suivants :

      * Projets
      * Portefeuilles
      * Modèles

  >[!NOTE]
  >
  >* Les tâches et les événements héritent du type de stockage du projet.
  >* Les tâches de modèles héritent du type de stockage du modèle
  >* Les programmes héritent du type de stockage du portefeuille.


Les documents stockés sur des objets dans le stockage Workfront sont gérés différemment de ceux stockés dans le stockage d’entreprise Adobe.

Pour plus d’informations, consultez [Présentation du stockage d’entreprise ](/help/quicksilver/review-and-approve-work/esm-overview.md).

Les sections suivantes décrivent le fonctionnement du stockage de documents pour les objets Workfront lorsque les options de stockage d’entreprise Workfront et Adobe sont en place.

### Gestion des documents pour les projets

Tenez compte des points suivants lorsque vous utilisez des projets :

* Lorsque vous créez un projet de stockage d’entreprise Adobe, Workfront crée un dossier dans la section Documents du projet où les documents sont enregistrés. Le nom du dossier est identique à celui du projet. Vous ne pouvez pas supprimer ni renommer manuellement le dossier. Le dossier est renommé si vous modifiez le nom du projet pour qu’il corresponde au nouveau nom du projet.
* Lorsque vous créez ou déplacez un projet de stockage d’entreprise Adobe vers un portfolio ou un programme de stockage Workfront hérité, le portfolio ou le programme est automatiquement converti en objet de stockage d’entreprise Adobe.
* Vous ne pouvez pas créer de projet de stockage Workfront pour un portefeuille ou un programme de stockage d’entreprise Adobe.

### Gestion des documents pour les portefeuilles

Tenez compte des points suivants lorsque vous utilisez des portfolios :

* Lorsque vous créez un portfolio de stockage d’entreprise Adobe, Workfront crée un dossier dans la section Documents du portfolio où les documents sont enregistrés. Le nom du dossier est identique à celui du portfolio. Vous ne pouvez pas supprimer ni renommer manuellement le dossier. Le dossier est renommé si vous modifiez le nom du portfolio pour qu’il corresponde au nouveau nom du portfolio.
* Lorsque vous créez ou déplacez un projet de stockage d’entreprise Adobe vers un portfolio de stockage Workfront hérité, le portfolio est automatiquement converti en objet de stockage d’entreprise Adobe.
* Si le portfolio converti disposait auparavant de documents joints, ils continuent à être stockés dans le stockage Workfront. Les nouveaux documents sont également stockés dans le stockage Workfront.
* Si le portfolio converti ne comportait aucun document joint dans le stockage Workfront, les nouveaux documents sont stockés dans le stockage d’entreprise Adobe.

### Gestion des documents pour les programmes

Tenez compte des points suivants lorsque vous utilisez des programmes :

* Lorsque vous créez un programme de stockage d’entreprise Adobe, Workfront crée un dossier dans la section Documents du programme où les documents sont enregistrés. Le nom du dossier est identique à celui du programme. Vous ne pouvez pas supprimer ni renommer manuellement le dossier. Le dossier est renommé si vous modifiez le nom du programme, afin qu’il corresponde au nouveau nom du programme.
* Lorsque vous créez ou déplacez un projet de stockage d’entreprise Adobe vers un portfolio de stockage Workfront hérité, le portfolio est automatiquement converti en objet de stockage d’entreprise Adobe.
* Si le programme converti disposait auparavant de documents joints, ils continuent à être stockés dans le stockage Workfront. Les nouveaux documents sont également stockés dans le stockage Workfront.
* Si aucun document n’était joint au programme converti dans le stockage Workfront, les nouveaux documents sont stockés dans le stockage d’entreprise Adobe.

### Gestion des documents pour les tâches

Tenez compte des points suivants lorsque vous utilisez des tâches :

* Les tâches héritent du type de stockage des projets.
* Lorsque vous chargez un document vers une tâche d’un projet de stockage Adobe, Workfront crée automatiquement un dossier dans la section Documents de la tâche. Le nom du dossier est identique à celui de la tâche.
* Vous pouvez renommer et supprimer le dossier de documents de la tâche de stockage d’entreprise Adobe, ce qui supprime également les documents du dossier. Après avoir ajouté de nouveaux documents à la tâche, le dossier est automatiquement recréé. Les documents supprimés ne sont pas replacés dans le dossier.
* Pour les projets de stockage d’entreprise Adobe, le dossier de documents d’une tâche s’affiche sous la forme d’un sous-dossier dans le dossier de documents automatiquement créé pour le projet.
* Vous ne pouvez pas copier ni déplacer une tâche d’un projet de stockage Workfront vers un projet de stockage Adobe. L&#39;inverse n&#39;est pas non plus possible.

### Gestion des documents pour les problèmes

Tenez compte des points suivants lorsque vous travaillez avec des problèmes :

* Les événements héritent du type de stockage des projets.
* Lorsque vous téléchargez un document vers un événement d’un projet de stockage Adobe, Workfront crée automatiquement un dossier dans la section Documents de l’événement. Le nom du dossier est identique à celui du problème.
* Vous pouvez renommer et supprimer le dossier de documents correspondant au problème de stockage d’entreprise Adobe, ce qui entraîne également la suppression des documents dans le dossier. Après avoir ajouté de nouveaux documents à l’événement, le dossier est automatiquement recréé. Les documents supprimés ne sont pas replacés dans le dossier.
* Pour les projets de stockage d’entreprise Adobe, le dossier de documents relatif à un événement s’affiche sous la forme d’un sous-dossier dans le dossier de documents automatiquement créé pour le projet.
* Vous ne pouvez pas copier ni déplacer un événement d’un projet de stockage Workfront vers un projet de stockage Adobe. L&#39;inverse n&#39;est pas non plus possible.

### Gestion des documents pour les modèles de projet

Tenez compte des points suivants lorsque vous utilisez des modèles :

* Lorsque vous créez un modèle de stockage d’entreprise Adobe, Workfront crée un dossier dans la section Documents du modèle où les documents sont enregistrés. Le nom du dossier est identique à celui du programme. Vous ne pouvez pas supprimer ni renommer manuellement le dossier. Le dossier est renommé si vous modifiez le nom du modèle afin qu’il corresponde au nouveau nom du modèle.
* Vous pouvez utiliser un modèle de stockage Workfront pour créer des projets de stockage Workfront ; un modèle de stockage Adobe pour créer un projet de stockage Adobe.
* Vous pouvez joindre un modèle de stockage Workfront à un projet de stockage Adobe, sans modifier l’emplacement de stockage du projet.
* Vous pouvez joindre un modèle de stockage Adobe à un projet de stockage Workfront, sans modifier l’emplacement de stockage du projet.

### Gestion des documents pour les tâches de modèles

Tenez compte des points suivants lorsque vous utilisez des tâches de modèles :

* Les tâches de modèles héritent du type de stockage des modèles.
* Lorsque vous chargez un document vers une tâche de modèle sur un modèle de stockage Adobe, Workfront crée automatiquement un dossier dans la section Documents de la tâche de modèle. Le nom du dossier est identique à celui de la tâche de modèle.
* Vous pouvez renommer et supprimer le dossier de documents de la tâche de modèle de stockage d’entreprise Adobe, ce qui supprime également les documents du dossier. Après avoir ajouté de nouveaux documents à la tâche de modèle, le dossier est automatiquement recréé. Les documents supprimés ne sont pas replacés dans le dossier.
* Pour les modèles de stockage d’entreprise Adobe, le dossier de documents d’une tâche de modèle s’affiche sous la forme d’un sous-dossier dans le dossier de documents automatiquement créé pour le modèle.
* Vous ne pouvez pas copier ni déplacer une tâche de modèle d’un modèle de stockage Workfront vers un modèle de stockage Adobe. L&#39;inverse n&#39;est pas non plus possible.
* Lorsque vous joignez un document à un événement que vous envoyez à une file d’attente des demandes associée au stockage Adobe, un dossier est créé pour chaque événement envoyé où les documents sont stockés. Le dossier est également ajouté en tant que sous-dossier au dossier de projet créé automatiquement dans la file d’attente des demandes.
