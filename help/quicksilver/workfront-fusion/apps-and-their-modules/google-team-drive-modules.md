---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Google Team Drive
description: Le [!DNL Adobe Workfront Fusion Google Team Drive] Les modules vous permettent de surveiller, de charger, de mettre à jour, de copier, de supprimer ou de récupérer des fichiers et de créer des dossiers dans vos [!DNL Google Shared] Conduis !
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# [!DNL Google Team Drive] modules

Le [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] Les modules vous permettent de surveiller, de charger, de mettre à jour, de copier, de supprimer ou de récupérer des fichiers et de créer des dossiers dans vos [!DNL Google Shared Drive].

Pour utiliser [!DNL Google Team Drive] avec [!DNL Adobe Workfront Fusion], il est nécessaire d’avoir une [!DNL G Suite] compte . Si vous n’en avez pas, vous pouvez créer une [!DNL G Suite] du compte [[!DNL G Suite] site d’inscription](https://gsuite.google.com/signup/businessstarter/welcome).

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Google Team Drive], ainsi que de la connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL Google Team Drive] modules, vous devez disposer d’un [!DNL Google Team Drive].

## [!DNL Google Team Drive] modules et leurs champs

Lorsque vous configurez [!DNL Google Team Drive] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Google Team Drive] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Les champs de la boîte de dialogue du module qui s’affichent dans **gras** (dans la variable [!DNL Workfront Fusion] scénario, **not** dans cet article de documentation) sont obligatoires.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL Fichiers de contrôle]

Renvoie les détails du fichier lorsqu’un nouveau fichier est ajouté et/ou modifié dans le dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Team Drive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td>[!UICONTROL Convertir [!DNL Google Documents] fichiers au format] </td> 
   <td> <p>Sélectionnez le format que vous souhaitez voir [!DNL Google Documents] fichiers convertis en .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Sheets] fichiers au format] </td> 
   <td> <p>Sélectionnez le format que vous souhaitez voir [!DNL Google Sheets] fichiers convertis en .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Slides] fichiers au format] </td> 
   <td> <p>Sélectionnez le format que vous souhaitez voir [!DNL Google Slides] fichiers convertis en .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Drawings] fichiers au format] </td> 
   <td> <p>Sélectionnez le format que vous souhaitez voir [!DNL Google Drawings] fichiers convertis en .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> Indiquez si vous souhaitez surveiller le dossier pour les nouveaux fichiers et les fichiers modifiés ou uniquement pour les nouveaux fichiers.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de fichiers téléchargés]</td> 
   <td> <p> Définition du nombre maximal de fichiers [!DNL Workfront Fusion] renverra pendant un cycle d'exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Chargement d’un fichier]](#upload-a-file)
* [[!UICONTROL Mettre à jour un fichier]](#update-a-file)
* [[!UICONTROL Copier un fichier]](#copy-a-file)
* [[!UICONTROL Suppression d’un fichier]](#delete-a-file)
* [[!UICONTROL Déplacer un fichier vers la corbeille]](#move-a-file-to-trash)
* [[!UICONTROL Obtention d’un fichier]](#get-a-file)
* [[!UICONTROL Obtention d’une liste de fichiers]](#get-a-file-list)
* [[!UICONTROL Création d’un dossier]](#create-a-folder)

#### [!UICONTROL Chargement d’un fichier]

Télécharge un fichier sur le lecteur partagé spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Team Drive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td> <p>[!UICONTROL Fichier source]</p> </td> 
   <td> <p>Indiquez le fichier à charger vers le lecteur partagé.</p> <p>Mappez le fichier que vous souhaitez charger à partir du module précédent (par exemple, [!UICONTROL HTTP] &gt;[!UICONTROL Obtenir un fichier] ou [!UICONTROL Dropbox] &gt;[!UICONTROL Obtenir un fichier)], ou saisissez manuellement le nom du fichier et les données du fichier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td> <p> Saisissez le titre du fichier qui sera affiché dans le dossier partagé.</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Team Drive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Saisissez (map) l’identifiant du fichier que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Fichier source]</p> </td> 
   <td>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>Saisissez le nouveau titre pour le fichier mis à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir un fichier]</td> 
   <td> <p> Activez cette option pour convertir le fichier en [!DNL Google] dans votre dossier partagé.</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Team Drive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> Sélectionnez le lecteur partagé contenant le fichier à copier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier cible dans lequel vous souhaitez copier le fichier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Saisissez (map) l’identifiant du fichier que vous souhaitez copier.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Nom du fichier de copie]</p> </td> 
   <td> <p>Saisissez le nouveau nom de fichier si vous souhaitez qu’il soit modifié à l’emplacement cible.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un fichier]

Supprime un fichier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Team Drive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Team Drive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Saisissez ou mappez l’identifiant du fichier que vous souhaitez déplacer vers la corbeille.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un fichier]

Récupère les détails du fichier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Team Drive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Documents] fichiers au format] </td> 
   <td> <p>Sélectionnez le format souhaité. [!DNL Google Documents] fichiers convertis en .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Sheets] fichiers au format] </td> 
   <td> <p>Sélectionnez le format souhaité. [!DNL Google Sheets] fichiers convertis en .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Slides] fichiers au format] </td> 
   <td> <p>Sélectionnez le format souhaité. [!DNL Google Slides] fichiers convertis en .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Drawings] fichiers au format] </td> 
   <td> <p>Sélectionnez le format souhaité. [!DNL Google Drawings] fichiers convertis en .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p> Saisissez ou mappez l’identifiant du fichier que vous souhaitez récupérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’une liste de fichiers]

Récupère les détails des fichiers et/ou des dossiers en fonction du terme de recherche.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Team Drive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
     <li> <p style="font-weight: bold;">[!UICONTROL Requête de recherche personnalisée]</p> <p>Saisissez le [!DNL Google] terme de requête de recherche. Pour plus d’informations, reportez-vous à la section [!DNL Google]'s <a href="https://developers.google.com/drive/api/v2/ref-search-terms">Documentation sur les requêtes de recherche</a>. Exemple: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Récupération]</td> 
   <td>Indiquez si vous souhaitez récupérer les fichiers, le dossier ou les deux.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de résultats renvoyés]</td> 
   <td> <p> Définition du nombre maximal de fichiers ou de dossiers [!DNL Workfront Fusion] renverra pendant un cycle d'exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Création d’un dossier]

Crée un dossier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Team Drive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
