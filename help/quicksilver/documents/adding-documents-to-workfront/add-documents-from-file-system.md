---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Ajout de documents à Adobe Workfront à partir de votre système de fichiers
description: Vous pouvez ajouter des documents à des projets, des tâches ou des problèmes dans plusieurs zones d’Adobe Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
source-git-commit: 873745b7a7e7902a3617a577b3ed0414f987a4ce
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 1%

---

# Ajout de documents à Adobe Workfront à partir de votre système de fichiers

Vous pouvez ajouter des documents à des projets, à des tâches ou à des problèmes dans les zones suivantes d’Adobe Workfront :

* La zone Documents globale
* Zone Documents pour un objet Workfront
* Carte connectée sur un panorama Workfront

Vous pouvez également charger de nouvelles versions de documents et ajouter des liens vers des documents provenant de fournisseurs cloud tiers, tels que Google Drive, Dropbox et Microsoft OneDrive. Pour plus d’informations sur l’ajout de nouvelles versions de documents, voir [Télécharger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md). Pour plus d’informations sur l’ajout de documents à partir de fournisseurs cloud tiers, voir [Liaison de documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Il n’existe aucune restriction quant aux types et tailles de fichiers que vous pouvez transférer vers Workfront. Toutefois, pour réussir, le chargement doit être terminé dans les cinq minutes et vous devez disposer d’un espace de stockage approprié.

Si vous avez besoin d’informations sur le téléchargement de nouvelles versions d’un document vers Workfront, reportez-vous à la section [Télécharger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p> Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Ajout de documents à Workfront

Vous pouvez ajouter de nouveaux documents à Workfront à partir du système de fichiers de votre poste de travail. Vous pouvez également lier des documents à partir d’applications tierces telles que Google Drive et SharePoint.

>[!NOTE]
>
>Bien qu’il n’existe aucune limite de taille pour les téléchargements de documents, les téléchargements de documents sont limités à 4 Go.

Pour ajouter un document :

1. Accédez au projet, à la tâche ou au problème auquel vous souhaitez ajouter un nouveau document.
1. Cliquez sur le bouton **Documents** , puis cliquez sur le bouton **Ajouter** menu déroulant.

   ![](assets/add-new-doc.png)

1. Selon le type de document à ajouter, effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Chargement de documents à partir de votre système de fichiers sur votre poste de travail</td> 
      <td> 
       <ol> 
        <li value="1">Dans la <strong>Ajouter</strong> menu déroulant, sélectionnez <strong>Document.</strong></li> 
        <li value="2"> <p>Recherchez et sélectionnez le document à ajouter à partir du système de fichiers de votre poste de travail.<br></p> <p>Vous pouvez sélectionner plusieurs documents en appuyant sur la touche Maj lorsque vous sélectionnez des fichiers supplémentaires.</p> </li> 
        <li value="3">Cliquez sur <strong>Ouvrir</strong>.</li> 
       </ol> 
       <p><b>REMARQUE</b>: vous pouvez également faire glisser des fichiers directement depuis votre gestionnaire de fichiers vers la liste de documents.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Téléchargement de documents à partir d’une application tierce, telle que Google Drive ou SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Dans la <strong>Ajouter</strong> menu déroulant, sélectionnez <strong>De &lt;name_of_third-party_application&gt;</strong>.</p> <p>Par exemple, pour charger un document à partir de Google Drive, cliquez sur <strong>À partir du lecteur Google</strong>.</p> </li> 
        <li value="2"> <p>Suivez les invites pour sélectionner le document dans l’application tierce.<br></p> <p>Pour plus d’informations sur les documents liés, voir <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Liaison de documents à partir d’applications externes</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Demande d’un document auprès d’un autre utilisateur Workfront</td> 
      <td> 
       <ol> 
        <li value="1">Dans la <strong>Ajouter</strong> menu déroulant, sélectionnez <strong>Demande d’un document</strong>.</li> 
        <li value="2">Dans le <strong>À qui le demandez-vous ?</strong> saisissez le nom de l’utilisateur à partir duquel vous demandez le document.</li> 
        <li value="3">Dans le <strong>Dites-leur ce que vous demandez.</strong> saisissez le nom du document.</li> 
        <li value="4"> <p>Cliquez sur <strong>Envoyer la requête</strong>.</p> <p>Votre requête s’affiche dans l’onglet Documents .</p> <p>Pour plus d’informations sur la demande de documents, voir <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Demande d’un document</a>.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

## Sécurité des documents

Le site Workfront empêche les virus et autres contenus malveillants d&#39;entrer sur le site par le biais de documents de la manière suivante :

* [Comment Workfront détecte les fichiers corrompus](#how-workfront-detects-corrupted-files)
* [Restrictions relatives aux noms de fichier](#file-name-restrictions)

### Comment Workfront détecte les fichiers corrompus {#how-workfront-detects-corrupted-files}

L’analyse des documents est activée pour votre organisation uniquement sur demande.

Si l’analyse des documents est activée, les fichiers de moins de 25 Mo sont analysés lors de leur chargement. Les fichiers de plus de 25 Mo ne sont pas analysés.

Si Workfront détecte un document corrompu, Workfront interrompt le processus de chargement et un message s’affiche indiquant que le fichier est corrompu. Vous recevez également une notification par courrier électronique lorsque Workfront détecte du contenu potentiellement malveillant et que le fichier est censé être supprimé.

Les fichiers corrompus sont supprimés dans les 24 heures suivant leur détection, sauf si vous les supprimez manuellement. Si vous supprimez un fichier corrompu, Workfront effectue le suivi de cette action en tant que mise à jour. Si vous autorisez Workfront à le supprimer, aucune mise à jour n’est enregistrée.

### Restrictions relatives aux noms de fichier {#file-name-restrictions}

Les fichiers chargés dans Workfront ne peuvent pas contenir certains caractères dans les noms de fichiers. Si un fichier contient l’un des caractères suivants, les caractères sont supprimés du nom du fichier lors du téléchargement du fichier : `! # % * \ | ' " / ? < > { } [ ]`.
