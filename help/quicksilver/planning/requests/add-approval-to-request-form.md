---
title: Ajout d’une approbation à un formulaire de demande dans Adobe Workfront Planning
description: Vous pouvez ajouter un processus d’approbation à un formulaire de demande Adobe Workfront Planning, afin de lancer une approbation pour chaque demande soumise, avant la création d’un enregistrement.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: de568156315ff9094d938600c91b55e185d53765
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 5%

---

# Ajouter une approbation à un formulaire de demande dans Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Vous pouvez ajouter un processus d’approbation à un formulaire de demande Adobe Workfront Planning, afin de lancer une approbation pour chaque demande soumise, avant la création d’un enregistrement.

Cet article décrit comment un responsable d’espace de travail peut ajouter une approbation à un formulaire de demande associé à un type d’enregistrement.

Pour plus d’informations sur la création d’un formulaire de demande dans Workfront Planning, voir [Création et gestion d’un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Pour plus d’informations sur la soumission d’une demande à un type d’enregistrement pour créer un enregistrement, voir [ Soumettre des demandes Adobe Workfront Planning pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Packages Adobe Workfront</p></td> 
   <td> 
<p>Tout package Workfront et tout package Planning</p>
Ou
<p>Tout package de workflow et tout package Planning</p>

<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérez les autorisations d’un espace de travail et d’un type d’enregistrement</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à l’ajout d’approbations à un formulaire de demande

* Vous pouvez ajouter un ou plusieurs approbateurs à un formulaire de demande. Vous ne pouvez ajouter que des utilisateurs en tant qu’approbateurs.
* Vous pouvez afficher les informations d&#39;approbation sur un enregistrement créé en soumettant un formulaire de demande dans les champs Date d&#39;approbation par et Date d&#39;approbation . Pour plus d’informations, consultez [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).
* Lorsque vous ajoutez plusieurs approbateurs à un formulaire de demande, tous les approbateurs doivent accepter la demande avant la création d&#39;un enregistrement dans Workfront Planning.
* Si tous les approbateurs approuvent la demande, un enregistrement est créé pour le type d&#39;enregistrement associé au formulaire de demande.
* Si au moins un approbateur rejette la demande et que tous les autres l&#39;approuvent, une demande est créée pour la zone Demandes de Workfront, mais aucun enregistrement n&#39;est créé pour le type d&#39;enregistrement associé au formulaire de demande.
* L’ajout d’approbations à un formulaire de demande est facultatif. Workfront Planning crée immédiatement un enregistrement lorsqu&#39;une demande est soumise, si le formulaire de demande n&#39;est pas associé à une approbation.

## Ajouter une approbation à un formulaire de demande

1. Commencez à créer un formulaire de demande pour un type d’enregistrement, comme décrit dans la section [Créer et gérer un formulaire de demande dans Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Cliquez sur **Configuration**.

   La zone **Configuration** s’affiche.

   ![Onglet Configuration](assets/configuration-tab.png)
1. Dans le champ **Approbateurs**, commencez à saisir le nom d’un utilisateur ou d’une équipe que vous souhaitez définir en tant qu’approbateur, puis sélectionnez-le lorsqu’il s’affiche dans la liste.
1. (Facultatif et conditionnel) Si vous avez défini plusieurs approbateurs et que vous n’en avez besoin que d’un seul pour prendre une décision, activez l’option **Une seule décision est requise**.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Vous pouvez ajouter un ou plusieurs approbateurs à un formulaire de demande.
   >
   >* Si vous ajoutez plusieurs approbateurs et que l&#39;option Une seule décision est obligatoire n&#39;est pas activée, tous les approbateurs doivent approuver la demande avant que Workfront Planning ne crée un enregistrement.
   >
   >* Si au moins un approbateur rejette la demande, celle-ci est rejetée et l&#39;enregistrement n&#39;est pas créé. La demande reste dans l’onglet Planification de la section Soumis de la zone Demandes de Workfront.
   >
   >* Si vous ajoutez plusieurs approbateurs et que l&#39;option Une seule décision est obligatoire n&#39;est pas activée, tous les approbateurs doivent prendre une décision avant qu&#39;une demande ne soit approuvée ou rejetée.
   >
   >* Si une équipe est définie en tant qu&#39;approbateur, une seule décision est requise de la part de l&#39;équipe.


1. (Facultatif) Cliquez sur **Publier** si vous n’avez jamais partagé le formulaire de demande auparavant

   Ou

   Cliquez sur **Partager** pour partager le formulaire, puis sur **Copier le lien**.
1. (Facultatif) Lorsqu’un utilisateur utilise le lien que vous partagez et soumet une demande, Workfront Planning envoie une notification d’approbation in-app et un e-mail aux approbateurs.

   >[!NOTE]
   >
   >   L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour que les utilisateurs puissent recevoir des notifications par e-mail et in-app.


   Pour plus d’informations sur l’approbation des demandes, voir [ Approuver une demande ](/help/quicksilver/planning/requests/approve-request.md).
