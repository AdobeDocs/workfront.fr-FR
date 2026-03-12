---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Ajouter des documents à Adobe Workfront à partir de votre système de fichiers
description: Vous pouvez ajouter des documents à des projets, des tâches ou des problèmes dans plusieurs zones d’Adobe Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
source-git-commit: 47f029fbbc165db36e750907c9a14bb3c0718d58
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 56%

---

# Ajouter des documents à Adobe Workfront à partir de votre système de fichiers

Workfront comporte actuellement deux versions de la zone Documents : la zone des documents hérités et la zone des nouveaux documents. La version utilisée par votre entreprise dépend du stockage Workfront hérité ou du stockage d’entreprise. Pour plus d’informations sur ces types de stockage, consultez [Présentation du stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

L’ajout de documents à Workfront diffère selon la version de la zone de documents utilisée par votre entreprise.

* [Ajoutez des documents à depuis votre système de fichiers dans la zone des documents hérités](#add-documents-from-your-file-system-in-the-legacy-documents-area)
* [Ajout de documents à Workfront dans la zone des nouveaux documents](#add-documents-to-workfront-in-the-new-documents-area)



## Conditions d’accès

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
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> 
   <p>Contributeur ou supérieur</p> 
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Stockage Workfront hérité : modifier l’accès aux documents</p> 
   <p>Stockage d’entreprise : l’accès en modification aux documents est activé par défaut et ne peut pas être modifié</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter des documents depuis votre système de fichiers dans la zone des documents hérités

Si votre organisation utilise un stockage Workfront hérité, la zone des documents hérités s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage Workfront, voir [Différences entre le stockage d’entreprise Adobe et le stockage Workfront hérité](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

Vous pouvez ajouter des documents à des projets, des tâches ou des problèmes dans les zones suivantes d’Adobe Workfront :

* La zone Documents globale
* La zone Documents pour un objet Workfront
* Une carte connectée sur un panorama Workfront

Vous pouvez également charger de nouvelles versions de documents et ajouter des liens vers des documents provenant de fournisseurs de cloud tiers, tels que Google Drive, Dropbox et Microsoft OneDrive. Pour plus d’informations sur l’ajout de nouvelles versions de documents, voir [Charger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md). Pour plus d’informations sur l’ajout de documents provenant de fournisseurs de cloud tiers, voir [Lier des documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Il n’y a aucune restriction sur les types et les tailles de fichiers que vous pouvez charger sur Workfront. Toutefois, pour une opération réussie, le chargement doit être effectué en moins de cinq minutes et vous devez disposer d’un espace de stockage adéquat.

Pour plus d’informations sur le chargement de nouvelles versions d’un document dans Workfront, voir [Charger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md).


### Ajout de documents à Workfront dans la zone des documents hérités

Vous pouvez ajouter de nouveaux documents à Workfront à partir du système de fichiers de votre poste de travail. Vous pouvez également lier des documents provenant d’applications tierces telles que Google Drive et SharePoint.

>[!IMPORTANT]
>
>* Vous pouvez charger jusqu’à 150 documents à la fois.
>* La taille du fichier n’est pas limitée.
>* Les téléchargements de documents sont limités à 4 Go.

Pour ajouter un document

1. Accédez au projet, à la tâche ou au problème auquel vous souhaitez ajouter un document.
1. Cliquez sur l’onglet **Documents**, puis sur le menu déroulant **Ajouter**.

   ![Ajouter un nouveau document](assets/add-new-doc.png)

1. Selon le type de document que vous souhaitez ajouter, effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Charger des documents à partir de votre système de fichiers sur votre poste de travail</td> 
      <td> 
       <ol> 
        <li value="1">Dans le menu déroulant <strong>Ajouter</strong>, sélectionnez <strong>Document.</strong></li> 
        <li value="2"> <p>Recherchez et sélectionnez le document que vous souhaitez ajouter dans le système de fichiers de votre poste de travail.<br></p> <p>Vous pouvez sélectionner plusieurs documents en appuyant sur la touche Maj lorsque vous sélectionnez des fichiers supplémentaires.</p> </li> 
        <li value="3">Cliquez sur <strong>Ouvrir</strong>.</li> 
       </ol> 
       <p><b>NOTE</b> : vous pouvez également faire glisser et déposer des fichiers directement depuis votre gestionnaire de fichiers dans la liste des documents.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Charger des documents à partir d’une application tierce telle que Google Drive ou SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Dans le menu déroulant <strong>Ajouter</strong>, sélectionnez <strong>Depuis &lt;name_of_third-party_application&gt;</strong>.</p> <p>Par exemple, pour charger un document de Google Drive, cliquez sur <strong>Depuis Google Drive</strong>.</p> </li> 
        <li value="2"> <p>Suivez les instructions pour sélectionner le document dans l’application tierce.<br></p> <p>Pour plus d’informations sur les documents liés, voir <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Lier des documents à partir d’applications externes</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Demander un document à un autre utilisateur ou une autre utilisatrice Workfront</td> 
      <td> 
       <ol> 
        <li value="1">Dans le menu déroulant <strong>Ajouter</strong>, sélectionnez <strong>Demander un document</strong>.</li> 
        <li value="2">Dans la zone <strong>À qui faites-vous la demande</strong>, tapez le nom de l’utilisateur ou de l’utilisatrice à qui vous demandez le document.</li> 
        <li value="3">Dans la zone <strong>Expliquez votre demande</strong>, tapez le nom du document.</li> 
        <li value="4"> <p>Cliquez sur <strong>Envoyer la demande</strong>.</p> <p>Votre demande s’affiche dans votre onglet Documents.</p> <p>Pour plus d’informations sur la demande de documents, voir <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Demander un document</a>.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>


## Ajout de documents à Workfront dans la zone des nouveaux documents

Vous pouvez ajouter des documents à des projets, des tâches ou des événements à l’aide du modèle de stockage d’entreprise. Pour plus d’informations sur le stockage d’entreprise, consultez [Présentation du stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Fonctionnalité actuellement non prise en charge dans la zone des nouveaux documents :

* Chargement de documents dans la zone globale des documents
* Ajout de liens vers des documents provenant de fournisseurs cloud tiers, tels que Google Drive, Dropbox et Microsoft OneDrive.
* Demande de documents
* Copier un lien vers un dossier
* Extraction de documents
* Collage d’images à partir du presse-papiers
* Ajout de dossiers intelligents


### Ajout de documents à Workfront dans la zone des nouveaux documents

Si votre entreprise utilise le stockage d’entreprise, la nouvelle zone de documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur le stockage d’entreprise, consultez [Présentation du stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

<!--
>[!IMPORTANT]
>
>* You can upload up to 150 documents at one time.
>* There is no limit on the file size. 
>* Document downloads are limited to 4GB.
-->

Pour ajouter un document

1. Accédez au projet, à la tâche ou au problème auquel vous souhaitez ajouter un document.
1. Cliquez sur le **Documents** dans le panneau de gauche.
1. Cliquez sur **Nouveau** sur le côté droit de la page ou glissez-déposez le fichier dans la zone de dépôt qui s’affiche. Vous pouvez ajouter plusieurs documents à la fois.

   ![Ajouter un nouveau document](assets/add-new-doc-new-doc.png)

Si vous avez besoin d’informations sur le chargement de nouvelles versions d’un document dans Workfront, consultez la section [Charger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md).

## Document Security for Enterprise Storage

Workfront empêche les virus et autres contenus malveillants d’accéder au site par le biais de documents, et ce de différentes manières :

**Détection des fichiers corrompus par Workfront**

La numérisation de documents est automatiquement activée pour les objets utilisant le modèle de stockage d’entreprise.

Tous les fichiers de moins de 500 Mo sont analysés lorsqu’ils sont chargés. Les fichiers de plus de 500 Mo ne sont pas analysés. Si Workfront détecte un document corrompu, il est automatiquement supprimé.

**Restrictions de nom de fichier**

Cette intégration étant créée à l’aide du stockage d’entreprise Adobe, il existe une structure appliquée et des conventions de nommage à connaître lors de la gestion des projets et des documents.

* Les noms d’objet doivent être uniques et ne peuvent pas être dupliqués
* Le stockage d’entreprise Adobe nécessite des noms uniques pour les objets homologue avec le même parent dans l’arborescence hiérarchique
* Les documents ne peuvent pas porter le même nom s&#39;ils appartiennent au même projet
* Les noms de document ne peuvent pas contenir les caractères spéciaux suivants : `\ / : * ? " | < >`
* Les noms de document sont limités à 255 caractères maximum

Compte tenu de ces limitations, Workfront renomme automatiquement les objets ou les documents selon les besoins afin d’éviter les conflits.


## Sécurité des documents pour le stockage Workfront hérité

Le site Workfront empêche les virus et autres contenus malveillants d’accéder au site par le biais de documents, et ce de différentes manières :

**Détection des fichiers corrompus par Workfront**

L’analyse des documents n’est possible pour votre organisation que sur demande.

Si l’analyse des documents est activée, les fichiers de moins de 25 Mo sont analysés lorsqu’ils sont téléchargés. Les fichiers de plus de 25 Mo ne sont pas analysés.

Si Workfront détecte un document corrompu, un message s’affiche indiquant que le fichier est corrompu. Vous recevez également une notification par e-mail lorsque Workfront détecte un contenu potentiellement malveillant et que le fichier doit être supprimé.

Les fichiers corrompus sont supprimés dans les 24 heures suivant leur détection, sauf si vous les supprimez manuellement. Si vous supprimez un fichier corrompu, Workfront suit cette action comme une mise à jour. Si vous autorisez Workfront à le supprimer, aucune mise à jour n’est enregistrée.

**Restrictions de nom de fichier**

Certains caractères ne peuvent pas figurer dans le nom des fichiers téléchargés vers Workfront. Si le nom d’un fichier contient l’un des caractères suivants, ces caractères sont supprimés du nom du fichier lorsque celui-ci est téléchargé : `! # % * \ | ' " / ? < > { } [ ]`.
