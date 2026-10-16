---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Ajouter un lien web en tant que document
description: Vous pouvez ajouter un site web à Adobe Workfront sous la forme d’un lien web et demander une approbation.
author: Courtney
feature: Digital Content and Documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 5e37582fe161e1a4689c35773cb1b3f6ead5a859
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 9%
---
# Ajouter un lien web en tant que document

Vous pouvez ajouter un site web à Adobe Workfront sous la forme d’un lien web à partir de la nouvelle zone Documents . Après l’avoir ajouté, vous pouvez demander une approbation sur la page web active de la même manière que vous demandez une approbation sur un fichier chargé.

Si votre entreprise utilise l’espace de stockage Adobe dans le cloud, la nouvelle zone Documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur l’espace de stockage dans le cloud Adobe, consultez [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tout package Workfront pour gérer les documents à l’aide du stockage Workfront hérité</p>
<p>Tout package de workflow pour gérer les documents à l’aide de l’espace de stockage dans le cloud Adobe</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou supérieur</p> 
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Stockage Workfront hérité : modifier l’accès aux documents</p> 
   <p>Espace de stockage Adobe : l’accès en modification aux documents est activé par défaut et ne peut pas être modifié</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter un lien web en tant que document

Vous pouvez charger une page web HTML dans Workfront sous la forme d’un lien web. Après l’avoir ajouté, vous pouvez demander une approbation sur la page web active de la même manière que vous demandez une approbation sur un fichier chargé. Pour plus d&#39;informations sur la façon dont Frame.io gère les liens web, consultez [Frame.io Web Links](https://support.frame.io/hc/en-us/articles/360041187574-Frame-io-Web-Links).

<!--
>[!IMPORTANT]
>
>A web page behind single sign-on or a login page can't be displayed for review.
-->

Pour ajouter un lien web :

1. Accédez au projet, à la tâche ou à l’événement sur lequel vous souhaitez ajouter le site web, puis sélectionnez **Documents** dans le panneau de gauche.
1. Cliquez sur **Nouveau** puis sélectionnez **Lien web**.
1. Saisissez un nom dans le champ **Nom du document**, puis saisissez l&#39;adresse du site web dans le champ **URL**.
1. Cliquez sur **Ajouter**.
   ![Ajouter un lien web en tant que document](assets/web-url.png)

Pour demander une approbation sur le lien web, voir [Créer un workflow d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

## Limites connues

* Un problème temporaire se produit avec les documents de lien web créés dans Frame.io. Si vous créez un lien web dans Frame.io, puis une approbation sur celui-ci dans Workfront, le document ne s’ouvrira pas dans Frame.io. Les liens web créés dans Workfront ne sont pas affectés. Jusqu’à ce que ce problème soit résolu, créez des documents de lien web dans Workfront avant de démarrer une approbation.
* Actuellement, vous ne pouvez pas créer de nouvelles versions de documents de lien web dans Frame.io. Si vous devez créer une nouvelle version d’un document de lien web, créez la nouvelle version dans Workfront.