---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Google Drive
description: Les modules  [!DNL Adobe Workfront Fusion Google Drive]  vous permettent de surveiller, rechercher, créer, mettre à jour, supprimer et gérer vos fichiers, dossiers ou lecteurs partagés dans votre  [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2941'
ht-degree: 11%

---

# Modules [!DNL Google Drive]

Les modules [!DNL Adobe Workfront Fusion] [!DNL Google Drive] vous permettent de surveiller, rechercher, créer, mettre à jour, supprimer et gérer vos fichiers, dossiers ou lecteurs partagés dans votre [!DNL Google Drive].

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez connecter votre compte [!DNL Google Drive] à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Connexion de [!DNL Google Drive] à [!DNL Workfront Fusion]

Si vous êtes [!DNL @gmail.com] ou [!DNL @googlemail.com] utilisateur, vous devez créer un client OAuth sur [le  [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) afin d&#39;obtenir [!UICONTROL l&#39;identifiant du client] et [!UICONTROL le secret du client].

Pour obtenir des instructions étape par étape sur la création du client OAuth (et obtenir [!UICONTROL ID client] et [!UICONTROL Secret client]), voir [Se connecter [!DNL Adobe Workfront Fusion] à [!DNL Google Services]  à l’aide d’un client OAuth personnalisé](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!UICONTROL Workfront Fusion], voir [Création d’une connexion à [!UICONTROL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## Modules [!DNL Google Drive] et leurs champs

Lorsque vous configurez des modules [!DNL Google Drive], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Google Drive] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [Déclencheurs](#triggers)
* [Actions](#actions)

### Déclencheurs

* [[!UICONTROL Fichiers De Contrôle Dans Le Dossier]](#watch-files-in-folder)
* [[!UICONTROL Watch All Files]](#watch-all-files)
* [[!UICONTROL Surveiller les fichiers partagés]](#watch-shared-files)
* [[!UICONTROL Regarder les commentaires]](#watch-comments)

#### [!UICONTROL Fichiers De Contrôle Dans Le Dossier]

Récupère les détails du fichier lorsqu’un fichier est ajouté ou modifié dans le dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Sélectionnez le dossier à surveiller]</td>
    <td >Sélectionnez le dossier sur votre lecteur dans lequel vous souhaitez voir les fichiers.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Quels fichiers regarder]</td>
   <td> <p>Sélectionnez le type de fichiers à regarder.</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convertir des fichiers [!DNL Google Documents] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir des fichiers [!DNL Google Spreadsheets] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir des fichiers [!DNL Google Slides] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir des fichiers [!DNL Google Drawings] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Drawings].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>Indiquez si vous souhaitez regarder les nouveaux fichiers et toutes les modifications, ou uniquement les nouveaux fichiers.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Nombre maximal de fichiers téléchargés]</td>
    <td>Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] téléchargera au cours d’un cycle (nombre de répétitions par exécution de scénario).</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch All Files]

Récupère les détails du fichier lorsqu’un fichier de votre [!DNL Google Drive] est ajouté ou modifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quels fichiers regarder]</td> 
   <td> <p>Sélectionnez le type de fichiers à regarder.</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convertir des fichiers [!DNL Google Documents] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir des fichiers [!DNL Google Spreadsheets] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir des fichiers [!DNL Google Slides] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir des fichiers [!DNL Google Drawings] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Drawings].</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Indiquez si vous souhaitez regarder les nouveaux fichiers et toutes les modifications, ou uniquement les nouveaux fichiers.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de fichiers téléchargés]</td> 
   <td>Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] téléchargera au cours d’un cycle (nombre de répétitions par exécution de scénario).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Surveiller les fichiers partagés]

Déclenche lorsqu’un nouveau fichier est partagé avec vous ou qu’un fichier partagé existant est mis à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sélectionnez le dossier à surveiller]</td> 
   <td>Sélectionnez le dossier partagé dans lequel vous souhaitez voir les fichiers.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quels fichiers regarder]</td> 
   <td> <p>Sélectionnez le type de fichiers à regarder.</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convertir des fichiers [!DNL Google Documents] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir des fichiers [!DNL Google Spreadsheets] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir des fichiers [!DNL Google Slides] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir des fichiers [!DNL Google Drawings] au format]</td>
    <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Drawings].</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Indiquez si vous souhaitez regarder les nouveaux fichiers et toutes les modifications, ou uniquement les nouveaux fichiers.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de fichiers téléchargés]</td> 
   <td>Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] téléchargera au cours d’un cycle (nombre de répétitions par exécution de scénario).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder les commentaires]

Se déclenche lorsqu’un commentaire est ajouté ou modifié dans le fichier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File]</td> 
   <td>Sélectionnez le fichier que vous souhaitez consulter pour les commentaires.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Choisissez si vous souhaitez uniquement surveiller toutes les modifications ou les nouveaux commentaires.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de commentaires renvoyés]</td> 
   <td>Définissez le nombre maximal de commentaires que [!DNL Workfront Fusion] renverra au cours d’un cycle (le nombre de répétitions par exécution de scénario).</td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Charger un fichier]](#upload-a-file)
* [[!UICONTROL Mettre à jour un fichier]](#update-a-file)
* [[!UICONTROL Copier un fichier]](#copy-a-file)
* [[!UICONTROL Supprimer un fichier]](#delete-a-file)
* [[!UICONTROL Déplacer un fichier/dossier vers la corbeille]](#move-a-filefolder-to-trash)
* [[!UICONTROL Obtenir un fichier]](#get-a-file)
* [[!UICONTROL Recherche de fichiers/dossiers]](#search-for-filesfolders)
* [[!UICONTROL Créer un dossier]](#create-a-folder)
* [[!UICONTROL Obtenir un lien de partage]](#get-a-share-link)

#### [!UICONTROL Charger un fichier]

Télécharge un fichier vers votre [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>Sélectionnez la destination vers laquelle vous souhaitez charger un fichier.</p> 
    <ul> 
     <li>[!DNL My Drive]</li> 
     <li>[!DNL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dossier cible]</td> 
   <td>Sélectionnez le dossier dans lequel vous souhaitez charger un fichier. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td>Indiquez si vous souhaitez utiliser un fichier transmis à partir d’un module précédent ou si vous souhaitez mapper le fichier manuellement.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File name]</td> 
   <td>Sélectionnez le nom du fichier. Cette option est disponible si vous sélectionnez "[!UICONTROL Map]" dans le champ [!UICONTROL fichier source].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>Sélectionnez le fichier de données à charger. Cette option est disponible si vous sélectionnez "[!UICONTROL Map]" dans le champ [!UICONTROL fichier source].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>Saisissez le titre du nouveau fichier.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir un fichier]</td> 
   <td>L’activation de cette option permet au module de convertir les fichiers au format [!DNL Google] correspondant.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un fichier]

Met à jour les métadonnées ou le contenu d’un fichier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>Sélectionnez la destination vers laquelle vous souhaitez charger un fichier.</p> 
    <ul> 
     <li>[!UICONTROL Mon lecteur]</li> 
     <li>[!UICONTROL Partagé avec moi]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Déplacer vers un dossier]</td> 
   <td>Si vous souhaitez déplacer le fichier vers un autre dossier, sélectionnez le dossier dans lequel vous souhaitez déplacer le fichier.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td>Mappez l’identifiant du fichier à mettre à jour.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>Saisissez un titre pour le fichier mis à jour.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modifier le contenu d’un fichier]</td> 
   <td>Indiquez si vous souhaitez remplacer le contenu du fichier.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td>Indiquez si vous souhaitez utiliser un fichier transmis à partir d’un module précédent ou si vous souhaitez mapper le fichier manuellement. Ce champ est disponible si vous avez choisi de modifier le contenu du fichier dans le champ précédent.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File name]</td> 
   <td>Sélectionnez le nom du fichier. Cette option est disponible si vous sélectionnez "[!UICONTROL Map]" dans le champ [!UICONTROL fichier source].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>Sélectionnez le fichier de données à charger. Cette option est disponible si vous sélectionnez "[!UICONTROL Map]" dans le champ [!UICONTROL fichier source].</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copier un fichier]

Copie un fichier vers le nouvel emplacement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>Sélectionnez la destination vers laquelle vous souhaitez charger un fichier.</p> 
    <ul> 
     <li>[!UICONTROL Mon lecteur]</li> 
     <li>[!UICONTROL Partagé avec moi]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dossier cible]</td> 
   <td>Sélectionnez le dossier dans lequel se trouve le fichier à copier/</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td>Mappez l’identifiant du fichier à mettre à jour.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom de la copie]</td> 
   <td>Saisissez le titre du nouveau fichier. Laissez ce champ vide si vous ne souhaitez pas modifier le nom de fichier d’origine.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un fichier]

Supprime définitivement un fichier ou un dossier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td>Mappez l’identifiant du fichier que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un fichier/dossier vers la corbeille]

Déplace un fichier ou un dossier vers la corbeille.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td>Mappez l’identifiant du fichier que vous souhaitez déplacer vers la corbeille.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un fichier]

Récupère le fichier avec l’identifiant spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Documents] au format]</td> 
   <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Documents].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Spreadsheets] au format]</td> 
   <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Spreadsheets].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Slides] au format]</td> 
   <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Slides].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Drawings] au format]</td> 
   <td>Sélectionnez le format de fichier vers lequel vous souhaitez convertir [!DNL Google Drawings].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td>Mappez l’identifiant du fichier que vous souhaitez récupérer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Recherche de fichiers/dossiers]

Recherche des fichiers ou des dossiers selon des critères de recherche.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>Sélectionnez la destination à rechercher.</p> 
    <ul> 
     <li>[!UICONTROL Mon lecteur]</li> 
     <li>[!UICONTROL Partagé avec moi]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Liste d’un dossier]</td> 
   <td>Accédez au dossier dans lequel vous souhaitez rechercher les fichiers ou les dossiers.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Récupération]</td> 
   <td> <p> Indiquez si vous souhaitez rechercher des fichiers, des dossiers ou les deux.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Search]</p> </td> 
   <td> <p>Sélectionnez le type de recherche que vous souhaitez effectuer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Rechercher dans les noms de fichier/dossier]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Saisissez une partie du nom de fichier ou du nom de fichier complet (y compris le suffixe) que vous souhaitez rechercher.</p> </li> 
       <li> <p><strong>[!UICONTROL Options de recherche]</strong> </p> <p>Indiquez si vous souhaitez rechercher le terme exact ou si vous souhaitez rechercher des noms contenant le terme recherché.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Texte intégral] search</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Saisissez le terme à rechercher dans votre [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>Entrer une requête de recherche personnalisée</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Saisissez la requête de recherche personnalisée. Pour plus d’informations, reportez-vous à la section [!UICONTROL Recherche de fichiers] de cet article.</p> </li> 
       <li> <p><strong>Ajoutez le dossier sélectionné ci-dessus à la requête</strong> </p> <p>Recherche le dossier dans la collection parents. Tous les fichiers et dossiers se trouvent ainsi directement dans le dossier sélectionné ci-dessus.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned results]</td> 
   <td>Définissez le nombre maximal de fichiers ou de dossiers que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Poursuivre l’exécution de l’itinéraire même si le module ne renvoie aucun résultat]</td> 
   <td>Activez cette option pour vous assurer que le scénario n’est pas arrêté si le module ne renvoie aucun résultat.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un dossier]

Crée un dossier à l’emplacement spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>Sélectionnez la destination vers laquelle vous souhaitez charger un fichier.</p> 
    <ul> 
     <li>[!UICONTROL Mon lecteur]</li> 
     <li>[!UICONTROL Partagé avec moi]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nouvel emplacement du dossier]</td> 
   <td>Accédez à l’emplacement où vous souhaitez créer un dossier.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom du nouveau dossier]</td> 
   <td>Saisissez le nom du dossier que vous créez.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Share folder]</td> 
   <td>Sélectionnez cette option si vous souhaitez partager le dossier avec toute personne disposant du lien [!UICONTROL Partager]. Sinon, le lien de partage est réservé au propriétaire uniquement.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un lien de partage]

Récupère le lien de partage d’un fichier dans Google Drive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Google Drive] à [!DNL Workfront Fusion], voir <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref"> Connexion de [!DNL Google Drive] à [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td>Mappez l’identifiant du fichier pour lequel vous souhaitez obtenir le lien de partage.</td> 
  </tr> 
 </tbody> 
</table>

## Dépannage

### Impossible de charger ou de mettre à jour un fichier

Il existe plusieurs situations entraînant l’échec du chargement ou de la mise à jour d’un fichier :

* Le fichier téléchargé est trop volumineux et dépasse la limite de taille de fichier maximale autorisée pour votre plan [!DNL Google Drive] ou vous avez dépassé la limite de stockage [!DNL Google Drive]. Vous pouvez mettre à niveau votre plan de stockage ou supprimer des fichiers existants du service [!DNL Google Drive].
* Le dossier sélectionné dans lequel le fichier devait être chargé n’existe plus. Le scénario s’arrête et il est alors nécessaire de sélectionner à nouveau un dossier cible.

## Recherche de fichiers

Dans le module Liste des fichiers d’un dossier, vous pouvez utiliser votre propre requête, qui se compose des éléments suivants :

* **[!UICONTROL Field]** - Attribut du fichier en cours de recherche, par exemple l’attribut `name` du fichier.

* **[!UICONTROL Opérateur]** - Test effectué sur les données pour fournir une correspondance, par exemple, `contains`.

* **[!UICONTROL Valeur]** - Contenu de l’attribut testé, par exemple, le nom du fichier `My cool document`.

Combinez des clauses avec les conjonctions `and` ou `or` et annulez la requête avec `not`.

* [Champs](#fields)
* [Types de valeurs](#value-types)
* [Opérateurs](#operators)
* [Exemples](#examples)

### Champs

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>champ </th> 
   <th>Type de valeur </th> 
   <th>Opérateurs</th> 
   <th> <p> Description</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>[!UICONTROL title]</code></td> 
   <td>chaîne</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Nom du fichier.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>chaîne </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> Texte complet du fichier, y compris le nom, la description, le contenu et le texte indexable.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> chaîne</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Type MIME du fichier.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> date<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Date de la dernière modification apportée au fichier.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> date<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Date à laquelle l’utilisateur a consulté un fichier pour la dernière fois.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>booléen </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Indique si le fichier est à la corbeille ou non.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>booléen </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>Indique si le fichier est en étoile ou non.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Si la collection [!UICONTROL parents] contient l’identifiant spécifié.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Utilisateurs qui détiennent le fichier.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Utilisateurs autorisés à modifier le fichier.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Utilisateurs autorisés à lire le fichier.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>booléen </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Fichiers qui se trouvent dans la collection "Partagé avec moi" de l’utilisateur.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>collection</td> 
   <td><code>has </code> </td> 
   <td> <p> Propriétés de fichier personnalisées publiques.</p> </td> 
  </tr> 
 </tbody> 
</table>

Tenez compte des points suivants concernant les opérateurs dans ces champs :

* L’opérateur `contains` n’effectue la correspondance de préfixe que pour un `title`.

  Par exemple, le titre &quot;HelloWorld&quot; correspond à `title contains 'Hello'`, mais pas à `title contains 'World'`.

* L’opérateur `contains` effectue uniquement la correspondance sur des jetons de chaîne entiers pour `fullText`.

  Par exemple, si le texte intégral d’un document contient la chaîne &quot;HelloWorld&quot;, seule la requête `fullText contains 'HelloWorld'` renvoie un résultat. Les requêtes telles que `fullText contains 'Hello'` ne renverraient aucun résultat dans ce scénario.

* L’opérateur `contains` correspond à une expression alphanumérique exacte si elle est entourée de guillemets doubles.

  Par exemple, si le `fullText` d’un document contient la chaîne &quot;Hello There world&quot;, la requête `fullText contains '"Hello there"'` renvoie un résultat, mais la requête `fullText contains '"Hello world"'` ne le fait pas.

  De plus, comme la recherche est alphanumérique, si le `fullText` d’un document contient la chaîne &quot;Hello_world&quot;, la requête `fullText contains '"Hello world"'` renvoie un résultat.

* Les champs de la date `type` ne sont actuellement pas comparables les uns aux autres, mais uniquement à des dates constantes.

### Types de valeurs

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Type de valeur</th> 
   <th> <p> Notes</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Chaîne </td> 
   <td> <p>Entourée de guillemets simples '. Échappez les guillemets simples dans les requêtes avec <code>\'</code>, par exemple, <code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Booléen </td> 
   <td> <p><code>true </code>ou <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Date </td> 
   <td> <p>Format RFC 3339, le fuseau horaire par défaut est UTC, par exemple <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Opérateurs

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Opérateur </th> 
   <th> <p>Notes</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>contains</code></td> 
   <td> <p>Le contenu d’une chaîne est présent dans l’autre chaîne.</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> Le contenu d’une chaîne ou d’une valeur booléenne est égal à l’autre.</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> Le contenu d’une chaîne ou d’une valeur booléenne n’est pas égal à l’autre.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> Une date est antérieure à une autre.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> Une date est antérieure ou égale à une autre.</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> Une date est postérieure à une autre.</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> Une date est ultérieure ou égale à une autre.</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>Un élément est contenu dans une collection.</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>Renvoie les fichiers qui correspondent aux deux clauses.</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>Renvoie les fichiers qui correspondent à l’une des clauses.</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>Négalise une clause de recherche.</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>Une collection contient un élément correspondant aux paramètres.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour les clauses composites, vous pouvez utiliser des parenthèses pour regrouper les clauses. Par exemple :
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` Cette recherche renvoie tous les fichiers avec une image ou un type MIME vidéo dont la dernière modification date du 4 juin 2012. Comme les opérateurs `and` et `or` sont évalués de gauche à droite, sans parenthèses, l’exemple ci-dessus renvoie uniquement les images modifiées après le 4 juin 2012, mais toutes les vidéos, même celles antérieures au 4 juin 2012.

### Exemples

Tous les exemples de cette page affichent le paramètre `<q>q</q>` non codé, où `title = 'hello'` est codé en tant que `title+%3d+%27hello%27`. Les bibliothèques clientes gèrent ce codage automatiquement.

* Recherchez des fichiers nommés &quot;hello&quot;.
  <pre>title = 'hello'</pre>
* Recherche de dossiers à l’aide du type MIME spécifique au dossier
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* Recherche de fichiers qui ne sont pas des dossiers
  <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* Recherchez des fichiers portant le nom &quot;hello&quot; et &quot;goodbye&quot;.
  <pre>Le titre contient "hello" et [!UICONTROL name] contient "goodbye"</pre>
* Recherchez des fichiers dont le nom ne contient pas le mot &quot;hello&quot;.
  <pre>pas le titre contient "hello"</pre>
* Recherchez des fichiers contenant le mot &quot;hello&quot; dans le contenu.
  <pre>fullText contient "hello"</pre>
* Recherchez des fichiers ne contenant pas le mot &quot;hello&quot; dans le contenu.
  <pre>not fullText contient "hello"</pre>
* Recherchez des fichiers contenant l’expression exacte &quot;hello world&quot; dans le contenu.
  <pre>fullText contient "hello world"'fullText contient "hello_world"</pre>
* Recherchez des fichiers avec une requête contenant le caractère &quot;\&quot; (par exemple, &quot;\authors&quot;).
  <pre>fullText contient "\\authors"</pre>
* Recherchez des fichiers pouvant être écrits par l’utilisateur &quot;test@example.org&quot;.
  <pre>'test@example.org' dans [!DNL writers]</pre>
* Recherchez l&#39;ID `1234567` dans la collection `parents`. Cette opération recherche tous les fichiers et dossiers situés directement dans le dossier dont l’ID est `1234567`.
  <pre>"1234567" dans [!UICONTROL parents]</pre>
* Recherchez l’ID d’alias `appDataFolder` dans la collection `parents`. Cela permet de trouver tous les fichiers et dossiers situés directement sous le [dossier Application Data](https://developers.google.com/drive/api/v2/appdata).
  <pre>'appDataFolder' dans les parents</pre>
* Recherchez des fichiers pouvant être écrits par les utilisateurs &quot;test@example.org&quot; et &quot;test2@example.org&quot;.
  <pre>'test@example.org' dans les auteurs et 'test2@example.org' dans les auteurs</pre>
* Recherchez les fichiers contenant le texte &quot;important&quot; qui se trouvent dans la corbeille.
  <pre>fullText contient "important" et trashed = true</pre>
* Recherche de fichiers modifiés après le 4 juin 2012
  <pre>modifiedDate &gt; '2012-06-04T12:00:00' // le fuseau horaire par défaut est UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:-08:00'</pre>
* Recherchez des fichiers partagés avec l’utilisateur autorisé dont le nom contient &quot;hello&quot;.
  <pre>sharedWithMe et le titre contient "hello"</pre>
* Recherchez des fichiers avec une [ propriété de fichier personnalisée ](https://developers.google.com/drive/api/v2/properties) nommée `additionalID` avec la valeur `8e8aceg2af2ge72e78`.
  <pre>Les propriétés ont { key='additionalID' et value='8e8aceg2af2ge72e78' et visibility='PRIVATE' }</pre>

La Source de ce guide est la [[!DNL Google Drive] documentation](https://developers.google.com/drive/api/v2/search-shareddrives).
