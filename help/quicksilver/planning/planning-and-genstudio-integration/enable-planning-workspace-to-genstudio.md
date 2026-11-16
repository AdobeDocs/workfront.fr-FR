---
title: Activation d’un Workspace Workfront Planning vers GenStudio for Performance Marketing
description: Vous pouvez rendre un espace de travail Adobe Workfront Planning disponible dans GenStudio for Performance Marketing lorsque vous avez accès aux deux applications.
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 9dc53e749a61247529d67ce077856ea6bea8e494
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 6%
---
# Activer un espace de travail Workfront Planning vers GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--Iskuhi said "ACPC projects" will be renamed when this will be released but not sure if it has been. Follow up with Syuzanna, Gurgen Mosesyan and possibly Himanshi Kumar - see slack threads -->

Lorsque votre société achète également Adobe GenStudio for Performance Marketing et que vous êtes client Adobe Workfront Planning, l’espace de travail GenStudio est également disponible dans Workfront Planning.

Si vous disposez déjà d’un espace de travail Planning dans Workfront Planning, vous pouvez l’activer pour GenStudio for Performance Marketing au lieu de recréer les mêmes données à partir de celui-ci dans GenStudio.

L’activation d’un espace de travail le lie à un projet Adobe Cloud Storage et mappe ses types d’enregistrements et ses champs à l’espace de travail GenStudio. Une fois la configuration terminée, vous pouvez ouvrir les enregistrements de l’espace de travail dans GenStudio.

Vous devez disposer des éléments suivants :

* Accès à Workfront Planning et GenStudio for Performance Marketing.
* Un projet Adobe Cloud Storage à lier à l’espace de travail. Un administrateur d’organisation peut en créer un dans le Adobe Admin Console.

  Pour plus d’informations, voir [Gérer le stockage Adobe](https://helpx.adobe.com/fr/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html). <!--ensure this site still works-->

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout Workfront ou workflow et tout package Planning</p> 
Ou
<p>Tout package Planning lorsqu’il est acheté en tant que produit autonome</p>

</td> 
   <tr> 
<td> 
   <p> Produits supplémentaires</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>

<tr> 
<td> 
   <p> Paramètres de Adobe Admin Console</p> </td> 
   <td> 
   <p> Vous devez créer des projets Adobe Storage Cloud dans Adobe Admin Console </p>

<p>Pour plus d’informations, voir <a href="https://helpx.adobe.com/fr/business/enterprise/manage-storage-assets/manage-storage/projects-in-business-storage.html#project-policies">Gestion des projets</a>

</td> 
  </tr>
  <tr>

<tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Norme de workflow</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Planning</p></td> 
   <td><p>Norme de planification</p>
   </td> 
  </tr>
<tr> 
   <td role="rowheader"><p>Configuration des niveaux d'accès Adobe Workfront</p></td> 
   <td> <p>Vous devez ajouter un workflow et un type de licence Planning au niveau d'accès Workfront lorsque vous disposez à la fois d'un workflow et d'un package Planning</p>   
</td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Rôles utilisateur Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Tout rôle d’utilisateur GenStudio si vous devez accéder aux campagnes, aux produits et aux personnes</li>
   <li>GenStudio System Manager si vous devez accéder à Activations <!--and Events--></li></ul>
   Pour plus d'informations, voir <a href="https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Rôles utilisateur et autorisations</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>  
   <p>Dans Workfront Planning : </p>
   <ul>
   <li><p>Gérer les autorisations pour l’espace de travail <!--to add new fields or record types to the GenStudio workspace--></p></li>
   <!--
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   -->
   </ul>
   <!--
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   -->
   <p>Dans Adobe GenStudio for Performance Marketing : <p>
   <ul>
   <!--
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   -->
   <li><p> Création d’autorisations dans Adobe GenStudio for Performance Marketing pour créer des éléments</p></li></ul>
   </td>  
</tbody> 
</table>

Pour plus d’informations sur l’accès à Adobe Workfront Planning, consultez [Aperçu de l’accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Pour plus d’informations sur Adobe GenStudio for Performance Marketing, consultez le [Guide de l’utilisateur d’Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/home).

+++ 

## Activer un espace de travail Workfront Planning vers GenStudio

1. Dans Workfront Planning, ouvrez l’espace de travail à activer.
1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’espace de travail, puis cliquez sur **Activer GenStudio**.

   La zone **Activer le GenStudio de l’espace de travail** s’ouvre avec les étapes suivantes :

   1. **Projet ACPC** : sélectionnez le **Projet ACPC** (projet Adobe Cloud Storage) que vous souhaitez synchroniser avec cet espace de travail, puis cliquez sur **Suivant**. Les utilisateurs accèdent à l’espace de travail dans GenStudio par l’intermédiaire de ce projet.

      ![Activer Workspace GenStudio - Étape du projet ACPC](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **Types d’enregistrement** : mappez les types d’enregistrement de l’espace de travail aux six types d’enregistrement requis par GenStudio :

      * Campagnes
      * Produits
      * Personas
      * Canaux
      * Régions
      * Activations

      Pour chacun, ouvrez la liste et sélectionnez le type d’enregistrement Planning correspondant, ou sélectionnez **Ajouter** pour le créer, puis cliquez sur **Suivant**.

      ![Activer Workspace GenStudio - Étape Types d’enregistrements](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **Champs** : mappez les champs pour chaque type d’enregistrement. Utilisez les onglets situés en haut de la boîte de dialogue pour passer d’un type d’enregistrement à un autre. Pour chaque champ, sélectionnez le champ Planning correspondant ou sélectionnez **Ajouter** pour créer un champ.

      Répétez la configuration des champs pour tous les types d’enregistrements.

      ![Activer Workspace GenStudio - Étape Champs](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. Examinez et traitez tous les avertissements.

      Par exemple, un nouveau champ peut devenir le champ principal pour le type d’enregistrement ou un alias de champ déjà utilisé est renommé (si vous avez déjà un champ nommé « Régions », celui importé peut devenir « Régions 2 »).

      Le mappage d’un champ **Statut** ajoute les options requises.

   1. Cliquez sur **Publier**.

      Un message de confirmation s’affiche lorsque l’espace de travail est activé. Les types d’enregistrements mappés sont marqués dans l’espace de travail.

      Les types d’enregistrements mappés pour être accessibles depuis GenStudio comportent une nouvelle icône **Adobe** sur leurs cartes.

      ![Type d’enregistrement des campagnes avec icône Adobe](assets/campaigns-record-type-card-with-adobe-icon.png)

1. Ouvrez GenStudio, sélectionnez **Campagnes**, puis cliquez sur le **projet ACPC** que vous avez initialement configuré pour cette configuration dans le coin inférieur gauche de l’écran. Examinez les types d’enregistrements et les champs importés.

   >[!TIP]
   >
   >Seuls les enregistrements autorisés par votre appartenance à un projet Adobe Cloud Storage s’affichent.
