---
product-area: projects
navigation-topic: manage-projects
title: Présentation de la gestion des documents pour les projets et les objets associés
description: Selon que votre administrateur Workfront choisit votre préférence de stockage par défaut, vous pouvez stocker des documents sur un stockage Workfront hérité ou un stockage dans le cloud Adobe. Cet article décrit comment gérer des documents pour des projets, des portfolios, des programmes, des modèles, des tâches et des événements.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: acd6989db41fad0a24015aac641c9821db1811f1
workflow-type: tm+mt
source-wordcount: '1976'
ht-degree: 0%

---

# Présentation de la gestion des documents pour les projets et les objets associés

Votre administrateur Adobe Workfront peut définir la valeur par défaut de la préférence de stockage de votre organisation pour indiquer où les documents doivent être stockés dans Workfront.

L’administrateur Workfront peut choisir l’une des options suivantes :

* Stockage Workfront
* Espace de stockage Adobe

Cette préférence permet de stocker automatiquement les documents joints aux objets Workfront dans l’un des emplacements de stockage disponibles.

>[!IMPORTANT]
>
>Votre instance Workfront peut ne pas avoir accès à la fois au stockage Workfront et Adobe. Certaines instances Workfront n’ont accès qu’à Workfront, tandis que d’autres n’ont accès qu’à l’espace de stockage dans le cloud Adobe par défaut. Aucune configuration n’est nécessaire pour les clients qui n’ont accès qu’à un seul type de stockage.

L’administrateur Workfront peut effectuer l’une des opérations suivantes :

* Choisissez l’une des deux options de stockage par défaut pour votre entreprise
* Permet de choisir le stockage à utiliser lors de la création de l&#39;un des objets suivants :

   * Projets
   * Portefeuilles
   * Modèles

Pour plus d’informations sur la définition des préférences de stockage pour Workfront, voir [Activer l’espace de stockage dans le cloud Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

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
* Uniquement l’espace de stockage dans le cloud Adobe. La zone Préférences de stockage dans les Préférences système n&#39;existe pas.
* Stockage Workfront et stockage dans le cloud Adobe L’administrateur Workfront peut choisir entre les options suivantes :

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


Les documents stockés sur des objets dans l’espace de stockage Workfront sont gérés différemment de ceux stockés dans l’espace de stockage cloud Adobe.

Pour plus d’informations, voir [Présentation de l’espace de stockage dans le cloud ](/help/quicksilver/review-and-approve-work/esm-overview.md).

Les sections suivantes décrivent le fonctionnement du stockage de documents pour les objets Workfront lorsque les options de stockage dans le cloud Workfront et Adobe existent dans le même environnement.

### Gestion des documents pour les projets

Tenez compte des points suivants lorsque vous utilisez des projets :

* Lorsque vous créez un projet d’espace de stockage Adobe, Workfront crée un dossier dans la section Documents du projet où les documents sont enregistrés. Le nom du dossier est identique à celui du projet. Vous ne pouvez pas supprimer ni renommer manuellement le dossier. Le dossier est renommé si vous modifiez le nom du projet pour qu’il corresponde au nouveau nom du projet.
* Lorsque vous créez ou déplacez un projet de stockage dans le cloud Adobe vers un portfolio ou un programme de stockage Workfront hérité, le portfolio ou le programme est automatiquement converti en objet de stockage dans le cloud Adobe, si le portfolio ou le programme ne sont pas associés à des documents avant l’ajout du projet.
* Vous ne pouvez pas créer de projet de stockage Workfront hérité pour un portfolio ou un programme de stockage dans le cloud Adobe.
* Lorsque vous importez un projet à partir de MS Project, Workfront crée un projet de stockage Workfront hérité, même lorsque votre administrateur Workfront a défini l’espace de stockage Adobe dans le cloud par défaut pour votre système.
* Lorsque vous créez des projets à l’aide d’une automatisation de Workfront Planning, Workfront utilise la préférence de stockage par défaut de votre système pour le projet. Vous devez acheter le package Planning pour accéder à Workfront Planning.

Pour plus d’informations, reportez-vous également à la section [Gestion des documents pour les modèles de projet](#document-management-for-project-templates) de cet article.

### Gestion des documents pour les portefeuilles

Tenez compte des points suivants lorsque vous utilisez des portfolios :

* Lorsque vous créez un portfolio de stockage dans le cloud Adobe, Workfront crée un dossier dans la section Documents du portfolio où les documents sont enregistrés. Le nom du dossier est identique à celui du portfolio. Vous ne pouvez pas supprimer ni renommer manuellement le dossier. Le dossier est renommé si vous modifiez le nom du portfolio pour qu’il corresponde au nouveau nom du portfolio.

* Lorsque vous ajoutez un projet de stockage dans le cloud Adobe à un portfolio de stockage Workfront hérité et qu’aucun document n’y est associé, le portfolio est converti en portfolio de stockage dans le cloud Adobe.
* Lorsque vous ajoutez un projet de stockage dans le cloud Adobe à un portfolio de stockage Workfront hérité auquel des documents sont associés, le stockage des documents du portfolio reste sur le stockage Workfront. Toutefois, l’icône de stockage Workfront héritée pour le portfolio ![icône de stockage de portfolio héritée](assets/legacy-storage-project-icon.png) est supprimée du portfolio.
* Vous ne pouvez pas ajouter un projet de stockage Workfront hérité à un portefeuille de stockage dans le cloud Adobe.

* Lorsque vous créez des portfolios à l’aide d’une automatisation de Workfront Planning, Workfront utilise la préférence de stockage par défaut de votre système pour le portefeuille. Vous devez acheter le package Planning pour accéder à Workfront Planning.

<!--
For preview/ Prod release: the third bullet above will need replacing with this:
* You cannot add an Adobe cloud storage project to a Legacy storage portfolio or a Legacy storage project to an Adobe storage portfolio. 
* Your administrator can convert a Legacy storage portfolio to Adobe cloud storage in the System Preferences area of Setup. All children objects (programs, projects, and documents) remain on Legacy storage. New projects will use Adobe cloud storage. New documents added to the portfolio will continue to be stored in Legacy storage.
  For information, see [Configure system preferences](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
-->

### Gestion des documents pour les programmes

Tenez compte des points suivants lorsque vous utilisez des programmes :

* Lorsque vous créez un programme d’espace de stockage Adobe, Workfront crée un dossier dans la section Documents du programme dans lequel les documents sont enregistrés. Le nom du dossier est identique au nom du programme. Vous ne pouvez pas supprimer ni renommer manuellement le dossier. Le dossier est renommé si vous modifiez le nom du programme, afin qu’il corresponde au nouveau nom du programme.

* Lorsque vous ajoutez un projet de stockage dans le cloud Adobe à un ancien programme de stockage Workfront et qu’aucun document n’y est associé, le programme est converti en programme de stockage dans le cloud Adobe. Le portefeuille du programme est également converti.
* Lorsque vous ajoutez un projet de stockage dans le cloud Adobe à un ancien programme de stockage Workfront et que des documents sont associés au programme, le stockage des documents du programme reste sur le stockage Workfront. Si le portfolio contient également des documents, son stockage de documents reste également sur le stockage Workfront ; dans le cas contraire, le portfolio est converti en stockage dans le cloud Adobe.

  L’icône de stockage Workfront héritée du programme ![icône de stockage de portfolio héritée](assets/legacy-storage-project-icon.png) est supprimée du programme.
* Vous ne pouvez pas ajouter un projet de stockage Workfront hérité à un programme de stockage dans le cloud Adobe.

* Lorsque vous créez des programmes à l’aide d’une automatisation de Workfront Planning, Workfront utilise la préférence de stockage par défaut de votre système pour le programme. Vous devez acheter le package Planning pour accéder à Workfront Planning.

<!--
For preview/Prod release - check for duplicates below with the bullets you want to keep above (??):

* You cannot add an Adobe cloud storage program to a Legacy storage portfolio, or a Legacy program to an Adobe cloud storage portfolio.
* You cannot add an Adobe cloud storage project to a Legacy storage program in a Legacy storage portfolio. (******* also take out bullet 2 above and maybe 3 too?? **********)
* When you add an Adobe cloud storage project to a Legacy storage program, the program is converted to Adobe storage. Existing Legacy storage documents remain in the Legacy storage.
* You cannot add a Legacy storage project to an Adobe cloud storage program, or an Adobe cloud storage project to a Legacy storage program. 
* You cannot create a project from an Adobe cloud storage template in a Legacy storage program. 
* You can create a project from a Legacy storage template in an Adobe cloud storage program, but the documents and folders on the template are not added to the new project. The project receives Adobe cloud storage.
-->

### Gestion des documents pour les tâches

Tenez compte des points suivants lorsque vous utilisez des tâches :

* Les tâches héritent du type de stockage des projets.
* Lorsque vous chargez un document vers une tâche d’un projet d’espace de stockage Adobe, Workfront crée automatiquement un dossier dans la section Documents de la tâche. Le nom du dossier est identique à celui de la tâche.
* Vous pouvez renommer et supprimer le dossier de documents de la tâche d’espace de stockage Adobe dans le cloud, ce qui supprime également les documents du dossier. Après avoir ajouté de nouveaux documents à la tâche, le dossier est automatiquement recréé. Les documents supprimés ne sont pas replacés dans le dossier.
* Pour les projets d’espace de stockage Adobe, le dossier de documents d’une tâche s’affiche sous la forme d’un sous-dossier dans le dossier de documents automatiquement créé pour le projet.
* Vous ne pouvez pas copier ni déplacer une tâche d’un projet de stockage Workfront hérité vers un projet de stockage dans le cloud Adobe. L&#39;inverse n&#39;est pas non plus possible.
* Les scénarios suivants existent lors de la conversion d&#39;une tâche en projet : <!--this info also duplicated in Convert tasks to projects-->
   * Une tâche de stockage Workfront héritée crée un projet de stockage Workfront hérité.
   * Une tâche de stockage dans le cloud Adobe crée un projet de stockage dans le cloud Adobe.
   * L’utilisation d’un modèle de stockage Workfront hérité pour convertir une tâche d’espace de stockage dans le cloud Adobe crée un projet d’espace de stockage dans le cloud Adobe.
   * L’utilisation d’un modèle de stockage dans le cloud Adobe pour convertir une tâche de stockage Workfront héritée crée un projet de stockage Workfront hérité.
* Vous ne pouvez pas ajouter de documents aux tâches d’espace de stockage Adobe dans le panneau Résumé .

### Gestion des documents pour les problèmes

Tenez compte des points suivants lorsque vous travaillez avec des problèmes :

* Les événements héritent du type de stockage des projets.
* Lorsque vous téléchargez un document vers un événement d’un projet d’espace de stockage Adobe, Workfront crée automatiquement un dossier dans la section Documents de l’événement. Le nom du dossier est identique à celui du problème.
* Vous pouvez renommer et supprimer le dossier de documents du problème d’espace de stockage dans le cloud Adobe, ce qui supprime également les documents du dossier. Après avoir ajouté de nouveaux documents à l’événement, le dossier est automatiquement recréé. Les documents supprimés ne sont pas replacés dans le dossier.
* Pour les projets d’espace de stockage Adobe, le dossier de documents relatif à un événement s’affiche sous la forme d’un sous-dossier dans le dossier de documents automatiquement créé pour le projet.
* Vous ne pouvez pas copier ni déplacer un problème d’un projet de stockage Workfront hérité vers un projet de stockage dans le cloud Adobe. L&#39;inverse n&#39;est pas non plus possible.
* Les scénarios suivants existent lors de la conversion d&#39;un événement en projet : <!--this info also duplicated in Convert an issue to a project-->
   * Un problème de stockage Workfront hérité crée un projet de stockage Workfront hérité.
   * Un problème d’espace de stockage dans le cloud Adobe crée un projet d’espace de stockage dans le cloud Adobe.
   * L’utilisation d’un modèle de stockage Workfront hérité pour convertir un problème de stockage dans le cloud Adobe crée un projet de stockage dans le cloud Adobe.
   * L’utilisation d’un modèle de stockage dans le cloud Adobe pour convertir un problème de stockage Workfront hérité crée un projet de stockage Workfront hérité.
* Vous ne pouvez pas ajouter de documents à des problèmes d’espace de stockage Adobe dans le panneau Résumé .

### Gestion des documents pour les demandes

* Lorsque vous envoyez une requête Workfront à laquelle est joint un document à un projet de stockage Workfront hérité fonctionnant en tant que file d’attente des requêtes, la zone Documents de la requête affiche le document à l’aide du type de stockage du projet, même si la préférence par défaut de stockage du système est l’espace de stockage dans le cloud Adobe.
* Lorsque vous joignez un document à un événement que vous envoyez à une file d’attente des demandes associée au stockage Adobe, un dossier est créé pour chaque événement envoyé où les documents sont stockés. Le dossier est également ajouté en tant que sous-dossier au dossier de projet créé automatiquement dans le projet de file d’attente des demandes.

### Gestion des documents pour les modèles de projet

Tenez compte des points suivants lorsque vous utilisez des modèles :

* Lorsque vous créez un modèle d’espace de stockage Adobe, Workfront crée un dossier dans la section Documents du modèle où les documents sont enregistrés. Le nom du dossier est identique à celui du programme. Vous ne pouvez pas supprimer ni renommer manuellement le dossier. Le dossier est renommé si vous modifiez le nom du modèle afin qu’il corresponde au nouveau nom du modèle.
* Vous pouvez utiliser un modèle de stockage Workfront hérité pour créer des projets de stockage Workfront hérités ; vous pouvez utiliser un modèle de stockage cloud Adobe pour créer un projet de stockage cloud Adobe.

<!--
for preview/prod release: 
* When creating projects using templates from a portfolio or program, the following scenarios exist: 
  * You cannot use an Adobe cloud storage template from a legacy Workfront storage portfolio or program to create a project.
  * You can create an Adobe cloud storage project for an Adobe storage portfolio or program using a Legacy storage template. Any template documents and folders are not attached to the new project. 
-->
* Vous pouvez joindre un modèle de stockage Workfront hérité à un projet de stockage dans le cloud Adobe sans modifier l’emplacement de stockage des documents dans le projet.
* Vous pouvez joindre un modèle de stockage dans le cloud Adobe à un projet de stockage Workfront hérité et cela ne modifie pas l’emplacement de stockage des documents sur le projet. Les documents du dossier de stockage dans le cloud Adobe pour le modèle sont ajoutés directement au projet, sans le dossier , tandis que les documents des dossiers de tâches de modèles sont ajoutés aux dossiers joints aux tâches du projet dans la section Documents des tâches.
* Lorsque vous enregistrez un projet en tant que modèle, le type de stockage du projet est transféré vers le modèle, quelle que soit la préférence de stockage définie par votre administrateur Workfront.


### Gestion des documents pour les tâches de modèles

Tenez compte des points suivants lorsque vous utilisez des tâches de modèles :

* Les tâches de modèles héritent du type de stockage des modèles.
* Lorsque vous téléchargez un document vers une tâche de modèle sur un modèle d’espace de stockage Adobe, Workfront crée automatiquement un dossier dans la section Documents de la tâche de modèle. Le nom du dossier est identique à celui de la tâche de modèle.
* Vous pouvez renommer et supprimer le dossier de documents de la tâche de modèle d’espace de stockage dans le cloud Adobe, ce qui supprime également les documents du dossier. Après avoir ajouté de nouveaux documents à la tâche de modèle, le dossier est automatiquement recréé. Les documents supprimés ne sont pas replacés dans le dossier.
* Pour les modèles d’espace de stockage Adobe, le dossier de documents d’une tâche de modèle s’affiche sous la forme d’un sous-dossier dans le dossier de documents automatiquement créé pour le modèle.
* Vous ne pouvez pas copier ni déplacer une tâche de modèle d’un modèle de stockage Workfront hérité vers un modèle de stockage dans le cloud Adobe. L&#39;inverse n&#39;est pas non plus possible.

