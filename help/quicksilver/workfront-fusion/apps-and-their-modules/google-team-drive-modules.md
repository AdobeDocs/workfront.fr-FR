---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Google Team Drive
description: Les modules  [!DNL Adobe Workfront Fusion Google Team Drive]  vous permettent de surveiller, télécharger, mettre à jour, copier, supprimer ou récupérer des fichiers et de créer des dossiers dans votre  [!DNL Google Shared] lecteur.
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 23%

---

# Modules [!DNL Google Team Drive]

Les modules [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] vous permettent de surveiller, charger, mettre à jour, copier, supprimer ou récupérer des fichiers et de créer des dossiers dans votre [!DNL Google Shared Drive].

Pour utiliser [!DNL Google Team Drive] avec [!DNL Adobe Workfront Fusion], il est nécessaire d&#39;avoir un compte [!DNL Google Workspace]. Si vous n&#39;en avez pas, vous pouvez créer un compte [!DNL Google Workspace] sur le [[!DNL Google Workspace] site d&#39;inscription](https://workspace.google.com/business/signup/welcome).

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Google Team Drive] et les connecter à plusieurs applications et services tiers.

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

## Conditions préalables

Pour utiliser les modules [!DNL Google Team Drive], vous devez disposer d&#39;un [!DNL Google Team Drive].

## Modules [!DNL Google Team Drive] et leurs champs

Lorsque vous configurez des modules [!DNL Google Team Drive], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Google Team Drive] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Les champs de la boîte de dialogue du module qui s’affichent en **bold** (dans le scénario [!DNL Workfront Fusion], **not** de cet article de documentation) sont obligatoires.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Déclencheurs

#### [!UICONTROL Fichiers de contrôle]

Renvoie les détails du fichier lorsqu’un nouveau fichier est ajouté et/ou modifié dans le dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Team Drive] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Sélectionnez le lecteur partagé à regarder.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier dans le lecteur partagé.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quels fichiers regarder]</td> 
   <td> <p> Sélectionnez le type de fichiers à regarder.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Documents] au format] </td> 
   <td> <p>Sélectionnez le format dans lequel vous souhaitez convertir les fichiers [!DNL Google Documents] de contrôle.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Sheets] au format] </td> 
   <td> <p>Sélectionnez le format dans lequel vous souhaitez convertir les fichiers [!DNL Google Sheets] de contrôle.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Slides] au format] </td> 
   <td> <p>Sélectionnez le format dans lequel vous souhaitez convertir les fichiers [!DNL Google Slides] de contrôle.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Drawings] au format] </td> 
   <td> <p>Sélectionnez le format dans lequel vous souhaitez convertir les fichiers [!DNL Google Drawings] de contrôle.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> Indiquez si vous souhaitez surveiller le dossier pour les nouveaux fichiers et les fichiers modifiés ou uniquement pour les nouveaux fichiers.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de fichiers téléchargés]</td> 
   <td> <p> Définissez le nombre maximal de fichiers que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Charger un fichier]](#upload-a-file)
* [[!UICONTROL Mettre à jour un fichier]](#update-a-file)
* [[!UICONTROL Copier un fichier]](#copy-a-file)
* [[!UICONTROL Supprimer un fichier]](#delete-a-file)
* [[!UICONTROL Déplacer un fichier vers la corbeille]](#move-a-file-to-trash)
* [[!UICONTROL Obtenir un fichier]](#get-a-file)
* [[!UICONTROL Obtenir une liste de fichiers]](#get-a-file-list)
* [[!UICONTROL Créer un dossier]](#create-a-folder)

#### [!UICONTROL Charger un fichier]

Télécharge un fichier sur le lecteur partagé spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Team Drive] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive] </td> 
   <td> <p>Sélectionnez le lecteur partagé sur lequel vous souhaitez charger un fichier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier dans le lecteur partagé.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>Indiquez le fichier à charger vers le lecteur partagé.</p> <p>Mappez le fichier que vous souhaitez charger à partir du module précédent (par exemple, [!UICONTROL HTTP] &gt;[!UICONTROL Obtenir un fichier] ou [!UICONTROL Dropbox] &gt;[!UICONTROL Obtenir un fichier)], ou saisissez manuellement le nom du fichier et les données du fichier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td> <p> Saisissez le titre du fichier qui s’affichera dans le dossier partagé.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir un fichier]</td> 
   <td> <p> Activez cette option pour convertir le fichier au format Google correspondant dans votre dossier partagé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un fichier]

Permet de modifier le nom du fichier et/ou le contenu du fichier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Team Drive] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Sélectionnez le lecteur partagé contenant le fichier que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier dans le lecteur partagé.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td> <p> Saisissez (map) l’identifiant du fichier que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>Saisissez le nouveau titre pour le fichier mis à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir un fichier]</td> 
   <td> <p> Activez cette option pour convertir le fichier au format [!DNL Google] correspondant dans votre dossier partagé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copier un fichier]

Copie un fichier spécifié dans le dossier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Team Drive] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Sélectionnez le lecteur partagé qui contient le fichier que vous souhaitez copier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier cible dans lequel vous souhaitez copier le fichier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td> <p> Saisissez (map) l’identifiant du fichier que vous souhaitez copier.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Nom du fichier de copie]</p> </td> 
   <td> <p>Saisissez le nouveau nom de fichier si vous souhaitez qu’il soit modifié à l’emplacement cible.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un fichier]

Supprime un fichier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Team Drive] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td> <p> Saisissez ou mappez l’identifiant du fichier à supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un fichier vers la corbeille]

Déplace un fichier spécifié vers la corbeille.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Team Drive] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td> <p> Saisissez ou mappez l’identifiant du fichier que vous souhaitez déplacer vers la corbeille.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un fichier]

Récupère les détails du fichier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Team Drive] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Documents] au format] </td> 
   <td> <p>Sélectionnez le format dans lequel vous souhaitez convertir les fichiers [!DNL Google Documents].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Sheets] au format] </td> 
   <td> <p>Sélectionnez le format dans lequel vous souhaitez convertir les fichiers [!DNL Google Sheets].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Slides] au format] </td> 
   <td> <p>Sélectionnez le format dans lequel vous souhaitez convertir les fichiers [!DNL Google Slides].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir des fichiers [!DNL Google Drawings] au format] </td> 
   <td> <p>Sélectionnez le format dans lequel vous souhaitez convertir les fichiers [!DNL Google Drawings].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td> <p> Saisissez ou mappez l’identifiant du fichier que vous souhaitez récupérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir une liste de fichiers]

Récupère les détails des fichiers et/ou des dossiers en fonction du terme de recherche.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Team Drive] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Sélectionnez le lecteur partagé à partir duquel vous souhaitez répertorier les fichiers.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier dans lequel vous souhaitez répertorier les fichiers.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Sélectionnez le type de recherche à effectuer - voir ci-dessous.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Query]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL Recherche dans les noms de fichier]</p> <p style="font-weight: normal;">Entrez le nom du fichier (y compris l’extension du fichier) lorsque l’option [!UICONTROL Rechercher un terme exact] est sélectionnée ou saisissez la partie du nom lorsque l’option [!UICONTROL Rechercher les noms contenant le terme recherché est sélectionnée.]</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Recherche de texte intégral]</p> <p>Saisissez le terme à rechercher dans les noms, descriptions et contenus des fichiers.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Requête de recherche personnalisée]</p> <p>Saisissez le terme de requête de recherche [!DNL Google]. Pour plus d’informations, reportez-vous à la <a href="https://developers.google.com/drive/api/v2/ref-search-terms">documentation sur les requêtes de recherche</a> de [!DNL Google]. Exemple : <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Récupération]</td> 
   <td>Indiquez si vous souhaitez récupérer les fichiers, le dossier ou les deux.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned results]</td> 
   <td> <p> Définissez le nombre maximal de fichiers ou de dossiers que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un dossier]

Crée un dossier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Team Drive] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Sélectionnez le lecteur partagé sur lequel vous souhaitez créer un dossier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier dans lequel vous souhaitez créer un dossier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom du nouveau dossier]</td> 
   <td> <p> Saisissez le nom du nouveau dossier.</p> </td> 
  </tr> 
 </tbody> 
</table>
